# Comparing `tmp/dagworks-sdk-0.0.6.tar.gz` & `tmp/dagworks-sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagworks-sdk-0.0.6.tar", last modified: Tue Jun  6 19:39:55 2023, max compression
+gzip compressed data, was "dagworks-sdk-0.0.7.tar", last modified: Mon Jun 19 04:12:43 2023, max compression
```

## Comparing `dagworks-sdk-0.0.6.tar` & `dagworks-sdk-0.0.7.tar`

### file list

```diff
@@ -1,184 +1,189 @@
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.978876 dagworks-sdk-0.0.6/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/LICENSE
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-06-06 19:39:55.978616 dagworks-sdk-0.0.6/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3655 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/README.md
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/pyproject.toml
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       14 2023-05-29 05:01:18.000000 dagworks-sdk-0.0.6/requirements-test.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      213 2023-05-29 05:01:18.000000 dagworks-sdk-0.0.6/requirements.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2023-06-06 19:39:55.978949 dagworks-sdk-0.0.6/setup.cfg
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/setup.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.907302 dagworks-sdk-0.0.6/src/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.910225 dagworks-sdk-0.0.6/src/dagworks/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1092 2023-06-06 19:39:24.000000 dagworks-sdk-0.0.6/src/dagworks/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.912854 dagworks-sdk-0.0.6/src/dagworks/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.915248 dagworks-sdk-0.0.6/src/dagworks/api/api_client/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      152 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.915654 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       47 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.918404 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3379 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2926 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5383 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4111 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4813 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.923274 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3035 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5855 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4711 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5053 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4516 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4994 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8029 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5693 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5511 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5779 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6327 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.925734 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4421 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5087 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6058 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6286 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5367 2023-05-29 05:37:49.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2817 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/client.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      470 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/errors.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.953955 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4237 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2443 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/api_key_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1982 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/dependency.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2706 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/documentation_asset_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1285 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3019 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/documentation_asset_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1268 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2766 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2480 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_function.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3778 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_node.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1692 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1175 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_node_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/organization_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/paged_api_key_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2238 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/paged_project_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2231 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/paged_run_log_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1649 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/phone_home_result.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1977 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1179 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_in_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4499 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1165 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3909 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_in_git.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_in_git_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1243 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_in_git_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5339 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1203 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1241 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_version_info.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5848 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_with_dag.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1244 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1282 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1422 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/python_type.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1791 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_data.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5416 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1185 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in_inputs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1171 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in_run_log.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6517 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1173 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_inputs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1163 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7054 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_with_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1214 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1204 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3710 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/task_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1198 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/task_run_result_summary.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      226 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/task_run_status.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3189 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2916 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1586 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/user_out.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4362 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/visibility_full.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3802 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/visibility_in.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2306 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/who_am_i_result.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      993 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/api_client/types.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9750 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/clients.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1168 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/constants.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/api/projecttypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.955916 dagworks-sdk-0.0.6/src/dagworks/cli/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2025 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/cli.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6513 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/initialize.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.956504 dagworks-sdk-0.0.6/src/dagworks/cli/templates/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.958930 dagworks-sdk-0.0.6/src/dagworks/cli/templates/common/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/common/.env.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/common/README.md.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/common/run.py.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.959288 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.960732 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/components/common.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.961079 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/config/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.962138 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.962523 dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.963104 dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.963779 dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.964120 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.966119 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.966459 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.968548 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.969042 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    14135 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/driver.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.972987 dagworks-sdk-0.0.6/src/dagworks/parsing/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/parsing/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2394 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/parsing/dagtypes.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7810 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/parsing/parse.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.973665 dagworks-sdk-0.0.6/src/dagworks/telemetry/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/telemetry/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/telemetry/telemetry.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.974925 dagworks-sdk-0.0.6/src/dagworks/tracking/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/tracking/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/tracking/example_tracking.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    13943 2023-06-06 19:39:24.000000 dagworks-sdk-0.0.6/src/dagworks/tracking/runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2411 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/src/dagworks/tracking/trackingtypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.976748 dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4695 2023-06-06 19:39:55.000000 dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8551 2023-06-06 19:39:55.000000 dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2023-06-06 19:39:55.000000 dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2023-06-06 19:39:55.000000 dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/entry_points.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      192 2023-06-06 19:39:55.000000 dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/requires.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2023-06-06 19:39:55.000000 dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2023-06-06 19:39:55.977994 dagworks-sdk-0.0.6/tests/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2970 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/tests/test_driver.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     8161 2023-05-29 05:01:18.000000 dagworks-sdk-0.0.6/tests/test_runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/tests/test_telemetry.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6099 2023-05-27 05:25:08.000000 dagworks-sdk-0.0.6/tests/test_tracking.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.253148 dagworks-sdk-0.0.7/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2212 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/LICENSE
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4695 2023-06-19 04:12:43.252996 dagworks-sdk-0.0.7/PKG-INFO
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3655 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/README.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/pyproject.toml
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       14 2023-06-05 16:25:20.000000 dagworks-sdk-0.0.7/requirements-test.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      213 2023-06-05 16:25:20.000000 dagworks-sdk-0.0.7/requirements.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       38 2023-06-19 04:12:43.253192 dagworks-sdk-0.0.7/setup.cfg
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      115 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/setup.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.223899 dagworks-sdk-0.0.7/src/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.225257 dagworks-sdk-0.0.7/src/dagworks/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1092 2023-06-19 04:10:39.000000 dagworks-sdk-0.0.7/src/dagworks/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.227394 dagworks-sdk-0.0.7/src/dagworks/api/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.228436 dagworks-sdk-0.0.7/src/dagworks/api/api_client/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      152 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.228683 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       47 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.229864 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3379 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2926 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5383 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4111 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4813 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.231656 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3035 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5855 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4711 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5053 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4516 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4994 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8029 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5693 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5511 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5779 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6327 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.232473 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4421 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5087 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6058 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6286 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5367 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2817 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/client.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      470 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/errors.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.241297 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4237 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2443 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/api_key_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1982 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/dependency.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2706 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/documentation_asset_in.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1285 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3019 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/documentation_asset_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1268 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2766 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2480 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_function.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3778 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_node.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1692 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_node_dependencies.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1175 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_node_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/organization_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2231 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/paged_api_key_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2238 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/paged_project_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2231 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/paged_run_log_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1649 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/phone_home_result.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1977 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_in.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1179 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_in_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4499 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1165 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_out_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3909 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_in_git.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1241 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_in_git_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1243 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_in_git_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5339 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1203 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1241 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_version_info.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5848 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_with_dag.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1244 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1282 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1422 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/python_type.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1791 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_data.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5416 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1204 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1185 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1171 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in_run_log.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6517 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1173 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1163 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7054 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_with_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1214 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_with_run_config.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1214 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1204 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3710 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/task_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1198 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/task_run_result_summary.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      226 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/task_run_status.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3189 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2916 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1586 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/user_out.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4362 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/visibility_full.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3802 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/visibility_in.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2306 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/who_am_i_result.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      993 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/api_client/types.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     9831 2023-06-19 04:07:36.000000 dagworks-sdk-0.0.7/src/dagworks/api/clients.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1161 2023-06-19 04:07:36.000000 dagworks-sdk-0.0.7/src/dagworks/api/constants.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1311 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/api/projecttypes.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.241773 dagworks-sdk-0.0.7/src/dagworks/cli/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2025 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/cli.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6513 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/initialize.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.241925 dagworks-sdk-0.0.7/src/dagworks/cli/templates/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.242635 dagworks-sdk-0.0.7/src/dagworks/cli/templates/common/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      123 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/common/.env.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      307 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       51 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2698 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      697 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.242788 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.243337 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      351 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      520 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2528 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.243538 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/config/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       26 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.244001 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      232 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      480 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      309 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      678 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.244155 dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.244529 dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1577 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.245000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      157 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      149 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      674 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.245161 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.246143 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      488 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3736 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      598 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2531 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1402 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      477 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.246288 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.247239 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1447 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      369 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      710 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      931 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      744 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.247386 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)   991302 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      679 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    14619 2023-06-19 04:07:36.000000 dagworks-sdk-0.0.7/src/dagworks/driver.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.249776 dagworks-sdk-0.0.7/src/dagworks/parsing/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/parsing/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2394 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/parsing/dagtypes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7810 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/parsing/parse.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.250070 dagworks-sdk-0.0.7/src/dagworks/telemetry/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/telemetry/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7465 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/telemetry/telemetry.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.251762 dagworks-sdk-0.0.7/src/dagworks/tracking/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2227 2023-06-19 04:07:43.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/dataframe_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5969 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/example_tracking.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5239 2023-06-19 04:07:43.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/pandas_col_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4623 2023-06-19 04:07:43.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/pandas_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6039 2023-06-19 04:07:43.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/polars_col_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4481 2023-06-19 04:07:43.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/polars_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8991 2023-06-19 04:07:43.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/runs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1759 2023-06-19 04:07:43.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2411 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/src/dagworks/tracking/trackingtypes.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.252431 dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4695 2023-06-19 04:12:43.000000 dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     8764 2023-06-19 04:12:43.000000 dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2023-06-19 04:12:43.000000 dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       50 2023-06-19 04:12:43.000000 dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      192 2023-06-19 04:12:43.000000 dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/requires.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        9 2023-06-19 04:12:43.000000 dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2023-06-19 04:12:43.252801 dagworks-sdk-0.0.7/tests/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2970 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/tests/test_driver.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3343 2023-06-05 16:25:15.000000 dagworks-sdk-0.0.7/tests/test_telemetry.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6103 2023-06-19 04:07:36.000000 dagworks-sdk-0.0.7/tests/test_tracking.py
```

### Comparing `dagworks-sdk-0.0.6/LICENSE` & `dagworks-sdk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/PKG-INFO` & `dagworks-sdk-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.6/README.md` & `dagworks-sdk-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/pyproject.toml` & `dagworks-sdk-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/__init__.py` & `dagworks-sdk-0.0.7/src/dagworks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = (0, 0, 6)
+__version__ = (0, 0, 7)
```

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/__init__.py` & `dagworks-sdk-0.0.7/src/dagworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_create_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_delete_api_key.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_get_api_keys.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_phone_home.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/auth/trackingserver_api_api_whoami.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_archive_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_create_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_latest_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_project_versions_bulk_by_id.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_get_projects_by_name.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/projects/trackingserver_api_api_update_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_get_runs_from_project_version.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/api/runs/trackingserver_api_api_log_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/client.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/client.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/__init__.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/api_key_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/dependency.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/dependency.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/documentation_asset_in.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/documentation_asset_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/documentation_asset_in_documentation.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/documentation_asset_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/documentation_asset_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/documentation_asset_out_documentation.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_dag.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_function.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_function.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_node.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_node.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_node_dependencies.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_node_dependencies.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/hamilton_node_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/hamilton_node_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/organization_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/organization_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/paged_api_key_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/paged_api_key_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/paged_project_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/paged_project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/paged_run_log_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/paged_run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/phone_home_result.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/phone_home_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_in.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_in_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_out_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_in_git.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_in_git.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_in_git_dag.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_in_git_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_in_git_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_in_git_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_version_info.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_with_dag.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_with_dag.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_with_dag_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/project_version_out_with_dag_version_info.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/python_type.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/python_type.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_data.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_data.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in_config.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in_inputs.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in_run_log.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in_run_log.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_in_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_in_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_config.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_inputs.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_with_run.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_with_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_with_run_config.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_with_run_config.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_with_run_inputs.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/run_log_out_with_run_tags.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/task_run.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/task_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/task_run_result_summary.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/task_run_result_summary.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/trackingserver_api_api_create_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/trackingserver_api_api_update_project_body_params.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/user_out.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/user_out.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/visibility_full.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/visibility_full.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/visibility_in.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/visibility_in.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/models/who_am_i_result.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/models/who_am_i_result.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/api_client/types.py` & `dagworks-sdk-0.0.7/src/dagworks/api/api_client/types.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/clients.py` & `dagworks-sdk-0.0.7/src/dagworks/api/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,23 +102,25 @@
         self,
         dag_run: DAGRun,
         project_version_id: int,
         config: Dict[str, Any],
         tags: Dict[str, str],
         inputs: Dict[str, Any],
         outputs: List[str],
-    ):
+    ) -> int:
         """Logs a DAG run to the DAGWorks API.
 
         :param project_version_id:
         :param dag_run: DAG run to log
         :param config: config used to create DAG
         :param tags: Tags to log with the DAG run
         :param inputs: Inputs used to pass into the DAG
         :param outputs: Outputs used to query the DAG
+
+        :return: Run ID
         """
         pass
 
 
 class BasicDAGWorksClient(DAGWorksClient):
     """Basic no-op DAGWorks client -- mocks out the above DAGWorks client for testing"""
 
@@ -217,15 +219,15 @@
         self,
         dag_run: DAGRun,
         project_version_id: int,
         config: Dict[str, Any],
         tags: Dict[str, str],
         inputs: Dict[str, Any],
         outputs: List[str],
-    ):
+    ) -> int:
         run_log_to_save = RunLogInRunLog()
         run_log_to_save.additional_properties = {
             "tasks": [task.to_dict() for task in dag_run.tasks]
         }
         config_to_save = RunLogInConfig()
         config_to_save.additional_properties = config
         run_log_in_tags = RunLogInTags()
@@ -241,12 +243,13 @@
             end_time=dag_run.end_time,
             run_log_schema_version=dag_run.schema_version,
             run_log=run_log_to_save,
             tags=run_log_in_tags,
             inputs=inputs_to_save,
             outputs=outputs,
         )
-        log_run_log.sync(
+        run_logged = log_run_log.sync(
             client=self.api_client,
             project_version_id=project_version_id,
             json_body=json_body,
         )
+        return run_logged.id
```

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/constants.py` & `dagworks-sdk-0.0.7/src/dagworks/api/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-# DAGWORKS_API_URL = "https://try.dagworks.io/api"
 DAGWORKS_API_URL = "https://api.app.dagworks.io"
+DAGWORKS_UI_URL = "https://app.dagworks.io"
```

### Comparing `dagworks-sdk-0.0.6/src/dagworks/api/projecttypes.py` & `dagworks-sdk-0.0.7/src/dagworks/api/projecttypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/__init__.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/cli.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/initialize.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/common/run.py.jinja2` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/common/run.sh.jinja2` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/components/common.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/components/data_loader.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/components/data_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/data_processing/template_data.json` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/components/transforms.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/hello_world/template_data.json` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/iris_loader.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/iris_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/model_fitting.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/machine_learning/components/models.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json` & `dagworks-sdk-0.0.7/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/driver.py` & `dagworks-sdk-0.0.7/src/dagworks/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -202,14 +202,16 @@
         dag_name: str,
         tags: Dict[str, str] = None,
         client_factory: Callable[
             [str, str, str], clients.DAGWorksClient
         ] = clients.BasicDAGWorksClient,
         adapter: base.HamiltonGraphAdapter = None,
         dagworks_api_url=os.environ.get("DAGWORKS_API_URL", constants.DAGWORKS_API_URL),
+        dagworks_ui_url=constants.DAGWORKS_UI_URL,  # We may want to change this later for
+        # on-prem deploys
     ):
         """Instantiates a DAGWorks driver. This:
         1. Requires a project to exist. Create one via https://app.dagworks.io/dashboard/projects.
         2. Sends over the shape of the DAG.
         3. Sets up execute() run-tracking.
 
         :param config: Configuration to use, same as standard Hamilton driver.
@@ -222,14 +224,15 @@
         :param tags: Optional key value string pairs to help identify and curate this instance of
         the DAG and subsequent execution runs. E.g. {"environment": "production"}.
         Currently all .execute() runs will be tagged with these.
         :param client_factory: Optional. Advanced use. Factory to use to create the underlying
         client.
         :param adapter: Optional. Adapter to use, same as standard Hamilton driver.
         :param dagworks_api_url: Optional. URL to use for the DAGWorks API.
+        :param dagworks_ui_url: Optional. URL to use for the DAGWorks UI.
         """
         super(Driver, self).__init__(config, *modules, adapter=adapter)
         if global_tracker.enabled:
             global_tracker.initialize(
                 username,
                 project=project_id,
                 adapter=get_adapter_representation(self.adapter),
@@ -245,14 +248,15 @@
         self.vcs_info = _derive_version_control_info(self.module_hash)
         self.initialized = False
         self.modules = modules
         self.project_version = None
         self.run_tags = tags if tags is not None else {}
         validate_tags(self.run_tags)
         self.dag_name = dag_name
+        self.dagworks_ui_url = dagworks_ui_url
 
     @global_tracker.track_calls()
     def initialize(self):
         """Initializes the driver. This:
         1. Validates authentication
         2. Creates a project if it does not already exist
         3. Sets initialization as true
@@ -291,16 +295,16 @@
         self,
         final_vars: List[Union[str, Callable]],
         overrides: Dict[str, Any] = None,
         display_graph: bool = False,
         inputs: Dict[str, Any] = None,
     ) -> Any:
         logger.warning(
-            f"\nCapturing execution run. Results can be found at "
-            f"https://app.dagworks.io/dashboard/project/{self.project}/runs\n"
+            f"\nCapturing execution run. All runs for project can be found at "
+            f"{self.dagworks_ui_url}/dashboard/project/{self.project}/runs"
         )
         return super(Driver, self).execute(final_vars, overrides, display_graph, inputs)
 
     @global_tracker.track_calls(
         tracking_generators={
             "final_vars": [("num_vars", safe_len)],
             "overrides": [("num_overrides", safe_len)],
@@ -338,15 +342,19 @@
                 )
                 tracking_state.clock_end(status=Status.SUCCESS)
                 return out
             except Exception as e:
                 tracking_state.clock_end(status=Status.FAILURE)
                 raise e
             finally:
-                self.client.log_dag_run(
+                logged_run = self.client.log_dag_run(
                     tracking_state.get(),
                     self.project_version.id,
                     config=filter_json_dict_to_serializable(self.config),
                     tags=self.run_tags,
                     inputs=filter_json_dict_to_serializable(inputs),
                     outputs=final_vars,
                 )
+                logger.warning(
+                    f"\nCaptured execution run. Results can be found at "
+                    f"{self.dagworks_ui_url}/dashboard/project/{self.project}/runs/{logged_run}\n"
+                )
```

### Comparing `dagworks-sdk-0.0.6/src/dagworks/parsing/__init__.py` & `dagworks-sdk-0.0.7/src/dagworks/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/parsing/dagtypes.py` & `dagworks-sdk-0.0.7/src/dagworks/parsing/dagtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/parsing/parse.py` & `dagworks-sdk-0.0.7/src/dagworks/parsing/parse.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/telemetry/__init__.py` & `dagworks-sdk-0.0.7/src/dagworks/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/telemetry/telemetry.py` & `dagworks-sdk-0.0.7/src/dagworks/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/tracking/__init__.py` & `dagworks-sdk-0.0.7/src/dagworks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/tracking/example_tracking.py` & `dagworks-sdk-0.0.7/src/dagworks/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks/tracking/trackingtypes.py` & `dagworks-sdk-0.0.7/src/dagworks/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/PKG-INFO` & `dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks-sdk-0.0.6/src/dagworks_sdk.egg-info/SOURCES.txt` & `dagworks-sdk-0.0.7/src/dagworks_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -133,20 +133,25 @@
 src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
 src/dagworks/parsing/__init__.py
 src/dagworks/parsing/dagtypes.py
 src/dagworks/parsing/parse.py
 src/dagworks/telemetry/__init__.py
 src/dagworks/telemetry/telemetry.py
 src/dagworks/tracking/__init__.py
+src/dagworks/tracking/dataframe_stats.py
 src/dagworks/tracking/example_tracking.py
+src/dagworks/tracking/pandas_col_stats.py
+src/dagworks/tracking/pandas_stats.py
+src/dagworks/tracking/polars_col_stats.py
+src/dagworks/tracking/polars_stats.py
 src/dagworks/tracking/runs.py
+src/dagworks/tracking/stats.py
 src/dagworks/tracking/trackingtypes.py
 src/dagworks_sdk.egg-info/PKG-INFO
 src/dagworks_sdk.egg-info/SOURCES.txt
 src/dagworks_sdk.egg-info/dependency_links.txt
 src/dagworks_sdk.egg-info/entry_points.txt
 src/dagworks_sdk.egg-info/requires.txt
 src/dagworks_sdk.egg-info/top_level.txt
 tests/test_driver.py
-tests/test_runs.py
 tests/test_telemetry.py
 tests/test_tracking.py
```

### Comparing `dagworks-sdk-0.0.6/tests/test_driver.py` & `dagworks-sdk-0.0.7/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/tests/test_telemetry.py` & `dagworks-sdk-0.0.7/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks-sdk-0.0.6/tests/test_tracking.py` & `dagworks-sdk-0.0.7/tests/test_tracking.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         dag_run: DAGRun,
         project_version_id: int,
         config: Dict[str, Any],
         tags: Dict[str, Any],
         inputs: Dict[str, Any],
         outputs: List[str],
     ):
-        pass
+        return 0
 
 
 def test_tracking_state():
     state = TrackingState("test")
     state.clock_start()
     state.update_task(
         task_name="foo",
```

