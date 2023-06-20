# Comparing `tmp/fastiot-0.9.tar.gz` & `tmp/fastiot-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastiot-0.9.tar", last modified: Thu Mar 30 16:55:25 2023, max compression
+gzip compressed data, was "fastiot-1.0.tar", last modified: Tue Jun 20 11:08:16 2023, max compression
```

## Comparing `fastiot-0.9.tar` & `fastiot-1.0.tar`

### file list

```diff
@@ -1,157 +1,156 @@
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.150799 fastiot-0.9/
--rw-r--r--   0 jenkinsuser  (1000)     1000       59 2023-02-03 14:30:38.000000 fastiot-0.9/.dockerignore
--rw-r--r--   0 jenkinsuser  (1000)     1000      374 2023-02-03 14:30:38.000000 fastiot-0.9/.gitignore
--rw-r--r--   0 jenkinsuser  (1000)     1000      716 2023-03-13 12:11:39.000000 fastiot-0.9/.readthedocs.yaml
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.134799 fastiot-0.9/.run/
--rw-r--r--   0 jenkinsuser  (1000)     1000     1778 2023-02-03 14:30:38.000000 fastiot-0.9/.run/FastAPI.run.xml
--rw-r--r--   0 jenkinsuser  (1000)     1000     1696 2023-02-03 14:30:38.000000 fastiot-0.9/DOCUMENTING.md
--rw-r--r--   0 jenkinsuser  (1000)     1000      245 2023-02-03 14:30:38.000000 fastiot-0.9/Jenkinsfile
--rw-r--r--   0 jenkinsuser  (1000)     1000    10174 2023-02-03 14:30:38.000000 fastiot-0.9/LICENSE
--rw-r--r--   0 jenkinsuser  (1000)     1000      475 2023-03-29 14:54:09.000000 fastiot-0.9/MANIFEST.in
--rw-r--r--   0 jenkinsuser  (1000)     1000     5941 2023-03-30 16:55:25.150799 fastiot-0.9/PKG-INFO
--rw-r--r--   0 jenkinsuser  (1000)     1000     4508 2023-03-22 14:29:11.000000 fastiot-0.9/README.md
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.134799 fastiot-0.9/bin/
--rwxr-xr-x   0 jenkinsuser  (1000)     1000     1344 2023-03-13 17:14:07.000000 fastiot-0.9/bin/fiot
--rw-r--r--   0 jenkinsuser  (1000)     1000      364 2023-02-03 14:30:38.000000 fastiot-0.9/configure.py
--rwxr-xr-x   0 jenkinsuser  (1000)     1000      400 2023-02-03 14:30:38.000000 fastiot-0.9/install.sh
--rw-r--r--   0 jenkinsuser  (1000)     1000     2941 2023-03-30 16:55:13.000000 fastiot-0.9/pyproject.toml
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.138799 fastiot-0.9/requirements/
--rw-r--r--   0 jenkinsuser  (1000)     1000     6402 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.all.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1340 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.compile.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     2243 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.dash.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1596 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.dev.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     3287 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.docs.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1788 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.fastapi.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1893 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.influxdb.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1236 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.mariadb.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1276 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.mongodb.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1715 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.opcua.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1236 2023-03-22 11:39:11.000000 fastiot-0.9/requirements/requirements.postgredb.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000     1179 2023-03-22 11:39:11.000000 fastiot-0.9/requirements.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000       38 2023-03-30 16:55:25.150799 fastiot-0.9/setup.cfg
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.134799 fastiot-0.9/src/
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.138799 fastiot-0.9/src/fastiot/
--rw-r--r--   0 jenkinsuser  (1000)     1000      383 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000       20 2023-03-30 16:55:13.000000 fastiot-0.9/src/fastiot/__version__.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.138799 fastiot-0.9/src/fastiot/cli/
--rw-r--r--   0 jenkinsuser  (1000)     1000      383 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000       83 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/cli_logging.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.138799 fastiot-0.9/src/fastiot/cli/commands/
--rw-r--r--   0 jenkinsuser  (1000)     1000       95 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/commands/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000    18451 2023-03-22 11:39:11.000000 fastiot-0.9/src/fastiot/cli/commands/build.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     9995 2023-03-30 12:54:10.000000 fastiot-0.9/src/fastiot/cli/commands/build_lib.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1511 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/commands/clean.py
--rw-r--r--   0 jenkinsuser  (1000)     1000    20691 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/cli/commands/config.py
--rw-r--r--   0 jenkinsuser  (1000)     1000    14954 2023-03-30 12:54:10.000000 fastiot-0.9/src/fastiot/cli/commands/create.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3433 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/commands/deploy.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3651 2023-03-22 11:39:11.000000 fastiot-0.9/src/fastiot/cli/commands/manage_requirements.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2490 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/commands/nuitka_compile.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     4108 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/commands/print.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     4163 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/commands/run_tests.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3745 2023-03-03 11:34:09.000000 fastiot-0.9/src/fastiot/cli/commands/start.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3151 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/commands/stop.py
--rwxr-xr-x   0 jenkinsuser  (1000)     1000      778 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/commands/version.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.138799 fastiot-0.9/src/fastiot/cli/common/
--rw-r--r--   0 jenkinsuser  (1000)     1000        0 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/common/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      200 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/common/docker_templates.py
--rw-r--r--   0 jenkinsuser  (1000)     1000    11914 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/cli/common/infrastructure_services.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1188 2023-03-22 11:39:11.000000 fastiot-0.9/src/fastiot/cli/constants.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      531 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/env.py
--rwxr-xr-x   0 jenkinsuser  (1000)     1000     1344 2023-03-13 17:14:07.000000 fastiot-0.9/src/fastiot/cli/fiot.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3027 2023-03-13 17:14:07.000000 fastiot-0.9/src/fastiot/cli/helper_fn.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2853 2023-03-29 09:54:09.000000 fastiot-0.9/src/fastiot/cli/import_configure.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1489 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/infrastructure_service_fn.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.142799 fastiot-0.9/src/fastiot/cli/model/
--rw-r--r--   0 jenkinsuser  (1000)     1000      599 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/model/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      380 2023-02-22 10:24:09.000000 fastiot-0.9/src/fastiot/cli/model/compose_info.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     4754 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/model/deployment.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2128 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/model/docker_template.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     7083 2023-03-30 15:08:01.000000 fastiot-0.9/src/fastiot/cli/model/infrastructure_service.py
--rw-r--r--   0 jenkinsuser  (1000)     1000    12138 2023-03-29 09:54:09.000000 fastiot-0.9/src/fastiot/cli/model/manifest.py
--rw-r--r--   0 jenkinsuser  (1000)     1000    10312 2023-03-30 12:54:10.000000 fastiot-0.9/src/fastiot/cli/model/project.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1655 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/model/service.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.142799 fastiot-0.9/src/fastiot/cli/templates/
--rw-r--r--   0 jenkinsuser  (1000)     1000     4692 2023-03-13 12:11:39.000000 fastiot-0.9/src/fastiot/cli/templates/Dockerfile.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000     1280 2023-02-20 16:31:42.000000 fastiot-0.9/src/fastiot/cli/templates/ansible-playbook.yaml.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000      113 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/ansible_hosts.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000      900 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/docker-bake.hcl.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000     1791 2023-02-24 12:34:10.000000 fastiot-0.9/src/fastiot/cli/templates/docker-compose.yaml.j2
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.142799 fastiot-0.9/src/fastiot/cli/templates/new_project/
--rw-r--r--   0 jenkinsuser  (1000)     1000       59 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/.dockerignore
--rw-r--r--   0 jenkinsuser  (1000)     1000        0 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/.env.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000      152 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/.env.production.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000      374 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/.gitignore
--rw-r--r--   0 jenkinsuser  (1000)     1000      181 2023-03-07 10:48:31.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/README.md.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000        0 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      234 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/configure.py.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000       47 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/deployment.yaml
--rw-r--r--   0 jenkinsuser  (1000)     1000      137 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/deployment.yaml.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000      193 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/dummy_test.py
--rwxr-xr-x   0 jenkinsuser  (1000)     1000      400 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/install.sh
--rw-r--r--   0 jenkinsuser  (1000)     1000       45 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_project/requirements.txt.j2
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.142799 fastiot-0.9/src/fastiot/cli/templates/new_service/
--rw-r--r--   0 jenkinsuser  (1000)     1000      125 2023-03-13 16:54:07.000000 fastiot-0.9/src/fastiot/cli/templates/new_service/.run.py.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000       70 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/cli/templates/new_service/manifest.yaml.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000     1714 2023-03-13 16:54:07.000000 fastiot-0.9/src/fastiot/cli/templates/new_service/servicename_service.py.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000      744 2023-03-13 12:11:39.000000 fastiot-0.9/src/fastiot/cli/templates/pyproject.toml.j2
--rw-r--r--   0 jenkinsuser  (1000)     1000     1734 2023-03-22 11:24:11.000000 fastiot-0.9/src/fastiot/cli/typer_app.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     6104 2023-02-20 14:44:16.000000 fastiot-0.9/src/fastiot/cli/version.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.142799 fastiot-0.9/src/fastiot/core/
--rw-r--r--   0 jenkinsuser  (1000)     1000      739 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/core/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000    14673 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/core/broker_connection.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      148 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/core/core_uuid.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     8636 2023-03-14 11:18:17.000000 fastiot-0.9/src/fastiot/core/data_models.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1686 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/core/logger.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      842 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/core/serialization.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     9074 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/core/service.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2344 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/core/service_annotations.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1664 2023-03-13 17:14:07.000000 fastiot-0.9/src/fastiot/core/subject_helper.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      351 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/core/time.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.146799 fastiot-0.9/src/fastiot/db/
--rw-r--r--   0 jenkinsuser  (1000)     1000      141 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/db/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3444 2023-03-13 17:14:07.000000 fastiot-0.9/src/fastiot/db/influxdb_helper_fn.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2584 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/db/mariadb_helper_fn.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      769 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/db/mariadb_schema_checks.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     4354 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/db/mongodb_helper_fn.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3529 2023-03-30 15:08:01.000000 fastiot-0.9/src/fastiot/db/redis_helper.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2113 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/db/time_scale_helper_fn.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.146799 fastiot-0.9/src/fastiot/env/
--rw-r--r--   0 jenkinsuser  (1000)     1000       94 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      666 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3143 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_basic.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1235 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_broker.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      374 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_constants_basic.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2124 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_constants_db.py
--rw-r--r--   0 jenkinsuser  (1000)     1000        1 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_elasticdb.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3078 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_influxdb.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2118 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_mariadb.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3049 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_mongodb.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1158 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_redis.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2155 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/env_timescaledb.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      663 2023-03-30 16:54:11.000000 fastiot-0.9/src/fastiot/env/helpers.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.146799 fastiot-0.9/src/fastiot/exceptions/
--rw-r--r--   0 jenkinsuser  (1000)     1000       44 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/exceptions/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      517 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/exceptions/exceptions.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.146799 fastiot-0.9/src/fastiot/msg/
--rw-r--r--   0 jenkinsuser  (1000)     1000      188 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/msg/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      657 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/msg/custom_db_data_type_conversion.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2812 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/msg/hist.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      126 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/msg/redis.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     2042 2023-03-14 11:18:17.000000 fastiot-0.9/src/fastiot/msg/thing.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      587 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/msg/time_series_msg.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1943 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/testlib.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.146799 fastiot-0.9/src/fastiot/util/
--rw-r--r--   0 jenkinsuser  (1000)     1000        0 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/util/__init__.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      779 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/util/case_conversions.py
--rw-r--r--   0 jenkinsuser  (1000)     1000       65 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/util/classproperty.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     6095 2023-03-13 17:14:07.000000 fastiot-0.9/src/fastiot/util/csv_reader.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     1580 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/util/object_helper.py
--rw-r--r--   0 jenkinsuser  (1000)     1000      176 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/util/ports.py
--rw-r--r--   0 jenkinsuser  (1000)     1000     3541 2023-02-03 14:30:38.000000 fastiot-0.9/src/fastiot/util/read_yaml.py
-drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-03-30 16:55:25.138799 fastiot-0.9/src/fastiot.egg-info/
--rw-r--r--   0 jenkinsuser  (1000)     1000     5941 2023-03-30 16:55:25.000000 fastiot-0.9/src/fastiot.egg-info/PKG-INFO
--rw-r--r--   0 jenkinsuser  (1000)     1000     4632 2023-03-30 16:55:25.000000 fastiot-0.9/src/fastiot.egg-info/SOURCES.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000        1 2023-03-30 16:55:25.000000 fastiot-0.9/src/fastiot.egg-info/dependency_links.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000       47 2023-03-30 16:55:25.000000 fastiot-0.9/src/fastiot.egg-info/entry_points.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000      700 2023-03-30 16:55:25.000000 fastiot-0.9/src/fastiot.egg-info/requires.txt
--rw-r--r--   0 jenkinsuser  (1000)     1000        8 2023-03-30 16:55:25.000000 fastiot-0.9/src/fastiot.egg-info/top_level.txt
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.034721 fastiot-1.0/
+-rw-r--r--   0 jenkinsuser  (1000)     1000       59 2023-02-03 14:30:38.000000 fastiot-1.0/.dockerignore
+-rw-r--r--   0 jenkinsuser  (1000)     1000      374 2023-02-03 14:30:38.000000 fastiot-1.0/.gitignore
+-rw-r--r--   0 jenkinsuser  (1000)     1000      716 2023-03-13 12:11:39.000000 fastiot-1.0/.readthedocs.yaml
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1696 2023-02-03 14:30:38.000000 fastiot-1.0/DOCUMENTING.md
+-rw-r--r--   0 jenkinsuser  (1000)     1000      245 2023-02-03 14:30:38.000000 fastiot-1.0/Jenkinsfile
+-rw-r--r--   0 jenkinsuser  (1000)     1000    10174 2023-02-03 14:30:38.000000 fastiot-1.0/LICENSE
+-rw-r--r--   0 jenkinsuser  (1000)     1000      475 2023-03-29 14:54:09.000000 fastiot-1.0/MANIFEST.in
+-rw-r--r--   0 jenkinsuser  (1000)     1000     6322 2023-06-20 11:08:16.034721 fastiot-1.0/PKG-INFO
+-rw-r--r--   0 jenkinsuser  (1000)     1000     4808 2023-05-23 09:44:09.000000 fastiot-1.0/README.md
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.022721 fastiot-1.0/bin/
+-rwxr-xr-x   0 jenkinsuser  (1000)     1000     1344 2023-03-13 17:14:07.000000 fastiot-1.0/bin/fiot
+-rw-r--r--   0 jenkinsuser  (1000)     1000      364 2023-02-03 14:30:38.000000 fastiot-1.0/configure.py
+-rwxr-xr-x   0 jenkinsuser  (1000)     1000      400 2023-02-03 14:30:38.000000 fastiot-1.0/install.sh
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3063 2023-06-20 11:08:03.000000 fastiot-1.0/pyproject.toml
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.022721 fastiot-1.0/requirements/
+-rw-r--r--   0 jenkinsuser  (1000)     1000     6536 2023-06-20 09:57:03.000000 fastiot-1.0/requirements/requirements.all.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000      582 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.compile.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1663 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.dash.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1655 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.dev.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2573 2023-06-20 09:57:03.000000 fastiot-1.0/requirements/requirements.docs.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1099 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.fastapi.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1257 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.influxdb.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000      478 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.mariadb.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000      518 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.mongodb.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000      957 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.opcua.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000      478 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.postgredb.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000      516 2023-06-20 09:47:18.000000 fastiot-1.0/requirements/requirements.redis.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000      421 2023-06-20 09:47:18.000000 fastiot-1.0/requirements.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000       38 2023-06-20 11:08:16.034721 fastiot-1.0/setup.cfg
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.018721 fastiot-1.0/src/
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.022721 fastiot-1.0/src/fastiot/
+-rw-r--r--   0 jenkinsuser  (1000)     1000      383 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000       20 2023-06-20 11:08:03.000000 fastiot-1.0/src/fastiot/__version__.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.026721 fastiot-1.0/src/fastiot/cli/
+-rw-r--r--   0 jenkinsuser  (1000)     1000      383 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000       83 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/cli_logging.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.026721 fastiot-1.0/src/fastiot/cli/commands/
+-rw-r--r--   0 jenkinsuser  (1000)     1000       95 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/commands/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000    18609 2023-04-19 15:19:11.000000 fastiot-1.0/src/fastiot/cli/commands/build.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     9995 2023-03-30 12:54:10.000000 fastiot-1.0/src/fastiot/cli/commands/build_lib.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1511 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/commands/clean.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000    23450 2023-06-06 16:24:09.000000 fastiot-1.0/src/fastiot/cli/commands/config.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000    15001 2023-04-20 08:49:08.000000 fastiot-1.0/src/fastiot/cli/commands/create.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3433 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/commands/deploy.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3744 2023-04-12 13:18:03.000000 fastiot-1.0/src/fastiot/cli/commands/manage_requirements.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2490 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/commands/nuitka_compile.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     4108 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/commands/print.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     4161 2023-04-18 09:54:10.000000 fastiot-1.0/src/fastiot/cli/commands/run_tests.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3912 2023-04-18 09:54:10.000000 fastiot-1.0/src/fastiot/cli/commands/start.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3151 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/commands/stop.py
+-rwxr-xr-x   0 jenkinsuser  (1000)     1000      778 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/commands/version.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.026721 fastiot-1.0/src/fastiot/cli/common/
+-rw-r--r--   0 jenkinsuser  (1000)     1000        0 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/common/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      200 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/common/docker_templates.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000    10334 2023-05-16 13:50:27.000000 fastiot-1.0/src/fastiot/cli/common/infrastructure_services.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1188 2023-06-16 10:12:09.000000 fastiot-1.0/src/fastiot/cli/constants.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1280 2023-04-19 16:13:33.000000 fastiot-1.0/src/fastiot/cli/env.py
+-rwxr-xr-x   0 jenkinsuser  (1000)     1000     1344 2023-03-13 17:14:07.000000 fastiot-1.0/src/fastiot/cli/fiot.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3339 2023-04-12 13:18:03.000000 fastiot-1.0/src/fastiot/cli/helper_fn.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2853 2023-03-29 09:54:09.000000 fastiot-1.0/src/fastiot/cli/import_configure.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1486 2023-03-31 14:03:52.000000 fastiot-1.0/src/fastiot/cli/infrastructure_service_fn.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.026721 fastiot-1.0/src/fastiot/cli/model/
+-rw-r--r--   0 jenkinsuser  (1000)     1000      599 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/model/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      437 2023-06-06 16:24:09.000000 fastiot-1.0/src/fastiot/cli/model/compose_info.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     5644 2023-06-06 16:24:09.000000 fastiot-1.0/src/fastiot/cli/model/deployment.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2128 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/model/docker_template.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     7083 2023-03-30 15:08:01.000000 fastiot-1.0/src/fastiot/cli/model/infrastructure_service.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000    12367 2023-06-16 10:12:09.000000 fastiot-1.0/src/fastiot/cli/model/manifest.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000    10312 2023-03-30 12:54:10.000000 fastiot-1.0/src/fastiot/cli/model/project.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1951 2023-04-19 15:19:11.000000 fastiot-1.0/src/fastiot/cli/model/service.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.030721 fastiot-1.0/src/fastiot/cli/templates/
+-rw-r--r--   0 jenkinsuser  (1000)     1000     5358 2023-05-08 08:24:09.000000 fastiot-1.0/src/fastiot/cli/templates/Dockerfile.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1280 2023-02-20 16:31:42.000000 fastiot-1.0/src/fastiot/cli/templates/ansible-playbook.yaml.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000      113 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/ansible_hosts.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000      900 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/docker-bake.hcl.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2514 2023-06-06 16:29:12.000000 fastiot-1.0/src/fastiot/cli/templates/docker-compose.yaml.j2
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.030721 fastiot-1.0/src/fastiot/cli/templates/new_project/
+-rw-r--r--   0 jenkinsuser  (1000)     1000       59 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/.dockerignore
+-rw-r--r--   0 jenkinsuser  (1000)     1000        0 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/.env.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000      152 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/.env.production.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000      374 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/.gitignore
+-rw-r--r--   0 jenkinsuser  (1000)     1000      181 2023-03-07 10:48:31.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/README.md.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000        0 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      234 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/configure.py.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000       47 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/deployment.yaml
+-rw-r--r--   0 jenkinsuser  (1000)     1000      137 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/deployment.yaml.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000      193 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/dummy_test.py
+-rwxr-xr-x   0 jenkinsuser  (1000)     1000      400 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/install.sh
+-rw-r--r--   0 jenkinsuser  (1000)     1000       45 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_project/requirements.txt.j2
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.030721 fastiot-1.0/src/fastiot/cli/templates/new_service/
+-rw-r--r--   0 jenkinsuser  (1000)     1000      125 2023-03-13 16:54:07.000000 fastiot-1.0/src/fastiot/cli/templates/new_service/.run.py.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000       70 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/cli/templates/new_service/manifest.yaml.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1714 2023-03-13 16:54:07.000000 fastiot-1.0/src/fastiot/cli/templates/new_service/servicename_service.py.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000      744 2023-03-13 12:11:39.000000 fastiot-1.0/src/fastiot/cli/templates/pyproject.toml.j2
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1964 2023-04-12 13:18:03.000000 fastiot-1.0/src/fastiot/cli/typer_app.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     6104 2023-02-20 14:44:16.000000 fastiot-1.0/src/fastiot/cli/version.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.030721 fastiot-1.0/src/fastiot/core/
+-rw-r--r--   0 jenkinsuser  (1000)     1000      739 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/core/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000    15042 2023-05-23 09:44:09.000000 fastiot-1.0/src/fastiot/core/broker_connection.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      148 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/core/core_uuid.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     8636 2023-03-14 11:18:17.000000 fastiot-1.0/src/fastiot/core/data_models.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1686 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/core/logger.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      981 2023-06-12 13:24:11.000000 fastiot-1.0/src/fastiot/core/serialization.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000    10368 2023-06-06 15:04:09.000000 fastiot-1.0/src/fastiot/core/service.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2401 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/core/service_annotations.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1664 2023-03-13 17:14:07.000000 fastiot-1.0/src/fastiot/core/subject_helper.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      351 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/core/time.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.030721 fastiot-1.0/src/fastiot/db/
+-rw-r--r--   0 jenkinsuser  (1000)     1000      141 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/db/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3465 2023-04-12 13:18:03.000000 fastiot-1.0/src/fastiot/db/influxdb_helper_fn.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2593 2023-04-12 13:18:03.000000 fastiot-1.0/src/fastiot/db/mariadb_helper_fn.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      769 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/db/mariadb_schema_checks.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     4372 2023-04-12 13:18:03.000000 fastiot-1.0/src/fastiot/db/mongodb_helper_fn.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3948 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/db/redis_helper.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2192 2023-04-12 13:18:03.000000 fastiot-1.0/src/fastiot/db/time_scale_helper_fn.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.034721 fastiot-1.0/src/fastiot/env/
+-rw-r--r--   0 jenkinsuser  (1000)     1000       94 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/env/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      666 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/env/env.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3202 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/env/env_basic.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1235 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/env/env_broker.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      374 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/env/env_constants_basic.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1880 2023-05-16 13:49:07.000000 fastiot-1.0/src/fastiot/env/env_constants_db.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3078 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/env/env_influxdb.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2118 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/env/env_mariadb.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     3049 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/env/env_mongodb.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1150 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/env/env_redis.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2155 2023-03-30 16:54:11.000000 fastiot-1.0/src/fastiot/env/env_timescaledb.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      664 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/env/helpers.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.034721 fastiot-1.0/src/fastiot/exceptions/
+-rw-r--r--   0 jenkinsuser  (1000)     1000       44 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/exceptions/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      517 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/exceptions/exceptions.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.034721 fastiot-1.0/src/fastiot/msg/
+-rw-r--r--   0 jenkinsuser  (1000)     1000      188 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/msg/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      657 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/msg/custom_db_data_type_conversion.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2812 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/msg/hist.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      126 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/msg/redis.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     2042 2023-03-14 11:18:17.000000 fastiot-1.0/src/fastiot/msg/thing.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      587 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/msg/time_series_msg.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     4964 2023-04-28 12:02:53.000000 fastiot-1.0/src/fastiot/testlib.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.034721 fastiot-1.0/src/fastiot/util/
+-rw-r--r--   0 jenkinsuser  (1000)     1000        0 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/util/__init__.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      784 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/util/case_conversions.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000       65 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/util/classproperty.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     5198 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/util/config_helper.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     6152 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/util/csv_reader.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1580 2023-02-03 14:30:38.000000 fastiot-1.0/src/fastiot/util/object_helper.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000      258 2023-03-31 14:03:52.000000 fastiot-1.0/src/fastiot/util/ports.py
+-rw-r--r--   0 jenkinsuser  (1000)     1000     1370 2023-05-22 13:04:10.000000 fastiot-1.0/src/fastiot/util/read_yaml.py
+drwxr-xr-x   0 jenkinsuser  (1000)     1000        0 2023-06-20 11:08:16.026721 fastiot-1.0/src/fastiot.egg-info/
+-rw-r--r--   0 jenkinsuser  (1000)     1000     6322 2023-06-20 11:08:15.000000 fastiot-1.0/src/fastiot.egg-info/PKG-INFO
+-rw-r--r--   0 jenkinsuser  (1000)     1000     4648 2023-06-20 11:08:16.000000 fastiot-1.0/src/fastiot.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000        1 2023-06-20 11:08:15.000000 fastiot-1.0/src/fastiot.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000       47 2023-06-20 11:08:15.000000 fastiot-1.0/src/fastiot.egg-info/entry_points.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000      727 2023-06-20 11:08:15.000000 fastiot-1.0/src/fastiot.egg-info/requires.txt
+-rw-r--r--   0 jenkinsuser  (1000)     1000        8 2023-06-20 11:08:15.000000 fastiot-1.0/src/fastiot.egg-info/top_level.txt
```

### Comparing `fastiot-0.9/.readthedocs.yaml` & `fastiot-1.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/DOCUMENTING.md` & `fastiot-1.0/DOCUMENTING.md`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/LICENSE` & `fastiot-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/PKG-INFO` & `fastiot-1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fastiot
-Version: 0.9
+Version: 1.0
 Summary: FastIoT Platform
 Author-email: Tilman Klaeger <tilman.klaeger@ivv-dd.fraunhofer.de>, Konstantin Merker <konstantin.merker@ivv-dd.fraunhofer.de>, Fraunhofer Institute for Process Engineering and Packaging IVV <info@ivv-dd.fraunhofer.de>
-Maintainer-email: Tilman Klaeger <tilman.klaeger@ivv-dd.fraunhofer.de>, Jialiang Yin <jialiang.yin@ivv-dd.fraunhofer.de>
+Maintainer-email: Tilman Klaeger <tilman.klaeger@ivv-dd.fraunhofer.de>, Tim Kaluza <tim.kaluza@ivv-dd.fraunhofer.de>, Jialiang Yin <jialiang.yin@ivv-dd.fraunhofer.de>
 Project-URL: Homepage, https://github.com/FraunhoferIVV/fastiot
 Project-URL: Source, https://github.com/FraunhoferIVV/fastiot
 Project-URL: Documentation, https://fastiot.readthedocs.io
 Keywords: Industrial IoT,IoT,Industry4.0,IIoT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -23,19 +23,20 @@
 Provides-Extra: dev
 Provides-Extra: fastapi
 Provides-Extra: influxdb
 Provides-Extra: mariadb
 Provides-Extra: mongodb
 Provides-Extra: opcua
 Provides-Extra: postgredb
+Provides-Extra: redis
 Provides-Extra: dash
 Provides-Extra: docs
 License-File: LICENSE
 
-# Fast-IoT (fastiot)
+# FastIoT (fastiot)
 
 FastIoT is a framework for rapid development of IIoT-Systems using Python as main programming language.
 It helps to set up a micro-service architecture and create services. The development has been started as basis for 
 various research projects at Fraunhofer IVV, Dresden, Germany.  
 
 To get started quickly it is equipped with a powerful command line interface (CLI): `fiot`.
 This helps setting up a new project, create new services and run tests. 
@@ -108,15 +109,20 @@
 
 To run services locally, in your IDE or within a container you may also refer to the complete documentation.
 
 ## Developing FastIoT
 
 Simply check out this project and install the dependencies listed in `requirements.txt`.
 To run all tests and sample services you may also install additional packages listed in 
-`requirements/requirements-all.txt`. 
+`requirements/requirements.all.txt`.
+Do *NOT* install fastiot when developing within this code.
+This will produce duplicates and may show weird errors. 
+If in doubt run `pip uninstall fastiot`.
+
+To make sure you can run commands like `fiot` you must add the `src`-directory to your Python Path: `export PYTHONPATH="$(pwd)/src:$PYTHONPATH`
 
 ### Project structure
 
 A detailed structure for all projects based on FastIoT is listed in the documentation. Here just the few most important 
 parts are listed:
 
 * `src/fastiot`: The core library and base with CLI, message handling, …
```

### Comparing `fastiot-0.9/README.md` & `fastiot-1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Fast-IoT (fastiot)
+# FastIoT (fastiot)
 
 FastIoT is a framework for rapid development of IIoT-Systems using Python as main programming language.
 It helps to set up a micro-service architecture and create services. The development has been started as basis for 
 various research projects at Fraunhofer IVV, Dresden, Germany.  
 
 To get started quickly it is equipped with a powerful command line interface (CLI): `fiot`.
 This helps setting up a new project, create new services and run tests. 
@@ -75,15 +75,20 @@
 
 To run services locally, in your IDE or within a container you may also refer to the complete documentation.
 
 ## Developing FastIoT
 
 Simply check out this project and install the dependencies listed in `requirements.txt`.
 To run all tests and sample services you may also install additional packages listed in 
-`requirements/requirements-all.txt`. 
+`requirements/requirements.all.txt`.
+Do *NOT* install fastiot when developing within this code.
+This will produce duplicates and may show weird errors. 
+If in doubt run `pip uninstall fastiot`.
+
+To make sure you can run commands like `fiot` you must add the `src`-directory to your Python Path: `export PYTHONPATH="$(pwd)/src:$PYTHONPATH`
 
 ### Project structure
 
 A detailed structure for all projects based on FastIoT is listed in the documentation. Here just the few most important 
 parts are listed:
 
 * `src/fastiot`: The core library and base with CLI, message handling, …
```

### Comparing `fastiot-0.9/bin/fiot` & `fastiot-1.0/bin/fiot`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/pyproject.toml` & `fastiot-1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,28 @@
     "setuptools>=67",
     "setuptools_scm[toml]>=6.2",
     "wheel",
 ]
 
 [project]
 name = "fastiot"
-version = "0.9"
+version = "1.0"
 maintainers = [
     { name = "Tilman Klaeger", email = "tilman.klaeger@ivv-dd.fraunhofer.de" },
+    { name = "Tim Kaluza", email = "tim.kaluza@ivv-dd.fraunhofer.de" },
     { name = "Jialiang Yin", email = "jialiang.yin@ivv-dd.fraunhofer.de" },
 ]
 keywords = [
     "Industrial IoT",
     "IoT",
     "Industry4.0",
     "IIoT",
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -36,21 +37,14 @@
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "pydantic>=1.9.0,<2",
     "msgpack>=1,<2",
     "nats-py>=2.1.0,<3",
     "PyYAML>=5,<7",
-    "typer>=0.4.1,<1",
-    "Jinja2>=2,<4",
-    "Redis>4",
-    "tomli~=2.0.1",
-    "tomli_w",
-    "build",
-    "pip-tools",
 ]
 
 [[project.authors]]
 name = "Tilman Klaeger"
 email = "tilman.klaeger@ivv-dd.fraunhofer.de"
 
 [[project.authors]]
@@ -70,14 +64,21 @@
 compile = [
     "Nuitka>=1.1.7,<2",
     "ordered-set",
 ]
 dev = [
     "pytest>=7.2,<8",
     "typer[all]>=0.4.1,<1",
+    "tomli~=2.0.1",
+    "tomli_w",
+    "build",
+    "pip-tools",
+    "typer>=0.4.1,<1",
+    "Jinja2>=2,<4",
+    "pytest-cov>=4.1.0",
 ]
 fastapi = [
     "fastapi",
     "aiofiles",
     "uvicorn[standard]",
 ]
 influxdb = [
@@ -92,14 +93,17 @@
 opcua = [
     "opcua>=0.98.8,<1",
     "asyncua",
 ]
 postgredb = [
     "psycopg2-binary>=2.9.3,<3",
 ]
+redis = [
+    "Redis>4",
+]
 dash = [
     "dash~=2.6.1",
     "plotly~=5.9.0",
     "numpy",
     "pandas",
     "dash-bootstrap-components",
     "xlsxwriter",
```

### Comparing `fastiot-0.9/requirements/requirements.all.txt` & `fastiot-1.0/requirements/requirements.all.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,128 +1,131 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    fiot config --update-requirements
+#    fiot extras set-requirements --update-requirements
 #
 
-aiocsv==1.2.3             # via influxdb-client
+aiocsv==1.2.4             # via influxdb-client
 aiofiles==23.1.0          # via asyncua, fastiot (pyproject.toml)
 aiohttp==3.8.4            # via influxdb-client
 aiosignal==1.3.1          # via aiohttp
-aiosqlite==0.18.0         # via asyncua
+aiosqlite==0.19.0         # via asyncua
 alabaster==0.7.13         # via sphinx
-anyio==3.6.2              # via starlette, watchfiles
+anyio==3.7.0              # via starlette, watchfiles
 async-timeout==4.0.2      # via aiohttp, redis
-asyncua==1.0.1            # via fastiot (pyproject.toml)
-attrs==22.2.0             # via aiohttp, pytest
+asyncua==1.0.2            # via fastiot (pyproject.toml)
+attrs==23.1.0             # via aiohttp
 autodoc-pydantic==1.8.0   # via fastiot (pyproject.toml)
 babel==2.12.1             # via sphinx
-beautifulsoup4==4.12.0    # via sphinx-material
+beautifulsoup4==4.12.2    # via sphinx-material
+blinker==1.6.2            # via flask
 brotli==1.0.9             # via flask-compress
 build==0.10.0             # via fastiot (pyproject.toml), pip-tools
-certifi==2022.12.7        # via influxdb-client, requests
+certifi==2023.5.7         # via influxdb-client, requests
 cffi==1.15.1              # via cryptography
 charset-normalizer==3.1.0  # via aiohttp, requests
 click==8.1.3              # via flask, pip-tools, sphinx-click, typer, uvicorn
 colorama==0.4.6           # via typer
-commonmark==0.9.1         # via recommonmark, rich
-cryptography==39.0.2      # via asyncua
+commonmark==0.9.1         # via recommonmark
+coverage[toml]==7.2.7     # via pytest-cov
+cryptography==41.0.1      # via asyncua
 css-html-js-minify==2.5.5  # via sphinx-material
 dash==2.6.2               # via dash-bootstrap-components, fastiot (pyproject.toml)
 dash-bootstrap-components==1.4.1  # via fastiot (pyproject.toml)
 dash-core-components==2.0.0  # via dash
 dash-html-components==2.0.0  # via dash
 dash-table==5.0.0         # via dash
 dnspython==2.3.0          # via pymongo
-docutils==0.18.1          # via myst-parser, recommonmark, sphinx, sphinx-click, sphinx-rtd-theme
-exceptiongroup==1.1.1     # via pytest
-fastapi==0.95.0           # via fastiot (pyproject.toml)
-flask==2.2.3              # via dash, flask-compress
+docutils==0.20.1          # via myst-parser, recommonmark, sphinx, sphinx-click
+exceptiongroup==1.1.1     # via anyio, pytest
+fastapi==0.97.0           # via fastiot (pyproject.toml)
+flask==2.3.2              # via dash, flask-compress
 flask-compress==1.13      # via dash
 frozenlist==1.3.3         # via aiohttp, aiosignal
 h11==0.14.0               # via uvicorn
 httptools==0.5.0          # via uvicorn
 idna==3.4                 # via anyio, requests, yarl
 imagesize==1.4.1          # via sphinx
 influxdb-client[async]==1.36.1  # via fastiot (pyproject.toml)
 iniconfig==2.0.0          # via pytest
 itsdangerous==2.1.2       # via flask
 jinja2==3.1.2             # via fastiot (pyproject.toml), flask, myst-parser, sphinx
 lxml==4.9.2               # via opcua, sphinx-material
-markdown-it-py==2.2.0     # via mdit-py-plugins, myst-parser
-markupsafe==2.1.2         # via jinja2, werkzeug
-mdit-py-plugins==0.3.5    # via myst-parser
+markdown-it-py==3.0.0     # via mdit-py-plugins, myst-parser, rich
+markupsafe==2.1.3         # via jinja2, werkzeug
+mdit-py-plugins==0.4.0    # via myst-parser
 mdurl==0.1.2              # via markdown-it-py
 msgpack==1.0.5            # via fastiot (pyproject.toml)
 multidict==6.0.4          # via aiohttp, yarl
-myst-parser==1.0.0        # via fastiot (pyproject.toml)
-nats-py==2.2.0            # via fastiot (pyproject.toml)
+myst-parser==2.0.0        # via fastiot (pyproject.toml)
+nats-py==2.3.1            # via fastiot (pyproject.toml)
 nest-asyncio==1.5.6       # via fastiot (pyproject.toml)
-nuitka==1.5.3             # via fastiot (pyproject.toml)
-numpy==1.24.2             # via fastiot (pyproject.toml), pandas
+nuitka==1.6.4             # via fastiot (pyproject.toml)
+numpy==1.25.0             # via fastiot (pyproject.toml), pandas
 opcua==0.98.13            # via fastiot (pyproject.toml)
 ordered-set==4.1.0        # via fastiot (pyproject.toml), nuitka
-packaging==23.0           # via build, pytest, sphinx
-pandas==1.5.3             # via fastiot (pyproject.toml)
-pip-tools==6.12.3         # via fastiot (pyproject.toml)
+packaging==23.1           # via build, pytest, sphinx
+pandas==2.0.2             # via fastiot (pyproject.toml)
+pip-tools==6.13.0         # via fastiot (pyproject.toml)
 plotly==5.9.0             # via dash, fastiot (pyproject.toml)
 pluggy==1.0.0             # via pytest
-psycopg2-binary==2.9.5    # via fastiot (pyproject.toml)
+psycopg2-binary==2.9.6    # via fastiot (pyproject.toml)
 pycparser==2.21           # via cffi
-pydantic==1.10.6          # via autodoc-pydantic, fastapi, fastiot (pyproject.toml)
-pygments==2.14.0          # via rich, sphinx
+pydantic==1.10.9          # via autodoc-pydantic, fastapi, fastiot (pyproject.toml)
+pygments==2.15.1          # via rich, sphinx
 pymongo==4.3.3            # via fastiot (pyproject.toml)
-pymysql==1.0.2            # via fastiot (pyproject.toml)
+pymysql==1.0.3            # via fastiot (pyproject.toml)
 pyproject-hooks==1.0.0    # via build
-pytest==7.2.2             # via fastiot (pyproject.toml)
+pytest==7.3.2             # via fastiot (pyproject.toml), pytest-cov
+pytest-cov==4.1.0         # via fastiot (pyproject.toml)
 python-dateutil==2.8.2    # via asyncua, influxdb-client, opcua, pandas
 python-dotenv==1.0.0      # via uvicorn
 python-slugify[unidecode]==8.0.1  # via sphinx-material
-pytz==2022.7.1            # via asyncua, opcua, pandas
+pytz==2023.3              # via asyncua, opcua, pandas
 pyyaml==6.0               # via fastiot (pyproject.toml), myst-parser, uvicorn
 reactivex==4.0.4          # via influxdb-client
 recommonmark==0.7.1       # via fastiot (pyproject.toml)
-redis==4.5.2              # via fastiot (pyproject.toml)
-requests==2.28.2          # via sphinx
-rich==12.6.0              # via typer
+redis==4.5.5              # via fastiot (pyproject.toml)
+requests==2.31.0          # via sphinx
+rich==13.4.2              # via typer
 shellingham==1.5.0.post1  # via typer
 six==1.16.0               # via python-dateutil
 sniffio==1.3.0            # via anyio
 snowballstemmer==2.2.0    # via sphinx
 sortedcontainers==2.4.0   # via asyncua
-soupsieve==2.4            # via beautifulsoup4
-sphinx==6.1.3             # via autodoc-pydantic, fastiot (pyproject.toml), myst-parser, recommonmark, sphinx-autodoc-typehints, sphinx-automodapi, sphinx-click, sphinx-material, sphinx-rtd-theme, sphinxcontrib-jquery
-sphinx-autodoc-typehints==1.22  # via fastiot (pyproject.toml)
+soupsieve==2.4.1          # via beautifulsoup4
+sphinx==7.0.1             # via autodoc-pydantic, fastiot (pyproject.toml), myst-parser, recommonmark, sphinx-autodoc-typehints, sphinx-automodapi, sphinx-click, sphinx-material, sphinx-rtd-theme
+sphinx-autodoc-typehints==1.23.2  # via fastiot (pyproject.toml)
 sphinx-automodapi==0.15.0  # via fastiot (pyproject.toml)
 sphinx-click==4.4.0       # via fastiot (pyproject.toml)
 sphinx-material==0.0.35   # via fastiot (pyproject.toml)
-sphinx-rtd-theme==1.2.0   # via fastiot (pyproject.toml)
+sphinx-rtd-theme==0.5.1   # via fastiot (pyproject.toml)
 sphinxcontrib-applehelp==1.0.4  # via sphinx
 sphinxcontrib-devhelp==1.0.2  # via sphinx
 sphinxcontrib-htmlhelp==2.0.1  # via sphinx
-sphinxcontrib-jquery==4.1  # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1  # via sphinx
 sphinxcontrib-qthelp==1.0.3  # via sphinx
 sphinxcontrib-serializinghtml==1.1.5  # via sphinx
-starlette==0.26.1         # via fastapi
+starlette==0.27.0         # via fastapi
 tenacity==8.2.2           # via plotly
 text-unidecode==1.3       # via python-slugify
-tomli==2.0.1              # via build, fastiot (pyproject.toml), pyproject-hooks, pytest
+tomli==2.0.1              # via build, coverage, fastiot (pyproject.toml), pyproject-hooks, pytest
 tomli-w==1.0.0            # via fastiot (pyproject.toml)
-typer[all]==0.7.0         # via fastiot (pyproject.toml)
-typing-extensions==4.5.0  # via pydantic, reactivex
+typer[all]==0.9.0         # via fastiot (pyproject.toml)
+typing-extensions==4.6.3  # via pydantic, reactivex, typer
+tzdata==2023.3            # via pandas
 unidecode==1.3.6          # via python-slugify
-urllib3==1.26.15          # via influxdb-client, requests
-uvicorn[standard]==0.21.1  # via fastiot (pyproject.toml)
+urllib3==2.0.3            # via influxdb-client, requests
+uvicorn[standard]==0.22.0  # via fastiot (pyproject.toml)
 uvloop==0.17.0            # via uvicorn
-watchfiles==0.18.1        # via uvicorn
-websockets==10.4          # via uvicorn
-werkzeug==2.2.3           # via flask
+watchfiles==0.19.0        # via uvicorn
+websockets==11.0.3        # via uvicorn
+werkzeug==2.3.6           # via flask
 wheel==0.40.0             # via pip-tools
-xlsxwriter==3.0.9         # via fastiot (pyproject.toml)
-yarl==1.8.2               # via aiohttp
-zstandard==0.20.0         # via nuitka
+xlsxwriter==3.1.2         # via fastiot (pyproject.toml)
+yarl==1.9.2               # via aiohttp
+zstandard==0.21.0         # via nuitka
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `fastiot-0.9/requirements/requirements.dash.txt` & `fastiot-1.0/requirements/requirements.dash.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,38 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    fiot config --update-requirements
+#    fiot extras set-requirements --update-requirements
 #
 
-async-timeout==4.0.2      # via redis
+blinker==1.6.2            # via flask
 brotli==1.0.9             # via flask-compress
-build==0.10.0             # via fastiot (pyproject.toml), pip-tools
-click==8.1.3              # via flask, pip-tools, typer
+click==8.1.3              # via flask
 dash==2.6.2               # via dash-bootstrap-components, fastiot (pyproject.toml)
 dash-bootstrap-components==1.4.1  # via fastiot (pyproject.toml)
 dash-core-components==2.0.0  # via dash
 dash-html-components==2.0.0  # via dash
 dash-table==5.0.0         # via dash
 dnspython==2.3.0          # via pymongo
-flask==2.2.3              # via dash, flask-compress
+flask==2.3.2              # via dash, flask-compress
 flask-compress==1.13      # via dash
 itsdangerous==2.1.2       # via flask
-jinja2==3.1.2             # via fastiot (pyproject.toml), flask
-markupsafe==2.1.2         # via jinja2, werkzeug
+jinja2==3.1.2             # via flask
+markupsafe==2.1.3         # via jinja2, werkzeug
 msgpack==1.0.5            # via fastiot (pyproject.toml)
-nats-py==2.2.0            # via fastiot (pyproject.toml)
+nats-py==2.3.1            # via fastiot (pyproject.toml)
 nest-asyncio==1.5.6       # via fastiot (pyproject.toml)
-numpy==1.24.2             # via fastiot (pyproject.toml), pandas
-packaging==23.0           # via build
-pandas==1.5.3             # via fastiot (pyproject.toml)
-pip-tools==6.12.3         # via fastiot (pyproject.toml)
+numpy==1.25.0             # via fastiot (pyproject.toml), pandas
+pandas==2.0.2             # via fastiot (pyproject.toml)
 plotly==5.9.0             # via dash, fastiot (pyproject.toml)
-pydantic==1.10.6          # via fastiot (pyproject.toml)
+pydantic==1.10.9          # via fastiot (pyproject.toml)
 pymongo==4.3.3            # via fastiot (pyproject.toml)
-pyproject-hooks==1.0.0    # via build
 python-dateutil==2.8.2    # via pandas
-pytz==2022.7.1            # via pandas
+pytz==2023.3              # via pandas
 pyyaml==6.0               # via fastiot (pyproject.toml)
-redis==4.5.2              # via fastiot (pyproject.toml)
 six==1.16.0               # via python-dateutil
 tenacity==8.2.2           # via plotly
-tomli==2.0.1              # via build, fastiot (pyproject.toml), pyproject-hooks
-tomli-w==1.0.0            # via fastiot (pyproject.toml)
-typer==0.7.0              # via fastiot (pyproject.toml)
-typing-extensions==4.5.0  # via pydantic
-werkzeug==2.2.3           # via flask
-wheel==0.40.0             # via pip-tools
-xlsxwriter==3.0.9         # via fastiot (pyproject.toml)
-
-# The following packages are considered to be unsafe in a requirements file:
-# pip
-# setuptools
+typing-extensions==4.6.3  # via pydantic
+tzdata==2023.3            # via pandas
+werkzeug==2.3.6           # via flask
+xlsxwriter==3.1.2         # via fastiot (pyproject.toml)
```

### Comparing `fastiot-0.9/requirements/requirements.dev.txt` & `fastiot-1.0/requirements/requirements.dev.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    fiot config --update-requirements
+#    fiot extras set-requirements --update-requirements
 #
 
-async-timeout==4.0.2      # via redis
-attrs==22.2.0             # via pytest
 build==0.10.0             # via fastiot (pyproject.toml), pip-tools
 click==8.1.3              # via pip-tools, typer
 colorama==0.4.6           # via typer
-commonmark==0.9.1         # via rich
+coverage[toml]==7.2.7     # via pytest-cov
 exceptiongroup==1.1.1     # via pytest
 iniconfig==2.0.0          # via pytest
 jinja2==3.1.2             # via fastiot (pyproject.toml)
-markupsafe==2.1.2         # via jinja2
+markdown-it-py==3.0.0     # via rich
+markupsafe==2.1.3         # via jinja2
+mdurl==0.1.2              # via markdown-it-py
 msgpack==1.0.5            # via fastiot (pyproject.toml)
-nats-py==2.2.0            # via fastiot (pyproject.toml)
-packaging==23.0           # via build, pytest
-pip-tools==6.12.3         # via fastiot (pyproject.toml)
+nats-py==2.3.1            # via fastiot (pyproject.toml)
+packaging==23.1           # via build, pytest
+pip-tools==6.13.0         # via fastiot (pyproject.toml)
 pluggy==1.0.0             # via pytest
-pydantic==1.10.6          # via fastiot (pyproject.toml)
-pygments==2.14.0          # via rich
+pydantic==1.10.9          # via fastiot (pyproject.toml)
+pygments==2.15.1          # via rich
 pyproject-hooks==1.0.0    # via build
-pytest==7.2.2             # via fastiot (pyproject.toml)
+pytest==7.3.2             # via fastiot (pyproject.toml), pytest-cov
+pytest-cov==4.1.0         # via fastiot (pyproject.toml)
 pyyaml==6.0               # via fastiot (pyproject.toml)
-redis==4.5.2              # via fastiot (pyproject.toml)
-rich==12.6.0              # via typer
+rich==13.4.2              # via typer
 shellingham==1.5.0.post1  # via typer
-tomli==2.0.1              # via build, fastiot (pyproject.toml), pyproject-hooks, pytest
+tomli==2.0.1              # via build, coverage, fastiot (pyproject.toml), pyproject-hooks, pytest
 tomli-w==1.0.0            # via fastiot (pyproject.toml)
-typer[all]==0.7.0         # via fastiot (pyproject.toml)
-typing-extensions==4.5.0  # via pydantic
+typer[all]==0.9.0         # via fastiot (pyproject.toml)
+typing-extensions==4.6.3  # via pydantic, typer
 wheel==0.40.0             # via pip-tools
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `fastiot-0.9/requirements/requirements.docs.txt` & `fastiot-1.0/requirements/requirements.docs.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,67 +1,53 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    fiot config --update-requirements
+#    fiot extras set-requirements --update-requirements
 #
 
 alabaster==0.7.13         # via sphinx
-async-timeout==4.0.2      # via redis
 autodoc-pydantic==1.8.0   # via fastiot (pyproject.toml)
 babel==2.12.1             # via sphinx
-beautifulsoup4==4.12.0    # via sphinx-material
-build==0.10.0             # via fastiot (pyproject.toml), pip-tools
-certifi==2022.12.7        # via requests
+beautifulsoup4==4.12.2    # via sphinx-material
+certifi==2023.5.7         # via requests
 charset-normalizer==3.1.0  # via requests
-click==8.1.3              # via pip-tools, sphinx-click, typer
+click==8.1.3              # via sphinx-click
 commonmark==0.9.1         # via recommonmark
 css-html-js-minify==2.5.5  # via sphinx-material
-docutils==0.18.1          # via myst-parser, recommonmark, sphinx, sphinx-click, sphinx-rtd-theme
+docutils==0.20.1          # via myst-parser, recommonmark, sphinx, sphinx-click
 idna==3.4                 # via requests
 imagesize==1.4.1          # via sphinx
-jinja2==3.1.2             # via fastiot (pyproject.toml), myst-parser, sphinx
+jinja2==3.1.2             # via myst-parser, sphinx
 lxml==4.9.2               # via sphinx-material
-markdown-it-py==2.2.0     # via mdit-py-plugins, myst-parser
-markupsafe==2.1.2         # via jinja2
-mdit-py-plugins==0.3.5    # via myst-parser
+markdown-it-py==3.0.0     # via mdit-py-plugins, myst-parser
+markupsafe==2.1.3         # via jinja2
+mdit-py-plugins==0.4.0    # via myst-parser
 mdurl==0.1.2              # via markdown-it-py
 msgpack==1.0.5            # via fastiot (pyproject.toml)
-myst-parser==1.0.0        # via fastiot (pyproject.toml)
-nats-py==2.2.0            # via fastiot (pyproject.toml)
-packaging==23.0           # via build, sphinx
-pip-tools==6.12.3         # via fastiot (pyproject.toml)
-pydantic==1.10.6          # via autodoc-pydantic, fastiot (pyproject.toml)
-pygments==2.14.0          # via sphinx
-pyproject-hooks==1.0.0    # via build
+myst-parser==2.0.0        # via fastiot (pyproject.toml)
+nats-py==2.3.1            # via fastiot (pyproject.toml)
+packaging==23.1           # via sphinx
+pydantic==1.10.9          # via autodoc-pydantic, fastiot (pyproject.toml)
+pygments==2.15.1          # via sphinx
 python-slugify[unidecode]==8.0.1  # via sphinx-material
 pyyaml==6.0               # via fastiot (pyproject.toml), myst-parser
 recommonmark==0.7.1       # via fastiot (pyproject.toml)
-redis==4.5.2              # via fastiot (pyproject.toml)
-requests==2.28.2          # via sphinx
+requests==2.31.0          # via sphinx
 snowballstemmer==2.2.0    # via sphinx
-soupsieve==2.4            # via beautifulsoup4
-sphinx==6.1.3             # via autodoc-pydantic, fastiot (pyproject.toml), myst-parser, recommonmark, sphinx-autodoc-typehints, sphinx-automodapi, sphinx-click, sphinx-material, sphinx-rtd-theme, sphinxcontrib-jquery
-sphinx-autodoc-typehints==1.22  # via fastiot (pyproject.toml)
+soupsieve==2.4.1          # via beautifulsoup4
+sphinx==7.0.1             # via autodoc-pydantic, fastiot (pyproject.toml), myst-parser, recommonmark, sphinx-autodoc-typehints, sphinx-automodapi, sphinx-click, sphinx-material, sphinx-rtd-theme
+sphinx-autodoc-typehints==1.23.2  # via fastiot (pyproject.toml)
 sphinx-automodapi==0.15.0  # via fastiot (pyproject.toml)
 sphinx-click==4.4.0       # via fastiot (pyproject.toml)
 sphinx-material==0.0.35   # via fastiot (pyproject.toml)
-sphinx-rtd-theme==1.2.0   # via fastiot (pyproject.toml)
+sphinx-rtd-theme==0.5.1   # via fastiot (pyproject.toml)
 sphinxcontrib-applehelp==1.0.4  # via sphinx
 sphinxcontrib-devhelp==1.0.2  # via sphinx
 sphinxcontrib-htmlhelp==2.0.1  # via sphinx
-sphinxcontrib-jquery==4.1  # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1  # via sphinx
 sphinxcontrib-qthelp==1.0.3  # via sphinx
 sphinxcontrib-serializinghtml==1.1.5  # via sphinx
 text-unidecode==1.3       # via python-slugify
-tomli==2.0.1              # via build, fastiot (pyproject.toml), pyproject-hooks
-tomli-w==1.0.0            # via fastiot (pyproject.toml)
-typer==0.7.0              # via fastiot (pyproject.toml)
-typing-extensions==4.5.0  # via pydantic
+typing-extensions==4.6.3  # via pydantic
 unidecode==1.3.6          # via python-slugify
-urllib3==1.26.15          # via requests
-wheel==0.40.0             # via pip-tools
-
-# The following packages are considered to be unsafe in a requirements file:
-# pip
-# setuptools
+urllib3==2.0.3            # via requests
```

### Comparing `fastiot-0.9/requirements/requirements.fastapi.txt` & `fastiot-1.0/requirements/requirements.fastapi.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,27 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    fiot config --update-requirements
+#    fiot extras set-requirements --update-requirements
 #
 
 aiofiles==23.1.0          # via fastiot (pyproject.toml)
-anyio==3.6.2              # via starlette, watchfiles
-async-timeout==4.0.2      # via redis
-build==0.10.0             # via fastiot (pyproject.toml), pip-tools
-click==8.1.3              # via pip-tools, typer, uvicorn
-fastapi==0.95.0           # via fastiot (pyproject.toml)
+anyio==3.7.0              # via starlette, watchfiles
+click==8.1.3              # via uvicorn
+exceptiongroup==1.1.1     # via anyio
+fastapi==0.97.0           # via fastiot (pyproject.toml)
 h11==0.14.0               # via uvicorn
 httptools==0.5.0          # via uvicorn
 idna==3.4                 # via anyio
-jinja2==3.1.2             # via fastiot (pyproject.toml)
-markupsafe==2.1.2         # via jinja2
 msgpack==1.0.5            # via fastiot (pyproject.toml)
-nats-py==2.2.0            # via fastiot (pyproject.toml)
-packaging==23.0           # via build
-pip-tools==6.12.3         # via fastiot (pyproject.toml)
-pydantic==1.10.6          # via fastapi, fastiot (pyproject.toml)
-pyproject-hooks==1.0.0    # via build
+nats-py==2.3.1            # via fastiot (pyproject.toml)
+pydantic==1.10.9          # via fastapi, fastiot (pyproject.toml)
 python-dotenv==1.0.0      # via uvicorn
 pyyaml==6.0               # via fastiot (pyproject.toml), uvicorn
-redis==4.5.2              # via fastiot (pyproject.toml)
 sniffio==1.3.0            # via anyio
-starlette==0.26.1         # via fastapi
-tomli==2.0.1              # via build, fastiot (pyproject.toml), pyproject-hooks
-tomli-w==1.0.0            # via fastiot (pyproject.toml)
-typer==0.7.0              # via fastiot (pyproject.toml)
-typing-extensions==4.5.0  # via pydantic
-uvicorn[standard]==0.21.1  # via fastiot (pyproject.toml)
+starlette==0.27.0         # via fastapi
+typing-extensions==4.6.3  # via pydantic
+uvicorn[standard]==0.22.0  # via fastiot (pyproject.toml)
 uvloop==0.17.0            # via uvicorn
-watchfiles==0.18.1        # via uvicorn
-websockets==10.4          # via uvicorn
-wheel==0.40.0             # via pip-tools
-
-# The following packages are considered to be unsafe in a requirements file:
-# pip
-# setuptools
+watchfiles==0.19.0        # via uvicorn
+websockets==11.0.3        # via uvicorn
```

### Comparing `fastiot-0.9/requirements/requirements.influxdb.txt` & `fastiot-1.0/requirements/requirements.influxdb.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,31 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    fiot config --update-requirements
+#    fiot extras set-requirements --update-requirements
 #
 
-aiocsv==1.2.3             # via influxdb-client
+aiocsv==1.2.4             # via influxdb-client
 aiohttp==3.8.4            # via influxdb-client
 aiosignal==1.3.1          # via aiohttp
-async-timeout==4.0.2      # via aiohttp, redis
-attrs==22.2.0             # via aiohttp
-build==0.10.0             # via fastiot (pyproject.toml), pip-tools
-certifi==2022.12.7        # via influxdb-client
+async-timeout==4.0.2      # via aiohttp
+attrs==23.1.0             # via aiohttp
+certifi==2023.5.7         # via influxdb-client
 charset-normalizer==3.1.0  # via aiohttp
-click==8.1.3              # via pip-tools, typer
 frozenlist==1.3.3         # via aiohttp, aiosignal
 idna==3.4                 # via yarl
 influxdb-client[async]==1.36.1  # via fastiot (pyproject.toml)
-jinja2==3.1.2             # via fastiot (pyproject.toml)
-markupsafe==2.1.2         # via jinja2
 msgpack==1.0.5            # via fastiot (pyproject.toml)
 multidict==6.0.4          # via aiohttp, yarl
-nats-py==2.2.0            # via fastiot (pyproject.toml)
-packaging==23.0           # via build
-pip-tools==6.12.3         # via fastiot (pyproject.toml)
-pydantic==1.10.6          # via fastiot (pyproject.toml)
-pyproject-hooks==1.0.0    # via build
+nats-py==2.3.1            # via fastiot (pyproject.toml)
+pydantic==1.10.9          # via fastiot (pyproject.toml)
 python-dateutil==2.8.2    # via influxdb-client
 pyyaml==6.0               # via fastiot (pyproject.toml)
 reactivex==4.0.4          # via influxdb-client
-redis==4.5.2              # via fastiot (pyproject.toml)
 six==1.16.0               # via python-dateutil
-tomli==2.0.1              # via build, fastiot (pyproject.toml), pyproject-hooks
-tomli-w==1.0.0            # via fastiot (pyproject.toml)
-typer==0.7.0              # via fastiot (pyproject.toml)
-typing-extensions==4.5.0  # via pydantic, reactivex
-urllib3==1.26.15          # via influxdb-client
-wheel==0.40.0             # via pip-tools
-yarl==1.8.2               # via aiohttp
+typing-extensions==4.6.3  # via pydantic, reactivex
+urllib3==2.0.3            # via influxdb-client
+yarl==1.9.2               # via aiohttp
 
 # The following packages are considered to be unsafe in a requirements file:
-# pip
 # setuptools
```

### Comparing `fastiot-0.9/requirements/requirements.opcua.txt` & `fastiot-1.0/requirements/requirements.opcua.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,24 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    fiot config --update-requirements
+#    fiot extras set-requirements --update-requirements
 #
 
 aiofiles==23.1.0          # via asyncua
-aiosqlite==0.18.0         # via asyncua
-async-timeout==4.0.2      # via redis
-asyncua==1.0.1            # via fastiot (pyproject.toml)
-build==0.10.0             # via fastiot (pyproject.toml), pip-tools
+aiosqlite==0.19.0         # via asyncua
+asyncua==1.0.2            # via fastiot (pyproject.toml)
 cffi==1.15.1              # via cryptography
-click==8.1.3              # via pip-tools, typer
-cryptography==39.0.2      # via asyncua
-jinja2==3.1.2             # via fastiot (pyproject.toml)
+cryptography==41.0.1      # via asyncua
 lxml==4.9.2               # via opcua
-markupsafe==2.1.2         # via jinja2
 msgpack==1.0.5            # via fastiot (pyproject.toml)
-nats-py==2.2.0            # via fastiot (pyproject.toml)
+nats-py==2.3.1            # via fastiot (pyproject.toml)
 opcua==0.98.13            # via fastiot (pyproject.toml)
-packaging==23.0           # via build
-pip-tools==6.12.3         # via fastiot (pyproject.toml)
 pycparser==2.21           # via cffi
-pydantic==1.10.6          # via fastiot (pyproject.toml)
-pyproject-hooks==1.0.0    # via build
+pydantic==1.10.9          # via fastiot (pyproject.toml)
 python-dateutil==2.8.2    # via asyncua, opcua
-pytz==2022.7.1            # via asyncua, opcua
+pytz==2023.3              # via asyncua, opcua
 pyyaml==6.0               # via fastiot (pyproject.toml)
-redis==4.5.2              # via fastiot (pyproject.toml)
 six==1.16.0               # via python-dateutil
 sortedcontainers==2.4.0   # via asyncua
-tomli==2.0.1              # via build, fastiot (pyproject.toml), pyproject-hooks
-tomli-w==1.0.0            # via fastiot (pyproject.toml)
-typer==0.7.0              # via fastiot (pyproject.toml)
-typing-extensions==4.5.0  # via pydantic
-wheel==0.40.0             # via pip-tools
-
-# The following packages are considered to be unsafe in a requirements file:
-# pip
-# setuptools
+typing-extensions==4.6.3  # via pydantic
```

### Comparing `fastiot-0.9/src/fastiot/cli/commands/build.py` & `fastiot-1.0/src/fastiot/cli/commands/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,17 @@
 
 def _create_all_docker_files(context: ProjectContext, services: Optional[List[str]] = None):
     for service in context.services:
         if services is None or service.name in services:
             _create_docker_file(service, context)
 
 
+
+
+
 def _create_docker_file(service: Service, context: ProjectContext):
     build_dir = os.path.join(context.project_root_dir, context.build_dir, DOCKER_BUILD_DIR)
     os.makedirs(build_dir, exist_ok=True)
 
     docker_filename = os.path.join(build_dir, 'Dockerfile.' + service.name)
 
     service_own_dockerfile = os.path.join(context.project_root_dir, 'src',
@@ -135,26 +138,27 @@
     if os.path.isfile(service_own_dockerfile):
         logging.debug("Using dockerfile from %s, not creating a new one", service.name)
         copyfile(service_own_dockerfile, docker_filename)
         return
 
     base_requirements_file = _set_requirements_file(context)
 
+    service.maintainer = _get_maintainer()
+    service.git_revision = _get_git_revision()
+
     with open(docker_filename, "w") as dockerfile:
         manifest = service.read_manifest()
         template = DockerTemplate.get(manifest.template)
         dockerfile_template = get_jinja_env(template_dir=template.dir).get_template(template.filename)
         dockerfile.write(dockerfile_template.render(service=service,
                                                     manifest=manifest,
                                                     context=context,
                                                     base_requirements_file=base_requirements_file,
                                                     extra_pypi=os.environ.get('FASTIOT_EXTRA_PYPI',
-                                                                              "www.piwheels.org/simple/"),
-                                                    maintainer=_get_maintainer()
-                                                    )
+                                                                              "www.piwheels.org/simple/"))
                          )
 
 
 def _set_requirements_file(context):
     if os.path.isfile(os.path.join(context.project_root_dir, 'requirements.txt')):
         base_requirements_file = 'requirements.txt'
     elif os.path.isfile(os.path.join(context.project_root_dir, 'requirements', 'requirements.txt')):
@@ -185,14 +189,21 @@
         author, mail = re.search("^Author: (.*) (<.*@.*>)$", git_log, re.MULTILINE).groups()
         maintainer = f"{author} using FastIoT {mail}"
     except (AttributeError, TypeError):
         maintainer = "FastIoT Framework <none@none>"
 
     return maintainer
 
+def _get_git_revision() -> str:
+    cmd = "git rev-parse HEAD"
+    try:
+        revision = subprocess.getoutput(cmd)
+    except (AttributeError, TypeError):
+        revision = ""
+    return revision
 
 def _docker_bake(context: ProjectContext,
                  tags: List[str],
                  build_mode: str,
                  services: Optional[List[str]] = None,
                  dry: bool = False,
                  platform: str = '',
```

### Comparing `fastiot-0.9/src/fastiot/cli/commands/build_lib.py` & `fastiot-1.0/src/fastiot/cli/commands/build_lib.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/commands/clean.py` & `fastiot-1.0/src/fastiot/cli/commands/clean.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/commands/config.py` & `fastiot-1.0/src/fastiot/cli/commands/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from fastiot.cli.model.compose_info import ServiceComposeInfo
 from fastiot.cli.model.infrastructure_service import InfrastructureService
 from fastiot.cli.model.manifest import MountConfigDirEnum
 from fastiot.cli.model.project import ProjectContext
 from fastiot.cli.typer_app import app, DEFAULT_CONTEXT_SETTINGS
 from fastiot.env import env_basic
 from fastiot.env.env_constants_basic import FASTIOT_CONFIG_DIR, FASTIOT_VOLUME_DIR
+from fastiot.util.ports import get_local_random_port
 
 
 @app.command(context_settings=DEFAULT_CONTEXT_SETTINGS)
 def config(deployments: Optional[List[str]] = typer.Argument(default=None,
                                                              shell_complete=_deployment_completion,
                                                              help="The deployment configs to generate. "
                                                                   "Default: all configs"),
@@ -84,79 +85,81 @@
         deployments = [context.integration_test_deployment]
 
     if deployments:
         deployment_names = _apply_checks_for_deployment_names(deployments=deployments)
     else:
         deployment_names = context.deployment_names
 
-    # This will set environment variables for externally opened ports, usually to be used for integration tests but also
-    # to access the services externally. When creating the compose infos for infrastructure services the env vars will
-    # be used, so no further access to the settings is needed.
-    if port_offset is None:
-        infrastructure_ports = {}
-    elif port_offset == 0:
-        infrastructure_ports = get_infrastructure_service_ports_randomly()
-    else:
-        infrastructure_ports = get_infrastructure_service_ports_monotonically_increasing(offset=port_offset)
-
-    if not isinstance(net, str):  # Workaround for https://github.com/tiangolo/typer/issues/106
-        net = net.default
-
     for deployment_name in deployment_names:
-        if use_port_import:  # We read in any previously set ports for the deployment in the build dir
-            temp_build_env = context.build_env_for_deployment(deployment_name)
-            for key, value in [(k, v) for k, v in temp_build_env.items() if k in infrastructure_ports]:
-                infrastructure_ports[key] = int(value)
 
         deployment_build_dir = context.deployment_build_dir(name=deployment_name)
         shutil.rmtree(deployment_build_dir, ignore_errors=True)
         os.makedirs(deployment_build_dir, exist_ok=True)
 
         env = context.env_for_deployment(name=deployment_name)
         deployment_config = context.deployment_by_name(name=deployment_name)
         env_additions = {}
         env_service_internal_modifications = {}
         infrastructure_services = _create_infrastructure_service_compose_infos(
             env=env,
             env_additions=env_additions,
             env_service_internal_modifications=env_service_internal_modifications,
-            infrastructure_ports=infrastructure_ports,
             deployment_config=deployment_config,
             is_integration_test_deployment=deployment_name == context.integration_test_deployment,
-            project_namespace=context.project_namespace
+            project_namespace=context.project_namespace,
+            port_offset=port_offset, use_port_import=use_port_import,
+            deployment_name=deployment_name
         )
+
+        local_port_offset = port_offset
+        if port_offset and port_offset > 0:  # Detect the highest used port as offset for our own services
+            for service in infrastructure_services:
+                for port in service.ports:
+                    port = int(port.split(':', 1)[0])
+                    port_offset = port + 1 if port > port_offset else port_offset
+
         services = _create_services_compose_infos(
             env=env,
             env_additions=env_additions,
+            env_service_internal_modifications=env_service_internal_modifications,
             deployment_config=deployment_config,
             docker_registry=docker_registry,
             tag=tag,
-            pull_always=pull_always
+            pull_always=pull_always,
+            local_port_offset=local_port_offset,
+            use_port_import=use_port_import
         )
 
         if deployment_config.config_dir and FASTIOT_CONFIG_DIR not in env:
             env_additions[FASTIOT_CONFIG_DIR] = os.path.join(context.deployment_dir(name=deployment_name),
                                                              deployment_config.config_dir)
 
         # Adjust relative paths in env_additions
         for key, value in env_additions.items():
             if value.startswith('./'):
                 env_additions[key] = os.path.join(context.deployment_dir(name=deployment_name), value)
 
 
+        # Collect additional, external docker networks
+        external_networks = []
+        for service in services:
+            external_networks += service.extra_networks
+
         shutil.copytree(context.deployment_dir(name=deployment_name), deployment_build_dir, dirs_exist_ok=True,
                         ignore=lambda _, __: ['deployment.yaml', '.env'])
 
         with open(os.path.join(deployment_build_dir, 'docker-compose.yaml'), "w") as docker_compose_file:
             docker_compose_template = get_jinja_env().get_template('docker-compose.yaml.j2')
             docker_compose_file.write(docker_compose_template.render(
                 docker_net_name=net,
                 environment_for_docker_compose_file=env_service_internal_modifications,
                 services=services + infrastructure_services,
-                env_file=env or env_additions
+                env_file=env or env_additions,
+                deployment_config=deployment_config,
+                external_networks=external_networks
             ))
 
         env_filename = context.env_file_for_deployment(name=deployment_name)
         env_file_content = ""
         if os.path.exists(env_filename):
             with open(env_filename, "r") as env_file:
                 env_file_content = env_file.read()
@@ -177,14 +180,16 @@
             if env_additions:
                 env_file.write("\n# The following content has been injected via fastiot cli:\n")
                 for key, value in env_additions.items():
                     env_file.write(f"\n{key}={value}")
                 env_file.write("\n")  # ending files with '\n' as it is a best practice for file management under linux
 
     logging.info("Successfully created configurations!")
+    logging.info("If you need to interact directly with any ports of services please have a look at the .env file in "
+                 "the directory builds/{deployment}.")
 
 
 def _apply_checks_for_deployment_names(deployments: List[str]) -> List[str]:
     context = ProjectContext.default
     if deployments:
         deployment_names = []
         for deployment in deployments:
@@ -195,44 +200,50 @@
     else:
         deployment_names = context.deployment_names
     return deployment_names
 
 
 def _create_services_compose_infos(env: Dict[str, str],
                                    env_additions: Dict[str, str],
+                                   env_service_internal_modifications: Dict[str, str],
                                    deployment_config: DeploymentConfig,
                                    docker_registry: str,
                                    tag: str,
-                                   pull_always: bool
+                                   pull_always: bool,
+                                   local_port_offset, use_port_import
                                    ) -> List[ServiceComposeInfo]:
     context: ProjectContext = ProjectContext.default
     result = []
     for name, service_config in deployment_config.services.items():
         if service_config is None:
             # This can only be the case for internal services as external ones need to define the image
             # We set the tag here for internal services.
             service_config = ServiceConfig(image=f"{context.project_namespace}/{name}", tag=tag)
 
         full_image_name = _get_full_image_name(deployment_config, docker_registry, service_config)
         manifest = _get_service_manifest(name, image_name=full_image_name, pull_always=pull_always)
 
         service_env = {**service_config.environment}
         volumes = _create_volumes(env, env_additions, service_env, deployment_config.config_dir, manifest)
-        ports = _create_ports(env, service_env, manifest)
+        ports = _create_ports(env, env_additions, env_service_internal_modifications, manifest,
+                              local_port_offset=local_port_offset, use_port_import=use_port_import,
+                              deployment_name=deployment_config.name)
         devices = _create_devices(env, service_env, manifest)
         extras = _create_compose_extras(manifest)
 
         result.append(ServiceComposeInfo(name=name,
                                          image=full_image_name,
                                          environment=service_env,
                                          ports=ports,
                                          volumes=volumes,
                                          devices=devices,
                                          privileged=manifest.privileged,
-                                         extras=extras))
+                                         extras=extras,
+                                         labels=service_config.labels,
+                                         extra_networks=service_config.extra_networks))
     return result
 
 
 def _get_full_image_name(deployment_config: DeploymentConfig,
                          docker_registry: str,
                          service_config: ServiceConfig):
     if service_config.docker_registry:
@@ -266,20 +277,43 @@
         service = context.get_service_by_name(service_name)
         return service.read_manifest(check_service_name=service_name)
 
     # No local service => Import from docker image
     return ServiceManifest.from_docker_image(image_name, pull_always=pull_always)
 
 
-def _create_ports(env: Dict[str, str], service_env: Dict[str, str], manifest: ServiceManifest) -> List[str]:
+def _create_ports(env: Dict[str, str], env_additions: Dict[str, str],
+                  env_service_internal_modifications: Dict[str, str], manifest: ServiceManifest,
+                  local_port_offset: Optional[int], use_port_import: bool,
+                  deployment_name: str
+                  ) -> List[str]:
+    context: ProjectContext = ProjectContext.default
+    build_env = context.build_env_for_deployment(deployment_name)
+
     ports = []
-    for port in manifest.ports:
-        external_port = int(env.get(port.env_variable, str(port.port)))
-        ports.append(f"{external_port}:{external_port}")
-        service_env[port.env_variable] = str(external_port)
+    for i, port in enumerate(manifest.ports):
+
+        if local_port_offset is None:  # Nothing has been defined, use default port for service
+            external_port = port.port
+        elif local_port_offset == 0:
+            external_port = get_local_random_port()
+        else:
+            external_port = local_port_offset + i
+
+        if use_port_import:  # If defined lookup already defined port in build dir
+            external_port = build_env.get(port.env_variable, external_port)
+
+        # Highest priority for ports the user has manually taken care of and defined it in his environment
+        external_port = env.get(port.env_variable, external_port)
+
+        env_service_internal_modifications[port.env_variable] = str(port.port)
+        env_additions[port.env_variable] = str(external_port)
+
+        ports.append(f"{external_port}:{port.port}")
+
     return ports
 
 
 def _create_volumes(env: Dict[str, str], env_additions: Dict[str, str], service_env: Dict[str, str],
                     config_dir: str, manifest: ServiceManifest) -> List[str]:
     volumes = []
     for volume in manifest.volumes:
@@ -317,22 +351,24 @@
         return yaml.dump(manifest.compose_extras).rstrip()
     return ""
 
 
 def _create_infrastructure_service_compose_infos(env: Dict[str, str],
                                                  env_additions: Dict[str, str],
                                                  env_service_internal_modifications: Dict[str, str],
-                                                 infrastructure_ports: Dict[str, int],
                                                  deployment_config: DeploymentConfig,
                                                  is_integration_test_deployment: bool,
-                                                 project_namespace: str
+                                                 project_namespace: str,
+                                                 port_offset, use_port_import, deployment_name
                                                  ) -> List[ServiceComposeInfo]:
     services_map = InfrastructureService.all
     result = []
 
+    infrastructure_ports = _set_infrastructure_ports(deployment_name, port_offset, use_port_import)
+
     for name, infrastructure_service_config in deployment_config.infrastructure_services.items():
 
         if name not in services_map:
             raise RuntimeError(f"Service with name '{name}' was not found in service list: {', '.join(services_map)}")
         service = services_map[name]
 
         if infrastructure_service_config.external is True:
@@ -353,16 +389,16 @@
             else:
                 value = env_var.default
             service_environment[env_var.name] = value
 
         service_ports: List[str] = []
         for port in service.ports:
             if port.env_var:
-                value = env.get(port.env_var, str(port.default_port_mount))
-                value = str(infrastructure_ports.get(port.env_var, value))
+                value = infrastructure_ports.get(port.env_var, str(port.default_port_mount))
+                value = str(env.get(port.env_var, value))
             else:
                 value = str(port.default_port_mount)
             if port.env_var not in env:
                 env_additions[port.env_var] = value
 
             env_service_internal_modifications[port.env_var] = str(port.container_port)
             service_ports.append(f'{value}:{port.container_port}')
@@ -409,7 +445,29 @@
             environment=service_environment,
             ports=service_ports,
             volumes=service_volumes,
             tmpfs=service_temp_volumes,
             extras=service_extensions
         ))
     return result
+
+
+def _set_infrastructure_ports(deployment_name, port_offset, use_port_import):
+
+    context: ProjectContext = ProjectContext.default
+
+
+    # This will set environment variables for externally opened ports, usually to be used for integration tests but also
+    # to access the services externally. When creating the compose infos for infrastructure services the env vars will
+    # be used, so no further access to the settings is needed.
+    if port_offset is None:
+        infrastructure_ports = {}
+    elif port_offset == 0:
+        infrastructure_ports = get_infrastructure_service_ports_randomly()
+    else:
+        infrastructure_ports = get_infrastructure_service_ports_monotonically_increasing(offset=port_offset)
+
+    if use_port_import:  # We read in any previously set ports for the deployment in the build dir
+        temp_build_env = context.build_env_for_deployment(deployment_name)
+        for key, value in [(k, v) for k, v in temp_build_env.items() if k in infrastructure_ports]:
+            infrastructure_ports[key] = int(value)
+    return infrastructure_ports
```

### Comparing `fastiot-0.9/src/fastiot/cli/commands/create.py` & `fastiot-1.0/src/fastiot/cli/commands/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,14 +223,15 @@
 def _find_service_package(project_config, service_package):
     """
     Find *the* package to place the service if not defined. Raise errors when no or to many packages are possible.
     """
     service_package_list = []
     for package in os.listdir(os.path.join(project_config.project_root_dir, "src")):
         if package != project_config.library_package and package != project_config.test_package and \
+                package != '__pycache__' and \
                 os.path.isdir(os.path.join(project_config.project_root_dir, 'src', package)):
             service_package_list.append(package)
     if len(service_package_list) == 0:
         logging.error("No service package found in project to place the service.")
         raise typer.Exit(4)
     # nothing given
     if not service_package and len(service_package_list) > 1:
```

### Comparing `fastiot-0.9/src/fastiot/cli/commands/deploy.py` & `fastiot-1.0/src/fastiot/cli/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/commands/manage_requirements.py` & `fastiot-1.0/src/fastiot/cli/commands/manage_requirements.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     # Base
     _run_pip_compile(file_name=os.path.join(context.project_root_dir, 'requirements.txt'),
                      upgrade=update_requirements, name='base')
 
     with open(pyproject_toml, "rb") as toml_file:
         toml_dict = tomli.load(toml_file)
 
-    if 'optional-dependencies' in toml_dict['project']:
+    if 'optional-dependencies' in toml_dict['project'] and toml_dict['project']['optional-dependencies']:
         os.makedirs(os.path.join(context.project_root_dir, 'requirements'), exist_ok=True)
         for extra_dep in toml_dict['project']['optional-dependencies'].keys():
             target_file = os.path.join(context.project_root_dir, 'requirements', f"requirements.{extra_dep}.txt")
             _run_pip_compile(file_name=target_file, cmd_extras=f"--extra={extra_dep}",
                              upgrade=update_requirements, name=extra_dep)
 
         target_file = os.path.join(context.project_root_dir, 'requirements', "requirements.all.txt")
@@ -71,12 +71,13 @@
     # Do some cleanup on the generated requirements file to avoid information leakage
     with open(file_name, 'r') as file:
         text = file.readlines()
 
     with open(file_name, "w") as file:
         for line in text:
             if "pip-compile --" in line or "pip-compile -" in line:
-                file.write("#    fiot config" + " --update-requirements\n" if upgrade else "\n")
+                file.write("#    fiot extras set-requirements")
+                file.write(" --update-requirements\n" if upgrade else "\n")
             elif "extra-index-url" in line or "trusted-host" in line:
                 continue
             else:
                 file.write(line)
```

### Comparing `fastiot-0.9/src/fastiot/cli/commands/nuitka_compile.py` & `fastiot-1.0/src/fastiot/cli/commands/nuitka_compile.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/commands/print.py` & `fastiot-1.0/src/fastiot/cli/commands/print.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/commands/run_tests.py` & `fastiot-1.0/src/fastiot/cli/commands/run_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         from fastiot.cli.commands.config import config  # pylint: disable=import-outside-toplevel
 
         logging.warning("No generated configuration could found in build/%s.\n"
                         "\tRunning config command to create one now.", context.test_package)
         config(use_test_deployment=True, port_offset=0)
 
     if start_deployment:
-        start(use_test_deployment=True, detach=True, project_name=None, service_names=None)
+        start(use_test_deployment=True, detach=True, project_name="", service_names=None)
 
     env = os.environ.copy()
     src_dir = os.path.join(context.project_root_dir, 'src')
     env['PYTHONPATH'] = src_dir
     cmd = _get_command_for_test_runner(test_runner=test_runner, src_dir=src_dir)
 
     exit_code = subprocess.call(cmd.split(),
```

### Comparing `fastiot-0.9/src/fastiot/cli/commands/start.py` & `fastiot-1.0/src/fastiot/cli/commands/start.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,30 +44,34 @@
             logging.warning("You have not configured any integration_test_deployment in your configure.py. Exiting.")
             raise typer.Exit(0)
 
     if deployment_name is None:
         logging.error("You have to define an environment to start or use the optional --use-test-deployment!")
         raise typer.Exit(-1)
 
+    cwd = os.path.join(context.project_root_dir, context.build_dir, DEPLOYMENTS_CONFIG_DIR,
+                       deployment_name)
+
     cmd = ["docker-compose"]
     project_name = project_name or getpass.getuser() + "__" + context.project_namespace + "__" + deployment_name
     cmd.append("--project-name=" + project_name)
 
+    if pull_always:
+        pull_cmd = cmd + ["pull"]
+        exit_code = subprocess.call(pull_cmd, cwd=cwd)
+        if exit_code != 0:
+            logging.warning("Pulling images was not successful. Trying to continue.")
+
     cmd.append("up")
     if detach:
         cmd.append("-d")
 
-    if pull_always:
-        cmd += ['--pull', 'always']
-
     if service_names is not None:
         cmd += service_names
 
-    cwd = os.path.join(context.project_root_dir, context.build_dir, DEPLOYMENTS_CONFIG_DIR,
-                       deployment_name)
     logging.debug("Running command to start the environment: %s", " ".join(cmd))
     os.environ['COMPOSE_HTTP_TIMEOUT'] = '300'
     exit_code = 0
     try:
         exit_code = subprocess.call(cmd, cwd=cwd)
     except KeyboardInterrupt:
         if not detach:
```

### Comparing `fastiot-0.9/src/fastiot/cli/commands/stop.py` & `fastiot-1.0/src/fastiot/cli/commands/stop.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/commands/version.py` & `fastiot-1.0/src/fastiot/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/common/infrastructure_services.py` & `fastiot-1.0/src/fastiot/cli/common/infrastructure_services.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 from typing import List
 
 from fastiot.cli.model.infrastructure_service import InfrastructureService, InfrastructureServicePort, \
     InfrastructureServiceEnvVar, InfrastructureServiceVolume, InfrastructureServiceComposeExtras
 from fastiot.env.env_constants_basic import FASTIOT_NATS_HOST, FASTIOT_NATS_PORT
 from fastiot.env.env_constants_db import FASTIOT_TIME_SCALE_DB_VOLUME, FASTIOT_REDIS_VOLUME, FASTIOT_MONGO_DB_VOLUME, \
     FASTIOT_MARIA_DB_VOLUME, FASTIOT_MARIA_DB_ENTRY, FASTIOT_INFLUX_DB_MODE, FASTIOT_INFLUX_DB_VOLUME, \
-    FASTIOT_ELASTICSEARCH_HOST, FASTIOT_ELASTICSEARCH_PORT, FASTIOT_ELASTICSEARCH_PASSWORD, \
-    FASTIOT_ELASTICSEARCH_VOLUME, FASTIOT_TIME_SCALE_DB_HOST, FASTIOT_TIME_SCALE_DB_PORT, FASTIOT_TIME_SCALE_DB_USER, \
+    FASTIOT_TIME_SCALE_DB_HOST, FASTIOT_TIME_SCALE_DB_PORT, FASTIOT_TIME_SCALE_DB_USER, \
     FASTIOT_TIME_SCALE_DB_PASSWORD, FASTIOT_TIME_SCALE_DB_DATABASE, FASTIOT_REDIS_HOST, FASTIOT_REDIS_PORT, \
     FASTIOT_REDIS_PASSWORD, FASTIOT_MONGO_DB_HOST, FASTIOT_MONGO_DB_PORT, FASTIOT_MONGO_DB_USER, \
     FASTIOT_MONGO_DB_PASSWORD, FASTIOT_MONGO_DB_MEM_LIMIT, FASTIOT_MARIA_DB_HOST, FASTIOT_MARIA_DB_PORT, \
     FASTIOT_MARIA_DB_USER, FASTIOT_MARIA_DB_PASSWORD, FASTIOT_INFLUX_DB_HOST, FASTIOT_INFLUX_DB_PORT, \
     FASTIOT_INFLUX_DB_USER, FASTIOT_INFLUX_DB_PASSWORD, FASTIOT_INFLUX_DB_ORG, FASTIOT_INFLUX_DB_BUCKET, \
     FASTIOT_INFLUX_DB_TOKEN
 
@@ -296,53 +295,7 @@
         InfrastructureServiceVolume(
             container_volume='/data',
             env_var=FASTIOT_REDIS_VOLUME
         )
     ]
 
 
-class ElasticSearch(InfrastructureService):
-    """
-    Definition of an ElasticDB Service
-    """
-    name: str = 'elasticsearch'
-    image: str = 'docker.elastic.co/elasticsearch/elasticsearch:7.17.8'
-
-    host_name_env_var = FASTIOT_ELASTICSEARCH_HOST
-    password_env_vars: List[str] = [FASTIOT_ELASTICSEARCH_PASSWORD]
-
-    ports: List[InfrastructureServicePort] = [
-        InfrastructureServicePort(
-            container_port=9200,
-            default_port_mount=9200,
-            env_var=FASTIOT_ELASTICSEARCH_PORT
-        )
-    ]
-    environment: List[InfrastructureServiceEnvVar] = [
-        InfrastructureServiceEnvVar(
-            name='ELASTIC_PASSWORD',
-            default='12345',
-            env_var=FASTIOT_ELASTICSEARCH_PASSWORD
-        ),
-        InfrastructureServiceEnvVar(
-            name='ES_JAVA_OPTS',
-            default='-Xmx256m -Xms256m',
-        ),
-        InfrastructureServiceEnvVar(
-            name='discovery.type',
-            default='single-node',
-        ),
-        InfrastructureServiceEnvVar(
-            name='cluster.name',
-            default='single-node-cluster',
-        ),
-        InfrastructureServiceEnvVar(
-            name='network.host',
-            default='0.0.0.0',
-        ),
-    ]
-    volumes: List[InfrastructureServiceVolume] = [
-        InfrastructureServiceVolume(
-            container_volume='/usr/share/elasticsearch/data',
-            env_var=FASTIOT_ELASTICSEARCH_VOLUME
-        )
-    ]
```

### Comparing `fastiot-0.9/src/fastiot/cli/constants.py` & `fastiot-1.0/src/fastiot/cli/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 CONFIG_KEY_EXTENSIONS = "extensions"
 # Base image used to build docker files if not defined otherwise in the manifest
 # Please note that we use buster instead of bullseye because it results in libc-bin segfaults on certain architectures
 # sometimes. See also: https://github.com/docker/buildx/issues/314
-DEFAULT_BASE_IMAGE = "python:3.10-slim-bullseye"
+DEFAULT_BASE_IMAGE = "python:3.10-slim-bookworm"
 CONFIGURE_FILE_NAME = "configure.py"
 DEPLOYMENTS_CONFIG_DIR = 'deployments'
 DEPLOYMENTS_CONFIG_FILE = 'deployment.yaml'
 MANIFEST_FILENAME = 'manifest.yaml'
 DOCKER_BUILD_DIR = 'docker'
 IMPORT_NAME_CONFIGURE_PY = 'fastiot_configure'
 BUILDER_NAME = 'fastiot_builder'
```

### Comparing `fastiot-0.9/src/fastiot/cli/fiot.py` & `fastiot-1.0/src/fastiot/cli/fiot.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/helper_fn.py` & `fastiot-1.0/src/fastiot/cli/helper_fn.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import glob
+import logging
 import os
 from pathlib import Path
 from typing import Dict, List, Optional
 
-from jinja2 import Environment, FileSystemLoader, StrictUndefined
+try:
+    from jinja2 import Environment, FileSystemLoader, StrictUndefined
+
+
+except ImportError:
+    logging.debug("Could not import Jinja. To use the CLI you need to install `fastiot[dev]`.")
+    # This warning should more present when starting the CLI, so just set this to debugging output.
+    Environment, FileSystemLoader, StrictUndefined = None, None, None
 
 from fastiot.cli.constants import DEPLOYMENTS_CONFIG_DIR, DEPLOYMENTS_CONFIG_FILE, MANIFEST_FILENAME, TEMPLATES_DIR
 from fastiot.cli.model import Service, DeploymentConfig
 
 _jinja_envs: Dict[str, Environment] = {}
 
 
@@ -24,15 +32,15 @@
 
 def find_services(package: Optional[str] = None,
                   path: Optional[str] = None,
                   services: Optional[List[str]] = None) -> List[Service]:
     """
     Find services in a package
 
-    :param package: The package name within your :file:`src`. If not defined the whole :path:`src` will be searched for
+    :param package: The package name within your :file:`src`. If not defined the whole :file:`src` will be searched for
                     suitable services containing a :file:`manifest.yaml` and a :file:`run.py`
     :param path: Optional, specify a search path, uses ``os.getcwd()`` as default
     :param services: Optional; if specified it will only include the listed services
     """
     path = path or os.getcwd()
     package = package or '*'
```

### Comparing `fastiot-0.9/src/fastiot/cli/import_configure.py` & `fastiot-1.0/src/fastiot/cli/import_configure.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/infrastructure_service_fn.py` & `fastiot-1.0/src/fastiot/cli/infrastructure_service_fn.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from fastiot.util.ports import get_local_random_port
 
 
 def get_infrastructure_service_ports_randomly() -> Dict[str, int]:
     """
     Get random environment variables for all ports.
 
-    On very busy machines this may to reuse of ports, if another service takes the port betweening determining its free
-    status and acutally starting the service.
+    On very busy machines this may to reuse of ports, if another service takes the port between determining its free
+    status and actually starting the service.
 
     :return: dict with the environment variables and the corresponding port numbers
     """
     ports = {}
     for service in InfrastructureService.all.values():
         for port in service.ports:
             ports[port.env_var] = get_local_random_port()
```

### Comparing `fastiot-0.9/src/fastiot/cli/model/__init__.py` & `fastiot-1.0/src/fastiot/cli/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/model/deployment.py` & `fastiot-1.0/src/fastiot/cli/model/deployment.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,18 @@
     docker_registry: str = ''
     """ The specified docker registry. If given it will override the docker_registry for the service, otherwise the
     locally  configured docker registry will be used."""
     tag: str = ''
     """ The specified tag. If given it will override the tag for the service """
     environment: Dict[str, str] = {}
     """ Includes all environment variables specifically for this service """
-
+    labels: list = []
+    """ Provide any docker labels like needed for Traefik """
+    extra_networks: list = []
+    """Hook this service to an external docker network by e.g. another deployment on the same host."""
 
 class AnsibleHost(BaseModel):
     """
     Represents a host for Ansible based deployments, used by
     :class:`fastiot.cli.models.deployment.DeploymentTargetSetup`
     """
     ip: str
@@ -58,14 +61,28 @@
     remote_user: Optional[str] = 'ubuntu'
     """ The remote user to use to logins for all hosts, defaults to ``ubuntu``"""
     link_prometheus: bool = False
     """ Set to ``True`` to enable automatically link the Prometheus-Client configuration copied by Ansible to host to
     the current project. Only works if you do *not* have :file:`docker-compose.override.yaml` in your deployment
     already."""
 
+class DeploymentLogging(BaseModel):
+    """
+    Adjust docker-compose logging configuration if needed. The defaults should fit well
+    """
+    log_driver: str = "local"
+    """
+    Set a logging driver. The docker default is ``json-file`` with recommandation for ``local`` (used as default here)
+    """
+    max_size: Optional[str] = "10m"
+    """ Maximum size for a single logfile, defaults to '10m' (10 MB) """
+    max_file: Optional[int] = 5
+    """ Maximum number of files to keep """
+    additional_options: Dict[str, str] = {}
+    """ Any additional options you may want to set for your selected driver """
 
 class DeploymentConfig(BaseModel):
     """
     Represents an imported config. All fields are already overwritten specified command line parameters, currently
     including environment, docker_registry and tag
     """
     name: str
@@ -84,14 +101,15 @@
     """ Specify a docker tag which acts as a default tag for all services (not infrastructure services). Overrides any
     docker tag specified by CLI. """
     config_dir: str = './config_dir'
     """ Specify a config dir. The config dir will get mounted to /etc/fastiot
 
         It defaults to :file:`config_dir`
     """
+    logging_config: DeploymentLogging = DeploymentLogging()
 
     @root_validator
     def check_services(cls, values):
         from fastiot.cli.model import InfrastructureService
         services = InfrastructureService.all
 
         for service in values.get("infrastructure_services"):
```

### Comparing `fastiot-0.9/src/fastiot/cli/model/docker_template.py` & `fastiot-1.0/src/fastiot/cli/model/docker_template.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/model/infrastructure_service.py` & `fastiot-1.0/src/fastiot/cli/model/infrastructure_service.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/model/manifest.py` & `fastiot-1.0/src/fastiot/cli/model/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,19 @@
           assetsDir: "static"
         }
 
 
     in your npm config or in case of vue js application in the file :file:`vue.config.js` use the `outputDir` variable
     as relative path here, e.g. ``dist: ../static``
     """
+    node_base_image: str = 'node:16-bookworm-slim'
+    """
+    If you need a different image for building your vue.js app (or whatever) you may define it here.
+    The default is currently set to ``node:16-buster-slim``.
+    """
 
 
 class ServiceManifest(BaseModel):
     """
     Every service needs a :file:`manifest.yaml` to describe the service.
 
     The following options may be used. The file always starts with a ``fastiot_service:`` in the first level. Then
```

### Comparing `fastiot-0.9/src/fastiot/cli/model/project.py` & `fastiot-1.0/src/fastiot/cli/model/project.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/model/service.py` & `fastiot-1.0/src/fastiot/cli/model/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """ data models for FastIoT and infrastructure services """
 import os
+import datetime
+
 from typing import List
 
 from pydantic import BaseModel
 
 from fastiot.cli.constants import MANIFEST_FILENAME
 from fastiot.cli.model import ServiceManifest
-
+from fastiot.cli.version import get_version
 
 class Service(BaseModel):
     """
     The model class for a service
     """
     name: str
+    build_date: str = datetime.datetime.now(datetime.timezone.utc).isoformat()
+    version: str = get_version()
     package: str
     cache: str = ""
     """
     The name to use as the cache on the set docker cache registry. The tag will
     be appended automatically (in case not empty), please do not specify it.
     Example: mypackage-cache
     """
@@ -25,14 +29,20 @@
     A list of extra caches used to speed up building which will all be read-only. It is intended if you want to read
     from other caches or different tags. Each extra cache must match a cache name extended by ':' followed by the tag
     for the cache. It is useful to always include the cache name followed by tag latest to always use latest cache for
     feature branches.
     Examples: mypackage-cache:latest, mypackage-cache:my-feature
     """
 
+    maintainer: str = ""
+    """ Used for docker labels """
+    git_revision: str = ""
+    """ Used for docker labels """
+
+
     def read_manifest(self, check_service_name: str = "") -> ServiceManifest:
         """ Reads out the service manifest, if not run before using the yaml-file otherwise just ``self.manifest``"""
         from fastiot.cli.model.project import ProjectContext  # pylint: disable=import-outside-toplevel
         default_context = ProjectContext.default
         manifest_path = os.path.join(default_context.project_root_dir, 'src',
                                      self.package, self.name, MANIFEST_FILENAME)
         return ServiceManifest.from_yaml_file(manifest_path, check_service_name=check_service_name)
```

### Comparing `fastiot-0.9/src/fastiot/cli/templates/Dockerfile.j2` & `fastiot-1.0/src/fastiot/cli/templates/Dockerfile.j2`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # As a convention, the workdir should always be the project root dir inside the container.
 WORKDIR /opt/fastiot
 
 # As a convention, the python source files should always be placed inside src-dir.
 RUN mkdir /opt/fastiot/src
 ENV PYTHONPATH=$PYTHONPATH:/opt/fastiot/src
 ENV PIP_ROOT_USER_ACTION=ignore
+ENV FASTIOT_WITHIN_CONTAINER=true
 
 # Install requirements
 COPY install.sh ./
 COPY {{ base_requirements_file }} ./requirements/
 RUN FASTIOT_EXTRA_PYPI={{extra_pypi}} /bin/bash -e install.sh
 
 {% if manifest.healthcheck.cmd != '' %}
@@ -27,15 +28,15 @@
     --start-period={{ manifest.healthcheck.start_period }} \
     --retries={{ manifest.healthcheck.retries }} \
     CMD {{ manifest.healthcheck.cmd }}
 {% endif %}
 
 {% if manifest.npm %}
 ### Stage: npm ###
-FROM node:14-buster-slim as build-npm
+FROM {{ manifest.npm.node_base_image }} as build-npm
 COPY src/{{ service.package }}/{{ service.name }}/{{manifest.npm.src}} src/{{ service.package }}/{{ service.name }}/{{manifest.npm.src}}
 WORKDIR src/{{ service.package }}/{{ service.name }}/{{manifest.npm.src}}
 RUN npm ci
 RUN npm run build
 WORKDIR /opt/fastiot
 {% endif %}
 
@@ -52,30 +53,36 @@
 COPY --from=build-npm src/{{ service.package }}/{{ service.name }}/{{manifest.npm.src}}/{{ manifest.npm.dist }} src/{{ service.package }}/{{ service.name }}/{{ manifest.npm.src }}/{{ manifest.npm.dist }}
 {% endif %}
 {% if context.library_package %}
 COPY src/{{context.library_package}} /opt/fastiot/src/{{context.library_package}}
 {% endif %}
 COPY src/{{ service.package }}/{{ service.name }} /opt/fastiot/src/{{ service.package }}/{{ service.name }}
 COPY src/{{ service.package }}/{{ service.name }}/manifest.yaml /opt/fastiot/manifest.yaml
-MAINTAINER {{ maintainer }}
+
+MAINTAINER {{ service.maintainer }}
+LABEL org.label-schema.schema-version="1.0"
+LABEL org.label-schema.name={{ service.name }}
+LABEL org.label-schema.build-date={{ service.build_date }}
+LABEL org.label-schema.maintainer="{{ service.maintainer }}"
+LABEL org.label-schema.version={{ service.version }}
 
 {%if not manifest.privileged%}
 USER fastiot
 {%endif%}
 
 
 CMD ["python",  "/opt/fastiot/src/{{ service.package }}/{{ service.name }}/run.py"]
 
 
 ### Stage: Compile ###
 FROM base as compile_lib
 # In release mode we want to compile everything and only copy compiled artifacts into release container.
 # The compilation takes place in this stage, so we need to compile it accordingly.
 RUN  apt-get update && apt-get install -y gcc make build-essential && apt-get clean -y
-RUN python3 -m pip install --extra-index-url http://{{ extra_pypi }} --trusted-host {{ extra_pypi }} "fastiot[compile]" --root-user-action=ignore
+RUN python3 -m pip install --extra-index-url http://{{ extra_pypi }} --trusted-host {{ extra_pypi }} "fastiot[dev,compile]"
 
 COPY configure.py /opt/fastiot/
 
 COPY src /opt/fastiot/src
 
 {% if context.library_package %}
 RUN fiot extras nuitka-compile --src-dir=/opt/fastiot/src --out-dir=/opt/fastiot/output {{ context.library_package }}
@@ -102,14 +109,20 @@
 {% endfor %}
 
 {% if manifest.npm %}
 COPY --from=build-npm src/{{ service.package }}/{{ service.name }}/{{manifest.npm.src}}/{{ manifest.npm.dist }} src/{{ service.package }}/{{ service.name }}/{{ manifest.npm.src }}/{{ manifest.npm.dist }}
 {% endif %}
 
 COPY src/{{ service.package }}/{{ service.name }}/manifest.yaml /opt/fastiot/manifest.yaml
-MAINTAINER {{ maintainer }}
+MAINTAINER {{ service.maintainer }}
+LABEL org.label-schema.schema-version="1.0"
+LABEL org.label-schema.name="{{ context.project_namespace }}-{{ service.name }}"
+LABEL org.label-schema.build-date={{ service.build_date }}
+LABEL org.label-schema.maintainer="{{ service.maintainer }}"
+LABEL org.label-schema.version={{ service.version }}
+LABEL org.label-schema.vcs-ref="{{ service.git_revision }}"
 
 {%if not manifest.privileged%}
 USER fastiot
 {%endif%}
 
 CMD ["python",  "/opt/fastiot/src/{{ service.package }}/{{ service.name }}/run.py"]
```

### Comparing `fastiot-0.9/src/fastiot/cli/templates/ansible-playbook.yaml.j2` & `fastiot-1.0/src/fastiot/cli/templates/ansible-playbook.yaml.j2`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/templates/docker-bake.hcl.j2` & `fastiot-1.0/src/fastiot/cli/templates/docker-bake.hcl.j2`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/templates/new_service/servicename_service.py.j2` & `fastiot-1.0/src/fastiot/cli/templates/new_service/servicename_service.py.j2`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/templates/pyproject.toml.j2` & `fastiot-1.0/src/fastiot/cli/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/cli/typer_app.py` & `fastiot-1.0/src/fastiot/cli/typer_app.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,16 +5,24 @@
 Here the typer app is initialized. If you want to add own commands you may consult the Typer documentation.
 Basically your commands will be decorated with an `@app.command()`. Replace `app` with `create_cmd`, `run_cmd`, or
 `stop_cmd` if you want to create subcommands of create, run or stop.
 """
 import importlib
 import logging
 import os
+import sys
 
-import typer
+from fastiot.cli.env import env_cli
+
+try:
+    import typer
+except ImportError:
+    if not env_cli.within_container:
+        logging.error("Could not import Typer. To use the CLI you need to install `fastiot[dev]`.")
+    sys.exit(1)
 
 from fastiot.env import env_basic
 
 DEFAULT_CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 
 # Main typer app to add new commands to.
 app = typer.Typer(
```

### Comparing `fastiot-0.9/src/fastiot/cli/version.py` & `fastiot-1.0/src/fastiot/cli/version.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/core/__init__.py` & `fastiot-1.0/src/fastiot/core/__init__.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/core/broker_connection.py` & `fastiot-1.0/src/fastiot/core/broker_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,18 @@
             await self._subscription_error_cb(err)
 
 
 class NatsBrokerSubscriptionReplySubject(NatsBrokerSubscription):
     def __init__(self,
                  subject: ReplySubject,
                  cb: SubscriptionReplyCallback,
-                 send_reply_fn: Callable[[Subject, Msg], Coroutine[None, None, None]]):
+                 send_reply_fn: Callable[[Subject, Msg], Coroutine[None, None, None]],
+                 **kwargs):
+        super().__init__(**kwargs)
+
         self._subject = subject
         self._cb = cb
         self._num_cb_params = len(signature(cb).parameters)
         self._send_reply_fn = send_reply_fn
         self._subscription = None
 
         cb_signature = signature(self._cb)
@@ -191,27 +194,32 @@
     async def request(self, subject: ReplySubject, msg: MsgReq,
                       timeout: float = env_broker.default_timeout) -> MsgResp:
         """
         Send a request on a subject.
 
         :param subject: The subject used for sending the request.
         :param msg: The request
-        :param timeout: The time to wait for an answer. Raises ErrTimeout if no answer is received in time.
-        :return The response
+        :param timeout: The time in seconds to wait for an answer. Raises ErrTimeout if no answer is received in time.
+        :return: The response
         """
         inbox = subject.make_generic_reply_inbox()
         msg_queue = asyncio.Queue()
         sub = await self.subscribe_msg_queue(subject=inbox, msg_queue=msg_queue)
         try:
             await self._send(subject=subject, msg=msg, reply=inbox)
             result = await asyncio.wait_for(msg_queue.get(), timeout=timeout)
         finally:
             await sub.unsubscribe()
         return result
 
+    @property
+    @abstractmethod
+    def is_connected(self) -> bool:
+        """ Return the connection status e.g. for health checks """
+
     def run_threadsafe_nowait(self, coro: Coroutine) -> concurrent.futures.Future:
         """
         Runs a coroutine on brokers event loop. This method is thread-safe. It
         can be useful if you want to interact with the broker from another
         thread.
 
         :param coro: The coroutine to run thread-safe on brokers event loop,
@@ -285,15 +293,15 @@
         Please note, that it will only timeout if the request times out. For
         purposes of simplicity it will wait forever, if the executing thread is
         occupied too much and the request cannot be scheduled.
 
         :param subject: The subject info to publish the request.
         :param msg: The request message.
         :param timeout: The timeout for the broker call.
-        :return The requested message.
+        :return: The requested message.
         """
         return self.run_threadsafe(
             coro=self.request(subject=subject, msg=msg, timeout=timeout)
         )
 
 
 class NatsBrokerConnection(BrokerConnection):
@@ -364,14 +372,17 @@
         reply_str = '' if reply is None else reply.name
         await self._client.publish(
             subject=subject.name,
             payload=payload,
             reply=reply_str
         )
 
+    @property
+    def is_connected(self):
+        return self._client.is_connected
 
 class SubscriptionDummy(Subscription):
     async def unsubscribe(self):
         pass
 
     def check_pending_error(self):
         pass
@@ -381,14 +392,18 @@
 
 
 class BrokerConnectionDummy(BrokerConnection):
     """
     A dummy broker implementation to mock dependencies.
     """
 
+    @property
+    def is_connected(self) -> bool:
+        return True
+
     async def subscribe(self,
                         subject: Subject,
                         cb: SubscriptionCallback) -> Subscription:
         return SubscriptionDummy()
 
     async def subscribe_reply_cb(self,
                                  subject: ReplySubject,
```

### Comparing `fastiot-0.9/src/fastiot/core/data_models.py` & `fastiot-1.0/src/fastiot/core/data_models.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/core/logger.py` & `fastiot-1.0/src/fastiot/core/logger.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/core/serialization.py` & `fastiot-1.0/src/fastiot/core/serialization.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 from fastiot.core.data_models import FastIoTData, Msg, MsgCls
 
 
 def serialize_to_bin(msg_cls: MsgCls, msg: Msg) -> bytes:
     """
     Serializes a msg to binary. It also applies some basic type checks.
+    Please be careful, msgpack will only serialize python primary data types.
+    Data types from numpy for example, cannot be serialized.
     """
     if issubclass(msg_cls, FastIoTData):
         if not isinstance(msg, msg_cls):
             raise TypeError(
                 f"Expected msg to be of type '{msg_cls}', but it is instead "
                 f"of type '{type(msg)}' instead."
             )
```

### Comparing `fastiot-0.9/src/fastiot/core/service.py` & `fastiot-1.0/src/fastiot/core/service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import asyncio
 import signal
-from typing import List
+from typing import List, Optional, Type
 
+from fastiot.cli.env import env_cli
 from fastiot.core.logger import logging
 from fastiot.core.broker_connection import BrokerConnection, NatsBrokerConnection, Subscription
 from fastiot.env import env_basic
 from fastiot.exceptions.exceptions import ShutdownRequestedInterruption
+from fastiot.testlib import populate_test_env
 
 
 class FastIoTService:
     """
     This is the most base class for all FastIoT Services. Your service must inherit from this class for everything to
     work.
     """
     @classmethod
     def main(cls, **kwargs):
         """
         Entrypoint of the class; this is the method to be started using e.g. a :file:`run.py` like generated when
         creating a new service. Do not overwrite, unless you know exactly what you are doing.
 
         :param kwargs: kwargs will be passed to class constructor.
+
         """
 
         async def run_main():
             app = None
             async def closed_cb():
                 # We want to request service shutdown if connection closes
                 nonlocal app
@@ -42,41 +45,53 @@
             )
             try:
                 app = cls(broker_connection=broker_connection, **kwargs)
                 await app.run()
             finally:
                 await broker_connection.close()
 
+        cls._try_setup_test_env()
+
         asyncio.run(run_main())
 
-    def __init__(self, broker_connection: BrokerConnection, **kwargs):
+    @staticmethod
+    def _try_setup_test_env():
+        if not env_cli.within_container and env_basic.config_dir == '/etc/fastiot':  # Test for default (= not set)
+            # Some helper for local development: Read in env vars like in unit tests
+            deployment_name = env_cli.use_local_deployment
+            logging.info("Service started locally. Population environment with variables from %s",
+                         deployment_name or "integration test")
+            populate_test_env(deployment_name=deployment_name)
+
+    def __init__(self, broker_connection: Optional[BrokerConnection] = None, **kwargs):
         super().__init__(**kwargs)
         self.broker_connection = broker_connection
         self._shutdown_event = asyncio.Event()
 
         self._subscription_fns = []
         self._reply_subscription_fns = []
         self._loop_fns = []
 
         self._tasks: List[asyncio.Task] = []
         self._subs: List[Subscription] = []
         self.service_id: str = env_basic.service_id  # Use to separate different services instantiated
         self._logger = logging
+        self._logger.info("Started service %s!", self.__class__.__name__)
 
     def _setup_annotations(self):
         # We cannot setup annotations inside __init__ because some services may have properties which rely on the
         # __init__ method to finish and would otherwise raise exceptions, e.g. a service that reads the config in the
         # __init__ and provides it's values via properties.
         self._subscription_fns = []
         self._reply_subscription_fns = []
         self._loop_fns = []
         for name in dir(self):
             if name.startswith('__'):
                 continue
-            attr = self.__getattribute__(name)
+            attr = getattr(self, name)
             if hasattr(attr, '_fastiot_subject'):
                 self._subscription_fns.append(attr)
             if hasattr(attr, '_fastiot_reply_subject'):
                 self._reply_subscription_fns.append(attr)
             if hasattr(attr, '_fastiot_is_loop'):
                 self._loop_fns.append(attr)
 
@@ -87,52 +102,52 @@
         """ Optionally overwrite this method to run any async stop commands like ``await self._server.stop()``` """
 
 
     def run_task(self, coro):
         """
         Creates an asyncio-Task which is managed by this class. If the execution
         of the coroutine raises an exception, they are logged and a service
-        shutdown is requested. If the task terminates reguarly, it is dropped
+        shutdown is requested. If the task terminates regularly, it is dropped
         and the module continuous to run.
 
         The task is awaited after _stop() has been called.
         """
         self._tasks.append(
             asyncio.create_task(self._exec_task(coro=coro))
         )
 
     async def _exec_task(self, coro):
         err = None
         try:
             await coro
-        except Exception as e:
+        except Exception as exception:  # pylint: disable=broad-exception-caught
             logging.exception("Uncaught exception raised inside task")
-            err = e
+            err = exception
         if err:
-            await self.request_shutdown("Task failed with an exception")
+            await self.request_shutdown("Task failed with an exception", exception=err)
 
     async def wait_for_shutdown(self, timeout: float = 0.0) -> bool:
         """
         Method to wait for service shutdown. This is helpfull if you have a loop
-        running forever till the service needs to shutdown.
+        running forever till the service needs to shut down.
 
         Shutdown may occur when some other parts of the service fail like
         database connection or broker connection.
 
         Per default, it will wait indefinetly, but you can specify a timeout. If
         timeout exceeds, it will not raise a timeout error, but instead return
-        false. Otherwise it will return true.
+        false. Otherwise, it will return true.
 
         Example:
         >>> while await self.wait_for_shutdown(1.0) is False:
         >>>     print("Still running...")
 
         :param timeout: Specify a time you want to wait for the shutdown. A
                         value of 0.0 (default) will wait indefinetly.
-        :result Return true if shutdown is requested, false if timeout occured.
+        :returns: Return true if shutdown is requested, false if timeout occured.
         """
         if timeout < 0:
             raise ValueError("Timeout must be greater or equal zero")
 
         if timeout == 0:
             await self._shutdown_event.wait()
             return True
@@ -149,31 +164,34 @@
 
     async def run_coro(self, coro):
         """
         Waits for coro or raises ShutdownRequestedInterruption if shutdown is
         requested.
 
         :param coro: The coroutine to wait for
-        :returns The result of the coroutine
+        :returns: The result of the coroutine
         """
         do_raise_err = True
         async def _wait_and_raise_interruption():
             nonlocal do_raise_err
             await self.wait_for_shutdown()
             if do_raise_err:
                 raise ShutdownRequestedInterruption()
 
-        for c in asyncio.as_completed([coro, _wait_and_raise_interruption()]):
-            result = await c
+        for coro_completed in asyncio.as_completed([coro, _wait_and_raise_interruption()]):
+            result = await coro_completed
             do_raise_err = False  # We don't want error to be raised if coroutine finished successfully.
             return result
 
     async def __aenter__(self):
         self._shutdown_event.clear()
         self._setup_annotations()
+        self._try_setup_test_env()
+        if not self.broker_connection:
+            self.broker_connection = await NatsBrokerConnection.connect()
         await self._start()
         await self._start_annotated_subs()
         await self._start_annotated_loops()
         await asyncio.sleep(0.0)  # pass control once so that stuff gets initialized
         return self
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
@@ -201,46 +219,51 @@
 
         await self.wait_for_shutdown()
 
         await self._stop_subs()
         await self._stop()
         await self._stop_tasks()
 
-    async def request_shutdown(self, reason: str = ''):
+    async def request_shutdown(self, reason: str = '', exception: Optional[Type[Exception]] = None ):
         """ Sets the shutdown request for all loops and tasks in the service to stop """
-        if self._shutdown_event.is_set() is False and reason:
-            logging.info("Initial shutdown requested with reason: %s.", str(reason))
+        if not self._shutdown_event.is_set() and (reason or exception):
+            if reason:
+                self._logger.info("Initial shutdown requested with reason: %s.", str(reason))
+            if exception:
+                self._logger.exception(exception)
         self._shutdown_event.set()
 
     async def _start_annotated_loops(self):
         for loop_fn in self._loop_fns:
             self.run_task(self._loop_task_cb(loop_fn=loop_fn))
 
     async def _start_annotated_subs(self):
         for subscription_fn in self._subscription_fns:
             sub = await self.broker_connection.subscribe(
-                subject=subscription_fn._fastiot_subject,
+                subject=subscription_fn._fastiot_subject,  # pylint: disable=protected-access
                 cb=subscription_fn
             )
             self._subs.append(sub)
 
         for subscription_fn in self._reply_subscription_fns:
             sub = await self.broker_connection.subscribe_reply_cb(
-                subject=subscription_fn._fastiot_reply_subject,
+                subject=subscription_fn._fastiot_reply_subject,  # pylint: disable=protected-access
                 cb=subscription_fn
             )
             self._subs.append(sub)
 
     async def _loop_task_cb(self, loop_fn):
         while True:
             awaitable = await loop_fn()
             try:
                 await self.run_coro(awaitable)
             except ShutdownRequestedInterruption:
                 break
+            except Exception:
+                break
 
     async def _stop_subs(self):
         for sub in self._subs:
             await sub.unsubscribe()
         self._subs = []
 
     async def _stop_tasks(self):
```

### Comparing `fastiot-0.9/src/fastiot/core/service_annotations.py` & `fastiot-1.0/src/fastiot/core/service_annotations.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from fastiot.core.data_models import Subject, ReplySubject
 
 
 def subscribe(subject: Subject):
     """
     Decorator method for methods subscribing to a subject. The decorated method must have either one or two arguments:
 
-      - subscribe_something(message: Type[FastIoTData])
-      - subscribe_something(subject_name: str, message: Type[FastIoTData])
+    - subscribe_something(message: Type[FastIoTData])
+    - subscribe_something(subject_name: str, message: Type[FastIoTData])
 
     See :ref:`publish-subscribe` for more details.
 
     :param subject: The subject (:class:`fastiot.core.data_models.Subject`) to subscribe.
     """
     def subscribe_wrapper_fn(fn):
         if not asyncio.iscoroutinefunction(fn):
@@ -21,15 +21,15 @@
         fn._fastiot_subject = subject
         return fn
     return subscribe_wrapper_fn
 
 
 def reply(subject: ReplySubject):
     """
-    Decorator for methods replying on the specified subject. This works similiar to
+    Decorator for methods replying on the specified subject. This works similar to
     :meth:`fastiot.core.service_annotations.subscribe` but you have to return a ``Msg`` as a reply
     message.
 
     :param subject: The subject to subscribe to for sending replies
     """
     def subscribe_wrapper_fn(fn):
         if not asyncio.iscoroutinefunction(fn):
@@ -38,24 +38,27 @@
         return fn
     return subscribe_wrapper_fn
 
 
 def loop(fn):
     """
     Decorator function for methods to run continuously. This will basically create a "while True loop" wrapper around
-    the provided function. This is purely syntactic suggar for run_task.
+    the provided function. This is purely syntactic sugar for run_task.
 
     Your method needs to return an awaitable that is awaited after each loop execution before the next iteration.
     However, the returned awaitable does not finish if a service shutdown is requested. It uses ``self.run_coro`` under
     the hood. But it is guaranteed, that the annotated loop function is awaited and not interrupted if a shutdown is
     requested.
 
     Example:
+
+    ..  code-block:: python
+
         @loop
         async def log_still_running(self):
-            logging.info("Service is still running.")
+            self._logger.info("Service is still running. Next message in 10 seconds.")
             return asyncio.sleep(10.0)
     """
     if not asyncio.iscoroutinefunction(fn):
         raise TypeError("Expected coroutine function for loop annotation")
     fn._fastiot_is_loop = True
     return fn
```

### Comparing `fastiot-0.9/src/fastiot/core/subject_helper.py` & `fastiot-1.0/src/fastiot/core/subject_helper.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/db/influxdb_helper_fn.py` & `fastiot-1.0/src/fastiot/db/influxdb_helper_fn.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,16 +41,16 @@
 async def create_async_influxdb_client_from_env():
     try:
         # pylint: disable=import-outside-toplevel
         from influxdb_client.client.influxdb_client_async import InfluxDBClientAsync
         from influxdb_client.client.exceptions import InfluxDBError
         from aiohttp.client_exceptions import ClientError
     except (ImportError, ModuleNotFoundError):
-        logging.error("You have to manually install `influxdb-client[async]>=1.30,<2` using your `requirements.txt` "
-                      "to make use of this helper.")
+        logging.error("You have to manually install `fastiot[influxdb]` or `influxdb-client[async]>=1.30,<2` using "
+                      "your `pyproject.toml` to make use of this helper.")
         sys.exit(5)
 
     sleep_time = 0.25
     num_tries = 50
     while num_tries > 0:
         try:
             client = InfluxDBClientAsync(
```

### Comparing `fastiot-0.9/src/fastiot/db/mariadb_helper_fn.py` & `fastiot-1.0/src/fastiot/db/mariadb_helper_fn.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,16 @@
                        user: str, password: str):
     # We found that mariadb initial start time takes very long in some environments. Therefore we need a timeout much
     # greater then two minutes.
     try:
         # pylint: disable=import-outside-toplevel
         import pymysql.cursors
     except (ImportError, ModuleNotFoundError):
-        logging.error("You have to manually install `PyMySQL>=1.0,<2` using your `requirements.txt` "
-                                 "to make use of this helper.")
+        logging.error("You have to manually install `fastiot[mariadb]` or `PyMySQL>=1.0,<2` using your "
+                      "`pyproject.toml` to make use of this helper.")
         sys.exit(5)
 
     for _ in range(10):
         try:
             db_client = pymysql.connect(
                 host=host,
                 port=port,
```

### Comparing `fastiot-0.9/src/fastiot/db/mariadb_schema_checks.py` & `fastiot-1.0/src/fastiot/db/mariadb_schema_checks.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/db/mongodb_helper_fn.py` & `fastiot-1.0/src/fastiot/db/mongodb_helper_fn.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
             # pylint: disable=import-outside-toplevel
             from bson.binary import UUID_SUBTYPE
             from bson.codec_options import CodecOptions
             from pymongo import MongoClient
             from pymongo.errors import ConnectionFailure
         except (ImportError, ModuleNotFoundError):
             logging.error("You have to manually install "
-                          "`pymongo>=4.1,<5` using your `requirements.txt` to make use of "
+                          "`pymongo>=4.1,<5` or `fastiot[mongo]` using your `pyproject.toml` to make use of "
                           "this helper.")
             sys.exit(5)
 
         mongo_client_kwargs = {
             "host": db_host,
             "port": db_port,
             "username": db_user,
```

### Comparing `fastiot-0.9/src/fastiot/db/redis_helper.py` & `fastiot-1.0/src/fastiot/db/redis_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,69 @@
 import logging
-
-import redis
+import sys
 
 from fastiot.core.serialization import serialize_to_bin, serialize_from_bin
 from fastiot.env.env import env_redis
 from fastiot.msg import RedisMsg
 
 
 class RedisClient:
     client = None
 
+
 async def connect_redis():
+    try:
+        import redis  # pylint: disable=import-outside-toplevel
+    except ImportError:
+        logging.error("You have to manually install `redis>=4.5,<5` or `fastiot[redis]` using your `pyproject.toml` "
+                      "to make use of this helper.")
+        sys.exit(5)
     client = redis.Redis(
         host=env_redis.host,
         port=env_redis.port)
     return client
 
+
 async def get_redis_client():
     if RedisClient.client is None:
         RedisClient.client = await connect_redis()
     return RedisClient.client
 
 
 class RedisHelper:
     """
     Saves files in the redis Database and sends the ID of the files  as  :class:`fastiot.msg.redis.RedisMsg`.
 
     You can send files by using :meth:`send_data` you must specify the data to send and the subject under which the data
-    should be published. The max number of Datasets you can store at once is specified by :var: `max_data_sets` .
+    should be published. The max number of Datasets you can store at once is specified by ``max_data_sets`` .
     If you add a Dataset above the given limit the first Dataset stored is deleted. When you have problems that an ID
-    is overwritten before you accessed the data you can change the :var:`id_buffer` to have more Ids before an ID is
+    is overwritten before you accessed the data you can change the ``id_buffer`` to have more Ids before an ID is
     reused.
 
     You can access the stored data with :meth:`get_data`. The Id of the Data has to be provided. and the returned data
     will be deserialized with :meth:`fastiot.core.serialization.serialize_from_bin`.
 
+    You have to add ``redis`` or ``fastiot[redis]`` to your requirements in :file:`pyproject.toml` or (old style)
+    :file:`requirements.txt`.
+
     .. seealso::
        :mod:`fastiot_sample_services.redis_producer`
           Example service for sending and receiving data over a Redis Server.
        :class:`fastiot.cli.common.infrastructure_services.RedisService`
           The infrastructure service definition for the Redis Server.
     """
 
     def __init__(self, broker_connection):
         self.broker_connection = broker_connection
         self.used_ids = []
         self.max_data_sets = 100
         """ The max number of Datasets you can store at once """
         self.id_counter = 0
         self.id_buffer = 2
-        """ :var:`max_data_sets` * :var:`id_buffer` is the total number of Ids, used before an id is overwritten """
+        """ ``max_data_sets`` * ``id_buffer`` is the total number of Ids, used before an id is overwritten """
 
     async def _create_id(self) -> int:
         if self.id_counter >= (self.max_data_sets * self.id_buffer):
             self.id_counter = 0
         while self.id_counter in self.used_ids:
             self.id_counter = self.id_counter + 1
         self.used_ids.append(self.id_counter)
```

### Comparing `fastiot-0.9/src/fastiot/db/time_scale_helper_fn.py` & `fastiot-1.0/src/fastiot/db/time_scale_helper_fn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# --------- apt-get install libpq-dev first to install psycopg2 !!! -----------
 import sys
 import time
 
 from fastiot import logging
 from fastiot.env.env import env_timescaledb
 from fastiot.exceptions import ServiceError
 
@@ -10,14 +9,17 @@
 def get_timescaledb_client_from_env():
     """
     For connecting TimeScaleDB, the environment variables can be set,
     if you want to use your own settings instead of default:
     :envvar:`FASTIOT_TIME_SCALE_DB_HOST`, :envvar:`FASTIOT_TIME_SCALE_DB_PORT`, :envvar:`FASTIOT_TIME_SCALE_DB_USER`,
     :envvar:`FASTIOT_TIME_SCALE_DB_PASSWORD`, :envvar:`FASTIOT_TIME_SCALE_DB_DATABASE`
 
+    *Attention*: You must have `libpq-dev` installed in your system (or your container), e.g.
+    :command:`apt-get install libpq-dev`.
+
     >>> time_scale_db_client = get_timescaledb_client_from_env()
     """
     db_client = get_timescaledb_client(
         host=env_timescaledb.host,
         port=env_timescaledb.port,
         user=env_timescaledb.user,
         password=env_timescaledb.password,
@@ -29,16 +31,16 @@
 def get_timescaledb_client(host: str, port: int, user: str, password: str,
                            database: str = None):
     try:
         # pylint: disable=import-outside-toplevel
         import psycopg2
         from psycopg2 import OperationalError
     except (ImportError, ModuleNotFoundError):
-        logging.error("You have to manually install `psycopg2>=2.9.3,<3` using your `requirements.txt` "
-                      "to make use of this helper.")
+        logging.error("You have to manually install `fastiot[postgredb]` or `psycopg2>=2.9.3,<3` using your "
+                      "`pyproject.toml` to make use of this helper.")
         sys.exit(5)
 
     client_parameters = {"user": user, "password": password, "host": host,
                          "port": port, "database": database}
 
     # We found that the postgres connection with docker sometimes failed, because of the env variables in
     # docker-compose.yaml are not really set. Try docker-compose up -d --force-recreate to start the test environment.
```

### Comparing `fastiot-0.9/src/fastiot/env/env.py` & `fastiot-1.0/src/fastiot/env/env.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/env/env_basic.py` & `fastiot-1.0/src/fastiot/env/env_basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     @property
     def service_id(self) -> str:
         """ .. envvar:: FASTIOT_SERVICE_ID
 
         Use this variable to differentiate between multiple instances of the same service. The result is available as
         ``self.service_id``. It is for example used to read a configuration file for each service with
-        :func:`fastiot.util.read_yaml.read_config`. See
+        :func:`fastiot.util.config_helper.read_config`. See :ref:`configuration_for_service` for more information.
         """
         return os.getenv(FASTIOT_SERVICE_ID, '')
 
     @property
     def log_dir(self) -> str:
         return os.path.join(self.volume_dir, 'logs')
```

### Comparing `fastiot-0.9/src/fastiot/env/env_broker.py` & `fastiot-1.0/src/fastiot/env/env_broker.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/env/env_constants_db.py` & `fastiot-1.0/src/fastiot/env/env_constants_db.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,11 +29,7 @@
 FASTIOT_INFLUX_DB_USER = 'FASTIOT_INFLUX_DB_USER'
 FASTIOT_INFLUX_DB_PASSWORD = 'FASTIOT_INFLUX_DB_PASSWORD'
 FASTIOT_INFLUX_DB_MODE = 'FASTIOT_INFLUX_DB_MODE'
 FASTIOT_INFLUX_DB_ORG = 'FASTIOT_INFLUX_DB_ORG'
 FASTIOT_INFLUX_DB_BUCKET = 'FASTIOT_INFLUX_DB_BUCKET'
 FASTIOT_INFLUX_DB_TOKEN = 'FASTIOT_INFLUX_DB_TOKEN'
 FASTIOT_INFLUX_DB_VOLUME = 'FASTIOT_INFLUX_DB_VOLUME'
-FASTIOT_ELASTICSEARCH_HOST = 'FASTIOT_ELASTICSEARCH_HOST'
-FASTIOT_ELASTICSEARCH_PORT = 'FASTIOT_ELASTICSEARCH_PORT'
-FASTIOT_ELASTICSEARCH_PASSWORD = 'FASTIOT_ELASTICSEARCH_PASSWORD'
-FASTIOT_ELASTICSEARCH_VOLUME = 'FASTIOT_ELASTICSEARCH_VOLUME'
```

### Comparing `fastiot-0.9/src/fastiot/env/env_influxdb.py` & `fastiot-1.0/src/fastiot/env/env_influxdb.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/env/env_mariadb.py` & `fastiot-1.0/src/fastiot/env/env_mariadb.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/env/env_mongodb.py` & `fastiot-1.0/src/fastiot/env/env_mongodb.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/env/env_redis.py` & `fastiot-1.0/src/fastiot/env/env_redis.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from fastiot.env.env_constants_db import FASTIOT_REDIS_HOST, FASTIOT_REDIS_PORT, FASTIOT_REDIS_PASSWORD
 
 
 class RedisEnv:
     """ Environment variables to connect to the Redis Server """
     @property
     def host(self) -> str:
-        """ .. envvar:: FASTIOT_INFLUX_DB_HOST
+        """ .. envvar:: FASTIOT_REDIS_HOST
 
-        Use to get/set the influx database host. This is usually either ``influxdb`` within the docker network or
-        ``localhost`` when developing against a local influxdb.
+        Use to get/set the redis database host. This is usually either ``redis`` within the docker network or
+        ``localhost`` when developing against a local redis server.
         """
         return os.getenv(FASTIOT_REDIS_HOST, 'localhost')
 
     @property
     def port(self) -> int:
-        """ .. envvar:: FASTIOT_INFLUX_DB_PORT
+        """ .. envvar:: FASTIOT_REDIS_PORT
 
-        Use to get/set the Redis port, defaults to 8086. """
+        Use to get/set the Redis port, defaults to 6379. """
         return int(os.getenv(FASTIOT_REDIS_PORT, RedisService().get_default_port()))
 
     @property
     def password(self) -> Optional[str]:
         """ .. envvar:: FASTIOT_REDIS_PASSWORD
 
         Use to get/set the Redis password.
```

### Comparing `fastiot-0.9/src/fastiot/env/env_timescaledb.py` & `fastiot-1.0/src/fastiot/env/env_timescaledb.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/env/helpers.py` & `fastiot-1.0/src/fastiot/env/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,13 +6,13 @@
     Helper function for parsing flag env variables (returns true or false).
 
     Please use this function for parsing boolean flags for unified behavior across fastiot. Please also note, that this
     function exists because a bool cast doesn't cut it because bool('false') is true why this function exists.
 
     :param env_var: The name of the env var
     :param default: The default flag if the env var doesn't exist in os environment.
-    :return The flag, true or false
+    :return: The flag, true or false
     """
     if env_var in os.environ:
         return os.environ[env_var].lower() == 'true'
 
     return default
```

### Comparing `fastiot-0.9/src/fastiot/exceptions/exceptions.py` & `fastiot-1.0/src/fastiot/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/msg/custom_db_data_type_conversion.py` & `fastiot-1.0/src/fastiot/msg/custom_db_data_type_conversion.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/msg/hist.py` & `fastiot-1.0/src/fastiot/msg/hist.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/msg/thing.py` & `fastiot-1.0/src/fastiot/msg/thing.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/msg/time_series_msg.py` & `fastiot-1.0/src/fastiot/msg/time_series_msg.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/util/case_conversions.py` & `fastiot-1.0/src/fastiot/util/case_conversions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict, List
 
 
 def kebab_case_to_snake_case(d: Dict):
     """
-    Converts keys of dictionary recursivly from kebab case, e.g. 'my-key' to snake case, e.g. 'my_key'.
+    Converts keys of dictionary recursively from kebab case, e.g. ``my-key`` to snake case, e.g. ``my_key``.
     """
 
     keys = list(d.keys())
     for key in keys:
 
         if isinstance(d[key], dict):
             kebab_case_to_snake_case(d=d[key])
```

### Comparing `fastiot-0.9/src/fastiot/util/csv_reader.py` & `fastiot-1.0/src/fastiot/util/csv_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 class CSVReader:
     """
     A class for csv file reading. It uses python-lib's csv package and does more strict checks on how the csv file
     must be formatted. Raises a CSVError if the file is incorrectly formatted.
 
     Example usage:
 
-    with CSVReader('my_file.csv',
-                   required_fields=['my_field1', 'my_field2'],
-                   optional_fields=['my_optional_field2']) as reader:
-        for data_row in reader:
-            print(data_row['my_field1'])
-            print(data_row['my_field2'])
-            print(data_row.get('my_optional_field2', 'unset'))
+    ..  code-block:: python
+
+        with CSVReader('my_file.csv',
+                       required_fields=['my_field1', 'my_field2'],
+                       optional_fields=['my_optional_field2']) as reader:
+            for data_row in reader:
+                print(data_row['my_field1'])
+                print(data_row['my_field2'])
+                print(data_row.get('my_optional_field2', 'unset'))
     """
 
     def __init__(self,
                  filename: str,
                  required_fields: Optional[List[str]] = None,
                  optional_fields: Optional[List[str]] = None,
                  checks: Optional[Dict[str, Callable[[str], bool]]] = None,
```

### Comparing `fastiot-0.9/src/fastiot/util/object_helper.py` & `fastiot-1.0/src/fastiot/util/object_helper.py`

 * *Files identical despite different names*

### Comparing `fastiot-0.9/src/fastiot/util/read_yaml.py` & `fastiot-1.0/src/fastiot/util/config_helper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,55 @@
 """ Providing methods to import yaml configuration per service"""
 
 import logging
 import os
 from typing import Optional, Dict, Union
 
 import yaml
+from pydantic import BaseModel
 
-from fastiot.core.service import FastIoTService
+from fastiot.core import FastIoTService
 from fastiot.env import env_basic
+from fastiot.util.case_conversions import kebab_case_to_snake_case
+
+
+class FastIoTConfigModel(BaseModel):
+    """
+    You may use this as a base class to provide a proper data model for your configurations.
+    This is a proper alternative to relying on reading in YAML-files and working with dictionaries
+    as done with :meth:`fastiot.util.config_helper.read_config`.
+
+    Please consult :ref:`configuration_for_service` for more information about handling configurations and a full
+    example.
+    """
+
+    @classmethod
+    def from_yaml_file(cls, filename: str):
+        """ Does the magic of import yaml to pydantic model, provided by a filename."""
+        with open(filename, 'r') as config_file:
+            config = yaml.safe_load(config_file)
+            kebab_case_to_snake_case(config)
+
+        config_object = cls(**config)
+        return config_object
+
+    @classmethod
+    def from_service(cls, service: Union[FastIoTService, str]):
+        """
+        Read in the configuration for your service, so just use it with :code:`MyServiceConfig.from_service(self)`
+        inside your service.
+
+        It is possible to read the configuration for a service instantiated multiple times.
+        If both service.yaml and service_id.yaml exist, service_id.yaml will be preferred.
+        Use the environment variable :envvar:`FASTIOT_SERVICE_ID` to set the individual service id for a service.
+
+        Also see :ref:`configuration_for_service` for more information about handling configurations.
+        """
+        filename = _get_config_file_name(service=service)
+        return cls.from_yaml_file(filename=filename)
 
 
 def _get_config_file_name(service: Union[FastIoTService, str]) -> Optional[str]:
     """
     Find the yaml config file for the given service.
 
     If both service.yaml and service_id.yaml exist, service_id.yaml will be preferred.
@@ -55,15 +93,15 @@
     Use the environment variable :envvar:`FASTIOT_SERVICE_ID` to set the individual service id for a service.
 
     Also see :ref:`configuration_for_service` for more information about handling configurations.
 
     Example passing your service to get a filename configuration automatically:
 
     >>> from fastiot.core import FastIoTService
-    >>> from fastiot.util.read_yaml import read_config
+    >>> from fastiot.util.config_helper import read_config
     >>>
     >>> class MyService(FastIoTService)
     >>>
     >>>     def __init__(self, **kwargs)
     >>>         super().__init__(**kwargs)
     >>>         my_config = read_config(self)
```

### Comparing `fastiot-0.9/src/fastiot.egg-info/PKG-INFO` & `fastiot-1.0/src/fastiot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fastiot
-Version: 0.9
+Version: 1.0
 Summary: FastIoT Platform
 Author-email: Tilman Klaeger <tilman.klaeger@ivv-dd.fraunhofer.de>, Konstantin Merker <konstantin.merker@ivv-dd.fraunhofer.de>, Fraunhofer Institute for Process Engineering and Packaging IVV <info@ivv-dd.fraunhofer.de>
-Maintainer-email: Tilman Klaeger <tilman.klaeger@ivv-dd.fraunhofer.de>, Jialiang Yin <jialiang.yin@ivv-dd.fraunhofer.de>
+Maintainer-email: Tilman Klaeger <tilman.klaeger@ivv-dd.fraunhofer.de>, Tim Kaluza <tim.kaluza@ivv-dd.fraunhofer.de>, Jialiang Yin <jialiang.yin@ivv-dd.fraunhofer.de>
 Project-URL: Homepage, https://github.com/FraunhoferIVV/fastiot
 Project-URL: Source, https://github.com/FraunhoferIVV/fastiot
 Project-URL: Documentation, https://fastiot.readthedocs.io
 Keywords: Industrial IoT,IoT,Industry4.0,IIoT
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -23,19 +23,20 @@
 Provides-Extra: dev
 Provides-Extra: fastapi
 Provides-Extra: influxdb
 Provides-Extra: mariadb
 Provides-Extra: mongodb
 Provides-Extra: opcua
 Provides-Extra: postgredb
+Provides-Extra: redis
 Provides-Extra: dash
 Provides-Extra: docs
 License-File: LICENSE
 
-# Fast-IoT (fastiot)
+# FastIoT (fastiot)
 
 FastIoT is a framework for rapid development of IIoT-Systems using Python as main programming language.
 It helps to set up a micro-service architecture and create services. The development has been started as basis for 
 various research projects at Fraunhofer IVV, Dresden, Germany.  
 
 To get started quickly it is equipped with a powerful command line interface (CLI): `fiot`.
 This helps setting up a new project, create new services and run tests. 
@@ -108,15 +109,20 @@
 
 To run services locally, in your IDE or within a container you may also refer to the complete documentation.
 
 ## Developing FastIoT
 
 Simply check out this project and install the dependencies listed in `requirements.txt`.
 To run all tests and sample services you may also install additional packages listed in 
-`requirements/requirements-all.txt`. 
+`requirements/requirements.all.txt`.
+Do *NOT* install fastiot when developing within this code.
+This will produce duplicates and may show weird errors. 
+If in doubt run `pip uninstall fastiot`.
+
+To make sure you can run commands like `fiot` you must add the `src`-directory to your Python Path: `export PYTHONPATH="$(pwd)/src:$PYTHONPATH`
 
 ### Project structure
 
 A detailed structure for all projects based on FastIoT is listed in the documentation. Here just the few most important 
 parts are listed:
 
 * `src/fastiot`: The core library and base with CLI, message handling, …
```

### Comparing `fastiot-0.9/src/fastiot.egg-info/SOURCES.txt` & `fastiot-1.0/src/fastiot.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 LICENSE
 MANIFEST.in
 README.md
 configure.py
 install.sh
 pyproject.toml
 requirements.txt
-.run/FastAPI.run.xml
 bin/fiot
 requirements/requirements.all.txt
 requirements/requirements.compile.txt
 requirements/requirements.dash.txt
 requirements/requirements.dev.txt
 requirements/requirements.docs.txt
 requirements/requirements.fastapi.txt
 requirements/requirements.influxdb.txt
 requirements/requirements.mariadb.txt
 requirements/requirements.mongodb.txt
 requirements/requirements.opcua.txt
 requirements/requirements.postgredb.txt
+requirements/requirements.redis.txt
 src/fastiot/__init__.py
 src/fastiot/__version__.py
 src/fastiot/testlib.py
 src/fastiot.egg-info/PKG-INFO
 src/fastiot.egg-info/SOURCES.txt
 src/fastiot.egg-info/dependency_links.txt
 src/fastiot.egg-info/entry_points.txt
@@ -107,15 +107,14 @@
 src/fastiot/db/time_scale_helper_fn.py
 src/fastiot/env/__init__.py
 src/fastiot/env/env.py
 src/fastiot/env/env_basic.py
 src/fastiot/env/env_broker.py
 src/fastiot/env/env_constants_basic.py
 src/fastiot/env/env_constants_db.py
-src/fastiot/env/env_elasticdb.py
 src/fastiot/env/env_influxdb.py
 src/fastiot/env/env_mariadb.py
 src/fastiot/env/env_mongodb.py
 src/fastiot/env/env_redis.py
 src/fastiot/env/env_timescaledb.py
 src/fastiot/env/helpers.py
 src/fastiot/exceptions/__init__.py
@@ -125,11 +124,12 @@
 src/fastiot/msg/hist.py
 src/fastiot/msg/redis.py
 src/fastiot/msg/thing.py
 src/fastiot/msg/time_series_msg.py
 src/fastiot/util/__init__.py
 src/fastiot/util/case_conversions.py
 src/fastiot/util/classproperty.py
+src/fastiot/util/config_helper.py
 src/fastiot/util/csv_reader.py
 src/fastiot/util/object_helper.py
 src/fastiot/util/ports.py
 src/fastiot/util/read_yaml.py
```

### Comparing `fastiot-0.9/src/fastiot.egg-info/requires.txt` & `fastiot-1.0/src/fastiot.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 pydantic<2,>=1.9.0
 msgpack<2,>=1
 nats-py<3,>=2.1.0
 PyYAML<7,>=5
-typer<1,>=0.4.1
-Jinja2<4,>=2
-Redis>4
-tomli~=2.0.1
-tomli_w
-build
-pip-tools
 
 [compile]
 Nuitka<2,>=1.1.7
 ordered-set
 
 [dash]
 dash~=2.6.1
@@ -23,14 +16,21 @@
 xlsxwriter
 nest_asyncio
 pymongo<5,>=4.1
 
 [dev]
 pytest<8,>=7.2
 typer[all]<1,>=0.4.1
+tomli~=2.0.1
+tomli_w
+build
+pip-tools
+typer<1,>=0.4.1
+Jinja2<4,>=2
+pytest-cov>=4.1.0
 
 [docs]
 sphinx>=5
 sphinx-automodapi
 sphinx-autodoc-typehints
 recommonmark
 myst-parser
@@ -55,7 +55,10 @@
 
 [opcua]
 opcua<1,>=0.98.8
 asyncua
 
 [postgredb]
 psycopg2-binary<3,>=2.9.3
+
+[redis]
+Redis>4
```

