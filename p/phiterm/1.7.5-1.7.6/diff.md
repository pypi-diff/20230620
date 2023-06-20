# Comparing `tmp/phiterm-1.7.5.tar.gz` & `tmp/phiterm-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.7.5.tar", last modified: Thu Jun 15 14:44:46 2023, max compression
+gzip compressed data, was "phiterm-1.7.6.tar", last modified: Tue Jun 20 14:07:11 2023, max compression
```

## Comparing `phiterm-1.7.5.tar` & `phiterm-1.7.6.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.667496 phiterm-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-15 14:44:21.000000 phiterm-1.7.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 14:44:46.667496 phiterm-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-15 14:44:21.000000 phiterm-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.647495 phiterm-1.7.5/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.651495 phiterm-1.7.5/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36914 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.655495 phiterm-1.7.5/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.655495 phiterm-1.7.5/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.655495 phiterm-1.7.5/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.655495 phiterm-1.7.5/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.655495 phiterm-1.7.5/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.655495 phiterm-1.7.5/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.655495 phiterm-1.7.5/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.655495 phiterm-1.7.5/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.647495 phiterm-1.7.5/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.659495 phiterm-1.7.5/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.659495 phiterm-1.7.5/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.659495 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.659495 phiterm-1.7.5/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.659495 phiterm-1.7.5/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.663496 phiterm-1.7.5/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/get_python_objects_from_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/prep_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.663496 phiterm-1.7.5/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.663496 phiterm-1.7.5/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    31062 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-15 14:44:21.000000 phiterm-1.7.5/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.647495 phiterm-1.7.5/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-15 14:44:46.000000 phiterm-1.7.5/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-15 14:44:46.000000 phiterm-1.7.5/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:44:46.000000 phiterm-1.7.5/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 14:44:46.000000 phiterm-1.7.5/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-15 14:44:46.000000 phiterm-1.7.5/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 14:44:46.000000 phiterm-1.7.5/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-15 14:44:21.000000 phiterm-1.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:44:46.667496 phiterm-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 14:44:21.000000 phiterm-1.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:44:46.667496 phiterm-1.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-15 14:44:21.000000 phiterm-1.7.5/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.072675 phiterm-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-06-20 14:06:51.000000 phiterm-1.7.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 14:07:11.072675 phiterm-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 14:06:51.000000 phiterm-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.060675 phiterm-1.7.6/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.060675 phiterm-1.7.6/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.060675 phiterm-1.7.6/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.060675 phiterm-1.7.6/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19858 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15784 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.060675 phiterm-1.7.6/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.060675 phiterm-1.7.6/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36914 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.064675 phiterm-1.7.6/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.068675 phiterm-1.7.6/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.060675 phiterm-1.7.6/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.068675 phiterm-1.7.6/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.068675 phiterm-1.7.6/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.068675 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.068675 phiterm-1.7.6/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.068675 phiterm-1.7.6/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.072675 phiterm-1.7.6/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/get_python_objects_from_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/prep_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.072675 phiterm-1.7.6/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.072675 phiterm-1.7.6/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30936 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-06-20 14:06:51.000000 phiterm-1.7.6/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.060675 phiterm-1.7.6/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 14:07:11.000000 phiterm-1.7.6/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 14:07:11.000000 phiterm-1.7.6/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:07:11.000000 phiterm-1.7.6/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-20 14:07:11.000000 phiterm-1.7.6/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-20 14:07:11.000000 phiterm-1.7.6/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 14:07:11.000000 phiterm-1.7.6/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-20 14:06:51.000000 phiterm-1.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:07:11.072675 phiterm-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-20 14:06:51.000000 phiterm-1.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:07:11.072675 phiterm-1.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-20 14:06:51.000000 phiterm-1.7.6/tests/test_backend_api.py
```

### Comparing `phiterm-1.7.5/LICENSE.md` & `phiterm-1.7.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/api/client.py` & `phiterm-1.7.6/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/api/routes.py` & `phiterm-1.7.6/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/api/user.py` & `phiterm-1.7.6/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/api/workspace.py` & `phiterm-1.7.6/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/aws/aws_operator.py` & `phiterm-1.7.6/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/cli/cli_app.py` & `phiterm-1.7.6/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/cli/cli_operator.py` & `phiterm-1.7.6/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/cli/dx/dx_app.py` & `phiterm-1.7.6/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.7.6/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.7.6/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.7.6/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/cli/wf/wf_app.py` & `phiterm-1.7.6/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/cli/ws/ws_app.py` & `phiterm-1.7.6/phiterm/cli/ws/ws_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/conf/auth.py` & `phiterm-1.7.6/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/conf/constants.py` & `phiterm-1.7.6/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/conf/phi_conf.py` & `phiterm-1.7.6/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/databox/databox_operator.py` & `phiterm-1.7.6/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/docker/docker_operator.py` & `phiterm-1.7.6/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/enums/user.py` & `phiterm-1.7.6/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/k8s/k8s_operator.py` & `phiterm-1.7.6/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.7.6/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.7.6/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.7.6/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.7.6/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/local/local_operator.py` & `phiterm-1.7.6/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/release/release_schemas.py` & `phiterm-1.7.6/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/release/ws_releases.py` & `phiterm-1.7.6/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/schemas/user.py` & `phiterm-1.7.6/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/schemas/user_schemas.py` & `phiterm-1.7.6/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/schemas/workspace.py` & `phiterm-1.7.6/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.7.6/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.7.6/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.7.6/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.7.6/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.7.6/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.7.6/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.7.6/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.7.6/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/cli_auth_server.py` & `phiterm-1.7.6/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/cli_console.py` & `phiterm-1.7.6/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/common.py` & `phiterm-1.7.6/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/dttm.py` & `phiterm-1.7.6/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/enums.py` & `phiterm-1.7.6/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/filesystem.py` & `phiterm-1.7.6/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/get_python_objects_from_module.py` & `phiterm-1.7.6/phiterm/utils/get_python_objects_from_module.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/git.py` & `phiterm-1.7.6/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/load_env.py` & `phiterm-1.7.6/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/log.py` & `phiterm-1.7.6/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/prep_infra_config.py` & `phiterm-1.7.6/phiterm/utils/prep_infra_config.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/pyproject.py` & `phiterm-1.7.6/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/utils/ws_filter.py` & `phiterm-1.7.6/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/workflow/wf_operator.py` & `phiterm-1.7.6/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/workflow/wf_utils.py` & `phiterm-1.7.6/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/workspace/phi_ws_data.py` & `phiterm-1.7.6/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/workspace/ws_enums.py` & `phiterm-1.7.6/phiterm/workspace/ws_enums.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 class WorkspaceVisibilityEnum(ExtendedEnum):
     PRIVATE = "PRIVATE"
     PUBLIC = "PUBLIC"
 
 
 class WorkspaceStarterTemplate(ExtendedEnum):
-    ai_app = "ai-app"
     ml_app = "ml-app"
     api_app = "api-app"
     llm_app = "llm-app"
     django_app = "django-app"
     streamlit_app = "streamlit-app"
     aws_dp = "data-platform"
     aws_spark_dp = "spark-data-platform"
```

### Comparing `phiterm-1.7.5/phiterm/workspace/ws_loader.py` & `phiterm-1.7.6/phiterm/workspace/ws_loader.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/workspace/ws_operator.py` & `phiterm-1.7.6/phiterm/workspace/ws_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,26 +21,24 @@
     WorkspaceConfigType,
     WorkspaceStarterTemplate,
 )
 from phiterm.workspace.exceptions import WorkspaceException
 from phiterm.utils.prep_infra_config import filter_and_prep_configs
 
 TEMPLATE_TO_NAME_MAP: Dict[WorkspaceStarterTemplate, str] = {
-    WorkspaceStarterTemplate.ai_app: "ai-app",
     WorkspaceStarterTemplate.ml_app: "ml-app",
     WorkspaceStarterTemplate.api_app: "api-app",
     WorkspaceStarterTemplate.llm_app: "llm-app",
     WorkspaceStarterTemplate.django_app: "django-app",
     WorkspaceStarterTemplate.streamlit_app: "streamlit-app",
     WorkspaceStarterTemplate.aws_dp: "data-platform",
     WorkspaceStarterTemplate.aws_spark_dp: "spark-data-platform",
     WorkspaceStarterTemplate.aws_snowflake_dp: "snowflake-data-platform",
 }
 TEMPLATE_TO_REPO_MAP: Dict[WorkspaceStarterTemplate, str] = {
-    WorkspaceStarterTemplate.ai_app: "https://github.com/phidatahq/ai-app.git",
     WorkspaceStarterTemplate.ml_app: "https://github.com/phidatahq/ml-app.git",
     WorkspaceStarterTemplate.api_app: "https://github.com/phidatahq/api-app.git",
     WorkspaceStarterTemplate.llm_app: "https://github.com/phidatahq/llm-app.git",
     WorkspaceStarterTemplate.django_app: "https://github.com/phidatahq/django-app.git",
     WorkspaceStarterTemplate.streamlit_app: "https://github.com/phidatahq/streamlit-app.git",
     WorkspaceStarterTemplate.aws_dp: "https://github.com/phidatahq/aws-dp-template.git",
     WorkspaceStarterTemplate.aws_spark_dp: "https://github.com/phidatahq/aws-spark-dp-template.git",
@@ -92,15 +90,15 @@
         template_choices = [str(idx) for idx, _ in enumerate(templates, start=1)]
         template_inp_raw = Prompt.ask(
             "Template Number", choices=template_choices, default="1", show_choices=False
         )
         # Convert input to int value.
         template_inp = str_to_int(template_inp_raw)
 
-        ws_template = WorkspaceStarterTemplate.ai_app
+        ws_template = WorkspaceStarterTemplate.llm_app
         if template_inp is not None:
             try:
                 ws_template = cast(
                     WorkspaceStarterTemplate,
                     WorkspaceStarterTemplate.from_str(templates[template_inp - 1]),
                 )
             except Exception as e:
```

### Comparing `phiterm-1.7.5/phiterm/workspace/ws_schemas.py` & `phiterm-1.7.6/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm/workspace/ws_utils.py` & `phiterm-1.7.6/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/phiterm.egg-info/SOURCES.txt` & `phiterm-1.7.6/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.7.5/pyproject.toml` & `phiterm-1.7.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.7.5"
+version = "1.7.6"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

