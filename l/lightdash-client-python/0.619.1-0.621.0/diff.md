# Comparing `tmp/lightdash_client_python-0.619.1.tar.gz` & `tmp/lightdash_client_python-0.621.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_client_python-0.619.1.tar", last modified: Mon Jun 19 12:41:42 2023, max compression
+gzip compressed data, was "lightdash_client_python-0.621.0.tar", last modified: Tue Jun 20 02:56:56 2023, max compression
```

## Comparing `lightdash_client_python-0.619.1.tar` & `lightdash_client_python-0.621.0.tar`

### file list

```diff
@@ -1,289 +1,1128 @@
--rw-r--r--   0        0        0      804 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      402 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/workflows/contributors-list.yml
--rw-r--r--   0        0        0     1849 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2335 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0     1115 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     3078 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.gitignore
--rw-r--r--   0        0        0     1040 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.openapi-generator-ignore
--rw-r--r--   0        0        0     6821 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.openapi-generator/FILES
--rw-r--r--   0        0        0        6 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.openapi-generator/VERSION
--rw-r--r--   0        0        0     1375 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    14088 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.pylintrc
--rw-r--r--   0        0        0      150 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.pypirc
--rw-r--r--   0        0        0        8 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.python-version
--rw-r--r--   0        0        0       32 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/.style.yapf
--rw-r--r--   0        0        0    11357 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/LICENSE
--rw-r--r--   0        0        0      717 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/Makefile
--rw-r--r--   0        0        0     3258 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/README.md
--rwxr-xr-x   0        0        0     1121 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/clean.sh
--rw-r--r--   0        0        0     2115 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/generate_clients.sh
--rw-r--r--   0        0        0      974 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/lint.sh
--rw-r--r--   0        0        0      211 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/openapi-python-client.yml
--rwxr-xr-x   0        0        0     1391 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/publish.sh
--rw-r--r--   0        0        0      152 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/schemas/README.md
--rw-r--r--   0        0        0     1299 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/schemas/download.sh
--rw-r--r--   0        0        0   233795 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/schemas/swagger.json
--rwxr-xr-x   0        0        0     1023 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/setup.sh
--rwxr-xr-x   0        0        0      958 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/dev/test_python.sh
--rw-r--r--   0        0        0      201 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/__init__.py
--rw-r--r--   0        0        0       47 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/charts/__init__.py
--rw-r--r--   0        0        0     4680 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/charts/post_chart_results.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/content/__init__.py
--rw-r--r--   0        0        0     4483 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/content/get_pinned_items.py
--rw-r--r--   0        0        0     5511 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/content/update_pinned_items_order.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exploring/__init__.py
--rw-r--r--   0        0        0     5017 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exploring/post_run_query.py
--rw-r--r--   0        0        0     5095 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exploring/post_run_underlying_data_query.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exports/__init__.py
--rw-r--r--   0        0        0     3848 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/exports/get_csv_url.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/__init__.py
--rw-r--r--   0        0        0     4403 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     2743 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     4847 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
--rw-r--r--   0        0        0     3651 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_slack_channels.py
--rw-r--r--   0        0        0     2734 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/__init__.py
--rw-r--r--   0        0        0     2573 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/create_email_one_time_passcode.py
--rw-r--r--   0        0        0     3501 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/delete_me.py
--rw-r--r--   0        0        0     3021 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/get_email_verification_status.py
--rw-r--r--   0        0        0     4793 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/join_organization.py
--rw-r--r--   0        0        0     4349 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/my_account/list_my_available_organizations.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/__init__.py
--rw-r--r--   0        0        0     4634 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/create_group_in_organization.py
--rw-r--r--   0        0        0     4256 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/delete_my_organization.py
--rw-r--r--   0        0        0     4057 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/delete_organization_member.py
--rw-r--r--   0        0        0     3589 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/get_my_organization.py
--rw-r--r--   0        0        0     3739 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_groups_in_organization.py
--rw-r--r--   0        0        0     3983 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_email_domains.py
--rw-r--r--   0        0        0     3859 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_members.py
--rw-r--r--   0        0        0     3771 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_projects.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/__init__.py
--rw-r--r--   0        0        0     4691 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/delete_validation_dismiss.py
--rw-r--r--   0        0        0     5756 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/get_latest_validation_results.py
--rw-r--r--   0        0        0     2639 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/get_project.py
--rw-r--r--   0        0        0     4187 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/list_charts_in_project.py
--rw-r--r--   0        0        0     4187 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/list_spaces_in_project.py
--rw-r--r--   0        0        0     6428 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/projects/validate_project.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/__init__.py
--rw-r--r--   0        0        0     2984 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/create_space_in_project.py
--rw-r--r--   0        0        0     4928 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/get_project_access_list.py
--rw-r--r--   0        0        0     4648 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
--rw-r--r--   0        0        0     4425 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
--rw-r--r--   0        0        0     4794 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
--rw-r--r--   0        0        0     5062 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/update_organization_member.py
--rw-r--r--   0        0        0     5026 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/update_project_access_for_user.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/__init__.py
--rw-r--r--   0        0        0     4176 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/delete_scheduler.py
--rw-r--r--   0        0        0     4147 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduled_jobs.py
--rw-r--r--   0        0        0     2633 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler.py
--rw-r--r--   0        0        0     4201 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler_job_status.py
--rw-r--r--   0        0        0     2620 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler_logs.py
--rw-r--r--   0        0        0     2919 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/schedulers/update_scheduler.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/share_links/__init__.py
--rw-r--r--   0        0        0     3960 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/share_links/get_share_url.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/spaces/__init__.py
--rw-r--r--   0        0        0     4429 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/spaces/delete_space.py
--rw-r--r--   0        0        0     2881 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/spaces/get_space.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/ssh_keypairs/__init__.py
--rw-r--r--   0        0        0     3542 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
--rw-r--r--   0        0        0        0 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/__init__.py
--rw-r--r--   0        0        0     4365 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/add_user_to_group.py
--rw-r--r--   0        0        0     3927 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/delete_group.py
--rw-r--r--   0        0        0     3949 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/get_group.py
--rw-r--r--   0        0        0     4073 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/get_group_members.py
--rw-r--r--   0        0        0     4348 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/api/user_groups/remove_user_from_group.py
--rw-r--r--   0        0        0     2906 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/client.py
--rw-r--r--   0        0        0      470 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/errors.py
--rw-r--r--   0        0        0    20611 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/__init__.py
--rw-r--r--   0        0        0     4166 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/additional_metric.py
--rw-r--r--   0        0        0     2422 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/allowed_email_domains.py
--rw-r--r--   0        0        0     2410 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_chart_summary_list_response.py
--rw-r--r--   0        0        0      152 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_chart_summary_list_response_status.py
--rw-r--r--   0        0        0     2106 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response.py
--rw-r--r--   0        0        0     1652 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response_results.py
--rw-r--r--   0        0        0      142 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response_status.py
--rw-r--r--   0        0        0     2254 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_metrics.py
--rw-r--r--   0        0        0      143 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_metrics_status.py
--rw-r--r--   0        0        0     2119 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
--rw-r--r--   0        0        0      157 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
--rw-r--r--   0        0        0      147 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_email_status_response_status.py
--rw-r--r--   0        0        0     2139 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload.py
--rw-r--r--   0        0        0     2386 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload_error.py
--rw-r--r--   0        0        0      146 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload_status.py
--rw-r--r--   0        0        0     2285 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_list_response.py
--rw-r--r--   0        0        0      145 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_list_response_status.py
--rw-r--r--   0        0        0     2359 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_members_response.py
--rw-r--r--   0        0        0      148 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_members_response_status.py
--rw-r--r--   0        0        0     1951 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_response.py
--rw-r--r--   0        0        0      141 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_group_response_status.py
--rw-r--r--   0        0        0     2208 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response.py
--rw-r--r--   0        0        0     1548 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response_results.py
--rw-r--r--   0        0        0      148 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response_status.py
--rw-r--r--   0        0        0     2157 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response.py
--rw-r--r--   0        0        0     1535 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response_results.py
--rw-r--r--   0        0        0      145 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response_status.py
--rw-r--r--   0        0        0     2019 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization.py
--rw-r--r--   0        0        0     2241 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_allowed_email_domains.py
--rw-r--r--   0        0        0      159 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_allowed_email_domains_status.py
--rw-r--r--   0        0        0     2270 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profile.py
--rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profile_status.py
--rw-r--r--   0        0        0     2519 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profiles.py
--rw-r--r--   0        0        0      154 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profiles_status.py
--rw-r--r--   0        0        0     2456 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_projects.py
--rw-r--r--   0        0        0      148 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_projects_status.py
--rw-r--r--   0        0        0      140 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_organization_status.py
--rw-r--r--   0        0        0     4825 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_pinned_items.py
--rw-r--r--   0        0        0      139 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_pinned_items_status.py
--rw-r--r--   0        0        0     2478 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_project_access_list_response.py
--rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_project_access_list_response_status.py
--rw-r--r--   0        0        0      143 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_project_response_status.py
--rw-r--r--   0        0        0     2140 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response.py
--rw-r--r--   0        0        0     2051 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response_results.py
--rw-r--r--   0        0        0      144 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response_status.py
--rw-r--r--   0        0        0     2383 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_scheduled_jobs_response.py
--rw-r--r--   0        0        0      149 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_scheduled_jobs_response_status.py
--rw-r--r--   0        0        0      155 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_scheduler_and_targets_response_status.py
--rw-r--r--   0        0        0      149 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_scheduler_logs_response_status.py
--rw-r--r--   0        0        0     2129 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_share_response.py
--rw-r--r--   0        0        0      141 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_share_response_status.py
--rw-r--r--   0        0        0     2376 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_slack_channels_response.py
--rw-r--r--   0        0        0      149 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_slack_channels_response_status.py
--rw-r--r--   0        0        0      141 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_space_response_status.py
--rw-r--r--   0        0        0     2410 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_space_summary_list_response.py
--rw-r--r--   0        0        0      152 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_space_summary_list_response_status.py
--rw-r--r--   0        0        0     2208 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_ssh_key_pair_response.py
--rw-r--r--   0        0        0      146 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_ssh_key_pair_response_status.py
--rw-r--r--   0        0        0     1937 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_success_empty.py
--rw-r--r--   0        0        0      140 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_success_empty_status.py
--rw-r--r--   0        0        0     2569 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_user_allowed_organizations_response.py
--rw-r--r--   0        0        0      160 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_user_allowed_organizations_response_status.py
--rw-r--r--   0        0        0     4732 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_validate_response.py
--rw-r--r--   0        0        0      144 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_validate_response_status.py
--rw-r--r--   0        0        0     1737 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_validation_dismiss_response.py
--rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/api_validation_dismiss_response_status.py
--rw-r--r--   0        0        0      316 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/chart_kind.py
--rw-r--r--   0        0        0     3776 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/chart_summary.py
--rw-r--r--   0        0        0      192 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/chart_type.py
--rw-r--r--   0        0        0      220 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/compact.py
--rw-r--r--   0        0        0      272 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/compact_or_alias_type_1.py
--rw-r--r--   0        0        0     1937 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/create_project_member.py
--rw-r--r--   0        0        0     2646 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/create_space.py
--rw-r--r--   0        0        0     3745 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_azure_dev_ops_project_config.py
--rw-r--r--   0        0        0     3814 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_bit_bucket_project_config.py
--rw-r--r--   0        0        0     2425 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_ide_project_config.py
--rw-r--r--   0        0        0     2229 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
--rw-r--r--   0        0        0     2494 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_metric.py
--rw-r--r--   0        0        0     3603 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_github_project_config.py
--rw-r--r--   0        0        0     3603 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_gitlab_project_config.py
--rw-r--r--   0        0        0     2957 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_local_project_config.py
--rw-r--r--   0        0        0     2733 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_none_project_config.py
--rw-r--r--   0        0        0     1664 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_environment_variable.py
--rw-r--r--   0        0        0      295 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type.py
--rw-r--r--   0        0        0      164 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_azuredevops.py
--rw-r--r--   0        0        0      156 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_bitbucket.py
--rw-r--r--   0        0        0      138 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_dbt.py
--rw-r--r--   0        0        0      166 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_dbtcloudide.py
--rw-r--r--   0        0        0      147 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_github.py
--rw-r--r--   0        0        0      147 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_gitlab.py
--rw-r--r--   0        0        0      141 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_type_none.py
--rw-r--r--   0        0        0     2051 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/delete_scheduler_response_201.py
--rw-r--r--   0        0        0      151 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/delete_scheduler_response_201_status.py
--rw-r--r--   0        0        0     2003 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/email_one_time_password.py
--rw-r--r--   0        0        0     2749 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/email_one_time_password_expiring.py
--rw-r--r--   0        0        0     2458 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/email_status.py
--rw-r--r--   0        0        0     1664 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/filter_group_response_type_0.py
--rw-r--r--   0        0        0     1674 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/filter_group_response_type_1.py
--rw-r--r--   0        0        0     4615 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/filters.py
--rw-r--r--   0        0        0     2247 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/group.py
--rw-r--r--   0        0        0     2163 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/group_member.py
--rw-r--r--   0        0        0     4963 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/metric_query_response.py
--rw-r--r--   0        0        0      383 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/metric_type.py
--rw-r--r--   0        0        0     2812 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization.py
--rw-r--r--   0        0        0     3539 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization_member_profile.py
--rw-r--r--   0        0        0     1670 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization_member_profile_update.py
--rw-r--r--   0        0        0      287 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization_member_role.py
--rw-r--r--   0        0        0     1991 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/organization_project.py
--rw-r--r--   0        0        0     2377 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
--rw-r--r--   0        0        0     2628 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/partial_pick_space_is_private_or_access.py
--rw-r--r--   0        0        0     2493 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
--rw-r--r--   0        0        0     6235 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0      267 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
--rw-r--r--   0        0        0     3905 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1841 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
--rw-r--r--   0        0        0     1565 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_group_name.py
--rw-r--r--   0        0        0     6859 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     6610 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     5207 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     3761 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     6625 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1532 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_group_name.py
--rw-r--r--   0        0        0     1566 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_organization_name.py
--rw-r--r--   0        0        0     2016 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     3781 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
--rw-r--r--   0        0        0     4585 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1757 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_share_url_path_or_params.py
--rw-r--r--   0        0        0     1502 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_name.py
--rw-r--r--   0        0        0     1768 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_name_or_is_private.py
--rw-r--r--   0        0        0     2609 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
--rw-r--r--   0        0        0     3420 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
--rw-r--r--   0        0        0     1601 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_space_share_user_uuid.py
--rw-r--r--   0        0        0     1619 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_ssh_key_pair_public_key.py
--rw-r--r--   0        0        0     3860 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
--rw-r--r--   0        0        0     2266 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
--rw-r--r--   0        0        0     2095 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/post_chart_results_json_body.py
--rw-r--r--   0        0        0     2540 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/project_member_profile.py
--rw-r--r--   0        0        0      260 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/project_member_role.py
--rw-r--r--   0        0        0      164 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/project_type.py
--rw-r--r--   0        0        0     1294 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/record_string_any.py
--rw-r--r--   0        0        0      193 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_item_type.py
--rw-r--r--   0        0        0      150 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_item_type_chart.py
--rw-r--r--   0        0        0      162 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_item_type_dashboard.py
--rw-r--r--   0        0        0      150 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_item_type_space.py
--rw-r--r--   0        0        0     2093 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_space_item.py
--rw-r--r--   0        0        0     3903 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/resource_view_space_item_data.py
--rw-r--r--   0        0        0     5334 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/run_query_request.py
--rw-r--r--   0        0        0     1933 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/run_query_request_filters.py
--rw-r--r--   0        0        0     1661 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduled_jobs.py
--rw-r--r--   0        0        0     4958 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_base.py
--rw-r--r--   0        0        0     2484 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_csv_options.py
--rw-r--r--   0        0        0      170 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_csv_options_limit_type_1.py
--rw-r--r--   0        0        0     2685 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_email_target.py
--rw-r--r--   0        0        0      156 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_format.py
--rw-r--r--   0        0        0     1272 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_image_options.py
--rw-r--r--   0        0        0      223 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_job_status.py
--rw-r--r--   0        0        0     5049 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_log.py
--rw-r--r--   0        0        0      167 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_log_target_type.py
--rw-r--r--   0        0        0      443 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_log_task.py
--rw-r--r--   0        0        0     2665 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/scheduler_slack_target.py
--rw-r--r--   0        0        0     3505 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/share_url.py
--rw-r--r--   0        0        0     1553 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/slack_channel.py
--rw-r--r--   0        0        0     1658 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/sort_field.py
--rw-r--r--   0        0        0     2115 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/space_share.py
--rw-r--r--   0        0        0     2480 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/space_summary.py
--rw-r--r--   0        0        0     2119 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/table_calculation.py
--rw-r--r--   0        0        0     2350 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/update_pinned_item_order.py
--rw-r--r--   0        0        0     1582 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/update_project_member.py
--rw-r--r--   0        0        0     1173 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/updated_by_user.py
--rw-r--r--   0        0        0     1993 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/user_allowed_organization.py
--rw-r--r--   0        0        0     1964 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validate_project_json_body.py
--rw-r--r--   0        0        0     6492 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_error_chart_response.py
--rw-r--r--   0        0        0     5966 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_error_dashboard_response.py
--rw-r--r--   0        0        0      260 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_error_type.py
--rw-r--r--   0        0        0     3709 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_response_base.py
--rw-r--r--   0        0        0      193 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/validation_source_type.py
--rw-r--r--   0        0        0     2633 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/view_statistics.py
--rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_bigquery.py
--rw-r--r--   0        0        0      159 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_databricks.py
--rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_postgres.py
--rw-r--r--   0        0        0      153 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_redshift.py
--rw-r--r--   0        0        0      156 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_snowflake.py
--rw-r--r--   0        0        0      144 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/warehouse_types_trino.py
--rw-r--r--   0        0        0      225 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/models/week_day.py
--rw-r--r--   0        0        0       26 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/py.typed
--rw-r--r--   0        0        0     1101 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/lightdash_client/types.py
--rw-r--r--   0        0        0     1624 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/pyproject.toml
--rw-r--r--   0        0        0      830 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/setup.py
--rw-r--r--   0        0        0      796 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/tests/__init__.py
--rw-r--r--   0        0        0      908 2023-06-19 12:41:42.000000 lightdash_client_python-0.619.1/tests/test_dummy.py
--rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.619.1/PKG-INFO
+-rw-r--r--   0        0        0      804 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      402 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.github/workflows/contributors-list.yml
+-rw-r--r--   0        0        0     1849 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2335 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0     1115 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3078 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.gitignore
+-rw-r--r--   0        0        0     1040 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.openapi-generator-ignore
+-rw-r--r--   0        0        0     1375 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    14088 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.pylintrc
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.pypirc
+-rw-r--r--   0        0        0        8 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.python-version
+-rw-r--r--   0        0        0       32 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/.style.yapf
+-rw-r--r--   0        0        0    11357 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/LICENSE
+-rw-r--r--   0        0        0     1079 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/Makefile
+-rw-r--r--   0        0        0     3258 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/README.md
+-rwxr-xr-x   0        0        0     1121 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/clean.sh
+-rw-r--r--   0        0        0      599 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/dereference_swagger_json.sh
+-rw-r--r--   0        0        0      521 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/download_swagger_json.sh
+-rw-r--r--   0        0        0     2128 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/generate_clients.sh
+-rw-r--r--   0        0        0      974 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/lint.sh
+-rw-r--r--   0        0        0      211 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/openapi-python-client.yml
+-rwxr-xr-x   0        0        0     1391 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/publish.sh
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/schemas/README.md
+-rw-r--r--   0        0        0   855477 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/schemas/dereferenced-swagger.json
+-rw-r--r--   0        0        0   235202 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/schemas/swagger.json
+-rwxr-xr-x   0        0        0     1023 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/setup.sh
+-rwxr-xr-x   0        0        0      958 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/dev/test_python.sh
+-rw-r--r--   0        0        0      111 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/docker/swagger-cli/Dockerfile
+-rw-r--r--   0        0        0       74 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/docker/swagger-cli/README.md
+-rw-r--r--   0        0        0      201 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/charts/__init__.py
+-rw-r--r--   0        0        0     4785 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/charts/post_chart_results.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/content/__init__.py
+-rw-r--r--   0        0        0     4628 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/content/get_pinned_items.py
+-rw-r--r--   0        0        0     5907 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/content/update_pinned_items_order.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/exploring/__init__.py
+-rw-r--r--   0        0        0     5259 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/exploring/post_run_query.py
+-rw-r--r--   0        0        0     5677 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/exploring/post_run_underlying_data_query.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/exports/__init__.py
+-rw-r--r--   0        0        0     3888 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/exports/get_csv_url.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/integrations/__init__.py
+-rw-r--r--   0        0        0     4572 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4538 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4992 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     3691 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/integrations/get_slack_channels.py
+-rw-r--r--   0        0        0     4570 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/my_account/__init__.py
+-rw-r--r--   0        0        0     4242 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/my_account/create_email_one_time_passcode.py
+-rw-r--r--   0        0        0     3554 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/my_account/delete_me.py
+-rw-r--r--   0        0        0     4835 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/my_account/get_email_verification_status.py
+-rw-r--r--   0        0        0     4950 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/my_account/join_organization.py
+-rw-r--r--   0        0        0     4402 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/my_account/list_my_available_organizations.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/__init__.py
+-rw-r--r--   0        0        0     5053 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/create_group_in_organization.py
+-rw-r--r--   0        0        0     5133 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/create_organization.py
+-rw-r--r--   0        0        0     4466 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/delete_my_organization.py
+-rw-r--r--   0        0        0     4319 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/delete_organization_member.py
+-rw-r--r--   0        0        0     3761 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/get_my_organization.py
+-rw-r--r--   0        0        0     3936 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/list_groups_in_organization.py
+-rw-r--r--   0        0        0     4049 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/list_organization_email_domains.py
+-rw-r--r--   0        0        0     3925 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/list_organization_members.py
+-rw-r--r--   0        0        0     3929 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/list_organization_projects.py
+-rw-r--r--   0        0        0     4681 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/update_my_organization.py
+-rw-r--r--   0        0        0     5263 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/organizations/update_organization_email_domains.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     4770 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/projects/delete_validation_dismiss.py
+-rw-r--r--   0        0        0     5993 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/projects/get_latest_validation_results.py
+-rw-r--r--   0        0        0     4113 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/projects/get_project.py
+-rw-r--r--   0        0        0     4227 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/projects/list_charts_in_project.py
+-rw-r--r--   0        0        0     4227 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/projects/list_spaces_in_project.py
+-rw-r--r--   0        0        0     6467 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/projects/validate_project.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/__init__.py
+-rw-r--r--   0        0        0     5622 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/add_space_share_to_user.py
+-rw-r--r--   0        0        0     4973 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/create_space_in_project.py
+-rw-r--r--   0        0        0     4968 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/get_project_access_list.py
+-rw-r--r--   0        0        0     5059 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
+-rw-r--r--   0        0        0     4715 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
+-rw-r--r--   0        0        0     5058 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
+-rw-r--r--   0        0        0     5274 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/update_organization_member.py
+-rw-r--r--   0        0        0     5485 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/update_project_access_for_user.py
+-rw-r--r--   0        0        0     5407 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/update_space.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/schedulers/__init__.py
+-rw-r--r--   0        0        0     4176 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/schedulers/delete_scheduler.py
+-rw-r--r--   0        0        0     4187 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/schedulers/get_scheduled_jobs.py
+-rw-r--r--   0        0        0     4117 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/schedulers/get_scheduler.py
+-rw-r--r--   0        0        0     4359 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/schedulers/get_scheduler_job_status.py
+-rw-r--r--   0        0        0     4147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/schedulers/get_scheduler_logs.py
+-rw-r--r--   0        0        0     4651 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/schedulers/update_scheduler.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/share_links/__init__.py
+-rw-r--r--   0        0        0     4723 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/share_links/create_share_url.py
+-rw-r--r--   0        0        0     4040 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/share_links/get_share_url.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/spaces/__init__.py
+-rw-r--r--   0        0        0     4521 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/spaces/delete_space.py
+-rw-r--r--   0        0        0     4499 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/spaces/get_space.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/ssh_keypairs/__init__.py
+-rw-r--r--   0        0        0     3621 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
+-rw-r--r--   0        0        0        0 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/user_groups/__init__.py
+-rw-r--r--   0        0        0     4498 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/user_groups/add_user_to_group.py
+-rw-r--r--   0        0        0     4019 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/user_groups/delete_group.py
+-rw-r--r--   0        0        0     3989 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/user_groups/get_group.py
+-rw-r--r--   0        0        0     4113 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/user_groups/get_group_members.py
+-rw-r--r--   0        0        0     4546 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/user_groups/remove_user_from_group.py
+-rw-r--r--   0        0        0     4921 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/api/user_groups/update_group.py
+-rw-r--r--   0        0        0     2906 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/client.py
+-rw-r--r--   0        0        0      470 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/errors.py
+-rw-r--r--   0        0        0   154171 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/__init__.py
+-rw-r--r--   0        0        0     1550 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/add_space_share.py
+-rw-r--r--   0        0        0     1632 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/add_space_share_to_user_json_body.py
+-rw-r--r--   0        0        0     2103 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/add_space_share_to_user_response_200.py
+-rw-r--r--   0        0        0      155 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/add_space_share_to_user_response_200_status.py
+-rw-r--r--   0        0        0     2049 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/add_user_to_group_response_200.py
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/add_user_to_group_response_200_status.py
+-rw-r--r--   0        0        0     4960 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/additional_metric.py
+-rw-r--r--   0        0        0      241 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/additional_metric_compact_type_0.py
+-rw-r--r--   0        0        0      281 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/additional_metric_compact_type_1.py
+-rw-r--r--   0        0        0      393 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/additional_metric_type.py
+-rw-r--r--   0        0        0     2428 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/allowed_email_domains.py
+-rw-r--r--   0        0        0      288 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/allowed_email_domains_role.py
+-rw-r--r--   0        0        0     2602 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_chart_summary_list_response.py
+-rw-r--r--   0        0        0     4165 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_chart_summary_list_response_results_item.py
+-rw-r--r--   0        0        0      230 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_chart_summary_list_response_results_item_chart_type.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_chart_summary_list_response_status.py
+-rw-r--r--   0        0        0     2106 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_csv_url_response.py
+-rw-r--r--   0        0        0     1652 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_csv_url_response_results.py
+-rw-r--r--   0        0        0      142 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_csv_url_response_status.py
+-rw-r--r--   0        0        0     2852 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     1809 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_integration_settings_results.py
+-rw-r--r--   0        0        0      155 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_integration_settings_status.py
+-rw-r--r--   0        0        0     2212 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     2373 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_metrics_results.py
+-rw-r--r--   0        0        0     2616 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py
+-rw-r--r--   0        0        0      143 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_metrics_status.py
+-rw-r--r--   0        0        0     2119 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
+-rw-r--r--   0        0        0      157 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
+-rw-r--r--   0        0        0     2289 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_email_status_response.py
+-rw-r--r--   0        0        0     2794 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_email_status_response_results.py
+-rw-r--r--   0        0        0     2885 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_email_status_response_results_otp.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_email_status_response_status.py
+-rw-r--r--   0        0        0     2139 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_error_payload.py
+-rw-r--r--   0        0        0     2386 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_error_payload_error.py
+-rw-r--r--   0        0        0      146 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_error_payload_status.py
+-rw-r--r--   0        0        0     2477 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_list_response.py
+-rw-r--r--   0        0        0     2392 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_list_response_results_item.py
+-rw-r--r--   0        0        0      145 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_list_response_status.py
+-rw-r--r--   0        0        0     2528 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_members_response.py
+-rw-r--r--   0        0        0     2290 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_members_response_results_item.py
+-rw-r--r--   0        0        0      148 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_members_response_status.py
+-rw-r--r--   0        0        0     2083 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_response.py
+-rw-r--r--   0        0        0     2346 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_response_results.py
+-rw-r--r--   0        0        0      141 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_group_response_status.py
+-rw-r--r--   0        0        0     2208 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_job_scheduled_response.py
+-rw-r--r--   0        0        0     1548 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_job_scheduled_response_results.py
+-rw-r--r--   0        0        0      148 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_job_scheduled_response_status.py
+-rw-r--r--   0        0        0     2157 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_job_status_response.py
+-rw-r--r--   0        0        0     1535 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_job_status_response_results.py
+-rw-r--r--   0        0        0      145 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_job_status_response_status.py
+-rw-r--r--   0        0        0     2093 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization.py
+-rw-r--r--   0        0        0     2401 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_allowed_email_domains.py
+-rw-r--r--   0        0        0     2660 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_allowed_email_domains_results.py
+-rw-r--r--   0        0        0      310 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_allowed_email_domains_results_role.py
+-rw-r--r--   0        0        0      159 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_allowed_email_domains_status.py
+-rw-r--r--   0        0        0     2344 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profile.py
+-rw-r--r--   0        0        0     3724 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profile_results.py
+-rw-r--r--   0        0        0      304 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profile_results_role.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profile_status.py
+-rw-r--r--   0        0        0     2630 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profiles.py
+-rw-r--r--   0        0        0     3778 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profiles_results_item.py
+-rw-r--r--   0        0        0      309 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profiles_results_item_role.py
+-rw-r--r--   0        0        0      154 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profiles_status.py
+-rw-r--r--   0        0        0     2567 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_projects.py
+-rw-r--r--   0        0        0     2214 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_projects_results_item.py
+-rw-r--r--   0        0        0      191 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_projects_results_item_type.py
+-rw-r--r--   0        0        0      148 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_projects_status.py
+-rw-r--r--   0        0        0     2868 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_results.py
+-rw-r--r--   0        0        0      140 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_organization_status.py
+-rw-r--r--   0        0        0     4572 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items.py
+-rw-r--r--   0        0        0     2327 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_0.py
+-rw-r--r--   0        0        0     7188 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1325 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2279 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      167 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2327 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_1.py
+-rw-r--r--   0        0        0     8030 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_1_data.py
+-rw-r--r--   0        0        0      350 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1325 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2279 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      159 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2264 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_2.py
+-rw-r--r--   0        0        0     3957 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_2_data.py
+-rw-r--r--   0        0        0      159 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_2_type.py
+-rw-r--r--   0        0        0      139 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_status.py
+-rw-r--r--   0        0        0     2619 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_access_list_response.py
+-rw-r--r--   0        0        0     2782 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_access_list_response_results_item.py
+-rw-r--r--   0        0        0      286 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_access_list_response_results_item_role.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_access_list_response_status.py
+-rw-r--r--   0        0        0     2117 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response.py
+-rw-r--r--   0        0        0    20753 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results.py
+-rw-r--r--   0        0        0     3504 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1827 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      168 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2631 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      188 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     4131 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1827 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      174 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     4313 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1827 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      180 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     4131 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1827 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      174 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     4224 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1827 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      186 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     3279 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1827 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      170 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0      182 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_type.py
+-rw-r--r--   0        0        0     5704 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1491 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      186 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     7010 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1491 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     7255 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1491 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     6277 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      214 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1491 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     4387 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1491 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      188 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     4324 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1491 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      178 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0      143 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_project_response_status.py
+-rw-r--r--   0        0        0     2140 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response.py
+-rw-r--r--   0        0        0     2185 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results.py
+-rw-r--r--   0        0        0     6459 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query.py
+-rw-r--r--   0        0        0     6194 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      283 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      323 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0      435 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8297 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1857 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1867 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1842 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1852 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1864 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3564 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     3446 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      318 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      221 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      144 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response_status.py
+-rw-r--r--   0        0        0     2545 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduled_jobs_response.py
+-rw-r--r--   0        0        0     1783 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduled_jobs_response_results_item.py
+-rw-r--r--   0        0        0      149 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduled_jobs_response_status.py
+-rw-r--r--   0        0        0     2333 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_and_targets_response.py
+-rw-r--r--   0        0        0     4174 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_and_targets_response_results.py
+-rw-r--r--   0        0        0     2851 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2871 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      155 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_and_targets_response_status.py
+-rw-r--r--   0        0        0     2225 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response.py
+-rw-r--r--   0        0        0     5755 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results.py
+-rw-r--r--   0        0        0     1849 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py
+-rw-r--r--   0        0        0     1851 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py
+-rw-r--r--   0        0        0     5967 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py
+-rw-r--r--   0        0        0     1464 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py
+-rw-r--r--   0        0        0      250 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_logs_item_status.py
+-rw-r--r--   0        0        0      194 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_logs_item_target_type.py
+-rw-r--r--   0        0        0      470 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_logs_item_task.py
+-rw-r--r--   0        0        0     4374 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py
+-rw-r--r--   0        0        0     2894 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2914 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     2024 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_users_item.py
+-rw-r--r--   0        0        0      149 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_status.py
+-rw-r--r--   0        0        0     2238 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_share_response.py
+-rw-r--r--   0        0        0     3586 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_share_response_results.py
+-rw-r--r--   0        0        0      141 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_share_response_status.py
+-rw-r--r--   0        0        0     2545 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_slack_channels_response.py
+-rw-r--r--   0        0        0     1680 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_slack_channels_response_results_item.py
+-rw-r--r--   0        0        0      149 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_slack_channels_response_status.py
+-rw-r--r--   0        0        0     2083 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response.py
+-rw-r--r--   0        0        0     5397 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results.py
+-rw-r--r--   0        0        0     2346 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_access_item.py
+-rw-r--r--   0        0        0      280 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_access_item_role.py
+-rw-r--r--   0        0        0     7661 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_dashboards_item.py
+-rw-r--r--   0        0        0     1333 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2288 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7951 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_queries_item.py
+-rw-r--r--   0        0        0      350 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1321 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2273 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      141 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_response_status.py
+-rw-r--r--   0        0        0     2602 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_summary_list_response.py
+-rw-r--r--   0        0        0     2625 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_summary_list_response_results_item.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_space_summary_list_response_status.py
+-rw-r--r--   0        0        0     2243 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_ssh_key_pair_response.py
+-rw-r--r--   0        0        0     1644 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_ssh_key_pair_response_results.py
+-rw-r--r--   0        0        0      146 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_ssh_key_pair_response_status.py
+-rw-r--r--   0        0        0     1937 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_success_empty.py
+-rw-r--r--   0        0        0      140 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_success_empty_status.py
+-rw-r--r--   0        0        0     2780 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_user_allowed_organizations_response.py
+-rw-r--r--   0        0        0     2120 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_user_allowed_organizations_response_results_item.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_user_allowed_organizations_response_status.py
+-rw-r--r--   0        0        0     4852 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response.py
+-rw-r--r--   0        0        0     7015 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_0.py
+-rw-r--r--   0        0        0      351 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_0_chart_type.py
+-rw-r--r--   0        0        0      285 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_0_error_type.py
+-rw-r--r--   0        0        0      214 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_0_source.py
+-rw-r--r--   0        0        0     6252 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_1.py
+-rw-r--r--   0        0        0      285 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_1_error_type.py
+-rw-r--r--   0        0        0      214 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_1_source.py
+-rw-r--r--   0        0        0     4129 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_2.py
+-rw-r--r--   0        0        0      285 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_2_error_type.py
+-rw-r--r--   0        0        0      214 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_results_item_type_2_source.py
+-rw-r--r--   0        0        0      144 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validate_response_status.py
+-rw-r--r--   0        0        0     1737 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validation_dismiss_response.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/api_validation_dismiss_response_status.py
+-rw-r--r--   0        0        0     5455 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/bigquery_credentials.py
+-rw-r--r--   0        0        0      184 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/bigquery_credentials_priority.py
+-rw-r--r--   0        0        0     1323 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/bigquery_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/bigquery_credentials_type.py
+-rw-r--r--   0        0        0      316 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_kind.py
+-rw-r--r--   0        0        0     4961 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_scheduler.py
+-rw-r--r--   0        0        0      161 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_scheduler_format.py
+-rw-r--r--   0        0        0     2583 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_scheduler_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1303 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_scheduler_options_type_1.py
+-rw-r--r--   0        0        0     3850 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_summary.py
+-rw-r--r--   0        0        0      204 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_summary_chart_type.py
+-rw-r--r--   0        0        0      192 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/chart_type.py
+-rw-r--r--   0        0        0      220 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/compact.py
+-rw-r--r--   0        0        0      232 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/compact_or_alias_type_0.py
+-rw-r--r--   0        0        0      272 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/compact_or_alias_type_1.py
+-rw-r--r--   0        0        0     2604 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_email_one_time_passcode_response_200.py
+-rw-r--r--   0        0        0     3046 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_email_one_time_passcode_response_200_results.py
+-rw-r--r--   0        0        0     2969 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_email_one_time_passcode_response_200_status.py
+-rw-r--r--   0        0        0     1641 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_group_in_organization_json_body.py
+-rw-r--r--   0        0        0     2466 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_group_in_organization_response_200.py
+-rw-r--r--   0        0        0     2455 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_group_in_organization_response_200_results.py
+-rw-r--r--   0        0        0      161 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_group_in_organization_response_200_status.py
+-rw-r--r--   0        0        0     1553 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_organization.py
+-rw-r--r--   0        0        0     1566 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_organization_json_body.py
+-rw-r--r--   0        0        0     2081 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_organization_response_200.py
+-rw-r--r--   0        0        0      154 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_organization_response_200_status.py
+-rw-r--r--   0        0        0     1968 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_project_member.py
+-rw-r--r--   0        0        0      266 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_project_member_role.py
+-rw-r--r--   0        0        0     1696 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_share_url.py
+-rw-r--r--   0        0        0     1724 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_share_url_json_body.py
+-rw-r--r--   0        0        0     2403 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_share_url_response_201.py
+-rw-r--r--   0        0        0     3637 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_share_url_response_201_results.py
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_share_url_response_201_status.py
+-rw-r--r--   0        0        0     2727 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space.py
+-rw-r--r--   0        0        0     2218 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_access_item.py
+-rw-r--r--   0        0        0      268 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_access_item_role.py
+-rw-r--r--   0        0        0     2951 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_json_body.py
+-rw-r--r--   0        0        0     2404 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_json_body_access_item.py
+-rw-r--r--   0        0        0      285 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_json_body_access_item_role.py
+-rw-r--r--   0        0        0     2356 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200.py
+-rw-r--r--   0        0        0     5940 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results.py
+-rw-r--r--   0        0        0     2517 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_access_item.py
+-rw-r--r--   0        0        0      295 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     8038 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1399 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2372 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     8388 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      365 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1387 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2357 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_response_200_status.py
+-rw-r--r--   0        0        0     2351 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_ssh_key_pair_response_201.py
+-rw-r--r--   0        0        0     1677 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_ssh_key_pair_response_201_results.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/create_ssh_key_pair_response_201_status.py
+-rw-r--r--   0        0        0     7206 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dashboard_basic_details.py
+-rw-r--r--   0        0        0     1263 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dashboard_basic_details_updated_by_user.py
+-rw-r--r--   0        0        0     2199 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dashboard_basic_details_validation_errors_item.py
+-rw-r--r--   0        0        0     5077 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dashboard_scheduler.py
+-rw-r--r--   0        0        0      165 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dashboard_scheduler_format.py
+-rw-r--r--   0        0        0     2635 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dashboard_scheduler_options_type_0.py
+-rw-r--r--   0        0        0      181 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dashboard_scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1323 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dashboard_scheduler_options_type_1.py
+-rw-r--r--   0        0        0     3796 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/databricks_credentials.py
+-rw-r--r--   0        0        0     1333 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/databricks_credentials_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/databricks_credentials_type.py
+-rw-r--r--   0        0        0     3902 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_azure_dev_ops_project_config.py
+-rw-r--r--   0        0        0     1741 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py
+-rw-r--r--   0        0        0      170 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_azure_dev_ops_project_config_type.py
+-rw-r--r--   0        0        0     3929 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_bit_bucket_project_config.py
+-rw-r--r--   0        0        0     1728 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_bit_bucket_project_config_type.py
+-rw-r--r--   0        0        0     2442 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_cloud_ide_project_config.py
+-rw-r--r--   0        0        0      169 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_cloud_ide_project_config_type.py
+-rw-r--r--   0        0        0     1710 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_cloud_integration.py
+-rw-r--r--   0        0        0     2445 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
+-rw-r--r--   0        0        0     2646 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py
+-rw-r--r--   0        0        0     2494 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_cloud_metric.py
+-rw-r--r--   0        0        0     3694 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_github_project_config.py
+-rw-r--r--   0        0        0     1710 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_github_project_config_environment_item.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_github_project_config_type.py
+-rw-r--r--   0        0        0     3694 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_gitlab_project_config.py
+-rw-r--r--   0        0        0     1710 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_gitlab_project_config_environment_item.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_gitlab_project_config_type.py
+-rw-r--r--   0        0        0     3051 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_local_project_config.py
+-rw-r--r--   0        0        0     1705 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_local_project_config_environment_item.py
+-rw-r--r--   0        0        0      146 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_local_project_config_type.py
+-rw-r--r--   0        0        0     2810 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_none_project_config.py
+-rw-r--r--   0        0        0     1700 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_none_project_config_environment_item.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_none_project_config_type.py
+-rw-r--r--   0        0        0     1708 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_0_environment_item.py
+-rw-r--r--   0        0        0      146 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_0_type.py
+-rw-r--r--   0        0        0     2415 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_1.py
+-rw-r--r--   0        0        0      166 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_1_type.py
+-rw-r--r--   0        0        0     1708 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_2_environment_item.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_2_type.py
+-rw-r--r--   0        0        0     1708 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_3_environment_item.py
+-rw-r--r--   0        0        0      158 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_3_type.py
+-rw-r--r--   0        0        0     1708 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_4_environment_item.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_4_type.py
+-rw-r--r--   0        0        0     1708 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_5_environment_item.py
+-rw-r--r--   0        0        0      164 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_5_type.py
+-rw-r--r--   0        0        0     1708 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_6_environment_item.py
+-rw-r--r--   0        0        0      148 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_6_type.py
+-rw-r--r--   0        0        0     1664 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_environment_variable.py
+-rw-r--r--   0        0        0      295 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_type.py
+-rw-r--r--   0        0        0      164 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_type_azuredevops.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_type_bitbucket.py
+-rw-r--r--   0        0        0      138 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_type_dbt.py
+-rw-r--r--   0        0        0      166 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_type_dbtcloudide.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_type_github.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_type_gitlab.py
+-rw-r--r--   0        0        0      141 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_type_none.py
+-rw-r--r--   0        0        0     2252 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0      169 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     2011 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_group_response_200.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_group_response_200_status.py
+-rw-r--r--   0        0        0     1981 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_me_response_200.py
+-rw-r--r--   0        0        0      144 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_me_response_200_status.py
+-rw-r--r--   0        0        0     2105 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_my_organization_response_200.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     2145 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_organization_member_response_200.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_organization_member_response_200_status.py
+-rw-r--r--   0        0        0     2051 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_scheduler_response_201.py
+-rw-r--r--   0        0        0      151 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     2011 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_space_response_204.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_space_response_204_status.py
+-rw-r--r--   0        0        0     1801 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_validation_dismiss_response_200.py
+-rw-r--r--   0        0        0      159 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/delete_validation_dismiss_response_200_status.py
+-rw-r--r--   0        0        0     2003 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/email_one_time_password.py
+-rw-r--r--   0        0        0     2749 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/email_one_time_password_expiring.py
+-rw-r--r--   0        0        0     2408 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/email_status.py
+-rw-r--r--   0        0        0     2654 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/email_status_expiring.py
+-rw-r--r--   0        0        0     2829 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/email_status_expiring_otp.py
+-rw-r--r--   0        0        0     1970 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/email_status_otp.py
+-rw-r--r--   0        0        0     1664 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/filter_group_response_type_0.py
+-rw-r--r--   0        0        0     1674 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/filter_group_response_type_1.py
+-rw-r--r--   0        0        0     5939 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/filters.py
+-rw-r--r--   0        0        0     1651 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1661 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1636 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1646 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/filters_metrics_type_1.py
+-rw-r--r--   0        0        0     2163 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_csv_url_response_200.py
+-rw-r--r--   0        0        0     1670 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_csv_url_response_200_results.py
+-rw-r--r--   0        0        0      145 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_csv_url_response_200_status.py
+-rw-r--r--   0        0        0     3113 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0     1870 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py
+-rw-r--r--   0        0        0      166 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     2411 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_dbt_cloud_metrics_response_200.py
+-rw-r--r--   0        0        0     2557 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py
+-rw-r--r--   0        0        0     2677 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py
+-rw-r--r--   0        0        0      154 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_dbt_cloud_metrics_response_200_status.py
+-rw-r--r--   0        0        0     2581 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_email_verification_status_response_200.py
+-rw-r--r--   0        0        0     3041 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_email_verification_status_response_200_results.py
+-rw-r--r--   0        0        0     2966 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_email_verification_status_response_200_results_otp.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_email_verification_status_response_200_status.py
+-rw-r--r--   0        0        0     2585 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_group_members_response_200.py
+-rw-r--r--   0        0        0     2308 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_group_members_response_200_results_item.py
+-rw-r--r--   0        0        0      151 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_group_members_response_200_status.py
+-rw-r--r--   0        0        0     2140 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_group_response_200.py
+-rw-r--r--   0        0        0     2364 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_group_response_200_results.py
+-rw-r--r--   0        0        0      144 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_group_response_200_status.py
+-rw-r--r--   0        0        0     5796 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200.py
+-rw-r--r--   0        0        0     7456 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0      369 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_chart_type.py
+-rw-r--r--   0        0        0      303 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_error_type.py
+-rw-r--r--   0        0        0      232 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_source.py
+-rw-r--r--   0        0        0     6573 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0      303 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_error_type.py
+-rw-r--r--   0        0        0      232 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_source.py
+-rw-r--r--   0        0        0     4450 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0      303 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_error_type.py
+-rw-r--r--   0        0        0      232 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_source.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200_status.py
+-rw-r--r--   0        0        0     2332 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_my_organization_response_200.py
+-rw-r--r--   0        0        0     2942 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_my_organization_response_200_results.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     5116 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200.py
+-rw-r--r--   0        0        0     2589 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0     7422 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1373 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2340 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      178 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2589 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0     8341 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py
+-rw-r--r--   0        0        0      361 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1373 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2340 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      170 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2514 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0     4018 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py
+-rw-r--r--   0        0        0      170 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_type.py
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_pinned_items_response_200_status.py
+-rw-r--r--   0        0        0     2701 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_access_list_response_200.py
+-rw-r--r--   0        0        0     2825 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_access_list_response_200_results_item.py
+-rw-r--r--   0        0        0      289 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_access_list_response_200_results_item_role.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_access_list_response_200_status.py
+-rw-r--r--   0        0        0     2174 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200.py
+-rw-r--r--   0        0        0    21372 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results.py
+-rw-r--r--   0        0        0     3557 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1845 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      171 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2661 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      191 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     4184 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1845 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      177 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     4366 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1845 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      183 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     4184 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1845 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      177 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     4277 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1845 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      189 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     3332 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1845 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      173 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0      185 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_type.py
+-rw-r--r--   0        0        0     5764 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1509 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      189 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     7070 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1509 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     7315 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1509 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     6356 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      217 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1509 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     4447 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1509 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      191 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     4384 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1509 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      181 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0      146 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_status.py
+-rw-r--r--   0        0        0     2602 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduled_jobs_response_200.py
+-rw-r--r--   0        0        0     1801 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduled_jobs_response_200_status.py
+-rw-r--r--   0        0        0     2373 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_job_status_response_200.py
+-rw-r--r--   0        0        0     1601 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_job_status_response_200_results.py
+-rw-r--r--   0        0        0      157 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_job_status_response_200_status.py
+-rw-r--r--   0        0        0     2282 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200.py
+-rw-r--r--   0        0        0     5980 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results.py
+-rw-r--r--   0        0        0     1867 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py
+-rw-r--r--   0        0        0     1869 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     6080 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py
+-rw-r--r--   0        0        0     1482 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py
+-rw-r--r--   0        0        0      253 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_status.py
+-rw-r--r--   0        0        0      197 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_target_type.py
+-rw-r--r--   0        0        0      473 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_task.py
+-rw-r--r--   0        0        0     4500 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py
+-rw-r--r--   0        0        0     2912 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2932 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     2042 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_logs_response_200_status.py
+-rw-r--r--   0        0        0     2208 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_response_200.py
+-rw-r--r--   0        0        0     3946 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_response_200_results.py
+-rw-r--r--   0        0        0     2813 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2833 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      148 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_scheduler_response_200_status.py
+-rw-r--r--   0        0        0     2352 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_share_url_response_200.py
+-rw-r--r--   0        0        0     3622 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_share_url_response_200_results.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_share_url_response_200_status.py
+-rw-r--r--   0        0        0     2602 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_slack_channels_response_200.py
+-rw-r--r--   0        0        0     1698 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_slack_channels_response_200_results_item.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_slack_channels_response_200_status.py
+-rw-r--r--   0        0        0     2140 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200.py
+-rw-r--r--   0        0        0     5484 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results.py
+-rw-r--r--   0        0        0     2380 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_access_item.py
+-rw-r--r--   0        0        0      283 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     7728 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1347 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2306 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     8046 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      353 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1335 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2291 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      144 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/get_space_response_200_status.py
+-rw-r--r--   0        0        0     2114 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/grant_project_access_to_user_json_body.py
+-rw-r--r--   0        0        0      279 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/grant_project_access_to_user_json_body_role.py
+-rw-r--r--   0        0        0     2153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/grant_project_access_to_user_response_200.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/grant_project_access_to_user_response_200_status.py
+-rw-r--r--   0        0        0     2247 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/group.py
+-rw-r--r--   0        0        0     2163 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/group_member.py
+-rw-r--r--   0        0        0     2061 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/join_organization_response_200.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/join_organization_response_200_status.py
+-rw-r--r--   0        0        0     2659 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_charts_in_project_response_200.py
+-rw-r--r--   0        0        0     4202 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_charts_in_project_response_200_results_item.py
+-rw-r--r--   0        0        0      233 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_charts_in_project_response_200_results_item_chart_type.py
+-rw-r--r--   0        0        0      155 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_charts_in_project_response_200_status.py
+-rw-r--r--   0        0        0     2786 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_groups_in_organization_response_200.py
+-rw-r--r--   0        0        0     2473 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_groups_in_organization_response_200_results_item.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_groups_in_organization_response_200_status.py
+-rw-r--r--   0        0        0     2854 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_my_available_organizations_response_200.py
+-rw-r--r--   0        0        0     2143 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_my_available_organizations_response_200_results_item.py
+-rw-r--r--   0        0        0      164 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_my_available_organizations_response_200_status.py
+-rw-r--r--   0        0        0     2534 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_email_domains_response_200.py
+-rw-r--r--   0        0        0     2723 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_email_domains_response_200_results.py
+-rw-r--r--   0        0        0      315 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_email_domains_response_200_results_role.py
+-rw-r--r--   0        0        0      164 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_email_domains_response_200_status.py
+-rw-r--r--   0        0        0     2763 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_members_response_200.py
+-rw-r--r--   0        0        0     3841 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_members_response_200_results_item.py
+-rw-r--r--   0        0        0      314 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_members_response_200_results_item_role.py
+-rw-r--r--   0        0        0      159 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_members_response_200_status.py
+-rw-r--r--   0        0        0     2825 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_projects_response_200.py
+-rw-r--r--   0        0        0     2351 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_projects_response_200_results_item.py
+-rw-r--r--   0        0        0      203 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_projects_response_200_results_item_type.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_organization_projects_response_200_status.py
+-rw-r--r--   0        0        0     2659 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_spaces_in_project_response_200.py
+-rw-r--r--   0        0        0     2643 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_spaces_in_project_response_200_results_item.py
+-rw-r--r--   0        0        0      155 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/list_spaces_in_project_response_200_status.py
+-rw-r--r--   0        0        0     5593 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response.py
+-rw-r--r--   0        0        0     5687 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_additional_metrics_item.py
+-rw-r--r--   0        0        0      265 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      305 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0      417 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     6943 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_filters.py
+-rw-r--r--   0        0        0     1755 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1765 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1740 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1750 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1762 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_sorts_item.py
+-rw-r--r--   0        0        0     3310 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_table_calculations_item.py
+-rw-r--r--   0        0        0     3138 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_table_calculations_item_format.py
+-rw-r--r--   0        0        0      300 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      203 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      383 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/metric_type.py
+-rw-r--r--   0        0        0      260 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/number_separator.py
+-rw-r--r--   0        0        0     2439 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0      308 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role.py
+-rw-r--r--   0        0        0     6547 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0      224 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
+-rw-r--r--   0        0        0     1541 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     4647 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1551 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      200 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     7465 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1541 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     7220 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1541 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5932 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1546 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      197 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     4480 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1526 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      185 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     3885 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_validation_response_base_name.py
+-rw-r--r--   0        0        0      280 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_validation_response_base_name_error_type.py
+-rw-r--r--   0        0        0      209 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/omit_validation_response_base_name_source.py
+-rw-r--r--   0        0        0     2812 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/organization.py
+-rw-r--r--   0        0        0     3616 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/organization_member_profile.py
+-rw-r--r--   0        0        0      294 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/organization_member_profile_role.py
+-rw-r--r--   0        0        0     2190 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/organization_member_profile_update.py
+-rw-r--r--   0        0        0      300 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/organization_member_profile_update_role.py
+-rw-r--r--   0        0        0      287 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/organization_member_role.py
+-rw-r--r--   0        0        0     2052 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/organization_project.py
+-rw-r--r--   0        0        0      176 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/organization_project_type.py
+-rw-r--r--   0        0        0     2377 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
+-rw-r--r--   0        0        0     2297 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/partial_pick_organization_member_profile_role.py
+-rw-r--r--   0        0        0      309 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/partial_pick_organization_member_profile_role_role.py
+-rw-r--r--   0        0        0     2898 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/partial_pick_space_is_private_or_access.py
+-rw-r--r--   0        0        0     2467 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/partial_pick_space_is_private_or_access_access_item.py
+-rw-r--r--   0        0        0      290 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/partial_pick_space_is_private_or_access_access_item_role.py
+-rw-r--r--   0        0        0     2771 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0      339 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role.py
+-rw-r--r--   0        0        0     7788 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0      267 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
+-rw-r--r--   0        0        0     1800 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5501 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1820 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      245 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     1841 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
+-rw-r--r--   0        0        0     1565 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_group_name.py
+-rw-r--r--   0        0        0     8412 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1800 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     8163 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1800 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     6781 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1810 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      235 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5251 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1765 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      219 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0    10058 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py
+-rw-r--r--   0        0        0     1888 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
+-rw-r--r--   0        0        0     3018 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
+-rw-r--r--   0        0        0     8114 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1894 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
+-rw-r--r--   0        0        0     1532 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_group_name.py
+-rw-r--r--   0        0        0     1566 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_organization_name.py
+-rw-r--r--   0        0        0     2016 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     3781 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
+-rw-r--r--   0        0        0     5636 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1664 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
+-rw-r--r--   0        0        0     1757 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_share_url_path_or_params.py
+-rw-r--r--   0        0        0     1502 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_name.py
+-rw-r--r--   0        0        0     1768 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_name_or_is_private.py
+-rw-r--r--   0        0        0     2609 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
+-rw-r--r--   0        0        0     3420 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
+-rw-r--r--   0        0        0    11798 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py
+-rw-r--r--   0        0        0      480 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_chart_type.py
+-rw-r--r--   0        0        0     1892 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
+-rw-r--r--   0        0        0     3024 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
+-rw-r--r--   0        0        0     1601 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_space_share_user_uuid.py
+-rw-r--r--   0        0        0     1619 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_ssh_key_pair_public_key.py
+-rw-r--r--   0        0        0     4465 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
+-rw-r--r--   0        0        0      314 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_error_type.py
+-rw-r--r--   0        0        0      243 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_source.py
+-rw-r--r--   0        0        0     2266 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
+-rw-r--r--   0        0        0     1281 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2223 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      157 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_0_type.py
+-rw-r--r--   0        0        0      340 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1281 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2223 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      149 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_1_type.py
+-rw-r--r--   0        0        0     3901 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_2_data.py
+-rw-r--r--   0        0        0      149 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/pinned_items_item_type_2_type.py
+-rw-r--r--   0        0        0     2297 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_json_body.py
+-rw-r--r--   0        0        0     7436 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_json_body_filters.py
+-rw-r--r--   0        0        0     1786 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1796 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1771 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1781 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     2282 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200.py
+-rw-r--r--   0        0        0     2328 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results.py
+-rw-r--r--   0        0        0     6734 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     6467 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      291 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      331 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0      443 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8770 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1900 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1910 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1885 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1895 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1907 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3673 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     3579 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      326 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      229 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_status.py
+-rw-r--r--   0        0        0     5961 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body.py
+-rw-r--r--   0        0        0     5721 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_additional_metrics_item.py
+-rw-r--r--   0        0        0      266 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      306 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0      418 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     1964 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_filters.py
+-rw-r--r--   0        0        0     1773 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_sorts_item.py
+-rw-r--r--   0        0        0     3333 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_table_calculations_item.py
+-rw-r--r--   0        0        0     3164 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_table_calculations_item_format.py
+-rw-r--r--   0        0        0      301 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      204 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     2214 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200.py
+-rw-r--r--   0        0        0     2238 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results.py
+-rw-r--r--   0        0        0     6602 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     6333 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      287 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      327 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0      439 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8544 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1880 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1890 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1865 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1875 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1887 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3621 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     3515 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      322 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      225 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      148 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_status.py
+-rw-r--r--   0        0        0     6614 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body.py
+-rw-r--r--   0        0        0     6122 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py
+-rw-r--r--   0        0        0      280 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      320 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0      432 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     2040 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py
+-rw-r--r--   0        0        0     1849 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py
+-rw-r--r--   0        0        0     3525 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py
+-rw-r--r--   0        0        0     3398 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py
+-rw-r--r--   0        0        0      315 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      218 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     2506 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200.py
+-rw-r--r--   0        0        0     2458 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results.py
+-rw-r--r--   0        0        0     7192 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     6873 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      301 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      341 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0      453 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     9494 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1980 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1990 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1965 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1975 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1963 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3867 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     3851 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      336 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      239 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/post_run_underlying_data_query_response_200_status.py
+-rw-r--r--   0        0        0     6628 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/postgres_credentials.py
+-rw-r--r--   0        0        0     1323 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/postgres_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/postgres_credentials_type.py
+-rw-r--r--   0        0        0    17112 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project.py
+-rw-r--r--   0        0        0     3120 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1728 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2451 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      170 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     3747 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1728 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     3929 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1728 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     3747 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1728 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     3840 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1728 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      168 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     2895 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1728 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      152 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0     2576 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_member_profile.py
+-rw-r--r--   0        0        0      267 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_member_profile_role.py
+-rw-r--r--   0        0        0      260 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_member_role.py
+-rw-r--r--   0        0        0      164 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_type.py
+-rw-r--r--   0        0        0     5336 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1392 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      168 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     6642 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1392 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     6887 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1392 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     5789 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      196 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1392 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     4019 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1392 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      170 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     3956 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1392 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/project_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0     1294 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/record_string_any.py
+-rw-r--r--   0        0        0     6383 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/redshift_credentials.py
+-rw-r--r--   0        0        0     1323 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/redshift_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/redshift_credentials_type.py
+-rw-r--r--   0        0        0     2099 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/remove_user_from_group_response_200.py
+-rw-r--r--   0        0        0      155 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/remove_user_from_group_response_200_status.py
+-rw-r--r--   0        0        0     2156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_chart_item.py
+-rw-r--r--   0        0        0     7730 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_chart_item_data.py
+-rw-r--r--   0        0        0      341 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_chart_item_data_chart_type.py
+-rw-r--r--   0        0        0     1283 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py
+-rw-r--r--   0        0        0     2225 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_chart_item_type.py
+-rw-r--r--   0        0        0     2224 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_dashboard_item.py
+-rw-r--r--   0        0        0     7050 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_dashboard_item_data.py
+-rw-r--r--   0        0        0     1299 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py
+-rw-r--r--   0        0        0     2245 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_dashboard_item_type.py
+-rw-r--r--   0        0        0      193 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_item_type.py
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_item_type_chart.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_item_type_dashboard.py
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_item_type_space.py
+-rw-r--r--   0        0        0     2093 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_space_item.py
+-rw-r--r--   0        0        0     3903 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_space_item_data.py
+-rw-r--r--   0        0        0      150 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/resource_view_space_item_type.py
+-rw-r--r--   0        0        0     2173 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/revoke_project_access_for_user_response_200.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/revoke_project_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     2153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/revoke_space_access_for_user_response_200.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/revoke_space_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     5741 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request.py
+-rw-r--r--   0        0        0     5549 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_additional_metrics_item.py
+-rw-r--r--   0        0        0      261 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      301 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0      413 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     1933 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_filters.py
+-rw-r--r--   0        0        0     1742 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_sorts_item.py
+-rw-r--r--   0        0        0     3216 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_table_calculations_item.py
+-rw-r--r--   0        0        0     3074 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_table_calculations_item_format.py
+-rw-r--r--   0        0        0      296 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      199 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     1661 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduled_jobs.py
+-rw-r--r--   0        0        0     3501 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_and_targets.py
+-rw-r--r--   0        0        0     2752 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py
+-rw-r--r--   0        0        0     2772 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py
+-rw-r--r--   0        0        0     4975 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_base.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_base_format.py
+-rw-r--r--   0        0        0     2570 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_base_options_type_0.py
+-rw-r--r--   0        0        0      176 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_base_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1298 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_base_options_type_1.py
+-rw-r--r--   0        0        0     2484 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_csv_options.py
+-rw-r--r--   0        0        0      170 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_csv_options_limit_type_1.py
+-rw-r--r--   0        0        0     2685 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_email_target.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_format.py
+-rw-r--r--   0        0        0     1272 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_image_options.py
+-rw-r--r--   0        0        0      223 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_job_status.py
+-rw-r--r--   0        0        0     5081 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_log.py
+-rw-r--r--   0        0        0     1314 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_log_details.py
+-rw-r--r--   0        0        0      223 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_log_status.py
+-rw-r--r--   0        0        0      167 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_log_target_type.py
+-rw-r--r--   0        0        0      443 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_log_task.py
+-rw-r--r--   0        0        0     2514 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_options_type_0.py
+-rw-r--r--   0        0        0      172 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1275 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_options_type_1.py
+-rw-r--r--   0        0        0     2665 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_slack_target.py
+-rw-r--r--   0        0        0      161 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_type_0_format.py
+-rw-r--r--   0        0        0     2587 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_type_0_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_type_0_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1306 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_type_0_options_type_1.py
+-rw-r--r--   0        0        0      161 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_type_1_format.py
+-rw-r--r--   0        0        0     2587 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_type_1_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_type_1_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1306 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_type_1_options_type_1.py
+-rw-r--r--   0        0        0     5085 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs.py
+-rw-r--r--   0        0        0     1773 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_charts_item.py
+-rw-r--r--   0        0        0     1775 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_dashboards_item.py
+-rw-r--r--   0        0        0     5482 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_logs_item.py
+-rw-r--r--   0        0        0     1388 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_logs_item_details.py
+-rw-r--r--   0        0        0      236 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_logs_item_status.py
+-rw-r--r--   0        0        0      180 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_logs_item_target_type.py
+-rw-r--r--   0        0        0      456 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_logs_item_task.py
+-rw-r--r--   0        0        0     3970 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_schedulers_item.py
+-rw-r--r--   0        0        0     2818 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2838 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     1948 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_users_item.py
+-rw-r--r--   0        0        0     3505 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/share_url.py
+-rw-r--r--   0        0        0     1553 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/slack_channel.py
+-rw-r--r--   0        0        0     5095 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/snowflake_credentials.py
+-rw-r--r--   0        0        0     1328 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/snowflake_credentials_start_of_week.py
+-rw-r--r--   0        0        0      157 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/snowflake_credentials_type.py
+-rw-r--r--   0        0        0     1658 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/sort_field.py
+-rw-r--r--   0        0        0     4902 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space.py
+-rw-r--r--   0        0        0     2154 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_access_item.py
+-rw-r--r--   0        0        0      262 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_access_item_role.py
+-rw-r--r--   0        0        0     7059 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_dashboard.py
+-rw-r--r--   0        0        0     1233 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_dashboard_updated_by_user.py
+-rw-r--r--   0        0        0     2161 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_dashboard_validation_errors_item.py
+-rw-r--r--   0        0        0     7166 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_dashboards_item.py
+-rw-r--r--   0        0        0     1255 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2189 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7345 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_queries_item.py
+-rw-r--r--   0        0        0      332 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1243 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2174 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7181 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_query.py
+-rw-r--r--   0        0        0      326 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_query_chart_type.py
+-rw-r--r--   0        0        0     1217 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_query_updated_by_user.py
+-rw-r--r--   0        0        0     2141 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_query_validation_errors_item.py
+-rw-r--r--   0        0        0     2100 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_share.py
+-rw-r--r--   0        0        0      257 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_share_role.py
+-rw-r--r--   0        0        0     2480 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/space_summary.py
+-rw-r--r--   0        0        0      276 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/table_calculation_format_separator.py
+-rw-r--r--   0        0        0      179 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/table_calculation_format_type.py
+-rw-r--r--   0        0        0     3643 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/trino_credentials.py
+-rw-r--r--   0        0        0     1308 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/trino_credentials_start_of_week.py
+-rw-r--r--   0        0        0      145 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/trino_credentials_type.py
+-rw-r--r--   0        0        0     2291 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_allowed_email_domains.py
+-rw-r--r--   0        0        0      294 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_allowed_email_domains_role.py
+-rw-r--r--   0        0        0     3167 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0     1885 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py
+-rw-r--r--   0        0        0      169 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     1519 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_group.py
+-rw-r--r--   0        0        0     1565 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_group_json_body.py
+-rw-r--r--   0        0        0     2191 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_group_response_200.py
+-rw-r--r--   0        0        0     2379 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_group_response_200_results.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_group_response_200_status.py
+-rw-r--r--   0        0        0     2239 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_my_organization_json_body.py
+-rw-r--r--   0        0        0     2105 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_my_organization_response_200.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     2184 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization.py
+-rw-r--r--   0        0        0     2429 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_email_domains_json_body.py
+-rw-r--r--   0        0        0      307 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_email_domains_json_body_role.py
+-rw-r--r--   0        0        0     2577 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_email_domains_response_200.py
+-rw-r--r--   0        0        0     2743 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_email_domains_response_200_results.py
+-rw-r--r--   0        0        0      317 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_email_domains_response_200_results_role.py
+-rw-r--r--   0        0        0      166 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_email_domains_response_200_status.py
+-rw-r--r--   0        0        0     2198 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_member_json_body.py
+-rw-r--r--   0        0        0      301 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_member_json_body_role.py
+-rw-r--r--   0        0        0     2469 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_member_response_200.py
+-rw-r--r--   0        0        0     3798 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_member_response_200_results.py
+-rw-r--r--   0        0        0      311 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_member_response_200_results_role.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_organization_member_response_200_status.py
+-rw-r--r--   0        0        0     2156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_item_order.py
+-rw-r--r--   0        0        0     1888 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_item_order_data.py
+-rw-r--r--   0        0        0      198 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_item_order_type.py
+-rw-r--r--   0        0        0     2395 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_json_body_item.py
+-rw-r--r--   0        0        0     1962 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_json_body_item_data.py
+-rw-r--r--   0        0        0      211 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_json_body_item_type.py
+-rw-r--r--   0        0        0     5624 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200.py
+-rw-r--r--   0        0        0     2731 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0     7685 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1407 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2383 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      186 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2731 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0     8653 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py
+-rw-r--r--   0        0        0      369 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1407 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2383 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      178 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2656 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0     4061 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py
+-rw-r--r--   0        0        0      178 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_type.py
+-rw-r--r--   0        0        0      158 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_items_order_response_200_status.py
+-rw-r--r--   0        0        0     1779 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_project_access_for_user_json_body.py
+-rw-r--r--   0        0        0      281 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_project_access_for_user_json_body_role.py
+-rw-r--r--   0        0        0     2173 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_project_access_for_user_response_200.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_project_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     1613 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_project_member.py
+-rw-r--r--   0        0        0      266 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_project_member_role.py
+-rw-r--r--   0        0        0     2259 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_scheduler_response_201.py
+-rw-r--r--   0        0        0     4018 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_scheduler_response_201_results.py
+-rw-r--r--   0        0        0     2828 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2848 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      151 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     1691 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space.py
+-rw-r--r--   0        0        0     1737 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_json_body.py
+-rw-r--r--   0        0        0     2191 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200.py
+-rw-r--r--   0        0        0     5587 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results.py
+-rw-r--r--   0        0        0     2410 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_access_item.py
+-rw-r--r--   0        0        0      286 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     7788 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1359 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2321 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     8124 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      356 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1347 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2306 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      147 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/update_space_response_200_status.py
+-rw-r--r--   0        0        0     1173 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/updated_by_user.py
+-rw-r--r--   0        0        0     1993 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/user_allowed_organization.py
+-rw-r--r--   0        0        0     1964 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validate_project_json_body.py
+-rw-r--r--   0        0        0     2259 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validate_project_response_200.py
+-rw-r--r--   0        0        0     1563 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validate_project_response_200_results.py
+-rw-r--r--   0        0        0      151 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validate_project_response_200_status.py
+-rw-r--r--   0        0        0     6843 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_chart_response.py
+-rw-r--r--   0        0        0      344 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_chart_response_chart_type.py
+-rw-r--r--   0        0        0      278 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_chart_response_error_type.py
+-rw-r--r--   0        0        0      207 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_chart_response_source.py
+-rw-r--r--   0        0        0     6189 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_dashboard_response.py
+-rw-r--r--   0        0        0      282 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_dashboard_response_error_type.py
+-rw-r--r--   0        0        0      211 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_dashboard_response_source.py
+-rw-r--r--   0        0        0     4002 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_table_response.py
+-rw-r--r--   0        0        0      278 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_table_response_error_type.py
+-rw-r--r--   0        0        0      207 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_table_response_source.py
+-rw-r--r--   0        0        0      260 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_error_type.py
+-rw-r--r--   0        0        0     3820 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_base.py
+-rw-r--r--   0        0        0      272 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_base_error_type.py
+-rw-r--r--   0        0        0      201 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_base_source.py
+-rw-r--r--   0        0        0     6733 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_0.py
+-rw-r--r--   0        0        0      339 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_0_chart_type.py
+-rw-r--r--   0        0        0      273 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_0_error_type.py
+-rw-r--r--   0        0        0      202 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_0_source.py
+-rw-r--r--   0        0        0     6045 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_1.py
+-rw-r--r--   0        0        0      273 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_1_error_type.py
+-rw-r--r--   0        0        0      202 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_1_source.py
+-rw-r--r--   0        0        0     3922 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_2.py
+-rw-r--r--   0        0        0      273 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_2_error_type.py
+-rw-r--r--   0        0        0      202 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_2_source.py
+-rw-r--r--   0        0        0      193 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_source_type.py
+-rw-r--r--   0        0        0     2067 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/validation_summary.py
+-rw-r--r--   0        0        0     2633 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/view_statistics.py
+-rw-r--r--   0        0        0     1359 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py
+-rw-r--r--   0        0        0      162 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_0_type.py
+-rw-r--r--   0        0        0     1359 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_1_type.py
+-rw-r--r--   0        0        0     1359 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_2_type.py
+-rw-r--r--   0        0        0      190 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_3_priority.py
+-rw-r--r--   0        0        0     1359 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_3_type.py
+-rw-r--r--   0        0        0     1359 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py
+-rw-r--r--   0        0        0      164 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_4_type.py
+-rw-r--r--   0        0        0     1359 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_credentials_type_5_type.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_types_bigquery.py
+-rw-r--r--   0        0        0      159 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_types_databricks.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_types_postgres.py
+-rw-r--r--   0        0        0      153 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_types_redshift.py
+-rw-r--r--   0        0        0      156 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_types_snowflake.py
+-rw-r--r--   0        0        0      144 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/warehouse_types_trino.py
+-rw-r--r--   0        0        0      225 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/models/week_day.py
+-rw-r--r--   0        0        0       26 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/py.typed
+-rw-r--r--   0        0        0     1101 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/lightdash_client/types.py
+-rw-r--r--   0        0        0     1624 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/setup.py
+-rw-r--r--   0        0        0      796 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/tests/__init__.py
+-rw-r--r--   0        0        0      908 2023-06-20 02:56:56.000000 lightdash_client_python-0.621.0/tests/test_dummy.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.621.0/PKG-INFO
```

### Comparing `lightdash_client_python-0.619.1/.github/CODEOWNERS` & `lightdash_client_python-0.621.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/.github/workflows/publish.yml` & `lightdash_client_python-0.621.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/.github/workflows/test-publish.yml` & `lightdash_client_python-0.621.0/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/.github/workflows/test.yml` & `lightdash_client_python-0.621.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/.gitignore` & `lightdash_client_python-0.621.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/.openapi-generator-ignore` & `lightdash_client_python-0.621.0/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/.pre-commit-config.yaml` & `lightdash_client_python-0.621.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/.pylintrc` & `lightdash_client_python-0.621.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/LICENSE` & `lightdash_client_python-0.621.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/README.md` & `lightdash_client_python-0.621.0/README.md`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/dev/clean.sh` & `lightdash_client_python-0.621.0/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/dev/generate_clients.sh` & `lightdash_client_python-0.621.0/dev/generate_clients.sh`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #
 
 # Constants
 SCRIPT_DIR="$(dirname "$(readlink -f "$0")")"
 PROJECT_DIR="$(dirname "$SCRIPT_DIR")"
 
 # Arguments
-schema_json="${PROJECT_DIR}/dev/schemas/swagger.json"
+schema_json="${PROJECT_DIR}/dev/schemas/dereferenced-swagger.json"
 config_yaml="${PROJECT_DIR}/dev/openapi-python-client.yml"
 output_dir="${PROJECT_DIR}"
 meta="setup"
 skip_validate_spec=1
 while (($# > 0)); do
   if [[ "$1" == "--schema-json" ]]; then
     schema_json="${2:?}"
```

### Comparing `lightdash_client_python-0.619.1/dev/lint.sh` & `lightdash_client_python-0.621.0/dev/lint.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/dev/publish.sh` & `lightdash_client_python-0.621.0/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/dev/schemas/swagger.json` & `lightdash_client_python-0.621.0/dev/schemas/swagger.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915249340355689%*

 * *Differences: {"'components'": "{'schemas': {'OrganizationMemberProfileUpdate': {replace: OrderedDict([('$ref', "*

 * *                 "'#/components/schemas/Partial_Pick_OrganizationMemberProfile.role__')])}, "*

 * *                 "'Pick_AllowedEmailDomains.Exclude_keyofAllowedEmailDomains.organizationUuid__': "*

 * *                 "{'required': {insert: [(1, 'emailDomains')], delete: [0]}}, 'TableCalculation': "*

 * *                 "{'properties': {'format': OrderedDict([('$ref', "*

 * *                 "'#/components/schemas/TableCalcu […]*

```diff
@@ -1651,14 +1651,23 @@
                     "median",
                     "string",
                     "date",
                     "boolean"
                 ],
                 "type": "string"
             },
+            "NumberSeparator": {
+                "enum": [
+                    "commaPeriod",
+                    "spacePeriod",
+                    "periodComma",
+                    "noSeparatorPeriod"
+                ],
+                "type": "string"
+            },
             "Omit_AllowedEmailDomains.organizationUuid_": {
                 "$ref": "#/components/schemas/Pick_AllowedEmailDomains.Exclude_keyofAllowedEmailDomains.organizationUuid__",
                 "description": "Construct a type with the properties of T except for those in type K."
             },
             "Omit_CreateBigqueryCredentials.SensitiveCredentialsFieldNames_": {
                 "$ref": "#/components/schemas/Pick_CreateBigqueryCredentials.Exclude_keyofCreateBigqueryCredentials.SensitiveCredentialsFieldNames__",
                 "description": "Construct a type with the properties of T except for those in type K."
@@ -1759,23 +1768,15 @@
                     "lastName",
                     "firstName",
                     "userUuid"
                 ],
                 "type": "object"
             },
             "OrganizationMemberProfileUpdate": {
-                "properties": {
-                    "role": {
-                        "$ref": "#/components/schemas/OrganizationMemberRole"
-                    }
-                },
-                "required": [
-                    "role"
-                ],
-                "type": "object"
+                "$ref": "#/components/schemas/Partial_Pick_OrganizationMemberProfile.role__"
             },
             "OrganizationMemberRole": {
                 "enum": [
                     "member",
                     "viewer",
                     "interactive_viewer",
                     "editor",
@@ -1819,14 +1820,24 @@
                     "name": {
                         "description": "The name of the organization",
                         "type": "string"
                     }
                 },
                 "type": "object"
             },
+            "Partial_Pick_OrganizationMemberProfile.role__": {
+                "description": "Make all properties in T optional",
+                "properties": {
+                    "role": {
+                        "$ref": "#/components/schemas/OrganizationMemberRole",
+                        "description": "The role of the user in the organization"
+                    }
+                },
+                "type": "object"
+            },
             "Partial_Pick_Space.isPrivate-or-access__": {
                 "description": "Make all properties in T optional",
                 "properties": {
                     "access": {
                         "items": {
                             "$ref": "#/components/schemas/SpaceShare"
                         },
@@ -1854,16 +1865,16 @@
                         "type": "array"
                     },
                     "role": {
                         "$ref": "#/components/schemas/OrganizationMemberRole"
                     }
                 },
                 "required": [
-                    "emailDomains",
                     "role",
+                    "emailDomains",
                     "projectUuids"
                 ],
                 "type": "object"
             },
             "Pick_CreateBigqueryCredentials.Exclude_keyofCreateBigqueryCredentials.SensitiveCredentialsFieldNames__": {
                 "description": "From T, pick a set of properties whose keys are in the union K",
                 "properties": {
@@ -3567,14 +3578,17 @@
                 ]
             },
             "TableCalculation": {
                 "properties": {
                     "displayName": {
                         "type": "string"
                     },
+                    "format": {
+                        "$ref": "#/components/schemas/TableCalculationFormat"
+                    },
                     "index": {
                         "format": "double",
                         "type": "number"
                     },
                     "name": {
                         "type": "string"
                     },
@@ -3585,14 +3599,39 @@
                 "required": [
                     "sql",
                     "displayName",
                     "name"
                 ],
                 "type": "object"
             },
+            "TableCalculationFormat": {
+                "properties": {
+                    "round": {
+                        "format": "double",
+                        "type": "number"
+                    },
+                    "separator": {
+                        "$ref": "#/components/schemas/NumberSeparator"
+                    },
+                    "type": {
+                        "$ref": "#/components/schemas/TableCalculationFormatType"
+                    }
+                },
+                "required": [
+                    "type"
+                ],
+                "type": "object"
+            },
+            "TableCalculationFormatType": {
+                "enum": [
+                    "default",
+                    "percent"
+                ],
+                "type": "string"
+            },
             "TrinoCredentials": {
                 "$ref": "#/components/schemas/Omit_CreateTrinoCredentials.SensitiveCredentialsFieldNames_"
             },
             "UpdateAllowedEmailDomains": {
                 "$ref": "#/components/schemas/Omit_AllowedEmailDomains.organizationUuid_"
             },
             "UpdateGroup": {
@@ -3949,15 +3988,15 @@
             "url": "https://docs.lightdash.com/help-and-contact/contact/contact_info/"
         },
         "description": "Open API documentation for all public Lightdash API endpoints",
         "license": {
             "name": "MIT"
         },
         "title": "Lightdash API",
-        "version": "0.618.1"
+        "version": "0.620.0"
     },
     "openapi": "3.0.0",
     "paths": {
         "/api/v1/csv/{jobId}": {
             "get": {
                 "description": "Get a Csv",
                 "operationId": "getCsvUrl",
```

### Comparing `lightdash_client_python-0.619.1/dev/setup.sh` & `lightdash_client_python-0.621.0/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/dev/test_python.sh` & `lightdash_client_python-0.621.0/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/charts/post_chart_results.py` & `lightdash_client_python-0.621.0/lightdash_client/api/share_links/create_share_url.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_run_query_response import ApiRunQueryResponse
-from ...models.post_chart_results_json_body import PostChartResultsJsonBody
+from ...models.create_share_url_json_body import CreateShareUrlJsonBody
+from ...models.create_share_url_response_201 import CreateShareUrlResponse201
 from ...types import Response
 
 
 def _get_kwargs(
-    chart_uuid: str,
     *,
     client: Client,
-    json_body: PostChartResultsJsonBody,
+    json_body: CreateShareUrlJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/saved/{chartUuid}/results".format(client.base_url, chartUuid=chart_uuid)
+    url = "{}/api/v1/share".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
@@ -32,147 +31,135 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiRunQueryResponse]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = ApiRunQueryResponse.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreateShareUrlResponse201]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = CreateShareUrlResponse201.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiRunQueryResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[CreateShareUrlResponse201]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    chart_uuid: str,
     *,
     client: Client,
-    json_body: PostChartResultsJsonBody,
-) -> Response[ApiRunQueryResponse]:
-    """Run a query for a chart
+    json_body: CreateShareUrlJsonBody,
+) -> Response[CreateShareUrlResponse201]:
+    """Given a full URL generates a short url id that can be used for sharing
 
     Args:
-        chart_uuid (str):
-        json_body (PostChartResultsJsonBody):
+        json_body (CreateShareUrlJsonBody): a full URL used to generate a short url id
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiRunQueryResponse]
+        Response[CreateShareUrlResponse201]
     """
 
     kwargs = _get_kwargs(
-        chart_uuid=chart_uuid,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    chart_uuid: str,
     *,
     client: Client,
-    json_body: PostChartResultsJsonBody,
-) -> Optional[ApiRunQueryResponse]:
-    """Run a query for a chart
+    json_body: CreateShareUrlJsonBody,
+) -> Optional[CreateShareUrlResponse201]:
+    """Given a full URL generates a short url id that can be used for sharing
 
     Args:
-        chart_uuid (str):
-        json_body (PostChartResultsJsonBody):
+        json_body (CreateShareUrlJsonBody): a full URL used to generate a short url id
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiRunQueryResponse
+        CreateShareUrlResponse201
     """
 
     return sync_detailed(
-        chart_uuid=chart_uuid,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
-    chart_uuid: str,
     *,
     client: Client,
-    json_body: PostChartResultsJsonBody,
-) -> Response[ApiRunQueryResponse]:
-    """Run a query for a chart
+    json_body: CreateShareUrlJsonBody,
+) -> Response[CreateShareUrlResponse201]:
+    """Given a full URL generates a short url id that can be used for sharing
 
     Args:
-        chart_uuid (str):
-        json_body (PostChartResultsJsonBody):
+        json_body (CreateShareUrlJsonBody): a full URL used to generate a short url id
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiRunQueryResponse]
+        Response[CreateShareUrlResponse201]
     """
 
     kwargs = _get_kwargs(
-        chart_uuid=chart_uuid,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    chart_uuid: str,
     *,
     client: Client,
-    json_body: PostChartResultsJsonBody,
-) -> Optional[ApiRunQueryResponse]:
-    """Run a query for a chart
+    json_body: CreateShareUrlJsonBody,
+) -> Optional[CreateShareUrlResponse201]:
+    """Given a full URL generates a short url id that can be used for sharing
 
     Args:
-        chart_uuid (str):
-        json_body (PostChartResultsJsonBody):
+        json_body (CreateShareUrlJsonBody): a full URL used to generate a short url id
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiRunQueryResponse
+        CreateShareUrlResponse201
     """
 
     return (
         await asyncio_detailed(
-            chart_uuid=chart_uuid,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/content/get_pinned_items.py` & `lightdash_client_python-0.621.0/lightdash_client/api/content/get_pinned_items.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_pinned_items import ApiPinnedItems
+from ...models.get_pinned_items_response_200 import GetPinnedItemsResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
@@ -30,52 +30,52 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiPinnedItems]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetPinnedItemsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiPinnedItems.from_dict(response.json())
+        response_200 = GetPinnedItemsResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiPinnedItems]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetPinnedItemsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-) -> Response[ApiPinnedItems]:
+) -> Response[GetPinnedItemsResponse200]:
     """Get pinned items
 
     Args:
         project_uuid (str):
         pinned_list_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiPinnedItems]
+        Response[GetPinnedItemsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         pinned_list_uuid=pinned_list_uuid,
         client=client,
     )
@@ -89,54 +89,54 @@
 
 
 def sync(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiPinnedItems]:
+) -> Optional[GetPinnedItemsResponse200]:
     """Get pinned items
 
     Args:
         project_uuid (str):
         pinned_list_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiPinnedItems
+        GetPinnedItemsResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         pinned_list_uuid=pinned_list_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-) -> Response[ApiPinnedItems]:
+) -> Response[GetPinnedItemsResponse200]:
     """Get pinned items
 
     Args:
         project_uuid (str):
         pinned_list_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiPinnedItems]
+        Response[GetPinnedItemsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         pinned_list_uuid=pinned_list_uuid,
         client=client,
     )
@@ -148,27 +148,27 @@
 
 
 async def asyncio(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiPinnedItems]:
+) -> Optional[GetPinnedItemsResponse200]:
     """Get pinned items
 
     Args:
         project_uuid (str):
         pinned_list_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiPinnedItems
+        GetPinnedItemsResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             pinned_list_uuid=pinned_list_uuid,
             client=client,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/content/update_pinned_items_order.py` & `lightdash_client_python-0.621.0/lightdash_client/api/content/update_pinned_items_order.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 from typing import List
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_pinned_items import ApiPinnedItems
-from ...models.update_pinned_item_order import UpdatePinnedItemOrder
+from ...models.update_pinned_items_order_json_body_item import UpdatePinnedItemsOrderJsonBodyItem
+from ...models.update_pinned_items_order_response_200 import UpdatePinnedItemsOrderResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: List["UpdatePinnedItemOrder"],
+    json_body: List["UpdatePinnedItemsOrderJsonBodyItem"],
 ) -> Dict[str, Any]:
     url = "{}/api/v1/projects/{projectUuid}/pinned-lists/{pinnedListUuid}/items/order".format(
         client.base_url, projectUuid=project_uuid, pinnedListUuid=pinned_list_uuid
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
@@ -40,54 +40,54 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiPinnedItems]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[UpdatePinnedItemsOrderResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiPinnedItems.from_dict(response.json())
+        response_200 = UpdatePinnedItemsOrderResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiPinnedItems]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[UpdatePinnedItemsOrderResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: List["UpdatePinnedItemOrder"],
-) -> Response[ApiPinnedItems]:
+    json_body: List["UpdatePinnedItemsOrderJsonBodyItem"],
+) -> Response[UpdatePinnedItemsOrderResponse200]:
     """Update pinned items order
 
     Args:
         project_uuid (str):
         pinned_list_uuid (str):
-        json_body (List['UpdatePinnedItemOrder']): the new order of the pinned items
+        json_body (List['UpdatePinnedItemsOrderJsonBodyItem']): the new order of the pinned items
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiPinnedItems]
+        Response[UpdatePinnedItemsOrderResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         pinned_list_uuid=pinned_list_uuid,
         client=client,
         json_body=json_body,
@@ -102,29 +102,29 @@
 
 
 def sync(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: List["UpdatePinnedItemOrder"],
-) -> Optional[ApiPinnedItems]:
+    json_body: List["UpdatePinnedItemsOrderJsonBodyItem"],
+) -> Optional[UpdatePinnedItemsOrderResponse200]:
     """Update pinned items order
 
     Args:
         project_uuid (str):
         pinned_list_uuid (str):
-        json_body (List['UpdatePinnedItemOrder']): the new order of the pinned items
+        json_body (List['UpdatePinnedItemsOrderJsonBodyItem']): the new order of the pinned items
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiPinnedItems
+        UpdatePinnedItemsOrderResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         pinned_list_uuid=pinned_list_uuid,
         client=client,
         json_body=json_body,
@@ -132,29 +132,29 @@
 
 
 async def asyncio_detailed(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: List["UpdatePinnedItemOrder"],
-) -> Response[ApiPinnedItems]:
+    json_body: List["UpdatePinnedItemsOrderJsonBodyItem"],
+) -> Response[UpdatePinnedItemsOrderResponse200]:
     """Update pinned items order
 
     Args:
         project_uuid (str):
         pinned_list_uuid (str):
-        json_body (List['UpdatePinnedItemOrder']): the new order of the pinned items
+        json_body (List['UpdatePinnedItemsOrderJsonBodyItem']): the new order of the pinned items
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiPinnedItems]
+        Response[UpdatePinnedItemsOrderResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         pinned_list_uuid=pinned_list_uuid,
         client=client,
         json_body=json_body,
@@ -167,29 +167,29 @@
 
 
 async def asyncio(
     project_uuid: str,
     pinned_list_uuid: str,
     *,
     client: Client,
-    json_body: List["UpdatePinnedItemOrder"],
-) -> Optional[ApiPinnedItems]:
+    json_body: List["UpdatePinnedItemsOrderJsonBodyItem"],
+) -> Optional[UpdatePinnedItemsOrderResponse200]:
     """Update pinned items order
 
     Args:
         project_uuid (str):
         pinned_list_uuid (str):
-        json_body (List['UpdatePinnedItemOrder']): the new order of the pinned items
+        json_body (List['UpdatePinnedItemsOrderJsonBodyItem']): the new order of the pinned items
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiPinnedItems
+        UpdatePinnedItemsOrderResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             pinned_list_uuid=pinned_list_uuid,
             client=client,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/exploring/post_run_query.py` & `lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,191 +3,174 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_run_query_response import ApiRunQueryResponse
-from ...models.run_query_request import RunQueryRequest
+from ...models.revoke_project_access_for_user_response_200 import RevokeProjectAccessForUserResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
-    explore_id: str,
+    user_uuid: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/explores/{exploreId}/runQuery".format(
-        client.base_url, projectUuid=project_uuid, exploreId=explore_id
+    url = "{}/api/v1/projects/{projectUuid}/access/{userUuid}".format(
+        client.base_url, projectUuid=project_uuid, userUuid=user_uuid
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "post",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiRunQueryResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[RevokeProjectAccessForUserResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiRunQueryResponse.from_dict(response.json())
+        response_200 = RevokeProjectAccessForUserResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiRunQueryResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[RevokeProjectAccessForUserResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
-    explore_id: str,
+    user_uuid: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
-) -> Response[ApiRunQueryResponse]:
-    """Run a query for explore
+) -> Response[RevokeProjectAccessForUserResponse200]:
+    """Remove a user's access to a project
 
     Args:
         project_uuid (str):
-        explore_id (str):
-        json_body (RunQueryRequest):
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiRunQueryResponse]
+        Response[RevokeProjectAccessForUserResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        explore_id=explore_id,
+        user_uuid=user_uuid,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
-    explore_id: str,
+    user_uuid: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
-) -> Optional[ApiRunQueryResponse]:
-    """Run a query for explore
+) -> Optional[RevokeProjectAccessForUserResponse200]:
+    """Remove a user's access to a project
 
     Args:
         project_uuid (str):
-        explore_id (str):
-        json_body (RunQueryRequest):
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiRunQueryResponse
+        RevokeProjectAccessForUserResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
-        explore_id=explore_id,
+        user_uuid=user_uuid,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
-    explore_id: str,
+    user_uuid: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
-) -> Response[ApiRunQueryResponse]:
-    """Run a query for explore
+) -> Response[RevokeProjectAccessForUserResponse200]:
+    """Remove a user's access to a project
 
     Args:
         project_uuid (str):
-        explore_id (str):
-        json_body (RunQueryRequest):
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiRunQueryResponse]
+        Response[RevokeProjectAccessForUserResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        explore_id=explore_id,
+        user_uuid=user_uuid,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
-    explore_id: str,
+    user_uuid: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
-) -> Optional[ApiRunQueryResponse]:
-    """Run a query for explore
+) -> Optional[RevokeProjectAccessForUserResponse200]:
+    """Remove a user's access to a project
 
     Args:
         project_uuid (str):
-        explore_id (str):
-        json_body (RunQueryRequest):
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiRunQueryResponse
+        RevokeProjectAccessForUserResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
-            explore_id=explore_id,
+            user_uuid=user_uuid,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/exploring/post_run_underlying_data_query.py` & `lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/create_space_in_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,29 +3,26 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_run_query_response import ApiRunQueryResponse
-from ...models.run_query_request import RunQueryRequest
+from ...models.create_space_in_project_json_body import CreateSpaceInProjectJsonBody
+from ...models.create_space_in_project_response_200 import CreateSpaceInProjectResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
-    explore_id: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
+    json_body: CreateSpaceInProjectJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/explores/{exploreId}/runUnderlyingDataQuery".format(
-        client.base_url, projectUuid=project_uuid, exploreId=explore_id
-    )
+    url = "{}/api/v1/projects/{projectUuid}/spaces".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
@@ -35,159 +32,147 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiRunQueryResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreateSpaceInProjectResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiRunQueryResponse.from_dict(response.json())
+        response_200 = CreateSpaceInProjectResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiRunQueryResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[CreateSpaceInProjectResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
-    explore_id: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
-) -> Response[ApiRunQueryResponse]:
-    """Run a query for underlying data results
+    json_body: CreateSpaceInProjectJsonBody,
+) -> Response[CreateSpaceInProjectResponse200]:
+    """Create a new space inside a project
 
     Args:
         project_uuid (str):
-        explore_id (str):
-        json_body (RunQueryRequest):
+        json_body (CreateSpaceInProjectJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiRunQueryResponse]
+        Response[CreateSpaceInProjectResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        explore_id=explore_id,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
-    explore_id: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
-) -> Optional[ApiRunQueryResponse]:
-    """Run a query for underlying data results
+    json_body: CreateSpaceInProjectJsonBody,
+) -> Optional[CreateSpaceInProjectResponse200]:
+    """Create a new space inside a project
 
     Args:
         project_uuid (str):
-        explore_id (str):
-        json_body (RunQueryRequest):
+        json_body (CreateSpaceInProjectJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiRunQueryResponse
+        CreateSpaceInProjectResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
-        explore_id=explore_id,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
-    explore_id: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
-) -> Response[ApiRunQueryResponse]:
-    """Run a query for underlying data results
+    json_body: CreateSpaceInProjectJsonBody,
+) -> Response[CreateSpaceInProjectResponse200]:
+    """Create a new space inside a project
 
     Args:
         project_uuid (str):
-        explore_id (str):
-        json_body (RunQueryRequest):
+        json_body (CreateSpaceInProjectJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiRunQueryResponse]
+        Response[CreateSpaceInProjectResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        explore_id=explore_id,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
-    explore_id: str,
     *,
     client: Client,
-    json_body: RunQueryRequest,
-) -> Optional[ApiRunQueryResponse]:
-    """Run a query for underlying data results
+    json_body: CreateSpaceInProjectJsonBody,
+) -> Optional[CreateSpaceInProjectResponse200]:
+    """Create a new space inside a project
 
     Args:
         project_uuid (str):
-        explore_id (str):
-        json_body (RunQueryRequest):
+        json_body (CreateSpaceInProjectJsonBody):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiRunQueryResponse
+        CreateSpaceInProjectResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
-            explore_id=explore_id,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/exports/get_csv_url.py` & `lightdash_client_python-0.621.0/lightdash_client/api/exports/get_csv_url.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_csv_url_response import ApiCsvUrlResponse
+from ...models.get_csv_url_response_200 import GetCsvUrlResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     job_id: str,
     *,
     client: Client,
@@ -27,50 +27,50 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiCsvUrlResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetCsvUrlResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiCsvUrlResponse.from_dict(response.json())
+        response_200 = GetCsvUrlResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiCsvUrlResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetCsvUrlResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     job_id: str,
     *,
     client: Client,
-) -> Response[ApiCsvUrlResponse]:
+) -> Response[GetCsvUrlResponse200]:
     """Get a Csv
 
     Args:
         job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiCsvUrlResponse]
+        Response[GetCsvUrlResponse200]
     """
 
     kwargs = _get_kwargs(
         job_id=job_id,
         client=client,
     )
 
@@ -82,50 +82,50 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     job_id: str,
     *,
     client: Client,
-) -> Optional[ApiCsvUrlResponse]:
+) -> Optional[GetCsvUrlResponse200]:
     """Get a Csv
 
     Args:
         job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiCsvUrlResponse
+        GetCsvUrlResponse200
     """
 
     return sync_detailed(
         job_id=job_id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     job_id: str,
     *,
     client: Client,
-) -> Response[ApiCsvUrlResponse]:
+) -> Response[GetCsvUrlResponse200]:
     """Get a Csv
 
     Args:
         job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiCsvUrlResponse]
+        Response[GetCsvUrlResponse200]
     """
 
     kwargs = _get_kwargs(
         job_id=job_id,
         client=client,
     )
 
@@ -135,26 +135,26 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     job_id: str,
     *,
     client: Client,
-) -> Optional[ApiCsvUrlResponse]:
+) -> Optional[GetCsvUrlResponse200]:
     """Get a Csv
 
     Args:
         job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiCsvUrlResponse
+        GetCsvUrlResponse200
     """
 
     return (
         await asyncio_detailed(
             job_id=job_id,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.621.0/lightdash_client/api/projects/list_spaces_in_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,76 +3,74 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_dbt_cloud_settings_delete_success import ApiDbtCloudSettingsDeleteSuccess
+from ...models.list_spaces_in_project_response_200 import ListSpacesInProjectResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/integrations/dbt-cloud/settings".format(
-        client.base_url, projectUuid=project_uuid
-    )
+    url = "{}/api/v1/projects/{projectUuid}/spaces".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiDbtCloudSettingsDeleteSuccess]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ListSpacesInProjectResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiDbtCloudSettingsDeleteSuccess.from_dict(response.json())
+        response_200 = ListSpacesInProjectResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiDbtCloudSettingsDeleteSuccess]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListSpacesInProjectResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[ApiDbtCloudSettingsDeleteSuccess]:
-    """Remove the dbt Cloud integration settings for a project
+) -> Response[ListSpacesInProjectResponse200]:
+    """List all spaces in a project
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiDbtCloudSettingsDeleteSuccess]
+        Response[ListSpacesInProjectResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
@@ -84,50 +82,50 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiDbtCloudSettingsDeleteSuccess]:
-    """Remove the dbt Cloud integration settings for a project
+) -> Optional[ListSpacesInProjectResponse200]:
+    """List all spaces in a project
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiDbtCloudSettingsDeleteSuccess
+        ListSpacesInProjectResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[ApiDbtCloudSettingsDeleteSuccess]:
-    """Remove the dbt Cloud integration settings for a project
+) -> Response[ListSpacesInProjectResponse200]:
+    """List all spaces in a project
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiDbtCloudSettingsDeleteSuccess]
+        Response[ListSpacesInProjectResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
@@ -137,26 +135,26 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiDbtCloudSettingsDeleteSuccess]:
-    """Remove the dbt Cloud integration settings for a project
+) -> Optional[ListSpacesInProjectResponse200]:
+    """List all spaces in a project
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiDbtCloudSettingsDeleteSuccess
+        ListSpacesInProjectResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.621.0/lightdash_client/api/schedulers/get_scheduler_logs.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,71 +3,74 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
+from ...models.get_scheduler_logs_response_200 import GetSchedulerLogsResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/integrations/dbt-cloud/settings".format(
-        client.base_url, projectUuid=project_uuid
-    )
+    url = "{}/api/v1/schedulers/{projectUuid}/logs".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetSchedulerLogsResponse200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = GetSchedulerLogsResponse200.from_dict(response.json())
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetSchedulerLogsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[Any]:
-    """Get the current dbt Cloud integration settings for a project
+) -> Response[GetSchedulerLogsResponse200]:
+    """Get scheduled logs
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[GetSchedulerLogsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
@@ -75,34 +78,84 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
+def sync(
+    project_uuid: str,
+    *,
+    client: Client,
+) -> Optional[GetSchedulerLogsResponse200]:
+    """Get scheduled logs
+
+    Args:
+        project_uuid (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        GetSchedulerLogsResponse200
+    """
+
+    return sync_detailed(
+        project_uuid=project_uuid,
+        client=client,
+    ).parsed
+
+
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[Any]:
-    """Get the current dbt Cloud integration settings for a project
+) -> Response[GetSchedulerLogsResponse200]:
+    """Get scheduled logs
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[GetSchedulerLogsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    project_uuid: str,
+    *,
+    client: Client,
+) -> Optional[GetSchedulerLogsResponse200]:
+    """Get scheduled logs
+
+    Args:
+        project_uuid (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        GetSchedulerLogsResponse200
+    """
+
+    return (
+        await asyncio_detailed(
+            project_uuid=project_uuid,
+            client=client,
+        )
+    ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_dbt_cloud_metrics.py` & `lightdash_client_python-0.621.0/lightdash_client/api/integrations/get_dbt_cloud_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_dbt_cloud_metrics import ApiDbtCloudMetrics
+from ...models.get_dbt_cloud_metrics_response_200 import GetDbtCloudMetricsResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     *,
     client: Client,
@@ -29,52 +29,52 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiDbtCloudMetrics]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetDbtCloudMetricsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiDbtCloudMetrics.from_dict(response.json())
+        response_200 = GetDbtCloudMetricsResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiDbtCloudMetrics]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetDbtCloudMetricsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[ApiDbtCloudMetrics]:
+) -> Response[GetDbtCloudMetricsResponse200]:
     """Get a list of dbt metric definitions from the dbt Cloud metadata api.
     The metrics are taken from the metadata from a single dbt Cloud job configured
     with the dbt Cloud integration settings for the project.
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiDbtCloudMetrics]
+        Response[GetDbtCloudMetricsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
@@ -86,54 +86,54 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiDbtCloudMetrics]:
+) -> Optional[GetDbtCloudMetricsResponse200]:
     """Get a list of dbt metric definitions from the dbt Cloud metadata api.
     The metrics are taken from the metadata from a single dbt Cloud job configured
     with the dbt Cloud integration settings for the project.
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiDbtCloudMetrics
+        GetDbtCloudMetricsResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[ApiDbtCloudMetrics]:
+) -> Response[GetDbtCloudMetricsResponse200]:
     """Get a list of dbt metric definitions from the dbt Cloud metadata api.
     The metrics are taken from the metadata from a single dbt Cloud job configured
     with the dbt Cloud integration settings for the project.
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiDbtCloudMetrics]
+        Response[GetDbtCloudMetricsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
@@ -143,28 +143,28 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiDbtCloudMetrics]:
+) -> Optional[GetDbtCloudMetricsResponse200]:
     """Get a list of dbt metric definitions from the dbt Cloud metadata api.
     The metrics are taken from the metadata from a single dbt Cloud job configured
     with the dbt Cloud integration settings for the project.
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiDbtCloudMetrics
+        GetDbtCloudMetricsResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/integrations/get_slack_channels.py` & `lightdash_client_python-0.621.0/lightdash_client/api/integrations/get_slack_channels.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_slack_channels_response import ApiSlackChannelsResponse
+from ...models.get_slack_channels_response_200 import GetSlackChannelsResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
@@ -26,46 +26,46 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSlackChannelsResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetSlackChannelsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSlackChannelsResponse.from_dict(response.json())
+        response_200 = GetSlackChannelsResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSlackChannelsResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetSlackChannelsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[ApiSlackChannelsResponse]:
+) -> Response[GetSlackChannelsResponse200]:
     """Get slack channels
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSlackChannelsResponse]
+        Response[GetSlackChannelsResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -75,42 +75,42 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[ApiSlackChannelsResponse]:
+) -> Optional[GetSlackChannelsResponse200]:
     """Get slack channels
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSlackChannelsResponse
+        GetSlackChannelsResponse200
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[ApiSlackChannelsResponse]:
+) -> Response[GetSlackChannelsResponse200]:
     """Get slack channels
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSlackChannelsResponse]
+        Response[GetSlackChannelsResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -118,23 +118,23 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[ApiSlackChannelsResponse]:
+) -> Optional[GetSlackChannelsResponse200]:
     """Get slack channels
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSlackChannelsResponse
+        GetSlackChannelsResponse200
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.621.0/lightdash_client/api/projects/get_project.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,71 +3,74 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
+from ...models.get_project_response_200 import GetProjectResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/integrations/dbt-cloud/settings".format(
-        client.base_url, projectUuid=project_uuid
-    )
+    url = "{}/api/v1/projects/{projectUuid}".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetProjectResponse200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = GetProjectResponse200.from_dict(response.json())
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetProjectResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[Any]:
-    """Update the dbt Cloud integration settings for a project
+) -> Response[GetProjectResponse200]:
+    """Get a project of an organiztion
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[GetProjectResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
@@ -75,34 +78,84 @@
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
+def sync(
+    project_uuid: str,
+    *,
+    client: Client,
+) -> Optional[GetProjectResponse200]:
+    """Get a project of an organiztion
+
+    Args:
+        project_uuid (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        GetProjectResponse200
+    """
+
+    return sync_detailed(
+        project_uuid=project_uuid,
+        client=client,
+    ).parsed
+
+
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[Any]:
-    """Update the dbt Cloud integration settings for a project
+) -> Response[GetProjectResponse200]:
+    """Get a project of an organiztion
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[GetProjectResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    project_uuid: str,
+    *,
+    client: Client,
+) -> Optional[GetProjectResponse200]:
+    """Get a project of an organiztion
+
+    Args:
+        project_uuid (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        GetProjectResponse200
+    """
+
+    return (
+        await asyncio_detailed(
+            project_uuid=project_uuid,
+            client=client,
+        )
+    ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/my_account/create_email_one_time_passcode.py` & `lightdash_client_python-0.621.0/lightdash_client/api/my_account/delete_me.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,95 +3,138 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
+from ...models.delete_me_response_200 import DeleteMeResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/user/me/email/otp".format(client.base_url)
+    url = "{}/api/v1/user/me".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "put",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[DeleteMeResponse200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = DeleteMeResponse200.from_dict(response.json())
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[DeleteMeResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[Any]:
-    """Create a new one-time passcode for the current user's primary email.
-    The user will receive an email with the passcode.
+) -> Response[DeleteMeResponse200]:
+    """Delete user
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[DeleteMeResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
+def sync(
+    *,
+    client: Client,
+) -> Optional[DeleteMeResponse200]:
+    """Delete user
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        DeleteMeResponse200
+    """
+
+    return sync_detailed(
+        client=client,
+    ).parsed
+
+
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[Any]:
-    """Create a new one-time passcode for the current user's primary email.
-    The user will receive an email with the passcode.
+) -> Response[DeleteMeResponse200]:
+    """Delete user
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[DeleteMeResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Client,
+) -> Optional[DeleteMeResponse200]:
+    """Delete user
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        DeleteMeResponse200
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/my_account/delete_me.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/list_organization_projects.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,69 +3,69 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.list_organization_projects_response_200 import ListOrganizationProjectsResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/user/me".format(client.base_url)
+    url = "{}/api/v1/org/projects".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ListOrganizationProjectsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = ListOrganizationProjectsResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListOrganizationProjectsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Delete user
+) -> Response[ListOrganizationProjectsResponse200]:
+    """Gets all projects of the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[ListOrganizationProjectsResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -75,42 +75,42 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Delete user
+) -> Optional[ListOrganizationProjectsResponse200]:
+    """Gets all projects of the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        ListOrganizationProjectsResponse200
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Delete user
+) -> Response[ListOrganizationProjectsResponse200]:
+    """Gets all projects of the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[ListOrganizationProjectsResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -118,23 +118,23 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Delete user
+) -> Optional[ListOrganizationProjectsResponse200]:
+    """Gets all projects of the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        ListOrganizationProjectsResponse200
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/my_account/get_email_verification_status.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/list_organization_email_domains.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,140 @@
 from http import HTTPStatus
 from typing import Any
 from typing import Dict
 from typing import Optional
-from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import Client
+from ...models.list_organization_email_domains_response_200 import ListOrganizationEmailDomainsResponse200
 from ...types import Response
-from ...types import UNSET
-from ...types import Unset
 
 
 def _get_kwargs(
     *,
     client: Client,
-    passcode: Union[Unset, None, str] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/user/me/email/status".format(client.base_url)
+    url = "{}/api/v1/org/allowedEmailDomains".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    params: Dict[str, Any] = {}
-    params["passcode"] = passcode
-
-    params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
-
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ListOrganizationEmailDomainsResponse200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = ListOrganizationEmailDomainsResponse200.from_dict(response.json())
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListOrganizationEmailDomainsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    passcode: Union[Unset, None, str] = UNSET,
-) -> Response[Any]:
-    """Get the verification status for the current user's primary email
-
-    Args:
-        passcode (Union[Unset, None, str]):
+) -> Response[ListOrganizationEmailDomainsResponse200]:
+    """Gets the allowed email domains for the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[ListOrganizationEmailDomainsResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        passcode=passcode,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio_detailed(
+def sync(
     *,
     client: Client,
-    passcode: Union[Unset, None, str] = UNSET,
-) -> Response[Any]:
-    """Get the verification status for the current user's primary email
+) -> Optional[ListOrganizationEmailDomainsResponse200]:
+    """Gets the allowed email domains for the current user's organization
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        ListOrganizationEmailDomainsResponse200
+    """
+
+    return sync_detailed(
+        client=client,
+    ).parsed
+
 
-    Args:
-        passcode (Union[Unset, None, str]):
+async def asyncio_detailed(
+    *,
+    client: Client,
+) -> Response[ListOrganizationEmailDomainsResponse200]:
+    """Gets the allowed email domains for the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[ListOrganizationEmailDomainsResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
-        passcode=passcode,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Client,
+) -> Optional[ListOrganizationEmailDomainsResponse200]:
+    """Gets the allowed email domains for the current user's organization
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        ListOrganizationEmailDomainsResponse200
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/my_account/join_organization.py` & `lightdash_client_python-0.621.0/lightdash_client/api/my_account/join_organization.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.join_organization_response_200 import JoinOrganizationResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     organization_uuid: str,
     *,
     client: Client,
@@ -29,51 +29,51 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[JoinOrganizationResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = JoinOrganizationResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[JoinOrganizationResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     organization_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
+) -> Response[JoinOrganizationResponse200]:
     """Add the current user to an organization that accepts users with a verified email domain.
     This will fail if the organization email domain does not match the user's primary email domain.
 
     Args:
         organization_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[JoinOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         organization_uuid=organization_uuid,
         client=client,
     )
 
@@ -85,52 +85,52 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     organization_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
+) -> Optional[JoinOrganizationResponse200]:
     """Add the current user to an organization that accepts users with a verified email domain.
     This will fail if the organization email domain does not match the user's primary email domain.
 
     Args:
         organization_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        JoinOrganizationResponse200
     """
 
     return sync_detailed(
         organization_uuid=organization_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     organization_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
+) -> Response[JoinOrganizationResponse200]:
     """Add the current user to an organization that accepts users with a verified email domain.
     This will fail if the organization email domain does not match the user's primary email domain.
 
     Args:
         organization_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[JoinOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         organization_uuid=organization_uuid,
         client=client,
     )
 
@@ -140,27 +140,27 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     organization_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
+) -> Optional[JoinOrganizationResponse200]:
     """Add the current user to an organization that accepts users with a verified email domain.
     This will fail if the organization email domain does not match the user's primary email domain.
 
     Args:
         organization_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        JoinOrganizationResponse200
     """
 
     return (
         await asyncio_detailed(
             organization_uuid=organization_uuid,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/my_account/list_my_available_organizations.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/list_groups_in_organization.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,70 +3,69 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_user_allowed_organizations_response import ApiUserAllowedOrganizationsResponse
+from ...models.list_groups_in_organization_response_200 import ListGroupsInOrganizationResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/user/me/allowedOrganizations".format(client.base_url)
+    url = "{}/api/v1/org/groups".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiUserAllowedOrganizationsResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ListGroupsInOrganizationResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiUserAllowedOrganizationsResponse.from_dict(response.json())
+        response_200 = ListGroupsInOrganizationResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiUserAllowedOrganizationsResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListGroupsInOrganizationResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[ApiUserAllowedOrganizationsResponse]:
-    """List the organizations that the current user can join.
-    This is based on the user's primary email domain and the organization's allowed email domains.
+) -> Response[ListGroupsInOrganizationResponse200]:
+    """Gets all the groups in the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiUserAllowedOrganizationsResponse]
+        Response[ListGroupsInOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -76,44 +75,42 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[ApiUserAllowedOrganizationsResponse]:
-    """List the organizations that the current user can join.
-    This is based on the user's primary email domain and the organization's allowed email domains.
+) -> Optional[ListGroupsInOrganizationResponse200]:
+    """Gets all the groups in the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiUserAllowedOrganizationsResponse
+        ListGroupsInOrganizationResponse200
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[ApiUserAllowedOrganizationsResponse]:
-    """List the organizations that the current user can join.
-    This is based on the user's primary email domain and the organization's allowed email domains.
+) -> Response[ListGroupsInOrganizationResponse200]:
+    """Gets all the groups in the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiUserAllowedOrganizationsResponse]
+        Response[ListGroupsInOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -121,24 +118,23 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[ApiUserAllowedOrganizationsResponse]:
-    """List the organizations that the current user can join.
-    This is based on the user's primary email domain and the organization's allowed email domains.
+) -> Optional[ListGroupsInOrganizationResponse200]:
+    """Gets all the groups in the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiUserAllowedOrganizationsResponse
+        ListGroupsInOrganizationResponse200
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/organizations/create_group_in_organization.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/update_my_organization.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,79 +3,78 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_group_response import ApiGroupResponse
-from ...models.pick_create_group_name import PickCreateGroupName
+from ...models.update_my_organization_json_body import UpdateMyOrganizationJsonBody
+from ...models.update_my_organization_response_200 import UpdateMyOrganizationResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: PickCreateGroupName,
+    json_body: UpdateMyOrganizationJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/org/groups".format(client.base_url)
+    url = "{}/api/v1/org".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "post",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiGroupResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[UpdateMyOrganizationResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiGroupResponse.from_dict(response.json())
+        response_200 = UpdateMyOrganizationResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiGroupResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[UpdateMyOrganizationResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: PickCreateGroupName,
-) -> Response[ApiGroupResponse]:
-    """Creates a new group in the current user's organization
+    json_body: UpdateMyOrganizationJsonBody,
+) -> Response[UpdateMyOrganizationResponse200]:
+    """Update the current user's organization
 
     Args:
-        json_body (PickCreateGroupName): From T, pick a set of properties whose keys are in the
-            union K
+        json_body (UpdateMyOrganizationJsonBody): the new organization settings
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiGroupResponse]
+        Response[UpdateMyOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
     )
 
@@ -86,53 +85,51 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-    json_body: PickCreateGroupName,
-) -> Optional[ApiGroupResponse]:
-    """Creates a new group in the current user's organization
+    json_body: UpdateMyOrganizationJsonBody,
+) -> Optional[UpdateMyOrganizationResponse200]:
+    """Update the current user's organization
 
     Args:
-        json_body (PickCreateGroupName): From T, pick a set of properties whose keys are in the
-            union K
+        json_body (UpdateMyOrganizationJsonBody): the new organization settings
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiGroupResponse
+        UpdateMyOrganizationResponse200
     """
 
     return sync_detailed(
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: PickCreateGroupName,
-) -> Response[ApiGroupResponse]:
-    """Creates a new group in the current user's organization
+    json_body: UpdateMyOrganizationJsonBody,
+) -> Response[UpdateMyOrganizationResponse200]:
+    """Update the current user's organization
 
     Args:
-        json_body (PickCreateGroupName): From T, pick a set of properties whose keys are in the
-            union K
+        json_body (UpdateMyOrganizationJsonBody): the new organization settings
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiGroupResponse]
+        Response[UpdateMyOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
         json_body=json_body,
     )
 
@@ -141,28 +138,27 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-    json_body: PickCreateGroupName,
-) -> Optional[ApiGroupResponse]:
-    """Creates a new group in the current user's organization
+    json_body: UpdateMyOrganizationJsonBody,
+) -> Optional[UpdateMyOrganizationResponse200]:
+    """Update the current user's organization
 
     Args:
-        json_body (PickCreateGroupName): From T, pick a set of properties whose keys are in the
-            union K
+        json_body (UpdateMyOrganizationJsonBody): the new organization settings
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiGroupResponse
+        UpdateMyOrganizationResponse200
     """
 
     return (
         await asyncio_detailed(
             client=client,
             json_body=json_body,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/organizations/delete_my_organization.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/delete_my_organization.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.delete_my_organization_response_200 import DeleteMyOrganizationResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     organization_uuid: str,
     *,
     client: Client,
@@ -27,50 +27,50 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[DeleteMyOrganizationResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = DeleteMyOrganizationResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[DeleteMyOrganizationResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     organization_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
+) -> Response[DeleteMyOrganizationResponse200]:
     """Deletes an organization and all users inside that organization
 
     Args:
         organization_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[DeleteMyOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         organization_uuid=organization_uuid,
         client=client,
     )
 
@@ -82,50 +82,50 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     organization_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
+) -> Optional[DeleteMyOrganizationResponse200]:
     """Deletes an organization and all users inside that organization
 
     Args:
         organization_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        DeleteMyOrganizationResponse200
     """
 
     return sync_detailed(
         organization_uuid=organization_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     organization_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
+) -> Response[DeleteMyOrganizationResponse200]:
     """Deletes an organization and all users inside that organization
 
     Args:
         organization_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[DeleteMyOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         organization_uuid=organization_uuid,
         client=client,
     )
 
@@ -135,26 +135,26 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     organization_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
+) -> Optional[DeleteMyOrganizationResponse200]:
     """Deletes an organization and all users inside that organization
 
     Args:
         organization_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        DeleteMyOrganizationResponse200
     """
 
     return (
         await asyncio_detailed(
             organization_uuid=organization_uuid,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/organizations/delete_organization_member.py` & `lightdash_client_python-0.621.0/lightdash_client/api/projects/list_charts_in_project.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,159 +3,159 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.list_charts_in_project_response_200 import ListChartsInProjectResponse200
 from ...types import Response
 
 
 def _get_kwargs(
-    user_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/org/user/{userUuid}".format(client.base_url, userUuid=user_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/charts".format(client.base_url, projectUuid=project_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ListChartsInProjectResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = ListChartsInProjectResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListChartsInProjectResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    user_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Deletes a user from the current user's organization
+) -> Response[ListChartsInProjectResponse200]:
+    """List all charts in a project
 
     Args:
-        user_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[ListChartsInProjectResponse200]
     """
 
     kwargs = _get_kwargs(
-        user_uuid=user_uuid,
+        project_uuid=project_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    user_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Deletes a user from the current user's organization
+) -> Optional[ListChartsInProjectResponse200]:
+    """List all charts in a project
 
     Args:
-        user_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        ListChartsInProjectResponse200
     """
 
     return sync_detailed(
-        user_uuid=user_uuid,
+        project_uuid=project_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    user_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Deletes a user from the current user's organization
+) -> Response[ListChartsInProjectResponse200]:
+    """List all charts in a project
 
     Args:
-        user_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[ListChartsInProjectResponse200]
     """
 
     kwargs = _get_kwargs(
-        user_uuid=user_uuid,
+        project_uuid=project_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    user_uuid: str,
+    project_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Deletes a user from the current user's organization
+) -> Optional[ListChartsInProjectResponse200]:
+    """List all charts in a project
 
     Args:
-        user_uuid (str):
+        project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        ListChartsInProjectResponse200
     """
 
     return (
         await asyncio_detailed(
-            user_uuid=user_uuid,
+            project_uuid=project_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/organizations/get_my_organization.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/list_organization_members.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,69 +3,69 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_organization import ApiOrganization
+from ...models.list_organization_members_response_200 import ListOrganizationMembersResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/org".format(client.base_url)
+    url = "{}/api/v1/org/users".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiOrganization]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ListOrganizationMembersResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiOrganization.from_dict(response.json())
+        response_200 = ListOrganizationMembersResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiOrganization]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ListOrganizationMembersResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[ApiOrganization]:
-    """Get the current user's organization
+) -> Response[ListOrganizationMembersResponse200]:
+    """Gets all the members of the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganization]
+        Response[ListOrganizationMembersResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -75,42 +75,42 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[ApiOrganization]:
-    """Get the current user's organization
+) -> Optional[ListOrganizationMembersResponse200]:
+    """Gets all the members of the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganization
+        ListOrganizationMembersResponse200
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[ApiOrganization]:
-    """Get the current user's organization
+) -> Response[ListOrganizationMembersResponse200]:
+    """Gets all the members of the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganization]
+        Response[ListOrganizationMembersResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -118,23 +118,23 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[ApiOrganization]:
-    """Get the current user's organization
+) -> Optional[ListOrganizationMembersResponse200]:
+    """Gets all the members of the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganization
+        ListOrganizationMembersResponse200
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_groups_in_organization.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/get_my_organization.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,69 +3,69 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_group_list_response import ApiGroupListResponse
+from ...models.get_my_organization_response_200 import GetMyOrganizationResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/org/groups".format(client.base_url)
+    url = "{}/api/v1/org".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiGroupListResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetMyOrganizationResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiGroupListResponse.from_dict(response.json())
+        response_200 = GetMyOrganizationResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiGroupListResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetMyOrganizationResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[ApiGroupListResponse]:
-    """Gets all the groups in the current user's organization
+) -> Response[GetMyOrganizationResponse200]:
+    """Get the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiGroupListResponse]
+        Response[GetMyOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -75,42 +75,42 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[ApiGroupListResponse]:
-    """Gets all the groups in the current user's organization
+) -> Optional[GetMyOrganizationResponse200]:
+    """Get the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiGroupListResponse
+        GetMyOrganizationResponse200
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[ApiGroupListResponse]:
-    """Gets all the groups in the current user's organization
+) -> Response[GetMyOrganizationResponse200]:
+    """Get the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiGroupListResponse]
+        Response[GetMyOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -118,23 +118,23 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[ApiGroupListResponse]:
-    """Gets all the groups in the current user's organization
+) -> Optional[GetMyOrganizationResponse200]:
+    """Get the current user's organization
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiGroupListResponse
+        GetMyOrganizationResponse200
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_email_domains.py` & `lightdash_client_python-0.621.0/lightdash_client/api/my_account/create_email_one_time_passcode.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,69 +3,70 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_organization_allowed_email_domains import ApiOrganizationAllowedEmailDomains
+from ...models.create_email_one_time_passcode_response_200 import CreateEmailOneTimePasscodeResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/org/allowedEmailDomains".format(client.base_url)
+    url = "{}/api/v1/user/me/email/otp".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "put",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiOrganizationAllowedEmailDomains]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreateEmailOneTimePasscodeResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiOrganizationAllowedEmailDomains.from_dict(response.json())
+        response_200 = CreateEmailOneTimePasscodeResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiOrganizationAllowedEmailDomains]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[CreateEmailOneTimePasscodeResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[ApiOrganizationAllowedEmailDomains]:
-    """Gets the allowed email domains for the current user's organization
+) -> Response[CreateEmailOneTimePasscodeResponse200]:
+    """Create a new one-time passcode for the current user's primary email.
+    The user will receive an email with the passcode.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganizationAllowedEmailDomains]
+        Response[CreateEmailOneTimePasscodeResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     response = httpx.request(
@@ -75,42 +76,44 @@
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[ApiOrganizationAllowedEmailDomains]:
-    """Gets the allowed email domains for the current user's organization
+) -> Optional[CreateEmailOneTimePasscodeResponse200]:
+    """Create a new one-time passcode for the current user's primary email.
+    The user will receive an email with the passcode.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganizationAllowedEmailDomains
+        CreateEmailOneTimePasscodeResponse200
     """
 
     return sync_detailed(
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[ApiOrganizationAllowedEmailDomains]:
-    """Gets the allowed email domains for the current user's organization
+) -> Response[CreateEmailOneTimePasscodeResponse200]:
+    """Create a new one-time passcode for the current user's primary email.
+    The user will receive an email with the passcode.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganizationAllowedEmailDomains]
+        Response[CreateEmailOneTimePasscodeResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
@@ -118,23 +121,24 @@
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[ApiOrganizationAllowedEmailDomains]:
-    """Gets the allowed email domains for the current user's organization
+) -> Optional[CreateEmailOneTimePasscodeResponse200]:
+    """Create a new one-time passcode for the current user's primary email.
+    The user will receive an email with the passcode.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganizationAllowedEmailDomains
+        CreateEmailOneTimePasscodeResponse200
     """
 
     return (
         await asyncio_detailed(
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_members.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/delete_organization_member.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,138 +3,159 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_organization_member_profiles import ApiOrganizationMemberProfiles
+from ...models.delete_organization_member_response_200 import DeleteOrganizationMemberResponse200
 from ...types import Response
 
 
 def _get_kwargs(
+    user_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/org/users".format(client.base_url)
+    url = "{}/api/v1/org/user/{userUuid}".format(client.base_url, userUuid=user_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiOrganizationMemberProfiles]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[DeleteOrganizationMemberResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiOrganizationMemberProfiles.from_dict(response.json())
+        response_200 = DeleteOrganizationMemberResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiOrganizationMemberProfiles]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[DeleteOrganizationMemberResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    user_uuid: str,
     *,
     client: Client,
-) -> Response[ApiOrganizationMemberProfiles]:
-    """Gets all the members of the current user's organization
+) -> Response[DeleteOrganizationMemberResponse200]:
+    """Deletes a user from the current user's organization
+
+    Args:
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganizationMemberProfiles]
+        Response[DeleteOrganizationMemberResponse200]
     """
 
     kwargs = _get_kwargs(
+        user_uuid=user_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    user_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiOrganizationMemberProfiles]:
-    """Gets all the members of the current user's organization
+) -> Optional[DeleteOrganizationMemberResponse200]:
+    """Deletes a user from the current user's organization
+
+    Args:
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganizationMemberProfiles
+        DeleteOrganizationMemberResponse200
     """
 
     return sync_detailed(
+        user_uuid=user_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    user_uuid: str,
     *,
     client: Client,
-) -> Response[ApiOrganizationMemberProfiles]:
-    """Gets all the members of the current user's organization
+) -> Response[DeleteOrganizationMemberResponse200]:
+    """Deletes a user from the current user's organization
+
+    Args:
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganizationMemberProfiles]
+        Response[DeleteOrganizationMemberResponse200]
     """
 
     kwargs = _get_kwargs(
+        user_uuid=user_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    user_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiOrganizationMemberProfiles]:
-    """Gets all the members of the current user's organization
+) -> Optional[DeleteOrganizationMemberResponse200]:
+    """Deletes a user from the current user's organization
+
+    Args:
+        user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganizationMemberProfiles
+        DeleteOrganizationMemberResponse200
     """
 
     return (
         await asyncio_detailed(
+            user_uuid=user_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/organizations/list_organization_projects.py` & `lightdash_client_python-0.621.0/lightdash_client/api/organizations/create_group_in_organization.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,138 +3,167 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_organization_projects import ApiOrganizationProjects
+from ...models.create_group_in_organization_json_body import CreateGroupInOrganizationJsonBody
+from ...models.create_group_in_organization_response_200 import CreateGroupInOrganizationResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
+    json_body: CreateGroupInOrganizationJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/org/projects".format(client.base_url)
+    url = "{}/api/v1/org/groups".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "get",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiOrganizationProjects]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreateGroupInOrganizationResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiOrganizationProjects.from_dict(response.json())
+        response_200 = CreateGroupInOrganizationResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiOrganizationProjects]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[CreateGroupInOrganizationResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-) -> Response[ApiOrganizationProjects]:
-    """Gets all projects of the current user's organization
+    json_body: CreateGroupInOrganizationJsonBody,
+) -> Response[CreateGroupInOrganizationResponse200]:
+    """Creates a new group in the current user's organization
+
+    Args:
+        json_body (CreateGroupInOrganizationJsonBody): From T, pick a set of properties whose keys
+            are in the union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganizationProjects]
+        Response[CreateGroupInOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     *,
     client: Client,
-) -> Optional[ApiOrganizationProjects]:
-    """Gets all projects of the current user's organization
+    json_body: CreateGroupInOrganizationJsonBody,
+) -> Optional[CreateGroupInOrganizationResponse200]:
+    """Creates a new group in the current user's organization
+
+    Args:
+        json_body (CreateGroupInOrganizationJsonBody): From T, pick a set of properties whose keys
+            are in the union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganizationProjects
+        CreateGroupInOrganizationResponse200
     """
 
     return sync_detailed(
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
     client: Client,
-) -> Response[ApiOrganizationProjects]:
-    """Gets all projects of the current user's organization
+    json_body: CreateGroupInOrganizationJsonBody,
+) -> Response[CreateGroupInOrganizationResponse200]:
+    """Creates a new group in the current user's organization
+
+    Args:
+        json_body (CreateGroupInOrganizationJsonBody): From T, pick a set of properties whose keys
+            are in the union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganizationProjects]
+        Response[CreateGroupInOrganizationResponse200]
     """
 
     kwargs = _get_kwargs(
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     *,
     client: Client,
-) -> Optional[ApiOrganizationProjects]:
-    """Gets all projects of the current user's organization
+    json_body: CreateGroupInOrganizationJsonBody,
+) -> Optional[CreateGroupInOrganizationResponse200]:
+    """Creates a new group in the current user's organization
+
+    Args:
+        json_body (CreateGroupInOrganizationJsonBody): From T, pick a set of properties whose keys
+            are in the union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganizationProjects
+        CreateGroupInOrganizationResponse200
     """
 
     return (
         await asyncio_detailed(
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/projects/delete_validation_dismiss.py` & `lightdash_client_python-0.621.0/lightdash_client/api/exploring/post_run_query.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,174 +3,191 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_validation_dismiss_response import ApiValidationDismissResponse
+from ...models.post_run_query_json_body import PostRunQueryJsonBody
+from ...models.post_run_query_response_200 import PostRunQueryResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
-    validation_id: float,
+    explore_id: str,
     *,
     client: Client,
+    json_body: PostRunQueryJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/validate/{validationId}".format(
-        client.base_url, projectUuid=project_uuid, validationId=validation_id
+    url = "{}/api/v1/projects/{projectUuid}/explores/{exploreId}/runQuery".format(
+        client.base_url, projectUuid=project_uuid, exploreId=explore_id
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
+    json_json_body = json_body.to_dict()
+
     return {
-        "method": "delete",
+        "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
+        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiValidationDismissResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PostRunQueryResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiValidationDismissResponse.from_dict(response.json())
+        response_200 = PostRunQueryResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiValidationDismissResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[PostRunQueryResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
-    validation_id: float,
+    explore_id: str,
     *,
     client: Client,
-) -> Response[ApiValidationDismissResponse]:
-    """Deletes a single validation error.
+    json_body: PostRunQueryJsonBody,
+) -> Response[PostRunQueryResponse200]:
+    """Run a query for explore
 
     Args:
         project_uuid (str):
-        validation_id (float):
+        explore_id (str):
+        json_body (PostRunQueryJsonBody): metricQuery for the chart to run
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiValidationDismissResponse]
+        Response[PostRunQueryResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        validation_id=validation_id,
+        explore_id=explore_id,
         client=client,
+        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
-    validation_id: float,
+    explore_id: str,
     *,
     client: Client,
-) -> Optional[ApiValidationDismissResponse]:
-    """Deletes a single validation error.
+    json_body: PostRunQueryJsonBody,
+) -> Optional[PostRunQueryResponse200]:
+    """Run a query for explore
 
     Args:
         project_uuid (str):
-        validation_id (float):
+        explore_id (str):
+        json_body (PostRunQueryJsonBody): metricQuery for the chart to run
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiValidationDismissResponse
+        PostRunQueryResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
-        validation_id=validation_id,
+        explore_id=explore_id,
         client=client,
+        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
-    validation_id: float,
+    explore_id: str,
     *,
     client: Client,
-) -> Response[ApiValidationDismissResponse]:
-    """Deletes a single validation error.
+    json_body: PostRunQueryJsonBody,
+) -> Response[PostRunQueryResponse200]:
+    """Run a query for explore
 
     Args:
         project_uuid (str):
-        validation_id (float):
+        explore_id (str):
+        json_body (PostRunQueryJsonBody): metricQuery for the chart to run
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiValidationDismissResponse]
+        Response[PostRunQueryResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        validation_id=validation_id,
+        explore_id=explore_id,
         client=client,
+        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
-    validation_id: float,
+    explore_id: str,
     *,
     client: Client,
-) -> Optional[ApiValidationDismissResponse]:
-    """Deletes a single validation error.
+    json_body: PostRunQueryJsonBody,
+) -> Optional[PostRunQueryResponse200]:
+    """Run a query for explore
 
     Args:
         project_uuid (str):
-        validation_id (float):
+        explore_id (str):
+        json_body (PostRunQueryJsonBody): metricQuery for the chart to run
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiValidationDismissResponse
+        PostRunQueryResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
-            validation_id=validation_id,
+            explore_id=explore_id,
             client=client,
+            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/projects/get_latest_validation_results.py` & `lightdash_client_python-0.621.0/lightdash_client/api/projects/get_latest_validation_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional
 from typing import Union
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_validate_response import ApiValidateResponse
+from ...models.get_latest_validation_results_response_200 import GetLatestValidationResultsResponse200
 from ...types import Response
 from ...types import UNSET
 from ...types import Unset
 
 
 def _get_kwargs(
     project_uuid: str,
@@ -40,54 +40,54 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "params": params,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiValidateResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetLatestValidationResultsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiValidateResponse.from_dict(response.json())
+        response_200 = GetLatestValidationResultsResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiValidateResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetLatestValidationResultsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
     from_settings: Union[Unset, None, bool] = UNSET,
     job_id: Union[Unset, None, str] = UNSET,
-) -> Response[ApiValidateResponse]:
+) -> Response[GetLatestValidationResultsResponse200]:
     """Get validation results for a project. This will return the results of the latest validation job.
 
     Args:
         project_uuid (str):
         from_settings (Union[Unset, None, bool]):
         job_id (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiValidateResponse]
+        Response[GetLatestValidationResultsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
         from_settings=from_settings,
         job_id=job_id,
@@ -103,28 +103,28 @@
 
 def sync(
     project_uuid: str,
     *,
     client: Client,
     from_settings: Union[Unset, None, bool] = UNSET,
     job_id: Union[Unset, None, str] = UNSET,
-) -> Optional[ApiValidateResponse]:
+) -> Optional[GetLatestValidationResultsResponse200]:
     """Get validation results for a project. This will return the results of the latest validation job.
 
     Args:
         project_uuid (str):
         from_settings (Union[Unset, None, bool]):
         job_id (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiValidateResponse
+        GetLatestValidationResultsResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         client=client,
         from_settings=from_settings,
         job_id=job_id,
@@ -133,28 +133,28 @@
 
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
     from_settings: Union[Unset, None, bool] = UNSET,
     job_id: Union[Unset, None, str] = UNSET,
-) -> Response[ApiValidateResponse]:
+) -> Response[GetLatestValidationResultsResponse200]:
     """Get validation results for a project. This will return the results of the latest validation job.
 
     Args:
         project_uuid (str):
         from_settings (Union[Unset, None, bool]):
         job_id (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiValidateResponse]
+        Response[GetLatestValidationResultsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
         from_settings=from_settings,
         job_id=job_id,
@@ -168,28 +168,28 @@
 
 async def asyncio(
     project_uuid: str,
     *,
     client: Client,
     from_settings: Union[Unset, None, bool] = UNSET,
     job_id: Union[Unset, None, str] = UNSET,
-) -> Optional[ApiValidateResponse]:
+) -> Optional[GetLatestValidationResultsResponse200]:
     """Get validation results for a project. This will return the results of the latest validation job.
 
     Args:
         project_uuid (str):
         from_settings (Union[Unset, None, bool]):
         job_id (Union[Unset, None, str]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiValidateResponse
+        GetLatestValidationResultsResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             client=client,
             from_settings=from_settings,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/projects/list_charts_in_project.py` & `lightdash_client_python-0.621.0/lightdash_client/api/spaces/get_space.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,159 +3,174 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_chart_summary_list_response import ApiChartSummaryListResponse
+from ...models.get_space_response_200 import GetSpaceResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/charts".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/spaces/{spaceUuid}".format(
+        client.base_url, projectUuid=project_uuid, spaceUuid=space_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiChartSummaryListResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetSpaceResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiChartSummaryListResponse.from_dict(response.json())
+        response_200 = GetSpaceResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiChartSummaryListResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetSpaceResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Response[ApiChartSummaryListResponse]:
-    """List all charts in a project
+) -> Response[GetSpaceResponse200]:
+    """Get details for a space in a project
 
     Args:
         project_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiChartSummaryListResponse]
+        Response[GetSpaceResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiChartSummaryListResponse]:
-    """List all charts in a project
+) -> Optional[GetSpaceResponse200]:
+    """Get details for a space in a project
 
     Args:
         project_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiChartSummaryListResponse
+        GetSpaceResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Response[ApiChartSummaryListResponse]:
-    """List all charts in a project
+) -> Response[GetSpaceResponse200]:
+    """Get details for a space in a project
 
     Args:
         project_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiChartSummaryListResponse]
+        Response[GetSpaceResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiChartSummaryListResponse]:
-    """List all charts in a project
+) -> Optional[GetSpaceResponse200]:
+    """Get details for a space in a project
 
     Args:
         project_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiChartSummaryListResponse
+        GetSpaceResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
+            space_uuid=space_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/projects/list_spaces_in_project.py` & `lightdash_client_python-0.621.0/lightdash_client/api/schedulers/get_scheduler_job_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,159 +3,163 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_space_summary_list_response import ApiSpaceSummaryListResponse
+from ...models.get_scheduler_job_status_response_200 import GetSchedulerJobStatusResponse200
 from ...types import Response
 
 
 def _get_kwargs(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/spaces".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/schedulers/job/{jobId}/status".format(client.base_url, jobId=job_id)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSpaceSummaryListResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetSchedulerJobStatusResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSpaceSummaryListResponse.from_dict(response.json())
+        response_200 = GetSchedulerJobStatusResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSpaceSummaryListResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetSchedulerJobStatusResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-) -> Response[ApiSpaceSummaryListResponse]:
-    """List all spaces in a project
+) -> Response[GetSchedulerJobStatusResponse200]:
+    """Get a generic job status
+    This method can be used when polling from the frontend
 
     Args:
-        project_uuid (str):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSpaceSummaryListResponse]
+        Response[GetSchedulerJobStatusResponse200]
     """
 
     kwargs = _get_kwargs(
-        project_uuid=project_uuid,
+        job_id=job_id,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-) -> Optional[ApiSpaceSummaryListResponse]:
-    """List all spaces in a project
+) -> Optional[GetSchedulerJobStatusResponse200]:
+    """Get a generic job status
+    This method can be used when polling from the frontend
 
     Args:
-        project_uuid (str):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSpaceSummaryListResponse
+        GetSchedulerJobStatusResponse200
     """
 
     return sync_detailed(
-        project_uuid=project_uuid,
+        job_id=job_id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-) -> Response[ApiSpaceSummaryListResponse]:
-    """List all spaces in a project
+) -> Response[GetSchedulerJobStatusResponse200]:
+    """Get a generic job status
+    This method can be used when polling from the frontend
 
     Args:
-        project_uuid (str):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSpaceSummaryListResponse]
+        Response[GetSchedulerJobStatusResponse200]
     """
 
     kwargs = _get_kwargs(
-        project_uuid=project_uuid,
+        job_id=job_id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    project_uuid: str,
+    job_id: str,
     *,
     client: Client,
-) -> Optional[ApiSpaceSummaryListResponse]:
-    """List all spaces in a project
+) -> Optional[GetSchedulerJobStatusResponse200]:
+    """Get a generic job status
+    This method can be used when polling from the frontend
 
     Args:
-        project_uuid (str):
+        job_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSpaceSummaryListResponse
+        GetSchedulerJobStatusResponse200
     """
 
     return (
         await asyncio_detailed(
-            project_uuid=project_uuid,
+            job_id=job_id,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/projects/validate_project.py` & `lightdash_client_python-0.621.0/lightdash_client/api/projects/validate_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_job_scheduled_response import ApiJobScheduledResponse
 from ...models.validate_project_json_body import ValidateProjectJsonBody
+from ...models.validate_project_response_200 import ValidateProjectResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     *,
     client: Client,
@@ -32,40 +32,40 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiJobScheduledResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ValidateProjectResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiJobScheduledResponse.from_dict(response.json())
+        response_200 = ValidateProjectResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiJobScheduledResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[ValidateProjectResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
     json_body: ValidateProjectJsonBody,
-) -> Response[ApiJobScheduledResponse]:
+) -> Response[ValidateProjectResponse200]:
     """Validate content inside a project. This will start a validation job and return the job id.
 
     Validation jobs scan all charts and dashboards inside a project to find any broken references
     to metrics or dimensions that aren't available. Results are available after the job is completed.
 
     Args:
         project_uuid (str):
@@ -73,15 +73,15 @@
             project, this is used in the CLI to validate a project without creating a preview
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiJobScheduledResponse]
+        Response[ValidateProjectResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
         json_body=json_body,
     )
@@ -95,15 +95,15 @@
 
 
 def sync(
     project_uuid: str,
     *,
     client: Client,
     json_body: ValidateProjectJsonBody,
-) -> Optional[ApiJobScheduledResponse]:
+) -> Optional[ValidateProjectResponse200]:
     """Validate content inside a project. This will start a validation job and return the job id.
 
     Validation jobs scan all charts and dashboards inside a project to find any broken references
     to metrics or dimensions that aren't available. Results are available after the job is completed.
 
     Args:
         project_uuid (str):
@@ -111,30 +111,30 @@
             project, this is used in the CLI to validate a project without creating a preview
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiJobScheduledResponse
+        ValidateProjectResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
     json_body: ValidateProjectJsonBody,
-) -> Response[ApiJobScheduledResponse]:
+) -> Response[ValidateProjectResponse200]:
     """Validate content inside a project. This will start a validation job and return the job id.
 
     Validation jobs scan all charts and dashboards inside a project to find any broken references
     to metrics or dimensions that aren't available. Results are available after the job is completed.
 
     Args:
         project_uuid (str):
@@ -142,15 +142,15 @@
             project, this is used in the CLI to validate a project without creating a preview
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiJobScheduledResponse]
+        Response[ValidateProjectResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
         json_body=json_body,
     )
@@ -162,15 +162,15 @@
 
 
 async def asyncio(
     project_uuid: str,
     *,
     client: Client,
     json_body: ValidateProjectJsonBody,
-) -> Optional[ApiJobScheduledResponse]:
+) -> Optional[ValidateProjectResponse200]:
     """Validate content inside a project. This will start a validation job and return the job id.
 
     Validation jobs scan all charts and dashboards inside a project to find any broken references
     to metrics or dimensions that aren't available. Results are available after the job is completed.
 
     Args:
         project_uuid (str):
@@ -178,15 +178,15 @@
             project, this is used in the CLI to validate a project without creating a preview
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiJobScheduledResponse
+        ValidateProjectResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             client=client,
             json_body=json_body,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/create_space_in_project.py` & `lightdash_client_python-0.621.0/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,115 +3,134 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.create_space import CreateSpace
+from ...models.create_ssh_key_pair_response_201 import CreateSshKeyPairResponse201
 from ...types import Response
 
 
 def _get_kwargs(
-    project_uuid: str,
     *,
     client: Client,
-    json_body: CreateSpace,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/spaces".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/ssh/key-pairs".format(client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[CreateSshKeyPairResponse201]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = CreateSshKeyPairResponse201.from_dict(response.json())
+
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[CreateSshKeyPairResponse201]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    project_uuid: str,
     *,
     client: Client,
-    json_body: CreateSpace,
-) -> Response[Any]:
-    """Create a new space inside a project
-
-    Args:
-        project_uuid (str):
-        json_body (CreateSpace):
-
+) -> Response[CreateSshKeyPairResponse201]:
+    """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[CreateSshKeyPairResponse201]
     """
 
     kwargs = _get_kwargs(
-        project_uuid=project_uuid,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
-async def asyncio_detailed(
-    project_uuid: str,
+def sync(
     *,
     client: Client,
-    json_body: CreateSpace,
-) -> Response[Any]:
-    """Create a new space inside a project
-
-    Args:
-        project_uuid (str):
-        json_body (CreateSpace):
+) -> Optional[CreateSshKeyPairResponse201]:
+    """
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        CreateSshKeyPairResponse201
+    """
 
+    return sync_detailed(
+        client=client,
+    ).parsed
+
+
+async def asyncio_detailed(
+    *,
+    client: Client,
+) -> Response[CreateSshKeyPairResponse201]:
+    """
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[CreateSshKeyPairResponse201]
     """
 
     kwargs = _get_kwargs(
-        project_uuid=project_uuid,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
+
+
+async def asyncio(
+    *,
+    client: Client,
+) -> Optional[CreateSshKeyPairResponse201]:
+    """
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        CreateSshKeyPairResponse201
+    """
+
+    return (
+        await asyncio_detailed(
+            client=client,
+        )
+    ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/get_project_access_list.py` & `lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/get_project_access_list.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_project_access_list_response import ApiProjectAccessListResponse
+from ...models.get_project_access_list_response_200 import GetProjectAccessListResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     *,
     client: Client,
@@ -27,52 +27,52 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiProjectAccessListResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetProjectAccessListResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiProjectAccessListResponse.from_dict(response.json())
+        response_200 = GetProjectAccessListResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiProjectAccessListResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetProjectAccessListResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[ApiProjectAccessListResponse]:
+) -> Response[GetProjectAccessListResponse200]:
     """Get access list for a project. This is a list of users that have been explictly granted access to
     the project.
     There may be other users that have access to the project via their organization membership.
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiProjectAccessListResponse]
+        Response[GetProjectAccessListResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
@@ -84,54 +84,54 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiProjectAccessListResponse]:
+) -> Optional[GetProjectAccessListResponse200]:
     """Get access list for a project. This is a list of users that have been explictly granted access to
     the project.
     There may be other users that have access to the project via their organization membership.
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiProjectAccessListResponse
+        GetProjectAccessListResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
     *,
     client: Client,
-) -> Response[ApiProjectAccessListResponse]:
+) -> Response[GetProjectAccessListResponse200]:
     """Get access list for a project. This is a list of users that have been explictly granted access to
     the project.
     There may be other users that have access to the project via their organization membership.
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiProjectAccessListResponse]
+        Response[GetProjectAccessListResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         client=client,
     )
 
@@ -141,28 +141,28 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiProjectAccessListResponse]:
+) -> Optional[GetProjectAccessListResponse200]:
     """Get access list for a project. This is a list of users that have been explictly granted access to
     the project.
     There may be other users that have access to the project via their organization membership.
 
     Args:
         project_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiProjectAccessListResponse
+        GetProjectAccessListResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/grant_project_access_to_user.py` & `lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/update_space.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,176 +3,195 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
-from ...models.create_project_member import CreateProjectMember
+from ...models.update_space_json_body import UpdateSpaceJsonBody
+from ...models.update_space_response_200 import UpdateSpaceResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-    json_body: CreateProjectMember,
+    json_body: UpdateSpaceJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/access".format(client.base_url, projectUuid=project_uuid)
+    url = "{}/api/v1/projects/{projectUuid}/spaces/{spaceUuid}".format(
+        client.base_url, projectUuid=project_uuid, spaceUuid=space_uuid
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
 
     return {
-        "method": "post",
+        "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[UpdateSpaceResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = UpdateSpaceResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[UpdateSpaceResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-    json_body: CreateProjectMember,
-) -> Response[ApiSuccessEmpty]:
-    """Grant a user access to a project
+    json_body: UpdateSpaceJsonBody,
+) -> Response[UpdateSpaceResponse200]:
+    """Update a space in a project
 
     Args:
         project_uuid (str):
-        json_body (CreateProjectMember):
+        space_uuid (str):
+        json_body (UpdateSpaceJsonBody): From T, pick a set of properties whose keys are in the
+            union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[UpdateSpaceResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
         json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-    json_body: CreateProjectMember,
-) -> Optional[ApiSuccessEmpty]:
-    """Grant a user access to a project
+    json_body: UpdateSpaceJsonBody,
+) -> Optional[UpdateSpaceResponse200]:
+    """Update a space in a project
 
     Args:
         project_uuid (str):
-        json_body (CreateProjectMember):
+        space_uuid (str):
+        json_body (UpdateSpaceJsonBody): From T, pick a set of properties whose keys are in the
+            union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        UpdateSpaceResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-    json_body: CreateProjectMember,
-) -> Response[ApiSuccessEmpty]:
-    """Grant a user access to a project
+    json_body: UpdateSpaceJsonBody,
+) -> Response[UpdateSpaceResponse200]:
+    """Update a space in a project
 
     Args:
         project_uuid (str):
-        json_body (CreateProjectMember):
+        space_uuid (str):
+        json_body (UpdateSpaceJsonBody): From T, pick a set of properties whose keys are in the
+            union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[UpdateSpaceResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
+        space_uuid=space_uuid,
         client=client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-    json_body: CreateProjectMember,
-) -> Optional[ApiSuccessEmpty]:
-    """Grant a user access to a project
+    json_body: UpdateSpaceJsonBody,
+) -> Optional[UpdateSpaceResponse200]:
+    """Update a space in a project
 
     Args:
         project_uuid (str):
-        json_body (CreateProjectMember):
+        space_uuid (str):
+        json_body (UpdateSpaceJsonBody): From T, pick a set of properties whose keys are in the
+            union K
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        UpdateSpaceResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
+            space_uuid=space_uuid,
             client=client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py` & `lightdash_client_python-0.621.0/lightdash_client/api/spaces/delete_space.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.delete_space_response_204 import DeleteSpaceResponse204
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
-    user_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/access/{userUuid}".format(
-        client.base_url, projectUuid=project_uuid, userUuid=user_uuid
+    url = "{}/api/v1/projects/{projectUuid}/spaces/{spaceUuid}".format(
+        client.base_url, projectUuid=project_uuid, spaceUuid=space_uuid
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
         "method": "delete",
@@ -30,147 +30,147 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[DeleteSpaceResponse204]:
+    if response.status_code == HTTPStatus.NO_CONTENT:
+        response_204 = DeleteSpaceResponse204.from_dict(response.json())
 
-        return response_200
+        return response_204
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[DeleteSpaceResponse204]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
-    user_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Remove a user's access to a project
+) -> Response[DeleteSpaceResponse204]:
+    """Delete a space from a project
 
     Args:
         project_uuid (str):
-        user_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[DeleteSpaceResponse204]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        user_uuid=user_uuid,
+        space_uuid=space_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
-    user_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Remove a user's access to a project
+) -> Optional[DeleteSpaceResponse204]:
+    """Delete a space from a project
 
     Args:
         project_uuid (str):
-        user_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        DeleteSpaceResponse204
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
-        user_uuid=user_uuid,
+        space_uuid=space_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
-    user_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Remove a user's access to a project
+) -> Response[DeleteSpaceResponse204]:
+    """Delete a space from a project
 
     Args:
         project_uuid (str):
-        user_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[DeleteSpaceResponse204]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        user_uuid=user_uuid,
+        space_uuid=space_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
-    user_uuid: str,
+    space_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Remove a user's access to a project
+) -> Optional[DeleteSpaceResponse204]:
+    """Delete a space from a project
 
     Args:
         project_uuid (str):
-        user_uuid (str):
+        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        DeleteSpaceResponse204
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
-            user_uuid=user_uuid,
+            space_uuid=space_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py` & `lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.revoke_space_access_for_user_response_200 import RevokeSpaceAccessForUserResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
     space_uuid: str,
     user_uuid: str,
@@ -31,54 +31,54 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[RevokeSpaceAccessForUserResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = RevokeSpaceAccessForUserResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[RevokeSpaceAccessForUserResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
     space_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
+) -> Response[RevokeSpaceAccessForUserResponse200]:
     """Remove a user's access to a space
 
     Args:
         project_uuid (str):
         space_uuid (str):
         user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[RevokeSpaceAccessForUserResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         space_uuid=space_uuid,
         user_uuid=user_uuid,
         client=client,
@@ -94,28 +94,28 @@
 
 def sync(
     project_uuid: str,
     space_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
+) -> Optional[RevokeSpaceAccessForUserResponse200]:
     """Remove a user's access to a space
 
     Args:
         project_uuid (str):
         space_uuid (str):
         user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        RevokeSpaceAccessForUserResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
         space_uuid=space_uuid,
         user_uuid=user_uuid,
         client=client,
@@ -124,28 +124,28 @@
 
 async def asyncio_detailed(
     project_uuid: str,
     space_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
+) -> Response[RevokeSpaceAccessForUserResponse200]:
     """Remove a user's access to a space
 
     Args:
         project_uuid (str):
         space_uuid (str):
         user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[RevokeSpaceAccessForUserResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
         space_uuid=space_uuid,
         user_uuid=user_uuid,
         client=client,
@@ -159,28 +159,28 @@
 
 async def asyncio(
     project_uuid: str,
     space_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
+) -> Optional[RevokeSpaceAccessForUserResponse200]:
     """Remove a user's access to a space
 
     Args:
         project_uuid (str):
         space_uuid (str):
         user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        RevokeSpaceAccessForUserResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
             space_uuid=space_uuid,
             user_uuid=user_uuid,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/update_organization_member.py` & `lightdash_client_python-0.621.0/lightdash_client/api/roles_permissions/update_organization_member.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_organization_member_profile import ApiOrganizationMemberProfile
-from ...models.organization_member_profile_update import OrganizationMemberProfileUpdate
+from ...models.update_organization_member_json_body import UpdateOrganizationMemberJsonBody
+from ...models.update_organization_member_response_200 import UpdateOrganizationMemberResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     user_uuid: str,
     *,
     client: Client,
-    json_body: OrganizationMemberProfileUpdate,
+    json_body: UpdateOrganizationMemberJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/org/users/{userUuid}".format(client.base_url, userUuid=user_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     json_json_body = json_body.to_dict()
@@ -32,52 +32,52 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiOrganizationMemberProfile]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[UpdateOrganizationMemberResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiOrganizationMemberProfile.from_dict(response.json())
+        response_200 = UpdateOrganizationMemberResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiOrganizationMemberProfile]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[UpdateOrganizationMemberResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     user_uuid: str,
     *,
     client: Client,
-    json_body: OrganizationMemberProfileUpdate,
-) -> Response[ApiOrganizationMemberProfile]:
+    json_body: UpdateOrganizationMemberJsonBody,
+) -> Response[UpdateOrganizationMemberResponse200]:
     """Updates the membership profile for a user in the current user's organization
 
     Args:
         user_uuid (str):
-        json_body (OrganizationMemberProfileUpdate):
+        json_body (UpdateOrganizationMemberJsonBody): the new membership profile
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganizationMemberProfile]
+        Response[UpdateOrganizationMemberResponse200]
     """
 
     kwargs = _get_kwargs(
         user_uuid=user_uuid,
         client=client,
         json_body=json_body,
     )
@@ -90,55 +90,55 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     user_uuid: str,
     *,
     client: Client,
-    json_body: OrganizationMemberProfileUpdate,
-) -> Optional[ApiOrganizationMemberProfile]:
+    json_body: UpdateOrganizationMemberJsonBody,
+) -> Optional[UpdateOrganizationMemberResponse200]:
     """Updates the membership profile for a user in the current user's organization
 
     Args:
         user_uuid (str):
-        json_body (OrganizationMemberProfileUpdate):
+        json_body (UpdateOrganizationMemberJsonBody): the new membership profile
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganizationMemberProfile
+        UpdateOrganizationMemberResponse200
     """
 
     return sync_detailed(
         user_uuid=user_uuid,
         client=client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     user_uuid: str,
     *,
     client: Client,
-    json_body: OrganizationMemberProfileUpdate,
-) -> Response[ApiOrganizationMemberProfile]:
+    json_body: UpdateOrganizationMemberJsonBody,
+) -> Response[UpdateOrganizationMemberResponse200]:
     """Updates the membership profile for a user in the current user's organization
 
     Args:
         user_uuid (str):
-        json_body (OrganizationMemberProfileUpdate):
+        json_body (UpdateOrganizationMemberJsonBody): the new membership profile
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiOrganizationMemberProfile]
+        Response[UpdateOrganizationMemberResponse200]
     """
 
     kwargs = _get_kwargs(
         user_uuid=user_uuid,
         client=client,
         json_body=json_body,
     )
@@ -149,28 +149,28 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     user_uuid: str,
     *,
     client: Client,
-    json_body: OrganizationMemberProfileUpdate,
-) -> Optional[ApiOrganizationMemberProfile]:
+    json_body: UpdateOrganizationMemberJsonBody,
+) -> Optional[UpdateOrganizationMemberResponse200]:
     """Updates the membership profile for a user in the current user's organization
 
     Args:
         user_uuid (str):
-        json_body (OrganizationMemberProfileUpdate):
+        json_body (UpdateOrganizationMemberJsonBody): the new membership profile
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiOrganizationMemberProfile
+        UpdateOrganizationMemberResponse200
     """
 
     return (
         await asyncio_detailed(
             user_uuid=user_uuid,
             client=client,
             json_body=json_body,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/roles_permissions/update_project_access_for_user.py` & `lightdash_client_python-0.621.0/lightdash_client/api/user_groups/remove_user_from_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,191 +3,174 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
-from ...models.update_project_member import UpdateProjectMember
+from ...models.remove_user_from_group_response_200 import RemoveUserFromGroupResponse200
 from ...types import Response
 
 
 def _get_kwargs(
-    project_uuid: str,
+    group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-    json_body: UpdateProjectMember,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/access/{userUuid}".format(
-        client.base_url, projectUuid=project_uuid, userUuid=user_uuid
+    url = "{}/api/v1/groups/{groupUuid}/members/{userUuid}".format(
+        client.base_url, groupUuid=group_uuid, userUuid=user_uuid
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
-    json_json_body = json_body.to_dict()
-
     return {
-        "method": "patch",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[RemoveUserFromGroupResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = RemoveUserFromGroupResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[RemoveUserFromGroupResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    project_uuid: str,
+    group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-    json_body: UpdateProjectMember,
-) -> Response[ApiSuccessEmpty]:
-    """Update a user's access to a project
+) -> Response[RemoveUserFromGroupResponse200]:
+    """Remove a user from a group
 
     Args:
-        project_uuid (str):
+        group_uuid (str):
         user_uuid (str):
-        json_body (UpdateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[RemoveUserFromGroupResponse200]
     """
 
     kwargs = _get_kwargs(
-        project_uuid=project_uuid,
+        group_uuid=group_uuid,
         user_uuid=user_uuid,
         client=client,
-        json_body=json_body,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    project_uuid: str,
+    group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-    json_body: UpdateProjectMember,
-) -> Optional[ApiSuccessEmpty]:
-    """Update a user's access to a project
+) -> Optional[RemoveUserFromGroupResponse200]:
+    """Remove a user from a group
 
     Args:
-        project_uuid (str):
+        group_uuid (str):
         user_uuid (str):
-        json_body (UpdateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        RemoveUserFromGroupResponse200
     """
 
     return sync_detailed(
-        project_uuid=project_uuid,
+        group_uuid=group_uuid,
         user_uuid=user_uuid,
         client=client,
-        json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
-    project_uuid: str,
+    group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-    json_body: UpdateProjectMember,
-) -> Response[ApiSuccessEmpty]:
-    """Update a user's access to a project
+) -> Response[RemoveUserFromGroupResponse200]:
+    """Remove a user from a group
 
     Args:
-        project_uuid (str):
+        group_uuid (str):
         user_uuid (str):
-        json_body (UpdateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[RemoveUserFromGroupResponse200]
     """
 
     kwargs = _get_kwargs(
-        project_uuid=project_uuid,
+        group_uuid=group_uuid,
         user_uuid=user_uuid,
         client=client,
-        json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    project_uuid: str,
+    group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-    json_body: UpdateProjectMember,
-) -> Optional[ApiSuccessEmpty]:
-    """Update a user's access to a project
+) -> Optional[RemoveUserFromGroupResponse200]:
+    """Remove a user from a group
 
     Args:
-        project_uuid (str):
+        group_uuid (str):
         user_uuid (str):
-        json_body (UpdateProjectMember):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        RemoveUserFromGroupResponse200
     """
 
     return (
         await asyncio_detailed(
-            project_uuid=project_uuid,
+            group_uuid=group_uuid,
             user_uuid=user_uuid,
             client=client,
-            json_body=json_body,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/delete_scheduler.py` & `lightdash_client_python-0.621.0/lightdash_client/api/schedulers/delete_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduled_jobs.py` & `lightdash_client_python-0.621.0/lightdash_client/api/schedulers/get_scheduled_jobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_scheduled_jobs_response import ApiScheduledJobsResponse
+from ...models.get_scheduled_jobs_response_200 import GetScheduledJobsResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     scheduler_uuid: str,
     *,
     client: Client,
@@ -27,50 +27,50 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiScheduledJobsResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetScheduledJobsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiScheduledJobsResponse.from_dict(response.json())
+        response_200 = GetScheduledJobsResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiScheduledJobsResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetScheduledJobsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     scheduler_uuid: str,
     *,
     client: Client,
-) -> Response[ApiScheduledJobsResponse]:
+) -> Response[GetScheduledJobsResponse200]:
     """Get scheduled jobs
 
     Args:
         scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiScheduledJobsResponse]
+        Response[GetScheduledJobsResponse200]
     """
 
     kwargs = _get_kwargs(
         scheduler_uuid=scheduler_uuid,
         client=client,
     )
 
@@ -82,50 +82,50 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     scheduler_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiScheduledJobsResponse]:
+) -> Optional[GetScheduledJobsResponse200]:
     """Get scheduled jobs
 
     Args:
         scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiScheduledJobsResponse
+        GetScheduledJobsResponse200
     """
 
     return sync_detailed(
         scheduler_uuid=scheduler_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     scheduler_uuid: str,
     *,
     client: Client,
-) -> Response[ApiScheduledJobsResponse]:
+) -> Response[GetScheduledJobsResponse200]:
     """Get scheduled jobs
 
     Args:
         scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiScheduledJobsResponse]
+        Response[GetScheduledJobsResponse200]
     """
 
     kwargs = _get_kwargs(
         scheduler_uuid=scheduler_uuid,
         client=client,
     )
 
@@ -135,26 +135,26 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     scheduler_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiScheduledJobsResponse]:
+) -> Optional[GetScheduledJobsResponse200]:
     """Get scheduled jobs
 
     Args:
         scheduler_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiScheduledJobsResponse
+        GetScheduledJobsResponse200
     """
 
     return (
         await asyncio_detailed(
             scheduler_uuid=scheduler_uuid,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,93 @@
-from http import HTTPStatus
+import datetime
 from typing import Any
 from typing import Dict
-from typing import Optional
+from typing import List
+from typing import Type
+from typing import TypeVar
 
-import httpx
+import attr
+from dateutil.parser import isoparse
 
-from ... import errors
-from ...client import Client
-from ...types import Response
-
-
-def _get_kwargs(
-    scheduler_uuid: str,
-    *,
-    client: Client,
-) -> Dict[str, Any]:
-    url = "{}/api/v1/schedulers/{schedulerUuid}".format(client.base_url, schedulerUuid=scheduler_uuid)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    return {
-        "method": "get",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    scheduler_uuid: str,
-    *,
-    client: Client,
-) -> Response[Any]:
-    """Get a scheduler
+T = TypeVar("T", bound="ApiSchedulerLogsResponseResultsSchedulersItemTargetsItemType0")
 
-    Args:
-        scheduler_uuid (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
-    Returns:
-        Response[Any]
+@attr.s(auto_attribs=True)
+class ApiSchedulerLogsResponseResultsSchedulersItemTargetsItemType0:
     """
-
-    kwargs = _get_kwargs(
-        scheduler_uuid=scheduler_uuid,
-        client=client,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio_detailed(
-    scheduler_uuid: str,
-    *,
-    client: Client,
-) -> Response[Any]:
-    """Get a scheduler
-
-    Args:
+    Attributes:
+        channel (str):
         scheduler_uuid (str):
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Any]
+        updated_at (datetime.datetime):
+        created_at (datetime.datetime):
+        scheduler_slack_target_uuid (str):
     """
 
-    kwargs = _get_kwargs(
-        scheduler_uuid=scheduler_uuid,
-        client=client,
-    )
+    channel: str
+    scheduler_uuid: str
+    updated_at: datetime.datetime
+    created_at: datetime.datetime
+    scheduler_slack_target_uuid: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        channel = self.channel
+        scheduler_uuid = self.scheduler_uuid
+        updated_at = self.updated_at.isoformat()
+
+        created_at = self.created_at.isoformat()
+
+        scheduler_slack_target_uuid = self.scheduler_slack_target_uuid
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "channel": channel,
+                "schedulerUuid": scheduler_uuid,
+                "updatedAt": updated_at,
+                "createdAt": created_at,
+                "schedulerSlackTargetUuid": scheduler_slack_target_uuid,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        channel = d.pop("channel")
+
+        scheduler_uuid = d.pop("schedulerUuid")
+
+        updated_at = isoparse(d.pop("updatedAt"))
+
+        created_at = isoparse(d.pop("createdAt"))
+
+        scheduler_slack_target_uuid = d.pop("schedulerSlackTargetUuid")
+
+        api_scheduler_logs_response_results_schedulers_item_targets_item_type_0 = cls(
+            channel=channel,
+            scheduler_uuid=scheduler_uuid,
+            updated_at=updated_at,
+            created_at=created_at,
+            scheduler_slack_target_uuid=scheduler_slack_target_uuid,
+        )
+
+        api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.additional_properties = d
+        return api_scheduler_logs_response_results_schedulers_item_targets_item_type_0
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
 
-    return _build_response(client=client, response=response)
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/get_scheduler_job_status.py` & `lightdash_client_python-0.621.0/lightdash_client/api/projects/delete_validation_dismiss.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,163 +3,174 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_job_status_response import ApiJobStatusResponse
+from ...models.delete_validation_dismiss_response_200 import DeleteValidationDismissResponse200
 from ...types import Response
 
 
 def _get_kwargs(
-    job_id: str,
+    project_uuid: str,
+    validation_id: float,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/schedulers/job/{jobId}/status".format(client.base_url, jobId=job_id)
+    url = "{}/api/v1/projects/{projectUuid}/validate/{validationId}".format(
+        client.base_url, projectUuid=project_uuid, validationId=validation_id
+    )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiJobStatusResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[DeleteValidationDismissResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiJobStatusResponse.from_dict(response.json())
+        response_200 = DeleteValidationDismissResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiJobStatusResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[DeleteValidationDismissResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    job_id: str,
+    project_uuid: str,
+    validation_id: float,
     *,
     client: Client,
-) -> Response[ApiJobStatusResponse]:
-    """Get a generic job status
-    This method can be used when polling from the frontend
+) -> Response[DeleteValidationDismissResponse200]:
+    """Deletes a single validation error.
 
     Args:
-        job_id (str):
+        project_uuid (str):
+        validation_id (float):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiJobStatusResponse]
+        Response[DeleteValidationDismissResponse200]
     """
 
     kwargs = _get_kwargs(
-        job_id=job_id,
+        project_uuid=project_uuid,
+        validation_id=validation_id,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
-    job_id: str,
+    project_uuid: str,
+    validation_id: float,
     *,
     client: Client,
-) -> Optional[ApiJobStatusResponse]:
-    """Get a generic job status
-    This method can be used when polling from the frontend
+) -> Optional[DeleteValidationDismissResponse200]:
+    """Deletes a single validation error.
 
     Args:
-        job_id (str):
+        project_uuid (str):
+        validation_id (float):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiJobStatusResponse
+        DeleteValidationDismissResponse200
     """
 
     return sync_detailed(
-        job_id=job_id,
+        project_uuid=project_uuid,
+        validation_id=validation_id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
-    job_id: str,
+    project_uuid: str,
+    validation_id: float,
     *,
     client: Client,
-) -> Response[ApiJobStatusResponse]:
-    """Get a generic job status
-    This method can be used when polling from the frontend
+) -> Response[DeleteValidationDismissResponse200]:
+    """Deletes a single validation error.
 
     Args:
-        job_id (str):
+        project_uuid (str):
+        validation_id (float):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiJobStatusResponse]
+        Response[DeleteValidationDismissResponse200]
     """
 
     kwargs = _get_kwargs(
-        job_id=job_id,
+        project_uuid=project_uuid,
+        validation_id=validation_id,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
-    job_id: str,
+    project_uuid: str,
+    validation_id: float,
     *,
     client: Client,
-) -> Optional[ApiJobStatusResponse]:
-    """Get a generic job status
-    This method can be used when polling from the frontend
+) -> Optional[DeleteValidationDismissResponse200]:
+    """Deletes a single validation error.
 
     Args:
-        job_id (str):
+        project_uuid (str):
+        validation_id (float):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiJobStatusResponse
+        DeleteValidationDismissResponse200
     """
 
     return (
         await asyncio_detailed(
-            job_id=job_id,
+            project_uuid=project_uuid,
+            validation_id=validation_id,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/schedulers/update_scheduler.py` & `lightdash_client_python-0.621.0/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,93 @@
-from http import HTTPStatus
+import datetime
 from typing import Any
 from typing import Dict
-from typing import Optional
+from typing import List
+from typing import Type
+from typing import TypeVar
 
-import httpx
+import attr
+from dateutil.parser import isoparse
 
-from ... import errors
-from ...client import Client
-from ...types import Response
-
-
-def _get_kwargs(
-    scheduler_uuid: str,
-    *,
-    client: Client,
-    json_body: Any,
-) -> Dict[str, Any]:
-    url = "{}/api/v1/schedulers/{schedulerUuid}".format(client.base_url, schedulerUuid=scheduler_uuid)
-
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
-
-    json_json_body = json_body
-
-    return {
-        "method": "patch",
-        "url": url,
-        "headers": headers,
-        "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
-        "json": json_json_body,
-    }
-
-
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[Any]:
-    if client.raise_on_unexpected_status:
-        raise errors.UnexpectedStatus(response.status_code, response.content)
-    else:
-        return None
-
-
-def _build_response(*, client: Client, response: httpx.Response) -> Response[Any]:
-    return Response(
-        status_code=HTTPStatus(response.status_code),
-        content=response.content,
-        headers=response.headers,
-        parsed=_parse_response(client=client, response=response),
-    )
-
-
-def sync_detailed(
-    scheduler_uuid: str,
-    *,
-    client: Client,
-    json_body: Any,
-) -> Response[Any]:
-    """Update a scheduler
+T = TypeVar("T", bound="SchedulerWithLogsSchedulersItemTargetsItemType0")
 
-    Args:
-        scheduler_uuid (str):
-        json_body (Any): the new scheduler data
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
-    Returns:
-        Response[Any]
+@attr.s(auto_attribs=True)
+class SchedulerWithLogsSchedulersItemTargetsItemType0:
     """
-
-    kwargs = _get_kwargs(
-        scheduler_uuid=scheduler_uuid,
-        client=client,
-        json_body=json_body,
-    )
-
-    response = httpx.request(
-        verify=client.verify_ssl,
-        **kwargs,
-    )
-
-    return _build_response(client=client, response=response)
-
-
-async def asyncio_detailed(
-    scheduler_uuid: str,
-    *,
-    client: Client,
-    json_body: Any,
-) -> Response[Any]:
-    """Update a scheduler
-
-    Args:
+    Attributes:
+        channel (str):
         scheduler_uuid (str):
-        json_body (Any): the new scheduler data
-
-    Raises:
-        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
-        httpx.TimeoutException: If the request takes longer than Client.timeout.
-
-    Returns:
-        Response[Any]
+        updated_at (datetime.datetime):
+        created_at (datetime.datetime):
+        scheduler_slack_target_uuid (str):
     """
 
-    kwargs = _get_kwargs(
-        scheduler_uuid=scheduler_uuid,
-        client=client,
-        json_body=json_body,
-    )
+    channel: str
+    scheduler_uuid: str
+    updated_at: datetime.datetime
+    created_at: datetime.datetime
+    scheduler_slack_target_uuid: str
+    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+
+    def to_dict(self) -> Dict[str, Any]:
+        channel = self.channel
+        scheduler_uuid = self.scheduler_uuid
+        updated_at = self.updated_at.isoformat()
+
+        created_at = self.created_at.isoformat()
+
+        scheduler_slack_target_uuid = self.scheduler_slack_target_uuid
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
+        field_dict.update(
+            {
+                "channel": channel,
+                "schedulerUuid": scheduler_uuid,
+                "updatedAt": updated_at,
+                "createdAt": created_at,
+                "schedulerSlackTargetUuid": scheduler_slack_target_uuid,
+            }
+        )
+
+        return field_dict
+
+    @classmethod
+    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        d = src_dict.copy()
+        channel = d.pop("channel")
+
+        scheduler_uuid = d.pop("schedulerUuid")
+
+        updated_at = isoparse(d.pop("updatedAt"))
+
+        created_at = isoparse(d.pop("createdAt"))
+
+        scheduler_slack_target_uuid = d.pop("schedulerSlackTargetUuid")
+
+        scheduler_with_logs_schedulers_item_targets_item_type_0 = cls(
+            channel=channel,
+            scheduler_uuid=scheduler_uuid,
+            updated_at=updated_at,
+            created_at=created_at,
+            scheduler_slack_target_uuid=scheduler_slack_target_uuid,
+        )
+
+        scheduler_with_logs_schedulers_item_targets_item_type_0.additional_properties = d
+        return scheduler_with_logs_schedulers_item_targets_item_type_0
+
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
 
-    return _build_response(client=client, response=response)
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/share_links/get_share_url.py` & `lightdash_client_python-0.621.0/lightdash_client/api/share_links/get_share_url.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_share_response import ApiShareResponse
+from ...models.get_share_url_response_200 import GetShareUrlResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     nano_id: str,
     *,
     client: Client,
@@ -27,50 +27,50 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiShareResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetShareUrlResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiShareResponse.from_dict(response.json())
+        response_200 = GetShareUrlResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiShareResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetShareUrlResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     nano_id: str,
     *,
     client: Client,
-) -> Response[ApiShareResponse]:
+) -> Response[GetShareUrlResponse200]:
     """Get a share url from a short url id
 
     Args:
         nano_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiShareResponse]
+        Response[GetShareUrlResponse200]
     """
 
     kwargs = _get_kwargs(
         nano_id=nano_id,
         client=client,
     )
 
@@ -82,50 +82,50 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     nano_id: str,
     *,
     client: Client,
-) -> Optional[ApiShareResponse]:
+) -> Optional[GetShareUrlResponse200]:
     """Get a share url from a short url id
 
     Args:
         nano_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiShareResponse
+        GetShareUrlResponse200
     """
 
     return sync_detailed(
         nano_id=nano_id,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     nano_id: str,
     *,
     client: Client,
-) -> Response[ApiShareResponse]:
+) -> Response[GetShareUrlResponse200]:
     """Get a share url from a short url id
 
     Args:
         nano_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiShareResponse]
+        Response[GetShareUrlResponse200]
     """
 
     kwargs = _get_kwargs(
         nano_id=nano_id,
         client=client,
     )
 
@@ -135,26 +135,26 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     nano_id: str,
     *,
     client: Client,
-) -> Optional[ApiShareResponse]:
+) -> Optional[GetShareUrlResponse200]:
     """Get a share url from a short url id
 
     Args:
         nano_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiShareResponse
+        GetShareUrlResponse200
     """
 
     return (
         await asyncio_detailed(
             nano_id=nano_id,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/spaces/delete_space.py` & `lightdash_client_python-0.621.0/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,174 +3,161 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.get_dbt_cloud_integration_settings_response_200 import GetDbtCloudIntegrationSettingsResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     project_uuid: str,
-    space_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/projects/{projectUuid}/spaces/{spaceUuid}".format(
-        client.base_url, projectUuid=project_uuid, spaceUuid=space_uuid
+    url = "{}/api/v1/projects/{projectUuid}/integrations/dbt-cloud/settings".format(
+        client.base_url, projectUuid=project_uuid
     )
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
-    if response.status_code == HTTPStatus.NO_CONTENT:
-        response_204 = ApiSuccessEmpty.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetDbtCloudIntegrationSettingsResponse200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = GetDbtCloudIntegrationSettingsResponse200.from_dict(response.json())
 
-        return response_204
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetDbtCloudIntegrationSettingsResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     project_uuid: str,
-    space_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Delete a space from a project
+) -> Response[GetDbtCloudIntegrationSettingsResponse200]:
+    """Get the current dbt Cloud integration settings for a project
 
     Args:
         project_uuid (str):
-        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[GetDbtCloudIntegrationSettingsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        space_uuid=space_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
     project_uuid: str,
-    space_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Delete a space from a project
+) -> Optional[GetDbtCloudIntegrationSettingsResponse200]:
+    """Get the current dbt Cloud integration settings for a project
 
     Args:
         project_uuid (str):
-        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        GetDbtCloudIntegrationSettingsResponse200
     """
 
     return sync_detailed(
         project_uuid=project_uuid,
-        space_uuid=space_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     project_uuid: str,
-    space_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Delete a space from a project
+) -> Response[GetDbtCloudIntegrationSettingsResponse200]:
+    """Get the current dbt Cloud integration settings for a project
 
     Args:
         project_uuid (str):
-        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[GetDbtCloudIntegrationSettingsResponse200]
     """
 
     kwargs = _get_kwargs(
         project_uuid=project_uuid,
-        space_uuid=space_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     project_uuid: str,
-    space_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Delete a space from a project
+) -> Optional[GetDbtCloudIntegrationSettingsResponse200]:
+    """Get the current dbt Cloud integration settings for a project
 
     Args:
         project_uuid (str):
-        space_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        GetDbtCloudIntegrationSettingsResponse200
     """
 
     return (
         await asyncio_detailed(
             project_uuid=project_uuid,
-            space_uuid=space_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py` & `lightdash_client_python-0.621.0/lightdash_client/api/user_groups/get_group.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,134 +3,159 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_ssh_key_pair_response import ApiSshKeyPairResponse
+from ...models.get_group_response_200 import GetGroupResponse200
 from ...types import Response
 
 
 def _get_kwargs(
+    group_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/ssh/key-pairs".format(client.base_url)
+    url = "{}/api/v1/groups/{groupUuid}".format(client.base_url, groupUuid=group_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "post",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSshKeyPairResponse]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = ApiSshKeyPairResponse.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetGroupResponse200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = GetGroupResponse200.from_dict(response.json())
 
-        return response_201
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSshKeyPairResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetGroupResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    group_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSshKeyPairResponse]:
-    """
+) -> Response[GetGroupResponse200]:
+    """Get group details
+
+    Args:
+        group_uuid (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSshKeyPairResponse]
+        Response[GetGroupResponse200]
     """
 
     kwargs = _get_kwargs(
+        group_uuid=group_uuid,
         client=client,
     )
 
     response = httpx.request(
         verify=client.verify_ssl,
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 def sync(
+    group_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSshKeyPairResponse]:
-    """
+) -> Optional[GetGroupResponse200]:
+    """Get group details
+
+    Args:
+        group_uuid (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSshKeyPairResponse
+        GetGroupResponse200
     """
 
     return sync_detailed(
+        group_uuid=group_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
+    group_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSshKeyPairResponse]:
-    """
+) -> Response[GetGroupResponse200]:
+    """Get group details
+
+    Args:
+        group_uuid (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSshKeyPairResponse]
+        Response[GetGroupResponse200]
     """
 
     kwargs = _get_kwargs(
+        group_uuid=group_uuid,
         client=client,
     )
 
     async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
         response = await _client.request(**kwargs)
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
+    group_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSshKeyPairResponse]:
-    """
+) -> Optional[GetGroupResponse200]:
+    """Get group details
+
+    Args:
+        group_uuid (str):
+
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSshKeyPairResponse
+        GetGroupResponse200
     """
 
     return (
         await asyncio_detailed(
+            group_uuid=group_uuid,
             client=client,
         )
     ).parsed
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/user_groups/add_user_to_group.py` & `lightdash_client_python-0.621.0/lightdash_client/api/user_groups/add_user_to_group.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.add_user_to_group_response_200 import AddUserToGroupResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     group_uuid: str,
     user_uuid: str,
     *,
@@ -30,52 +30,52 @@
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[AddUserToGroupResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = AddUserToGroupResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[AddUserToGroupResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
+) -> Response[AddUserToGroupResponse200]:
     """Add a Lightdash user to a group
 
     Args:
         group_uuid (str):
         user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[AddUserToGroupResponse200]
     """
 
     kwargs = _get_kwargs(
         group_uuid=group_uuid,
         user_uuid=user_uuid,
         client=client,
     )
@@ -89,54 +89,54 @@
 
 
 def sync(
     group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
+) -> Optional[AddUserToGroupResponse200]:
     """Add a Lightdash user to a group
 
     Args:
         group_uuid (str):
         user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        AddUserToGroupResponse200
     """
 
     return sync_detailed(
         group_uuid=group_uuid,
         user_uuid=user_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
+) -> Response[AddUserToGroupResponse200]:
     """Add a Lightdash user to a group
 
     Args:
         group_uuid (str):
         user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[AddUserToGroupResponse200]
     """
 
     kwargs = _get_kwargs(
         group_uuid=group_uuid,
         user_uuid=user_uuid,
         client=client,
     )
@@ -148,27 +148,27 @@
 
 
 async def asyncio(
     group_uuid: str,
     user_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
+) -> Optional[AddUserToGroupResponse200]:
     """Add a Lightdash user to a group
 
     Args:
         group_uuid (str):
         user_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        AddUserToGroupResponse200
     """
 
     return (
         await asyncio_detailed(
             group_uuid=group_uuid,
             user_uuid=user_uuid,
             client=client,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/user_groups/delete_group.py` & `lightdash_client_python-0.621.0/lightdash_client/api/user_groups/get_group_members.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,74 +3,74 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_success_empty import ApiSuccessEmpty
+from ...models.get_group_members_response_200 import GetGroupMembersResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     group_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
-    url = "{}/api/v1/groups/{groupUuid}".format(client.base_url, groupUuid=group_uuid)
+    url = "{}/api/v1/groups/{groupUuid}/members".format(client.base_url, groupUuid=group_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "delete",
+        "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiSuccessEmpty]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetGroupMembersResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiSuccessEmpty.from_dict(response.json())
+        response_200 = GetGroupMembersResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiSuccessEmpty]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetGroupMembersResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     group_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Delete a group
+) -> Response[GetGroupMembersResponse200]:
+    """View members of a group
 
     Args:
         group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[GetGroupMembersResponse200]
     """
 
     kwargs = _get_kwargs(
         group_uuid=group_uuid,
         client=client,
     )
 
@@ -82,50 +82,50 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     group_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Delete a group
+) -> Optional[GetGroupMembersResponse200]:
+    """View members of a group
 
     Args:
         group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        GetGroupMembersResponse200
     """
 
     return sync_detailed(
         group_uuid=group_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     group_uuid: str,
     *,
     client: Client,
-) -> Response[ApiSuccessEmpty]:
-    """Delete a group
+) -> Response[GetGroupMembersResponse200]:
+    """View members of a group
 
     Args:
         group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiSuccessEmpty]
+        Response[GetGroupMembersResponse200]
     """
 
     kwargs = _get_kwargs(
         group_uuid=group_uuid,
         client=client,
     )
 
@@ -135,26 +135,26 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     group_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiSuccessEmpty]:
-    """Delete a group
+) -> Optional[GetGroupMembersResponse200]:
+    """View members of a group
 
     Args:
         group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiSuccessEmpty
+        GetGroupMembersResponse200
     """
 
     return (
         await asyncio_detailed(
             group_uuid=group_uuid,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/api/user_groups/get_group.py` & `lightdash_client_python-0.621.0/lightdash_client/api/user_groups/delete_group.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,74 +3,74 @@
 from typing import Dict
 from typing import Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.api_group_response import ApiGroupResponse
+from ...models.delete_group_response_200 import DeleteGroupResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     group_uuid: str,
     *,
     client: Client,
 ) -> Dict[str, Any]:
     url = "{}/api/v1/groups/{groupUuid}".format(client.base_url, groupUuid=group_uuid)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     return {
-        "method": "get",
+        "method": "delete",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[ApiGroupResponse]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[DeleteGroupResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ApiGroupResponse.from_dict(response.json())
+        response_200 = DeleteGroupResponse200.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[ApiGroupResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[DeleteGroupResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     group_uuid: str,
     *,
     client: Client,
-) -> Response[ApiGroupResponse]:
-    """Get group details
+) -> Response[DeleteGroupResponse200]:
+    """Delete a group
 
     Args:
         group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiGroupResponse]
+        Response[DeleteGroupResponse200]
     """
 
     kwargs = _get_kwargs(
         group_uuid=group_uuid,
         client=client,
     )
 
@@ -82,50 +82,50 @@
     return _build_response(client=client, response=response)
 
 
 def sync(
     group_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiGroupResponse]:
-    """Get group details
+) -> Optional[DeleteGroupResponse200]:
+    """Delete a group
 
     Args:
         group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiGroupResponse
+        DeleteGroupResponse200
     """
 
     return sync_detailed(
         group_uuid=group_uuid,
         client=client,
     ).parsed
 
 
 async def asyncio_detailed(
     group_uuid: str,
     *,
     client: Client,
-) -> Response[ApiGroupResponse]:
-    """Get group details
+) -> Response[DeleteGroupResponse200]:
+    """Delete a group
 
     Args:
         group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[ApiGroupResponse]
+        Response[DeleteGroupResponse200]
     """
 
     kwargs = _get_kwargs(
         group_uuid=group_uuid,
         client=client,
     )
 
@@ -135,26 +135,26 @@
     return _build_response(client=client, response=response)
 
 
 async def asyncio(
     group_uuid: str,
     *,
     client: Client,
-) -> Optional[ApiGroupResponse]:
-    """Get group details
+) -> Optional[DeleteGroupResponse200]:
+    """Delete a group
 
     Args:
         group_uuid (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        ApiGroupResponse
+        DeleteGroupResponse200
     """
 
     return (
         await asyncio_detailed(
             group_uuid=group_uuid,
             client=client,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/client.py` & `lightdash_client_python-0.621.0/lightdash_client/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/allowed_email_domains.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_organization_allowed_email_domains_results.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.organization_member_role import OrganizationMemberRole
+from ..models.api_organization_allowed_email_domains_results_role import ApiOrganizationAllowedEmailDomainsResultsRole
 
-T = TypeVar("T", bound="AllowedEmailDomains")
+T = TypeVar("T", bound="ApiOrganizationAllowedEmailDomainsResults")
 
 
 @attr.s(auto_attribs=True)
-class AllowedEmailDomains:
+class ApiOrganizationAllowedEmailDomainsResults:
     """
     Attributes:
         project_uuids (List[str]):
-        role (OrganizationMemberRole):
+        role (ApiOrganizationAllowedEmailDomainsResultsRole):
         email_domains (List[str]):
         organization_uuid (str):
     """
 
     project_uuids: List[str]
-    role: OrganizationMemberRole
+    role: ApiOrganizationAllowedEmailDomainsResultsRole
     email_domains: List[str]
     organization_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project_uuids = self.project_uuids
 
@@ -51,29 +51,29 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         project_uuids = cast(List[str], d.pop("projectUuids"))
 
-        role = OrganizationMemberRole(d.pop("role"))
+        role = ApiOrganizationAllowedEmailDomainsResultsRole(d.pop("role"))
 
         email_domains = cast(List[str], d.pop("emailDomains"))
 
         organization_uuid = d.pop("organizationUuid")
 
-        allowed_email_domains = cls(
+        api_organization_allowed_email_domains_results = cls(
             project_uuids=project_uuids,
             role=role,
             email_domains=email_domains,
             organization_uuid=organization_uuid,
         )
 
-        allowed_email_domains.additional_properties = d
-        return allowed_email_domains
+        api_organization_allowed_email_domains_results.additional_properties = d
+        return api_organization_allowed_email_domains_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_chart_summary_list_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_chart_summary_list_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_chart_summary_list_response_status import ApiChartSummaryListResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.chart_summary import ChartSummary
+    from ..models.api_chart_summary_list_response_results_item import ApiChartSummaryListResponseResultsItem
 
 
 T = TypeVar("T", bound="ApiChartSummaryListResponse")
 
 
 @attr.s(auto_attribs=True)
 class ApiChartSummaryListResponse:
     """
     Attributes:
-        results (List['ChartSummary']):
+        results (List['ApiChartSummaryListResponseResultsItem']):
         status (ApiChartSummaryListResponseStatus):
     """
 
-    results: List["ChartSummary"]
+    results: List["ApiChartSummaryListResponseResultsItem"]
     status: ApiChartSummaryListResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
@@ -46,21 +46,21 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.chart_summary import ChartSummary
+        from ..models.api_chart_summary_list_response_results_item import ApiChartSummaryListResponseResultsItem
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = ChartSummary.from_dict(results_item_data)
+            results_item = ApiChartSummaryListResponseResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
         status = ApiChartSummaryListResponseStatus(d.pop("status"))
 
         api_chart_summary_list_response = cls(
             results=results,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_csv_url_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_csv_url_response_results.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_csv_url_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_metrics.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_dbt_cloud_metrics_status import ApiDbtCloudMetricsStatus
 
 if TYPE_CHECKING:
-    from ..models.dbt_cloud_metadata_response_metrics import DbtCloudMetadataResponseMetrics
+    from ..models.api_dbt_cloud_metrics_results import ApiDbtCloudMetricsResults
 
 
 T = TypeVar("T", bound="ApiDbtCloudMetrics")
 
 
 @attr.s(auto_attribs=True)
 class ApiDbtCloudMetrics:
     """
     Attributes:
-        results (DbtCloudMetadataResponseMetrics): Response from dbt cloud metadata api containing a list of metric
+        results (ApiDbtCloudMetricsResults): Response from dbt cloud metadata api containing a list of metric
             definitions
         status (ApiDbtCloudMetricsStatus):
     """
 
-    results: "DbtCloudMetadataResponseMetrics"
+    results: "ApiDbtCloudMetricsResults"
     status: ApiDbtCloudMetricsStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
         status = self.status.value
@@ -43,18 +43,18 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dbt_cloud_metadata_response_metrics import DbtCloudMetadataResponseMetrics
+        from ..models.api_dbt_cloud_metrics_results import ApiDbtCloudMetricsResults
 
         d = src_dict.copy()
-        results = DbtCloudMetadataResponseMetrics.from_dict(d.pop("results"))
+        results = ApiDbtCloudMetricsResults.from_dict(d.pop("results"))
 
         status = ApiDbtCloudMetricsStatus(d.pop("status"))
 
         api_dbt_cloud_metrics = cls(
             results=results,
             status=status,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_dbt_cloud_settings_delete_success.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_settings_delete_success.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_error_payload.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_error_payload_error.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_error_payload_error.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_group_list_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_group_list_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_group_list_response_status import ApiGroupListResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.group import Group
+    from ..models.api_group_list_response_results_item import ApiGroupListResponseResultsItem
 
 
 T = TypeVar("T", bound="ApiGroupListResponse")
 
 
 @attr.s(auto_attribs=True)
 class ApiGroupListResponse:
     """
     Attributes:
-        results (List['Group']):
+        results (List['ApiGroupListResponseResultsItem']):
         status (ApiGroupListResponseStatus):
     """
 
-    results: List["Group"]
+    results: List["ApiGroupListResponseResultsItem"]
     status: ApiGroupListResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
@@ -46,21 +46,21 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.group import Group
+        from ..models.api_group_list_response_results_item import ApiGroupListResponseResultsItem
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = Group.from_dict(results_item_data)
+            results_item = ApiGroupListResponseResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
         status = ApiGroupListResponseStatus(d.pop("status"))
 
         api_group_list_response = cls(
             results=results,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_group_members_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_group_members_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_group_members_response_status import ApiGroupMembersResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.group_member import GroupMember
+    from ..models.api_group_members_response_results_item import ApiGroupMembersResponseResultsItem
 
 
 T = TypeVar("T", bound="ApiGroupMembersResponse")
 
 
 @attr.s(auto_attribs=True)
 class ApiGroupMembersResponse:
     """
     Attributes:
-        results (List['GroupMember']):
+        results (List['ApiGroupMembersResponseResultsItem']):
         status (ApiGroupMembersResponseStatus):
     """
 
-    results: List["GroupMember"]
+    results: List["ApiGroupMembersResponseResultsItem"]
     status: ApiGroupMembersResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
@@ -46,21 +46,21 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.group_member import GroupMember
+        from ..models.api_group_members_response_results_item import ApiGroupMembersResponseResultsItem
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = GroupMember.from_dict(results_item_data)
+            results_item = ApiGroupMembersResponseResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
         status = ApiGroupMembersResponseStatus(d.pop("status"))
 
         api_group_members_response = cls(
             results=results,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_group_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/update_group_response_200.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
-from ..models.api_group_response_status import ApiGroupResponseStatus
+from ..models.update_group_response_200_status import UpdateGroupResponse200Status
 
 if TYPE_CHECKING:
-    from ..models.group import Group
+    from ..models.update_group_response_200_results import UpdateGroupResponse200Results
 
 
-T = TypeVar("T", bound="ApiGroupResponse")
+T = TypeVar("T", bound="UpdateGroupResponse200")
 
 
 @attr.s(auto_attribs=True)
-class ApiGroupResponse:
+class UpdateGroupResponse200:
     """
     Attributes:
-        results (Group):
-        status (ApiGroupResponseStatus):
+        results (UpdateGroupResponse200Results):
+        status (UpdateGroupResponse200Status):
     """
 
-    results: "Group"
-    status: ApiGroupResponseStatus
+    results: "UpdateGroupResponse200Results"
+    status: UpdateGroupResponse200Status
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
         status = self.status.value
 
@@ -42,28 +42,28 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.group import Group
+        from ..models.update_group_response_200_results import UpdateGroupResponse200Results
 
         d = src_dict.copy()
-        results = Group.from_dict(d.pop("results"))
+        results = UpdateGroupResponse200Results.from_dict(d.pop("results"))
 
-        status = ApiGroupResponseStatus(d.pop("status"))
+        status = UpdateGroupResponse200Status(d.pop("status"))
 
-        api_group_response = cls(
+        update_group_response_200 = cls(
             results=results,
             status=status,
         )
 
-        api_group_response.additional_properties = d
-        return api_group_response
+        update_group_response_200.additional_properties = d
+        return update_group_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_job_scheduled_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_job_scheduled_response_results.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_job_scheduled_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_job_status_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_job_status_response_results.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_job_status_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_organization.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_organization.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_organization_status import ApiOrganizationStatus
 
 if TYPE_CHECKING:
-    from ..models.organization import Organization
+    from ..models.api_organization_results import ApiOrganizationResults
 
 
 T = TypeVar("T", bound="ApiOrganization")
 
 
 @attr.s(auto_attribs=True)
 class ApiOrganization:
     """
     Attributes:
-        results (Organization): Details of a user's Organization
+        results (ApiOrganizationResults): Details of a user's Organization
         status (ApiOrganizationStatus):
     """
 
-    results: "Organization"
+    results: "ApiOrganizationResults"
     status: ApiOrganizationStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
         status = self.status.value
@@ -42,18 +42,18 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.organization import Organization
+        from ..models.api_organization_results import ApiOrganizationResults
 
         d = src_dict.copy()
-        results = Organization.from_dict(d.pop("results"))
+        results = ApiOrganizationResults.from_dict(d.pop("results"))
 
         status = ApiOrganizationStatus(d.pop("status"))
 
         api_organization = cls(
             results=results,
             status=status,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_organization_allowed_email_domains.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_organization_allowed_email_domains.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_organization_allowed_email_domains_status import ApiOrganizationAllowedEmailDomainsStatus
 
 if TYPE_CHECKING:
-    from ..models.allowed_email_domains import AllowedEmailDomains
+    from ..models.api_organization_allowed_email_domains_results import ApiOrganizationAllowedEmailDomainsResults
 
 
 T = TypeVar("T", bound="ApiOrganizationAllowedEmailDomains")
 
 
 @attr.s(auto_attribs=True)
 class ApiOrganizationAllowedEmailDomains:
     """
     Attributes:
-        results (AllowedEmailDomains):
+        results (ApiOrganizationAllowedEmailDomainsResults):
         status (ApiOrganizationAllowedEmailDomainsStatus):
     """
 
-    results: "AllowedEmailDomains"
+    results: "ApiOrganizationAllowedEmailDomainsResults"
     status: ApiOrganizationAllowedEmailDomainsStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
         status = self.status.value
@@ -42,18 +42,18 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.allowed_email_domains import AllowedEmailDomains
+        from ..models.api_organization_allowed_email_domains_results import ApiOrganizationAllowedEmailDomainsResults
 
         d = src_dict.copy()
-        results = AllowedEmailDomains.from_dict(d.pop("results"))
+        results = ApiOrganizationAllowedEmailDomainsResults.from_dict(d.pop("results"))
 
         status = ApiOrganizationAllowedEmailDomainsStatus(d.pop("status"))
 
         api_organization_allowed_email_domains = cls(
             results=results,
             status=status,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profile.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_organization_member_profile_status import ApiOrganizationMemberProfileStatus
 
 if TYPE_CHECKING:
-    from ..models.organization_member_profile import OrganizationMemberProfile
+    from ..models.api_organization_member_profile_results import ApiOrganizationMemberProfileResults
 
 
 T = TypeVar("T", bound="ApiOrganizationMemberProfile")
 
 
 @attr.s(auto_attribs=True)
 class ApiOrganizationMemberProfile:
     """
     Attributes:
-        results (OrganizationMemberProfile): Profile for a user's membership in an organization
+        results (ApiOrganizationMemberProfileResults): Profile for a user's membership in an organization
         status (ApiOrganizationMemberProfileStatus):
     """
 
-    results: "OrganizationMemberProfile"
+    results: "ApiOrganizationMemberProfileResults"
     status: ApiOrganizationMemberProfileStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
         status = self.status.value
@@ -42,18 +42,18 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.organization_member_profile import OrganizationMemberProfile
+        from ..models.api_organization_member_profile_results import ApiOrganizationMemberProfileResults
 
         d = src_dict.copy()
-        results = OrganizationMemberProfile.from_dict(d.pop("results"))
+        results = ApiOrganizationMemberProfileResults.from_dict(d.pop("results"))
 
         status = ApiOrganizationMemberProfileStatus(d.pop("status"))
 
         api_organization_member_profile = cls(
             results=results,
             status=status,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_organization_member_profiles.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profiles.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_organization_member_profiles_status import ApiOrganizationMemberProfilesStatus
 
 if TYPE_CHECKING:
-    from ..models.organization_member_profile import OrganizationMemberProfile
+    from ..models.api_organization_member_profiles_results_item import ApiOrganizationMemberProfilesResultsItem
 
 
 T = TypeVar("T", bound="ApiOrganizationMemberProfiles")
 
 
 @attr.s(auto_attribs=True)
 class ApiOrganizationMemberProfiles:
     """
     Attributes:
-        results (List['OrganizationMemberProfile']):
+        results (List['ApiOrganizationMemberProfilesResultsItem']):
         status (ApiOrganizationMemberProfilesStatus):
     """
 
-    results: List["OrganizationMemberProfile"]
+    results: List["ApiOrganizationMemberProfilesResultsItem"]
     status: ApiOrganizationMemberProfilesStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
@@ -46,21 +46,21 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.organization_member_profile import OrganizationMemberProfile
+        from ..models.api_organization_member_profiles_results_item import ApiOrganizationMemberProfilesResultsItem
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = OrganizationMemberProfile.from_dict(results_item_data)
+            results_item = ApiOrganizationMemberProfilesResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
         status = ApiOrganizationMemberProfilesStatus(d.pop("status"))
 
         api_organization_member_profiles = cls(
             results=results,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_organization_projects.py` & `lightdash_client_python-0.621.0/lightdash_client/models/create_organization_response_200.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,66 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
+from typing import Union
 
 import attr
 
-from ..models.api_organization_projects_status import ApiOrganizationProjectsStatus
+from ..models.create_organization_response_200_status import CreateOrganizationResponse200Status
+from ..types import UNSET
+from ..types import Unset
 
-if TYPE_CHECKING:
-    from ..models.organization_project import OrganizationProject
-
-
-T = TypeVar("T", bound="ApiOrganizationProjects")
+T = TypeVar("T", bound="CreateOrganizationResponse200")
 
 
 @attr.s(auto_attribs=True)
-class ApiOrganizationProjects:
-    """List of projects in the current organization
-
+class CreateOrganizationResponse200:
+    """
     Attributes:
-        results (List['OrganizationProject']):
-        status (ApiOrganizationProjectsStatus):
+        status (CreateOrganizationResponse200Status):
+        results (Union[Unset, Any]):
     """
 
-    results: List["OrganizationProject"]
-    status: ApiOrganizationProjectsStatus
+    status: CreateOrganizationResponse200Status
+    results: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = []
-        for results_item_data in self.results:
-            results_item = results_item_data.to_dict()
-
-            results.append(results_item)
-
         status = self.status.value
 
+        results = self.results
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
                 "status": status,
             }
         )
+        if results is not UNSET:
+            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.organization_project import OrganizationProject
-
         d = src_dict.copy()
-        results = []
-        _results = d.pop("results")
-        for results_item_data in _results:
-            results_item = OrganizationProject.from_dict(results_item_data)
-
-            results.append(results_item)
+        status = CreateOrganizationResponse200Status(d.pop("status"))
 
-        status = ApiOrganizationProjectsStatus(d.pop("status"))
+        results = d.pop("results", UNSET)
 
-        api_organization_projects = cls(
-            results=results,
+        create_organization_response_200 = cls(
             status=status,
+            results=results,
         )
 
-        api_organization_projects.additional_properties = d
-        return api_organization_projects
+        create_organization_response_200.additional_properties = d
+        return create_organization_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_project_access_list_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_project_access_list_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_project_access_list_response_status import ApiProjectAccessListResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.project_member_profile import ProjectMemberProfile
+    from ..models.api_project_access_list_response_results_item import ApiProjectAccessListResponseResultsItem
 
 
 T = TypeVar("T", bound="ApiProjectAccessListResponse")
 
 
 @attr.s(auto_attribs=True)
 class ApiProjectAccessListResponse:
     """
     Attributes:
-        results (List['ProjectMemberProfile']):
+        results (List['ApiProjectAccessListResponseResultsItem']):
         status (ApiProjectAccessListResponseStatus):
     """
 
-    results: List["ProjectMemberProfile"]
+    results: List["ApiProjectAccessListResponseResultsItem"]
     status: ApiProjectAccessListResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
@@ -46,21 +46,21 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.project_member_profile import ProjectMemberProfile
+        from ..models.api_project_access_list_response_results_item import ApiProjectAccessListResponseResultsItem
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = ProjectMemberProfile.from_dict(results_item_data)
+            results_item = ApiProjectAccessListResponseResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
         status = ApiProjectAccessListResponseStatus(d.pop("status"))
 
         api_project_access_list_response = cls(
             results=results,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_run_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_run_query_response_results.py` & `lightdash_client_python-0.621.0/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,61 @@
 from typing import Any
 from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
-if TYPE_CHECKING:
-    from ..models.metric_query_response import MetricQueryResponse
-
-
-T = TypeVar("T", bound="ApiRunQueryResponseResults")
+T = TypeVar("T", bound="PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1")
 
 
 @attr.s(auto_attribs=True)
-class ApiRunQueryResponseResults:
+class PostRunQueryResponse200ResultsMetricQueryFiltersDimensionsType1:
     """
     Attributes:
-        rows (List[Any]):
-        metric_query (MetricQueryResponse):
+        and_ (List[Any]):
+        id (str):
     """
 
-    rows: List[Any]
-    metric_query: "MetricQueryResponse"
+    and_: List[Any]
+    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        rows = self.rows
+        and_ = self.and_
 
-        metric_query = self.metric_query.to_dict()
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "rows": rows,
-                "metricQuery": metric_query,
+                "and": and_,
+                "id": id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.metric_query_response import MetricQueryResponse
-
         d = src_dict.copy()
-        rows = cast(List[Any], d.pop("rows"))
+        and_ = cast(List[Any], d.pop("and"))
 
-        metric_query = MetricQueryResponse.from_dict(d.pop("metricQuery"))
+        id = d.pop("id")
 
-        api_run_query_response_results = cls(
-            rows=rows,
-            metric_query=metric_query,
+        post_run_query_response_200_results_metric_query_filters_dimensions_type_1 = cls(
+            and_=and_,
+            id=id,
         )
 
-        api_run_query_response_results.additional_properties = d
-        return api_run_query_response_results
+        post_run_query_response_200_results_metric_query_filters_dimensions_type_1.additional_properties = d
+        return post_run_query_response_200_results_metric_query_filters_dimensions_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_scheduled_jobs_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_slack_channels_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
-from ..models.api_scheduled_jobs_response_status import ApiScheduledJobsResponseStatus
+from ..models.api_slack_channels_response_status import ApiSlackChannelsResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.scheduled_jobs import ScheduledJobs
+    from ..models.api_slack_channels_response_results_item import ApiSlackChannelsResponseResultsItem
 
 
-T = TypeVar("T", bound="ApiScheduledJobsResponse")
+T = TypeVar("T", bound="ApiSlackChannelsResponse")
 
 
 @attr.s(auto_attribs=True)
-class ApiScheduledJobsResponse:
+class ApiSlackChannelsResponse:
     """
     Attributes:
-        results (List['ScheduledJobs']):
-        status (ApiScheduledJobsResponseStatus):
+        results (List['ApiSlackChannelsResponseResultsItem']):
+        status (ApiSlackChannelsResponseStatus):
     """
 
-    results: List["ScheduledJobs"]
-    status: ApiScheduledJobsResponseStatus
+    results: List["ApiSlackChannelsResponseResultsItem"]
+    status: ApiSlackChannelsResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
 
@@ -46,33 +46,33 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.scheduled_jobs import ScheduledJobs
+        from ..models.api_slack_channels_response_results_item import ApiSlackChannelsResponseResultsItem
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = ScheduledJobs.from_dict(results_item_data)
+            results_item = ApiSlackChannelsResponseResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
-        status = ApiScheduledJobsResponseStatus(d.pop("status"))
+        status = ApiSlackChannelsResponseStatus(d.pop("status"))
 
-        api_scheduled_jobs_response = cls(
+        api_slack_channels_response = cls(
             results=results,
             status=status,
         )
 
-        api_scheduled_jobs_response.additional_properties = d
-        return api_scheduled_jobs_response
+        api_slack_channels_response.additional_properties = d
+        return api_slack_channels_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_share_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/update_my_organization_response_200.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
+from typing import Union
 
 import attr
 
-from ..models.api_share_response_status import ApiShareResponseStatus
+from ..models.update_my_organization_response_200_status import UpdateMyOrganizationResponse200Status
+from ..types import UNSET
+from ..types import Unset
 
-if TYPE_CHECKING:
-    from ..models.share_url import ShareUrl
-
-
-T = TypeVar("T", bound="ApiShareResponse")
+T = TypeVar("T", bound="UpdateMyOrganizationResponse200")
 
 
 @attr.s(auto_attribs=True)
-class ApiShareResponse:
+class UpdateMyOrganizationResponse200:
     """
     Attributes:
-        results (ShareUrl): A ShareUrl maps a short shareable id to a full URL
-            in the Lightdash UI. This allows very long URLs
-            to be represented by short ids.
-        status (ApiShareResponseStatus):
+        status (UpdateMyOrganizationResponse200Status):
+        results (Union[Unset, Any]):
     """
 
-    results: "ShareUrl"
-    status: ApiShareResponseStatus
+    status: UpdateMyOrganizationResponse200Status
+    results: Union[Unset, Any] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        results = self.results.to_dict()
-
         status = self.status.value
 
+        results = self.results
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "results": results,
                 "status": status,
             }
         )
+        if results is not UNSET:
+            field_dict["results"] = results
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.share_url import ShareUrl
-
         d = src_dict.copy()
-        results = ShareUrl.from_dict(d.pop("results"))
+        status = UpdateMyOrganizationResponse200Status(d.pop("status"))
 
-        status = ApiShareResponseStatus(d.pop("status"))
+        results = d.pop("results", UNSET)
 
-        api_share_response = cls(
-            results=results,
+        update_my_organization_response_200 = cls(
             status=status,
+            results=results,
         )
 
-        api_share_response.additional_properties = d
-        return api_share_response
+        update_my_organization_response_200.additional_properties = d
+        return update_my_organization_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_slack_channels_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_scheduled_jobs_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
-from ..models.api_slack_channels_response_status import ApiSlackChannelsResponseStatus
+from ..models.api_scheduled_jobs_response_status import ApiScheduledJobsResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.slack_channel import SlackChannel
+    from ..models.api_scheduled_jobs_response_results_item import ApiScheduledJobsResponseResultsItem
 
 
-T = TypeVar("T", bound="ApiSlackChannelsResponse")
+T = TypeVar("T", bound="ApiScheduledJobsResponse")
 
 
 @attr.s(auto_attribs=True)
-class ApiSlackChannelsResponse:
+class ApiScheduledJobsResponse:
     """
     Attributes:
-        results (List['SlackChannel']):
-        status (ApiSlackChannelsResponseStatus):
+        results (List['ApiScheduledJobsResponseResultsItem']):
+        status (ApiScheduledJobsResponseStatus):
     """
 
-    results: List["SlackChannel"]
-    status: ApiSlackChannelsResponseStatus
+    results: List["ApiScheduledJobsResponseResultsItem"]
+    status: ApiScheduledJobsResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
 
@@ -46,33 +46,33 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.slack_channel import SlackChannel
+        from ..models.api_scheduled_jobs_response_results_item import ApiScheduledJobsResponseResultsItem
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = SlackChannel.from_dict(results_item_data)
+            results_item = ApiScheduledJobsResponseResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
-        status = ApiSlackChannelsResponseStatus(d.pop("status"))
+        status = ApiScheduledJobsResponseStatus(d.pop("status"))
 
-        api_slack_channels_response = cls(
+        api_scheduled_jobs_response = cls(
             results=results,
             status=status,
         )
 
-        api_slack_channels_response.additional_properties = d
-        return api_slack_channels_response
+        api_scheduled_jobs_response.additional_properties = d
+        return api_scheduled_jobs_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_space_summary_list_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_space_summary_list_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_space_summary_list_response_status import ApiSpaceSummaryListResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.space_summary import SpaceSummary
+    from ..models.api_space_summary_list_response_results_item import ApiSpaceSummaryListResponseResultsItem
 
 
 T = TypeVar("T", bound="ApiSpaceSummaryListResponse")
 
 
 @attr.s(auto_attribs=True)
 class ApiSpaceSummaryListResponse:
     """
     Attributes:
-        results (List['SpaceSummary']):
+        results (List['ApiSpaceSummaryListResponseResultsItem']):
         status (ApiSpaceSummaryListResponseStatus):
     """
 
-    results: List["SpaceSummary"]
+    results: List["ApiSpaceSummaryListResponseResultsItem"]
     status: ApiSpaceSummaryListResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
@@ -46,21 +46,21 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.space_summary import SpaceSummary
+        from ..models.api_space_summary_list_response_results_item import ApiSpaceSummaryListResponseResultsItem
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = SpaceSummary.from_dict(results_item_data)
+            results_item = ApiSpaceSummaryListResponseResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
         status = ApiSpaceSummaryListResponseStatus(d.pop("status"))
 
         api_space_summary_list_response = cls(
             results=results,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_ssh_key_pair_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_ssh_key_pair_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_ssh_key_pair_response_status import ApiSshKeyPairResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.pick_ssh_key_pair_public_key import PickSshKeyPairPublicKey
+    from ..models.api_ssh_key_pair_response_results import ApiSshKeyPairResponseResults
 
 
 T = TypeVar("T", bound="ApiSshKeyPairResponse")
 
 
 @attr.s(auto_attribs=True)
 class ApiSshKeyPairResponse:
     """
     Attributes:
-        results (PickSshKeyPairPublicKey): From T, pick a set of properties whose keys are in the union K
+        results (ApiSshKeyPairResponseResults): From T, pick a set of properties whose keys are in the union K
         status (ApiSshKeyPairResponseStatus):
     """
 
-    results: "PickSshKeyPairPublicKey"
+    results: "ApiSshKeyPairResponseResults"
     status: ApiSshKeyPairResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = self.results.to_dict()
 
         status = self.status.value
@@ -42,18 +42,18 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.pick_ssh_key_pair_public_key import PickSshKeyPairPublicKey
+        from ..models.api_ssh_key_pair_response_results import ApiSshKeyPairResponseResults
 
         d = src_dict.copy()
-        results = PickSshKeyPairPublicKey.from_dict(d.pop("results"))
+        results = ApiSshKeyPairResponseResults.from_dict(d.pop("results"))
 
         status = ApiSshKeyPairResponseStatus(d.pop("status"))
 
         api_ssh_key_pair_response = cls(
             results=results,
             status=status,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_success_empty.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_success_empty.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_user_allowed_organizations_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_user_allowed_organizations_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,31 @@
 from typing import TypeVar
 
 import attr
 
 from ..models.api_user_allowed_organizations_response_status import ApiUserAllowedOrganizationsResponseStatus
 
 if TYPE_CHECKING:
-    from ..models.user_allowed_organization import UserAllowedOrganization
+    from ..models.api_user_allowed_organizations_response_results_item import (
+        ApiUserAllowedOrganizationsResponseResultsItem,
+    )
 
 
 T = TypeVar("T", bound="ApiUserAllowedOrganizationsResponse")
 
 
 @attr.s(auto_attribs=True)
 class ApiUserAllowedOrganizationsResponse:
     """
     Attributes:
-        results (List['UserAllowedOrganization']):
+        results (List['ApiUserAllowedOrganizationsResponseResultsItem']):
         status (ApiUserAllowedOrganizationsResponseStatus):
     """
 
-    results: List["UserAllowedOrganization"]
+    results: List["ApiUserAllowedOrganizationsResponseResultsItem"]
     status: ApiUserAllowedOrganizationsResponseStatus
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         results = []
         for results_item_data in self.results:
             results_item = results_item_data.to_dict()
@@ -46,21 +48,23 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.user_allowed_organization import UserAllowedOrganization
+        from ..models.api_user_allowed_organizations_response_results_item import (
+            ApiUserAllowedOrganizationsResponseResultsItem,
+        )
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
-            results_item = UserAllowedOrganization.from_dict(results_item_data)
+            results_item = ApiUserAllowedOrganizationsResponseResultsItem.from_dict(results_item_data)
 
             results.append(results_item)
 
         status = ApiUserAllowedOrganizationsResponseStatus(d.pop("status"))
 
         api_user_allowed_organizations_response = cls(
             results=results,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_validate_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/get_latest_validation_results_response_200.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,52 +4,67 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.api_validate_response_status import ApiValidateResponseStatus
+from ..models.get_latest_validation_results_response_200_status import GetLatestValidationResultsResponse200Status
 
 if TYPE_CHECKING:
-    from ..models.validation_error_chart_response import ValidationErrorChartResponse
-    from ..models.validation_error_dashboard_response import ValidationErrorDashboardResponse
-    from ..models.validation_error_table_response import ValidationErrorTableResponse
+    from ..models.get_latest_validation_results_response_200_results_item_type_0 import (
+        GetLatestValidationResultsResponse200ResultsItemType0,
+    )
+    from ..models.get_latest_validation_results_response_200_results_item_type_1 import (
+        GetLatestValidationResultsResponse200ResultsItemType1,
+    )
+    from ..models.get_latest_validation_results_response_200_results_item_type_2 import (
+        GetLatestValidationResultsResponse200ResultsItemType2,
+    )
 
 
-T = TypeVar("T", bound="ApiValidateResponse")
+T = TypeVar("T", bound="GetLatestValidationResultsResponse200")
 
 
 @attr.s(auto_attribs=True)
-class ApiValidateResponse:
+class GetLatestValidationResultsResponse200:
     """
     Attributes:
-        results (List[Union['ValidationErrorChartResponse', 'ValidationErrorDashboardResponse',
-            'ValidationErrorTableResponse']]):
-        status (ApiValidateResponseStatus):
+        results (List[Union['GetLatestValidationResultsResponse200ResultsItemType0',
+            'GetLatestValidationResultsResponse200ResultsItemType1',
+            'GetLatestValidationResultsResponse200ResultsItemType2']]):
+        status (GetLatestValidationResultsResponse200Status):
     """
 
     results: List[
-        Union["ValidationErrorChartResponse", "ValidationErrorDashboardResponse", "ValidationErrorTableResponse"]
+        Union[
+            "GetLatestValidationResultsResponse200ResultsItemType0",
+            "GetLatestValidationResultsResponse200ResultsItemType1",
+            "GetLatestValidationResultsResponse200ResultsItemType2",
+        ]
     ]
-    status: ApiValidateResponseStatus
+    status: GetLatestValidationResultsResponse200Status
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.validation_error_chart_response import ValidationErrorChartResponse
-        from ..models.validation_error_dashboard_response import ValidationErrorDashboardResponse
+        from ..models.get_latest_validation_results_response_200_results_item_type_0 import (
+            GetLatestValidationResultsResponse200ResultsItemType0,
+        )
+        from ..models.get_latest_validation_results_response_200_results_item_type_1 import (
+            GetLatestValidationResultsResponse200ResultsItemType1,
+        )
 
         results = []
         for results_item_data in self.results:
             results_item: Dict[str, Any]
 
-            if isinstance(results_item_data, ValidationErrorChartResponse):
+            if isinstance(results_item_data, GetLatestValidationResultsResponse200ResultsItemType0):
                 results_item = results_item_data.to_dict()
 
-            elif isinstance(results_item_data, ValidationErrorDashboardResponse):
+            elif isinstance(results_item_data, GetLatestValidationResultsResponse200ResultsItemType1):
                 results_item = results_item_data.to_dict()
 
             else:
                 results_item = results_item_data.to_dict()
 
             results.append(results_item)
 
@@ -64,63 +79,71 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.validation_error_chart_response import ValidationErrorChartResponse
-        from ..models.validation_error_dashboard_response import ValidationErrorDashboardResponse
-        from ..models.validation_error_table_response import ValidationErrorTableResponse
+        from ..models.get_latest_validation_results_response_200_results_item_type_0 import (
+            GetLatestValidationResultsResponse200ResultsItemType0,
+        )
+        from ..models.get_latest_validation_results_response_200_results_item_type_1 import (
+            GetLatestValidationResultsResponse200ResultsItemType1,
+        )
+        from ..models.get_latest_validation_results_response_200_results_item_type_2 import (
+            GetLatestValidationResultsResponse200ResultsItemType2,
+        )
 
         d = src_dict.copy()
         results = []
         _results = d.pop("results")
         for results_item_data in _results:
 
             def _parse_results_item(
                 data: object,
             ) -> Union[
-                "ValidationErrorChartResponse", "ValidationErrorDashboardResponse", "ValidationErrorTableResponse"
+                "GetLatestValidationResultsResponse200ResultsItemType0",
+                "GetLatestValidationResultsResponse200ResultsItemType1",
+                "GetLatestValidationResultsResponse200ResultsItemType2",
             ]:
                 try:
                     if not isinstance(data, dict):
                         raise TypeError()
-                    componentsschemas_validation_response_type_0 = ValidationErrorChartResponse.from_dict(data)
+                    results_item_type_0 = GetLatestValidationResultsResponse200ResultsItemType0.from_dict(data)
 
-                    return componentsschemas_validation_response_type_0
+                    return results_item_type_0
                 except:  # noqa: E722
                     pass
                 try:
                     if not isinstance(data, dict):
                         raise TypeError()
-                    componentsschemas_validation_response_type_1 = ValidationErrorDashboardResponse.from_dict(data)
+                    results_item_type_1 = GetLatestValidationResultsResponse200ResultsItemType1.from_dict(data)
 
-                    return componentsschemas_validation_response_type_1
+                    return results_item_type_1
                 except:  # noqa: E722
                     pass
                 if not isinstance(data, dict):
                     raise TypeError()
-                componentsschemas_validation_response_type_2 = ValidationErrorTableResponse.from_dict(data)
+                results_item_type_2 = GetLatestValidationResultsResponse200ResultsItemType2.from_dict(data)
 
-                return componentsschemas_validation_response_type_2
+                return results_item_type_2
 
             results_item = _parse_results_item(results_item_data)
 
             results.append(results_item)
 
-        status = ApiValidateResponseStatus(d.pop("status"))
+        status = GetLatestValidationResultsResponse200Status(d.pop("status"))
 
-        api_validate_response = cls(
+        get_latest_validation_results_response_200 = cls(
             results=results,
             status=status,
         )
 
-        api_validate_response.additional_properties = d
-        return api_validate_response
+        get_latest_validation_results_response_200.additional_properties = d
+        return get_latest_validation_results_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/api_validation_dismiss_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_validation_dismiss_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/chart_summary.py` & `lightdash_client_python-0.621.0/lightdash_client/models/chart_summary.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.chart_type import ChartType
+from ..models.chart_summary_chart_type import ChartSummaryChartType
 from ..types import UNSET
 from ..types import Unset
 
 T = TypeVar("T", bound="ChartSummary")
 
 
 @attr.s(auto_attribs=True)
@@ -23,26 +23,26 @@
         organization_uuid (str):
         uuid (str):
         project_uuid (str):
         space_uuid (str):
         space_name (str):
         description (Union[Unset, str]):
         pinned_list_uuid (Optional[str]):
-        chart_type (Union[Unset, ChartType]):
+        chart_type (Union[Unset, ChartSummaryChartType]):
     """
 
     name: str
     organization_uuid: str
     uuid: str
     project_uuid: str
     space_uuid: str
     space_name: str
     pinned_list_uuid: Optional[str]
     description: Union[Unset, str] = UNSET
-    chart_type: Union[Unset, ChartType] = UNSET
+    chart_type: Union[Unset, ChartSummaryChartType] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         organization_uuid = self.organization_uuid
         uuid = self.uuid
         project_uuid = self.project_uuid
@@ -90,19 +90,19 @@
         space_name = d.pop("spaceName")
 
         description = d.pop("description", UNSET)
 
         pinned_list_uuid = d.pop("pinnedListUuid")
 
         _chart_type = d.pop("chartType", UNSET)
-        chart_type: Union[Unset, ChartType]
+        chart_type: Union[Unset, ChartSummaryChartType]
         if isinstance(_chart_type, Unset):
             chart_type = UNSET
         else:
-            chart_type = ChartType(_chart_type)
+            chart_type = ChartSummaryChartType(_chart_type)
 
         chart_summary = cls(
             name=name,
             organization_uuid=organization_uuid,
             uuid=uuid,
             project_uuid=project_uuid,
             space_uuid=space_uuid,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/create_project_member.py` & `lightdash_client_python-0.621.0/lightdash_client/models/create_project_member.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.project_member_role import ProjectMemberRole
+from ..models.create_project_member_role import CreateProjectMemberRole
 
 T = TypeVar("T", bound="CreateProjectMember")
 
 
 @attr.s(auto_attribs=True)
 class CreateProjectMember:
     """
     Attributes:
         send_email (bool):
-        role (ProjectMemberRole):
+        role (CreateProjectMemberRole):
         email (str):
     """
 
     send_email: bool
-    role: ProjectMemberRole
+    role: CreateProjectMemberRole
     email: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         send_email = self.send_email
         role = self.role.value
 
@@ -44,15 +44,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         send_email = d.pop("sendEmail")
 
-        role = ProjectMemberRole(d.pop("role"))
+        role = CreateProjectMemberRole(d.pop("role"))
 
         email = d.pop("email")
 
         create_project_member = cls(
             send_email=send_email,
             role=role,
             email=email,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/create_space.py` & `lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_json_body.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,32 +8,32 @@
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.space_share import SpaceShare
+    from ..models.create_space_in_project_json_body_access_item import CreateSpaceInProjectJsonBodyAccessItem
 
 
-T = TypeVar("T", bound="CreateSpace")
+T = TypeVar("T", bound="CreateSpaceInProjectJsonBody")
 
 
 @attr.s(auto_attribs=True)
-class CreateSpace:
+class CreateSpaceInProjectJsonBody:
     """
     Attributes:
         name (str):
         is_private (Union[Unset, bool]):
-        access (Union[Unset, List['SpaceShare']]):
+        access (Union[Unset, List['CreateSpaceInProjectJsonBodyAccessItem']]):
     """
 
     name: str
     is_private: Union[Unset, bool] = UNSET
-    access: Union[Unset, List["SpaceShare"]] = UNSET
+    access: Union[Unset, List["CreateSpaceInProjectJsonBodyAccessItem"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         is_private = self.is_private
         access: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.access, Unset):
@@ -55,36 +55,36 @@
         if access is not UNSET:
             field_dict["access"] = access
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.space_share import SpaceShare
+        from ..models.create_space_in_project_json_body_access_item import CreateSpaceInProjectJsonBodyAccessItem
 
         d = src_dict.copy()
         name = d.pop("name")
 
         is_private = d.pop("isPrivate", UNSET)
 
         access = []
         _access = d.pop("access", UNSET)
         for access_item_data in _access or []:
-            access_item = SpaceShare.from_dict(access_item_data)
+            access_item = CreateSpaceInProjectJsonBodyAccessItem.from_dict(access_item_data)
 
             access.append(access_item)
 
-        create_space = cls(
+        create_space_in_project_json_body = cls(
             name=name,
             is_private=is_private,
             access=access,
         )
 
-        create_space.additional_properties = d
-        return create_space
+        create_space_in_project_json_body.additional_properties = d
+        return create_space_in_project_json_body
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_azure_dev_ops_project_config.py` & `lightdash_client_python-0.621.0/lightdash_client/models/dbt_azure_dev_ops_project_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.dbt_project_type_azuredevops import DbtProjectTypeAZUREDEVOPS
+from ..models.dbt_azure_dev_ops_project_config_type import DbtAzureDevOpsProjectConfigType
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+    from ..models.dbt_azure_dev_ops_project_config_environment_item import DbtAzureDevOpsProjectConfigEnvironmentItem
 
 
 T = TypeVar("T", bound="DbtAzureDevOpsProjectConfig")
 
 
 @attr.s(auto_attribs=True)
 class DbtAzureDevOpsProjectConfig:
     """
     Attributes:
-        type (DbtProjectTypeAZUREDEVOPS):
+        type (DbtAzureDevOpsProjectConfigType):
         personal_access_token (str):
         organization (str):
         project (str):
         repository (str):
         branch (str):
         project_sub_path (str):
         target (Union[Unset, str]):
-        environment (Union[Unset, List['DbtProjectEnvironmentVariable']]):
+        environment (Union[Unset, List['DbtAzureDevOpsProjectConfigEnvironmentItem']]):
     """
 
-    type: DbtProjectTypeAZUREDEVOPS
+    type: DbtAzureDevOpsProjectConfigType
     personal_access_token: str
     organization: str
     project: str
     repository: str
     branch: str
     project_sub_path: str
     target: Union[Unset, str] = UNSET
-    environment: Union[Unset, List["DbtProjectEnvironmentVariable"]] = UNSET
+    environment: Union[Unset, List["DbtAzureDevOpsProjectConfigEnvironmentItem"]] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         personal_access_token = self.personal_access_token
         organization = self.organization
         project = self.project
@@ -79,18 +79,20 @@
         if environment is not UNSET:
             field_dict["environment"] = environment
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+        from ..models.dbt_azure_dev_ops_project_config_environment_item import (
+            DbtAzureDevOpsProjectConfigEnvironmentItem,
+        )
 
         d = src_dict.copy()
-        type = DbtProjectTypeAZUREDEVOPS(d.pop("type"))
+        type = DbtAzureDevOpsProjectConfigType(d.pop("type"))
 
         personal_access_token = d.pop("personal_access_token")
 
         organization = d.pop("organization")
 
         project = d.pop("project")
 
@@ -101,15 +103,15 @@
         project_sub_path = d.pop("project_sub_path")
 
         target = d.pop("target", UNSET)
 
         environment = []
         _environment = d.pop("environment", UNSET)
         for environment_item_data in _environment or []:
-            environment_item = DbtProjectEnvironmentVariable.from_dict(environment_item_data)
+            environment_item = DbtAzureDevOpsProjectConfigEnvironmentItem.from_dict(environment_item_data)
 
             environment.append(environment_item)
 
         dbt_azure_dev_ops_project_config = cls(
             type=type,
             personal_access_token=personal_access_token,
             organization=organization,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_bit_bucket_project_config.py` & `lightdash_client_python-0.621.0/lightdash_client/models/dbt_bit_bucket_project_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,48 +4,48 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.dbt_project_type_bitbucket import DbtProjectTypeBITBUCKET
+from ..models.dbt_bit_bucket_project_config_type import DbtBitBucketProjectConfigType
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+    from ..models.dbt_bit_bucket_project_config_environment_item import DbtBitBucketProjectConfigEnvironmentItem
 
 
 T = TypeVar("T", bound="DbtBitBucketProjectConfig")
 
 
 @attr.s(auto_attribs=True)
 class DbtBitBucketProjectConfig:
     """
     Attributes:
-        type (DbtProjectTypeBITBUCKET):
+        type (DbtBitBucketProjectConfigType):
         username (str):
         personal_access_token (str):
         repository (str):
         branch (str):
         project_sub_path (str):
         target (Union[Unset, str]):
-        environment (Union[Unset, List['DbtProjectEnvironmentVariable']]):
+        environment (Union[Unset, List['DbtBitBucketProjectConfigEnvironmentItem']]):
         host_domain (Union[Unset, str]):
     """
 
-    type: DbtProjectTypeBITBUCKET
+    type: DbtBitBucketProjectConfigType
     username: str
     personal_access_token: str
     repository: str
     branch: str
     project_sub_path: str
     target: Union[Unset, str] = UNSET
-    environment: Union[Unset, List["DbtProjectEnvironmentVariable"]] = UNSET
+    environment: Union[Unset, List["DbtBitBucketProjectConfigEnvironmentItem"]] = UNSET
     host_domain: Union[Unset, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         username = self.username
         personal_access_token = self.personal_access_token
@@ -81,18 +81,18 @@
         if host_domain is not UNSET:
             field_dict["host_domain"] = host_domain
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+        from ..models.dbt_bit_bucket_project_config_environment_item import DbtBitBucketProjectConfigEnvironmentItem
 
         d = src_dict.copy()
-        type = DbtProjectTypeBITBUCKET(d.pop("type"))
+        type = DbtBitBucketProjectConfigType(d.pop("type"))
 
         username = d.pop("username")
 
         personal_access_token = d.pop("personal_access_token")
 
         repository = d.pop("repository")
 
@@ -101,15 +101,15 @@
         project_sub_path = d.pop("project_sub_path")
 
         target = d.pop("target", UNSET)
 
         environment = []
         _environment = d.pop("environment", UNSET)
         for environment_item_data in _environment or []:
-            environment_item = DbtProjectEnvironmentVariable.from_dict(environment_item_data)
+            environment_item = DbtBitBucketProjectConfigEnvironmentItem.from_dict(environment_item_data)
 
             environment.append(environment_item)
 
         host_domain = d.pop("host_domain", UNSET)
 
         dbt_bit_bucket_project_config = cls(
             type=type,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_ide_project_config.py` & `lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_config_type_1.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from typing import Dict
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.dbt_project_type_dbtcloudide import DbtProjectTypeDBTCLOUDIDE
+from ..models.dbt_project_config_type_1_type import DbtProjectConfigType1Type
 
-T = TypeVar("T", bound="DbtCloudIDEProjectConfig")
+T = TypeVar("T", bound="DbtProjectConfigType1")
 
 
 @attr.s(auto_attribs=True)
-class DbtCloudIDEProjectConfig:
+class DbtProjectConfigType1:
     """
     Attributes:
-        type (DbtProjectTypeDBTCLOUDIDE):
+        type (DbtProjectConfigType1Type):
         api_key (str):
         account_id (Union[float, str]):
         environment_id (Union[float, str]):
         project_id (Union[float, str]):
     """
 
-    type: DbtProjectTypeDBTCLOUDIDE
+    type: DbtProjectConfigType1Type
     api_key: str
     account_id: Union[float, str]
     environment_id: Union[float, str]
     project_id: Union[float, str]
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
@@ -57,15 +57,15 @@
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = DbtProjectTypeDBTCLOUDIDE(d.pop("type"))
+        type = DbtProjectConfigType1Type(d.pop("type"))
 
         api_key = d.pop("api_key")
 
         def _parse_account_id(data: object) -> Union[float, str]:
             return cast(Union[float, str], data)
 
         account_id = _parse_account_id(d.pop("account_id"))
@@ -76,16 +76,16 @@
         environment_id = _parse_environment_id(d.pop("environment_id"))
 
         def _parse_project_id(data: object) -> Union[float, str]:
             return cast(Union[float, str], data)
 
         project_id = _parse_project_id(d.pop("project_id"))
 
-        dbt_cloud_ide_project_config = cls(
+        dbt_project_config_type_1 = cls(
             type=type,
             api_key=api_key,
             account_id=account_id,
             environment_id=environment_id,
             project_id=project_id,
         )
 
-        return dbt_cloud_ide_project_config
+        return dbt_project_config_type_1
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_metadata_response_metrics.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_dbt_cloud_metrics_results.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
 if TYPE_CHECKING:
-    from ..models.dbt_cloud_metric import DbtCloudMetric
+    from ..models.api_dbt_cloud_metrics_results_metrics_item import ApiDbtCloudMetricsResultsMetricsItem
 
 
-T = TypeVar("T", bound="DbtCloudMetadataResponseMetrics")
+T = TypeVar("T", bound="ApiDbtCloudMetricsResults")
 
 
 @attr.s(auto_attribs=True)
-class DbtCloudMetadataResponseMetrics:
+class ApiDbtCloudMetricsResults:
     """Response from dbt cloud metadata api containing a list of metric definitions
 
     Attributes:
-        metrics (List['DbtCloudMetric']): A list of dbt metric definitions from the dbt cloud metadata api
+        metrics (List['ApiDbtCloudMetricsResultsMetricsItem']): A list of dbt metric definitions from the dbt cloud
+            metadata api
     """
 
-    metrics: List["DbtCloudMetric"]
+    metrics: List["ApiDbtCloudMetricsResultsMetricsItem"]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         metrics = []
         for metrics_item_data in self.metrics:
             metrics_item = metrics_item_data.to_dict()
 
@@ -40,30 +41,30 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dbt_cloud_metric import DbtCloudMetric
+        from ..models.api_dbt_cloud_metrics_results_metrics_item import ApiDbtCloudMetricsResultsMetricsItem
 
         d = src_dict.copy()
         metrics = []
         _metrics = d.pop("metrics")
         for metrics_item_data in _metrics:
-            metrics_item = DbtCloudMetric.from_dict(metrics_item_data)
+            metrics_item = ApiDbtCloudMetricsResultsMetricsItem.from_dict(metrics_item_data)
 
             metrics.append(metrics_item)
 
-        dbt_cloud_metadata_response_metrics = cls(
+        api_dbt_cloud_metrics_results = cls(
             metrics=metrics,
         )
 
-        dbt_cloud_metadata_response_metrics.additional_properties = d
-        return dbt_cloud_metadata_response_metrics
+        api_dbt_cloud_metrics_results.additional_properties = d
+        return api_dbt_cloud_metrics_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_cloud_metric.py` & `lightdash_client_python-0.621.0/lightdash_client/models/dbt_cloud_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_github_project_config.py` & `lightdash_client_python-0.621.0/lightdash_client/models/dbt_github_project_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,46 +4,46 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.dbt_project_type_github import DbtProjectTypeGITHUB
+from ..models.dbt_github_project_config_type import DbtGithubProjectConfigType
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+    from ..models.dbt_github_project_config_environment_item import DbtGithubProjectConfigEnvironmentItem
 
 
 T = TypeVar("T", bound="DbtGithubProjectConfig")
 
 
 @attr.s(auto_attribs=True)
 class DbtGithubProjectConfig:
     """
     Attributes:
-        type (DbtProjectTypeGITHUB):
+        type (DbtGithubProjectConfigType):
         personal_access_token (str):
         repository (str):
         branch (str):
         project_sub_path (str):
         target (Union[Unset, str]):
-        environment (Union[Unset, List['DbtProjectEnvironmentVariable']]):
+        environment (Union[Unset, List['DbtGithubProjectConfigEnvironmentItem']]):
         host_domain (Union[Unset, str]):
     """
 
-    type: DbtProjectTypeGITHUB
+    type: DbtGithubProjectConfigType
     personal_access_token: str
     repository: str
     branch: str
     project_sub_path: str
     target: Union[Unset, str] = UNSET
-    environment: Union[Unset, List["DbtProjectEnvironmentVariable"]] = UNSET
+    environment: Union[Unset, List["DbtGithubProjectConfigEnvironmentItem"]] = UNSET
     host_domain: Union[Unset, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         personal_access_token = self.personal_access_token
         repository = self.repository
@@ -77,33 +77,33 @@
         if host_domain is not UNSET:
             field_dict["host_domain"] = host_domain
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+        from ..models.dbt_github_project_config_environment_item import DbtGithubProjectConfigEnvironmentItem
 
         d = src_dict.copy()
-        type = DbtProjectTypeGITHUB(d.pop("type"))
+        type = DbtGithubProjectConfigType(d.pop("type"))
 
         personal_access_token = d.pop("personal_access_token")
 
         repository = d.pop("repository")
 
         branch = d.pop("branch")
 
         project_sub_path = d.pop("project_sub_path")
 
         target = d.pop("target", UNSET)
 
         environment = []
         _environment = d.pop("environment", UNSET)
         for environment_item_data in _environment or []:
-            environment_item = DbtProjectEnvironmentVariable.from_dict(environment_item_data)
+            environment_item = DbtGithubProjectConfigEnvironmentItem.from_dict(environment_item_data)
 
             environment.append(environment_item)
 
         host_domain = d.pop("host_domain", UNSET)
 
         dbt_github_project_config = cls(
             type=type,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_gitlab_project_config.py` & `lightdash_client_python-0.621.0/lightdash_client/models/dbt_gitlab_project_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,46 +4,46 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.dbt_project_type_gitlab import DbtProjectTypeGITLAB
+from ..models.dbt_gitlab_project_config_type import DbtGitlabProjectConfigType
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+    from ..models.dbt_gitlab_project_config_environment_item import DbtGitlabProjectConfigEnvironmentItem
 
 
 T = TypeVar("T", bound="DbtGitlabProjectConfig")
 
 
 @attr.s(auto_attribs=True)
 class DbtGitlabProjectConfig:
     """
     Attributes:
-        type (DbtProjectTypeGITLAB):
+        type (DbtGitlabProjectConfigType):
         personal_access_token (str):
         repository (str):
         branch (str):
         project_sub_path (str):
         target (Union[Unset, str]):
-        environment (Union[Unset, List['DbtProjectEnvironmentVariable']]):
+        environment (Union[Unset, List['DbtGitlabProjectConfigEnvironmentItem']]):
         host_domain (Union[Unset, str]):
     """
 
-    type: DbtProjectTypeGITLAB
+    type: DbtGitlabProjectConfigType
     personal_access_token: str
     repository: str
     branch: str
     project_sub_path: str
     target: Union[Unset, str] = UNSET
-    environment: Union[Unset, List["DbtProjectEnvironmentVariable"]] = UNSET
+    environment: Union[Unset, List["DbtGitlabProjectConfigEnvironmentItem"]] = UNSET
     host_domain: Union[Unset, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         personal_access_token = self.personal_access_token
         repository = self.repository
@@ -77,33 +77,33 @@
         if host_domain is not UNSET:
             field_dict["host_domain"] = host_domain
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+        from ..models.dbt_gitlab_project_config_environment_item import DbtGitlabProjectConfigEnvironmentItem
 
         d = src_dict.copy()
-        type = DbtProjectTypeGITLAB(d.pop("type"))
+        type = DbtGitlabProjectConfigType(d.pop("type"))
 
         personal_access_token = d.pop("personal_access_token")
 
         repository = d.pop("repository")
 
         branch = d.pop("branch")
 
         project_sub_path = d.pop("project_sub_path")
 
         target = d.pop("target", UNSET)
 
         environment = []
         _environment = d.pop("environment", UNSET)
         for environment_item_data in _environment or []:
-            environment_item = DbtProjectEnvironmentVariable.from_dict(environment_item_data)
+            environment_item = DbtGitlabProjectConfigEnvironmentItem.from_dict(environment_item_data)
 
             environment.append(environment_item)
 
         host_domain = d.pop("host_domain", UNSET)
 
         dbt_gitlab_project_config = cls(
             type=type,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_local_project_config.py` & `lightdash_client_python-0.621.0/lightdash_client/models/project_dbt_connection_type_0.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.dbt_project_type_dbt import DbtProjectTypeDBT
+from ..models.project_dbt_connection_type_0_type import ProjectDbtConnectionType0Type
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+    from ..models.project_dbt_connection_type_0_environment_item import ProjectDbtConnectionType0EnvironmentItem
 
 
-T = TypeVar("T", bound="DbtLocalProjectConfig")
+T = TypeVar("T", bound="ProjectDbtConnectionType0")
 
 
 @attr.s(auto_attribs=True)
-class DbtLocalProjectConfig:
+class ProjectDbtConnectionType0:
     """
     Attributes:
-        type (DbtProjectTypeDBT):
+        type (ProjectDbtConnectionType0Type):
         target (Union[Unset, str]):
-        environment (Union[Unset, List['DbtProjectEnvironmentVariable']]):
+        environment (Union[Unset, List['ProjectDbtConnectionType0EnvironmentItem']]):
         profiles_dir (Union[Unset, str]):
         project_dir (Union[Unset, str]):
     """
 
-    type: DbtProjectTypeDBT
+    type: ProjectDbtConnectionType0Type
     target: Union[Unset, str] = UNSET
-    environment: Union[Unset, List["DbtProjectEnvironmentVariable"]] = UNSET
+    environment: Union[Unset, List["ProjectDbtConnectionType0EnvironmentItem"]] = UNSET
     profiles_dir: Union[Unset, str] = UNSET
     project_dir: Union[Unset, str] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         target = self.target
@@ -66,34 +66,34 @@
         if project_dir is not UNSET:
             field_dict["project_dir"] = project_dir
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+        from ..models.project_dbt_connection_type_0_environment_item import ProjectDbtConnectionType0EnvironmentItem
 
         d = src_dict.copy()
-        type = DbtProjectTypeDBT(d.pop("type"))
+        type = ProjectDbtConnectionType0Type(d.pop("type"))
 
         target = d.pop("target", UNSET)
 
         environment = []
         _environment = d.pop("environment", UNSET)
         for environment_item_data in _environment or []:
-            environment_item = DbtProjectEnvironmentVariable.from_dict(environment_item_data)
+            environment_item = ProjectDbtConnectionType0EnvironmentItem.from_dict(environment_item_data)
 
             environment.append(environment_item)
 
         profiles_dir = d.pop("profiles_dir", UNSET)
 
         project_dir = d.pop("project_dir", UNSET)
 
-        dbt_local_project_config = cls(
+        project_dbt_connection_type_0 = cls(
             type=type,
             target=target,
             environment=environment,
             profiles_dir=profiles_dir,
             project_dir=project_dir,
         )
 
-        return dbt_local_project_config
+        return project_dbt_connection_type_0
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_none_project_config.py` & `lightdash_client_python-0.621.0/lightdash_client/models/dbt_none_project_config.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,38 +4,38 @@
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.dbt_project_type_none import DbtProjectTypeNONE
+from ..models.dbt_none_project_config_type import DbtNoneProjectConfigType
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+    from ..models.dbt_none_project_config_environment_item import DbtNoneProjectConfigEnvironmentItem
 
 
 T = TypeVar("T", bound="DbtNoneProjectConfig")
 
 
 @attr.s(auto_attribs=True)
 class DbtNoneProjectConfig:
     """
     Attributes:
-        type (DbtProjectTypeNONE):
+        type (DbtNoneProjectConfigType):
         target (Union[Unset, str]):
-        environment (Union[Unset, List['DbtProjectEnvironmentVariable']]):
+        environment (Union[Unset, List['DbtNoneProjectConfigEnvironmentItem']]):
         hide_refresh_button (Union[Unset, bool]):
     """
 
-    type: DbtProjectTypeNONE
+    type: DbtNoneProjectConfigType
     target: Union[Unset, str] = UNSET
-    environment: Union[Unset, List["DbtProjectEnvironmentVariable"]] = UNSET
+    environment: Union[Unset, List["DbtNoneProjectConfigEnvironmentItem"]] = UNSET
     hide_refresh_button: Union[Unset, bool] = UNSET
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         target = self.target
         environment: Union[Unset, List[Dict[str, Any]]] = UNSET
@@ -61,25 +61,25 @@
         if hide_refresh_button is not UNSET:
             field_dict["hideRefreshButton"] = hide_refresh_button
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dbt_project_environment_variable import DbtProjectEnvironmentVariable
+        from ..models.dbt_none_project_config_environment_item import DbtNoneProjectConfigEnvironmentItem
 
         d = src_dict.copy()
-        type = DbtProjectTypeNONE(d.pop("type"))
+        type = DbtNoneProjectConfigType(d.pop("type"))
 
         target = d.pop("target", UNSET)
 
         environment = []
         _environment = d.pop("environment", UNSET)
         for environment_item_data in _environment or []:
-            environment_item = DbtProjectEnvironmentVariable.from_dict(environment_item_data)
+            environment_item = DbtNoneProjectConfigEnvironmentItem.from_dict(environment_item_data)
 
             environment.append(environment_item)
 
         hide_refresh_button = d.pop("hideRefreshButton", UNSET)
 
         dbt_none_project_config = cls(
             type=type,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/dbt_project_environment_variable.py` & `lightdash_client_python-0.621.0/lightdash_client/models/dbt_project_environment_variable.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/delete_scheduler_response_201.py` & `lightdash_client_python-0.621.0/lightdash_client/models/delete_scheduler_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/email_one_time_password.py` & `lightdash_client_python-0.621.0/lightdash_client/models/email_one_time_password.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/email_one_time_password_expiring.py` & `lightdash_client_python-0.621.0/lightdash_client/models/email_one_time_password_expiring.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/email_status.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_email_status_response_results.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,32 +8,34 @@
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.email_one_time_password import EmailOneTimePassword
+    from ..models.api_email_status_response_results_otp import ApiEmailStatusResponseResultsOtp
 
 
-T = TypeVar("T", bound="EmailStatus")
+T = TypeVar("T", bound="ApiEmailStatusResponseResults")
 
 
 @attr.s(auto_attribs=True)
-class EmailStatus:
-    """
+class ApiEmailStatusResponseResults:
+    """Verification status of an email address
+
     Attributes:
         is_verified (bool):
         email (str):
-        otp (Union[Unset, EmailOneTimePassword]):
+        otp (Union[Unset, ApiEmailStatusResponseResultsOtp]): One time passcode information
+            If there is no active passcode, this will be undefined
     """
 
     is_verified: bool
     email: str
-    otp: Union[Unset, "EmailOneTimePassword"] = UNSET
+    otp: Union[Unset, "ApiEmailStatusResponseResultsOtp"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         is_verified = self.is_verified
         email = self.email
         otp: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.otp, Unset):
@@ -50,36 +52,36 @@
         if otp is not UNSET:
             field_dict["otp"] = otp
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.email_one_time_password import EmailOneTimePassword
+        from ..models.api_email_status_response_results_otp import ApiEmailStatusResponseResultsOtp
 
         d = src_dict.copy()
         is_verified = d.pop("isVerified")
 
         email = d.pop("email")
 
         _otp = d.pop("otp", UNSET)
-        otp: Union[Unset, EmailOneTimePassword]
+        otp: Union[Unset, ApiEmailStatusResponseResultsOtp]
         if isinstance(_otp, Unset):
             otp = UNSET
         else:
-            otp = EmailOneTimePassword.from_dict(_otp)
+            otp = ApiEmailStatusResponseResultsOtp.from_dict(_otp)
 
-        email_status = cls(
+        api_email_status_response_results = cls(
             is_verified=is_verified,
             email=email,
             otp=otp,
         )
 
-        email_status.additional_properties = d
-        return email_status
+        api_email_status_response_results.additional_properties = d
+        return api_email_status_response_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/filter_group_response_type_0.py` & `lightdash_client_python-0.621.0/lightdash_client/models/filter_group_response_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/filter_group_response_type_1.py` & `lightdash_client_python-0.621.0/lightdash_client/models/filter_group_response_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/group.py` & `lightdash_client_python-0.621.0/lightdash_client/models/group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/group_member.py` & `lightdash_client_python-0.621.0/lightdash_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/metric_query_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,43 +9,43 @@
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.additional_metric import AdditionalMetric
-    from ..models.filters import Filters
-    from ..models.sort_field import SortField
-    from ..models.table_calculation import TableCalculation
+    from ..models.metric_query_response_additional_metrics_item import MetricQueryResponseAdditionalMetricsItem
+    from ..models.metric_query_response_filters import MetricQueryResponseFilters
+    from ..models.metric_query_response_sorts_item import MetricQueryResponseSortsItem
+    from ..models.metric_query_response_table_calculations_item import MetricQueryResponseTableCalculationsItem
 
 
 T = TypeVar("T", bound="MetricQueryResponse")
 
 
 @attr.s(auto_attribs=True)
 class MetricQueryResponse:
     """
     Attributes:
-        table_calculations (List['TableCalculation']):
+        table_calculations (List['MetricQueryResponseTableCalculationsItem']):
         limit (float):
-        sorts (List['SortField']):
-        filters (Filters):
+        sorts (List['MetricQueryResponseSortsItem']):
+        filters (MetricQueryResponseFilters):
         metrics (List[str]):
         dimensions (List[str]):
-        additional_metrics (Union[Unset, List['AdditionalMetric']]):
+        additional_metrics (Union[Unset, List['MetricQueryResponseAdditionalMetricsItem']]):
     """
 
-    table_calculations: List["TableCalculation"]
+    table_calculations: List["MetricQueryResponseTableCalculationsItem"]
     limit: float
-    sorts: List["SortField"]
-    filters: "Filters"
+    sorts: List["MetricQueryResponseSortsItem"]
+    filters: "MetricQueryResponseFilters"
     metrics: List[str]
     dimensions: List[str]
-    additional_metrics: Union[Unset, List["AdditionalMetric"]] = UNSET
+    additional_metrics: Union[Unset, List["MetricQueryResponseAdditionalMetricsItem"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         table_calculations = []
         for table_calculations_item_data in self.table_calculations:
             table_calculations_item = table_calculations_item_data.to_dict()
 
@@ -87,46 +87,46 @@
         if additional_metrics is not UNSET:
             field_dict["additionalMetrics"] = additional_metrics
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.additional_metric import AdditionalMetric
-        from ..models.filters import Filters
-        from ..models.sort_field import SortField
-        from ..models.table_calculation import TableCalculation
+        from ..models.metric_query_response_additional_metrics_item import MetricQueryResponseAdditionalMetricsItem
+        from ..models.metric_query_response_filters import MetricQueryResponseFilters
+        from ..models.metric_query_response_sorts_item import MetricQueryResponseSortsItem
+        from ..models.metric_query_response_table_calculations_item import MetricQueryResponseTableCalculationsItem
 
         d = src_dict.copy()
         table_calculations = []
         _table_calculations = d.pop("tableCalculations")
         for table_calculations_item_data in _table_calculations:
-            table_calculations_item = TableCalculation.from_dict(table_calculations_item_data)
+            table_calculations_item = MetricQueryResponseTableCalculationsItem.from_dict(table_calculations_item_data)
 
             table_calculations.append(table_calculations_item)
 
         limit = d.pop("limit")
 
         sorts = []
         _sorts = d.pop("sorts")
         for sorts_item_data in _sorts:
-            sorts_item = SortField.from_dict(sorts_item_data)
+            sorts_item = MetricQueryResponseSortsItem.from_dict(sorts_item_data)
 
             sorts.append(sorts_item)
 
-        filters = Filters.from_dict(d.pop("filters"))
+        filters = MetricQueryResponseFilters.from_dict(d.pop("filters"))
 
         metrics = cast(List[str], d.pop("metrics"))
 
         dimensions = cast(List[str], d.pop("dimensions"))
 
         additional_metrics = []
         _additional_metrics = d.pop("additionalMetrics", UNSET)
         for additional_metrics_item_data in _additional_metrics or []:
-            additional_metrics_item = AdditionalMetric.from_dict(additional_metrics_item_data)
+            additional_metrics_item = MetricQueryResponseAdditionalMetricsItem.from_dict(additional_metrics_item_data)
 
             additional_metrics.append(additional_metrics_item)
 
         metric_query_response = cls(
             table_calculations=table_calculations,
             limit=limit,
             sorts=sorts,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/organization.py` & `lightdash_client_python-0.621.0/lightdash_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/organization_member_profile.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_organization_member_profile_results.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from typing import List
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.organization_member_role import OrganizationMemberRole
+from ..models.api_organization_member_profile_results_role import ApiOrganizationMemberProfileResultsRole
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="OrganizationMemberProfile")
+T = TypeVar("T", bound="ApiOrganizationMemberProfileResults")
 
 
 @attr.s(auto_attribs=True)
-class OrganizationMemberProfile:
+class ApiOrganizationMemberProfileResults:
     """Profile for a user's membership in an organization
 
     Attributes:
         is_active (bool): Whether the user has accepted their invite to the organization
-        role (OrganizationMemberRole):
+        role (ApiOrganizationMemberProfileResultsRole): The role of the user in the organization
         organization_uuid (str): Unique identifier for the organization the user is a member of
         email (str):
         last_name (str):
         first_name (str):
         user_uuid (str): Unique identifier for the user
         is_invite_expired (Union[Unset, bool]): Whether the user's invite to the organization has expired
     """
 
     is_active: bool
-    role: OrganizationMemberRole
+    role: ApiOrganizationMemberProfileResultsRole
     organization_uuid: str
     email: str
     last_name: str
     first_name: str
     user_uuid: str
     is_invite_expired: Union[Unset, bool] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -69,41 +69,41 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         is_active = d.pop("isActive")
 
-        role = OrganizationMemberRole(d.pop("role"))
+        role = ApiOrganizationMemberProfileResultsRole(d.pop("role"))
 
         organization_uuid = d.pop("organizationUuid")
 
         email = d.pop("email")
 
         last_name = d.pop("lastName")
 
         first_name = d.pop("firstName")
 
         user_uuid = d.pop("userUuid")
 
         is_invite_expired = d.pop("isInviteExpired", UNSET)
 
-        organization_member_profile = cls(
+        api_organization_member_profile_results = cls(
             is_active=is_active,
             role=role,
             organization_uuid=organization_uuid,
             email=email,
             last_name=last_name,
             first_name=first_name,
             user_uuid=user_uuid,
             is_invite_expired=is_invite_expired,
         )
 
-        organization_member_profile.additional_properties = d
-        return organization_member_profile
+        api_organization_member_profile_results.additional_properties = d
+        return api_organization_member_profile_results
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/organization_member_profile_update.py` & `lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.organization_member_role import OrganizationMemberRole
-
-T = TypeVar("T", bound="OrganizationMemberProfileUpdate")
+T = TypeVar("T", bound="PostChartResultsJsonBodyFiltersMetricsType1")
 
 
 @attr.s(auto_attribs=True)
-class OrganizationMemberProfileUpdate:
+class PostChartResultsJsonBodyFiltersMetricsType1:
     """
     Attributes:
-        role (OrganizationMemberRole):
+        and_ (List[Any]):
+        id (str):
     """
 
-    role: OrganizationMemberRole
+    and_: List[Any]
+    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        role = self.role.value
+        and_ = self.and_
+
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "role": role,
+                "and": and_,
+                "id": id,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        role = OrganizationMemberRole(d.pop("role"))
+        and_ = cast(List[Any], d.pop("and"))
+
+        id = d.pop("id")
 
-        organization_member_profile_update = cls(
-            role=role,
+        post_chart_results_json_body_filters_metrics_type_1 = cls(
+            and_=and_,
+            id=id,
         )
 
-        organization_member_profile_update.additional_properties = d
-        return organization_member_profile_update
+        post_chart_results_json_body_filters_metrics_type_1.additional_properties = d
+        return post_chart_results_json_body_filters_metrics_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/organization_project.py` & `lightdash_client_python-0.621.0/lightdash_client/models/organization_project.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.project_type import ProjectType
+from ..models.organization_project_type import OrganizationProjectType
 
 T = TypeVar("T", bound="OrganizationProject")
 
 
 @attr.s(auto_attribs=True)
 class OrganizationProject:
     """Summary of a project under an organization
 
     Attributes:
-        type (ProjectType):
+        type (OrganizationProjectType):
         name (str):
         project_uuid (str): The unique identifier of the project
     """
 
-    type: ProjectType
+    type: OrganizationProjectType
     name: str
     project_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
@@ -43,15 +43,15 @@
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        type = ProjectType(d.pop("type"))
+        type = OrganizationProjectType(d.pop("type"))
 
         name = d.pop("name")
 
         project_uuid = d.pop("projectUuid")
 
         organization_project = cls(
             type=type,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py` & `lightdash_client_python-0.621.0/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/partial_pick_space_is_private_or_access.py` & `lightdash_client_python-0.621.0/lightdash_client/models/partial_pick_space_is_private_or_access.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,31 +8,31 @@
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.space_share import SpaceShare
+    from ..models.partial_pick_space_is_private_or_access_access_item import PartialPickSpaceIsPrivateOrAccessAccessItem
 
 
 T = TypeVar("T", bound="PartialPickSpaceIsPrivateOrAccess")
 
 
 @attr.s(auto_attribs=True)
 class PartialPickSpaceIsPrivateOrAccess:
     """Make all properties in T optional
 
     Attributes:
         is_private (Union[Unset, bool]):
-        access (Union[Unset, List['SpaceShare']]):
+        access (Union[Unset, List['PartialPickSpaceIsPrivateOrAccessAccessItem']]):
     """
 
     is_private: Union[Unset, bool] = UNSET
-    access: Union[Unset, List["SpaceShare"]] = UNSET
+    access: Union[Unset, List["PartialPickSpaceIsPrivateOrAccessAccessItem"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         is_private = self.is_private
         access: Union[Unset, List[Dict[str, Any]]] = UNSET
         if not isinstance(self.access, Unset):
             access = []
@@ -49,23 +49,25 @@
         if access is not UNSET:
             field_dict["access"] = access
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.space_share import SpaceShare
+        from ..models.partial_pick_space_is_private_or_access_access_item import (
+            PartialPickSpaceIsPrivateOrAccessAccessItem,
+        )
 
         d = src_dict.copy()
         is_private = d.pop("isPrivate", UNSET)
 
         access = []
         _access = d.pop("access", UNSET)
         for access_item_data in _access or []:
-            access_item = SpaceShare.from_dict(access_item_data)
+            access_item = PartialPickSpaceIsPrivateOrAccessAccessItem.from_dict(access_item_data)
 
             access.append(access_item)
 
         partial_pick_space_is_private_or_access = cls(
             is_private=is_private,
             access=access,
         )
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py` & `lightdash_client_python-0.621.0/lightdash_client/models/update_allowed_email_domains.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,70 +3,70 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.organization_member_role import OrganizationMemberRole
+from ..models.update_allowed_email_domains_role import UpdateAllowedEmailDomainsRole
 
-T = TypeVar("T", bound="PickAllowedEmailDomainsExcludeKeyofAllowedEmailDomainsOrganizationUuid")
+T = TypeVar("T", bound="UpdateAllowedEmailDomains")
 
 
 @attr.s(auto_attribs=True)
-class PickAllowedEmailDomainsExcludeKeyofAllowedEmailDomainsOrganizationUuid:
-    """From T, pick a set of properties whose keys are in the union K
+class UpdateAllowedEmailDomains:
+    """Construct a type with the properties of T except for those in type K.
 
     Attributes:
+        role (UpdateAllowedEmailDomainsRole):
         email_domains (List[str]):
-        role (OrganizationMemberRole):
         project_uuids (List[str]):
     """
 
+    role: UpdateAllowedEmailDomainsRole
     email_domains: List[str]
-    role: OrganizationMemberRole
     project_uuids: List[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        email_domains = self.email_domains
-
         role = self.role.value
 
+        email_domains = self.email_domains
+
         project_uuids = self.project_uuids
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "emailDomains": email_domains,
                 "role": role,
+                "emailDomains": email_domains,
                 "projectUuids": project_uuids,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        email_domains = cast(List[str], d.pop("emailDomains"))
+        role = UpdateAllowedEmailDomainsRole(d.pop("role"))
 
-        role = OrganizationMemberRole(d.pop("role"))
+        email_domains = cast(List[str], d.pop("emailDomains"))
 
         project_uuids = cast(List[str], d.pop("projectUuids"))
 
-        pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid = cls(
-            email_domains=email_domains,
+        update_allowed_email_domains = cls(
             role=role,
+            email_domains=email_domains,
             project_uuids=project_uuids,
         )
 
-        pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.additional_properties = d
-        return pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid
+        update_allowed_email_domains.additional_properties = d
+        return update_allowed_email_domains
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.621.0/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,73 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority import (
-    PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority,
+from ..models.omit_create_bigquery_credentials_sensitive_credentials_field_names_priority import (
+    OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority,
+)
+from ..models.omit_create_bigquery_credentials_sensitive_credentials_field_names_type import (
+    OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesType,
 )
-from ..models.warehouse_types_bigquery import WarehouseTypesBIGQUERY
-from ..models.week_day import WeekDay
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar(
-    "T", bound="PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNames"
-)
+if TYPE_CHECKING:
+    from ..models.omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week import (
+        OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
+    )
+
+
+T = TypeVar("T", bound="OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNames")
 
 
 @attr.s(auto_attribs=True)
-class PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNames:
-    """From T, pick a set of properties whose keys are in the union K
+class OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNames:
+    """Construct a type with the properties of T except for those in type K.
 
     Attributes:
-        type (WarehouseTypesBIGQUERY):
+        type (OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesType):
         project (str):
         dataset (str):
         threads (Union[Unset, float]):
-        start_of_week (Union[Unset, None, WeekDay]):
+        start_of_week (Union[Unset, None, OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesStartOfWeek]):
         timeout_seconds (Union[Unset, float]):
-        priority (Union[Unset,
-            PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority]):
+        priority (Union[Unset, OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority]):
         retries (Union[Unset, float]):
         location (Union[Unset, str]):
         maximum_bytes_billed (Union[Unset, float]):
     """
 
-    type: WarehouseTypesBIGQUERY
+    type: OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesType
     project: str
     dataset: str
     threads: Union[Unset, float] = UNSET
-    start_of_week: Union[Unset, None, WeekDay] = UNSET
+    start_of_week: Union[Unset, None, "OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesStartOfWeek"] = UNSET
     timeout_seconds: Union[Unset, float] = UNSET
-    priority: Union[
-        Unset, PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority
-    ] = UNSET
+    priority: Union[Unset, OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority] = UNSET
     retries: Union[Unset, float] = UNSET
     location: Union[Unset, str] = UNSET
     maximum_bytes_billed: Union[Unset, float] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         project = self.project
         dataset = self.dataset
         threads = self.threads
-        start_of_week: Union[Unset, None, int] = UNSET
+        start_of_week: Union[Unset, None, Dict[str, Any]] = UNSET
         if not isinstance(self.start_of_week, Unset):
-            start_of_week = self.start_of_week.value if self.start_of_week else None
+            start_of_week = self.start_of_week.to_dict() if self.start_of_week else None
 
         timeout_seconds = self.timeout_seconds
         priority: Union[Unset, str] = UNSET
         if not isinstance(self.priority, Unset):
             priority = self.priority.value
 
         retries = self.retries
@@ -95,73 +98,68 @@
         if maximum_bytes_billed is not UNSET:
             field_dict["maximumBytesBilled"] = maximum_bytes_billed
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week import (
+            OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
+        )
+
         d = src_dict.copy()
-        type = WarehouseTypesBIGQUERY(d.pop("type"))
+        type = OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesType(d.pop("type"))
 
         project = d.pop("project")
 
         dataset = d.pop("dataset")
 
         threads = d.pop("threads", UNSET)
 
         _start_of_week = d.pop("startOfWeek", UNSET)
-        start_of_week: Union[Unset, None, WeekDay]
+        start_of_week: Union[Unset, None, OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesStartOfWeek]
         if _start_of_week is None:
             start_of_week = None
         elif isinstance(_start_of_week, Unset):
             start_of_week = UNSET
         else:
-            start_of_week = WeekDay(_start_of_week)
+            start_of_week = OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesStartOfWeek.from_dict(
+                _start_of_week
+            )
 
         timeout_seconds = d.pop("timeoutSeconds", UNSET)
 
         _priority = d.pop("priority", UNSET)
-        priority: Union[
-            Unset,
-            PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority,
-        ]
+        priority: Union[Unset, OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority]
         if isinstance(_priority, Unset):
             priority = UNSET
         else:
-            priority = PickCreateBigqueryCredentialsExcludeKeyofCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority(
-                _priority
-            )
+            priority = OmitCreateBigqueryCredentialsSensitiveCredentialsFieldNamesPriority(_priority)
 
         retries = d.pop("retries", UNSET)
 
         location = d.pop("location", UNSET)
 
         maximum_bytes_billed = d.pop("maximumBytesBilled", UNSET)
 
-        pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names = (
-            cls(
-                type=type,
-                project=project,
-                dataset=dataset,
-                threads=threads,
-                start_of_week=start_of_week,
-                timeout_seconds=timeout_seconds,
-                priority=priority,
-                retries=retries,
-                location=location,
-                maximum_bytes_billed=maximum_bytes_billed,
-            )
+        omit_create_bigquery_credentials_sensitive_credentials_field_names = cls(
+            type=type,
+            project=project,
+            dataset=dataset,
+            threads=threads,
+            start_of_week=start_of_week,
+            timeout_seconds=timeout_seconds,
+            priority=priority,
+            retries=retries,
+            location=location,
+            maximum_bytes_billed=maximum_bytes_billed,
         )
 
-        pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.additional_properties = (
-            d
-        )
-        return (
-            pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names
-        )
+        omit_create_bigquery_credentials_sensitive_credentials_field_names.additional_properties = d
+        return omit_create_bigquery_credentials_sensitive_credentials_field_names
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.621.0/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.warehouse_types_databricks import WarehouseTypesDATABRICKS
-from ..models.week_day import WeekDay
+from ..models.get_project_response_200_results_warehouse_connection_type_4_type import (
+    GetProjectResponse200ResultsWarehouseConnectionType4Type,
+)
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar(
-    "T", bound="PickCreateDatabricksCredentialsExcludeKeyofCreateDatabricksCredentialsSensitiveCredentialsFieldNames"
-)
+if TYPE_CHECKING:
+    from ..models.get_project_response_200_results_warehouse_connection_type_4_start_of_week import (
+        GetProjectResponse200ResultsWarehouseConnectionType4StartOfWeek,
+    )
+
+
+T = TypeVar("T", bound="GetProjectResponse200ResultsWarehouseConnectionType4")
 
 
 @attr.s(auto_attribs=True)
-class PickCreateDatabricksCredentialsExcludeKeyofCreateDatabricksCredentialsSensitiveCredentialsFieldNames:
-    """From T, pick a set of properties whose keys are in the union K
+class GetProjectResponse200ResultsWarehouseConnectionType4:
+    """Construct a type with the properties of T except for those in type K.
 
     Attributes:
-        type (WarehouseTypesDATABRICKS):
+        type (GetProjectResponse200ResultsWarehouseConnectionType4Type):
         database (str):
         server_host_name (str):
         http_path (str):
-        start_of_week (Union[Unset, None, WeekDay]):
+        start_of_week (Union[Unset, None, GetProjectResponse200ResultsWarehouseConnectionType4StartOfWeek]):
         catalog (Union[Unset, str]):
     """
 
-    type: WarehouseTypesDATABRICKS
+    type: GetProjectResponse200ResultsWarehouseConnectionType4Type
     database: str
     server_host_name: str
     http_path: str
-    start_of_week: Union[Unset, None, WeekDay] = UNSET
+    start_of_week: Union[Unset, None, "GetProjectResponse200ResultsWarehouseConnectionType4StartOfWeek"] = UNSET
     catalog: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         database = self.database
         server_host_name = self.server_host_name
         http_path = self.http_path
-        start_of_week: Union[Unset, None, int] = UNSET
+        start_of_week: Union[Unset, None, Dict[str, Any]] = UNSET
         if not isinstance(self.start_of_week, Unset):
-            start_of_week = self.start_of_week.value if self.start_of_week else None
+            start_of_week = self.start_of_week.to_dict() if self.start_of_week else None
 
         catalog = self.catalog
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
@@ -65,47 +71,49 @@
         if catalog is not UNSET:
             field_dict["catalog"] = catalog
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.get_project_response_200_results_warehouse_connection_type_4_start_of_week import (
+            GetProjectResponse200ResultsWarehouseConnectionType4StartOfWeek,
+        )
+
         d = src_dict.copy()
-        type = WarehouseTypesDATABRICKS(d.pop("type"))
+        type = GetProjectResponse200ResultsWarehouseConnectionType4Type(d.pop("type"))
 
         database = d.pop("database")
 
         server_host_name = d.pop("serverHostName")
 
         http_path = d.pop("httpPath")
 
         _start_of_week = d.pop("startOfWeek", UNSET)
-        start_of_week: Union[Unset, None, WeekDay]
+        start_of_week: Union[Unset, None, GetProjectResponse200ResultsWarehouseConnectionType4StartOfWeek]
         if _start_of_week is None:
             start_of_week = None
         elif isinstance(_start_of_week, Unset):
             start_of_week = UNSET
         else:
-            start_of_week = WeekDay(_start_of_week)
+            start_of_week = GetProjectResponse200ResultsWarehouseConnectionType4StartOfWeek.from_dict(_start_of_week)
 
         catalog = d.pop("catalog", UNSET)
 
-        pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names = cls(
+        get_project_response_200_results_warehouse_connection_type_4 = cls(
             type=type,
             database=database,
             server_host_name=server_host_name,
             http_path=http_path,
             start_of_week=start_of_week,
             catalog=catalog,
         )
 
-        pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.additional_properties = (
-            d
-        )
-        return pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names
+        get_project_response_200_results_warehouse_connection_type_4.additional_properties = d
+        return get_project_response_200_results_warehouse_connection_type_4
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_group_name.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_create_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.621.0/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,63 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.warehouse_types_postgres import WarehouseTypesPOSTGRES
-from ..models.week_day import WeekDay
+from ..models.omit_create_postgres_credentials_sensitive_credentials_field_names_type import (
+    OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesType,
+)
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar(
-    "T", bound="PickCreatePostgresCredentialsExcludeKeyofCreatePostgresCredentialsSensitiveCredentialsFieldNames"
-)
+if TYPE_CHECKING:
+    from ..models.omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week import (
+        OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
+    )
+
+
+T = TypeVar("T", bound="OmitCreatePostgresCredentialsSensitiveCredentialsFieldNames")
 
 
 @attr.s(auto_attribs=True)
-class PickCreatePostgresCredentialsExcludeKeyofCreatePostgresCredentialsSensitiveCredentialsFieldNames:
-    """From T, pick a set of properties whose keys are in the union K
+class OmitCreatePostgresCredentialsSensitiveCredentialsFieldNames:
+    """Construct a type with the properties of T except for those in type K.
 
     Attributes:
-        type (WarehouseTypesPOSTGRES):
+        type (OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesType):
         schema (str):
         host (str):
         port (float):
         dbname (str):
         role (Union[Unset, str]):
         threads (Union[Unset, float]):
-        start_of_week (Union[Unset, None, WeekDay]):
+        start_of_week (Union[Unset, None, OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesStartOfWeek]):
         use_ssh_tunnel (Union[Unset, bool]):
         ssh_tunnel_host (Union[Unset, str]):
         ssh_tunnel_port (Union[Unset, float]):
         ssh_tunnel_user (Union[Unset, str]):
         ssh_tunnel_public_key (Union[Unset, str]):
         keepalives_idle (Union[Unset, float]):
         sslmode (Union[Unset, str]):
         search_path (Union[Unset, str]):
     """
 
-    type: WarehouseTypesPOSTGRES
+    type: OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesType
     schema: str
     host: str
     port: float
     dbname: str
     role: Union[Unset, str] = UNSET
     threads: Union[Unset, float] = UNSET
-    start_of_week: Union[Unset, None, WeekDay] = UNSET
+    start_of_week: Union[Unset, None, "OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesStartOfWeek"] = UNSET
     use_ssh_tunnel: Union[Unset, bool] = UNSET
     ssh_tunnel_host: Union[Unset, str] = UNSET
     ssh_tunnel_port: Union[Unset, float] = UNSET
     ssh_tunnel_user: Union[Unset, str] = UNSET
     ssh_tunnel_public_key: Union[Unset, str] = UNSET
     keepalives_idle: Union[Unset, float] = UNSET
     sslmode: Union[Unset, str] = UNSET
@@ -63,17 +69,17 @@
 
         schema = self.schema
         host = self.host
         port = self.port
         dbname = self.dbname
         role = self.role
         threads = self.threads
-        start_of_week: Union[Unset, None, int] = UNSET
+        start_of_week: Union[Unset, None, Dict[str, Any]] = UNSET
         if not isinstance(self.start_of_week, Unset):
-            start_of_week = self.start_of_week.value if self.start_of_week else None
+            start_of_week = self.start_of_week.to_dict() if self.start_of_week else None
 
         use_ssh_tunnel = self.use_ssh_tunnel
         ssh_tunnel_host = self.ssh_tunnel_host
         ssh_tunnel_port = self.ssh_tunnel_port
         ssh_tunnel_user = self.ssh_tunnel_user
         ssh_tunnel_public_key = self.ssh_tunnel_public_key
         keepalives_idle = self.keepalives_idle
@@ -114,37 +120,43 @@
         if search_path is not UNSET:
             field_dict["searchPath"] = search_path
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week import (
+            OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
+        )
+
         d = src_dict.copy()
-        type = WarehouseTypesPOSTGRES(d.pop("type"))
+        type = OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesType(d.pop("type"))
 
         schema = d.pop("schema")
 
         host = d.pop("host")
 
         port = d.pop("port")
 
         dbname = d.pop("dbname")
 
         role = d.pop("role", UNSET)
 
         threads = d.pop("threads", UNSET)
 
         _start_of_week = d.pop("startOfWeek", UNSET)
-        start_of_week: Union[Unset, None, WeekDay]
+        start_of_week: Union[Unset, None, OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesStartOfWeek]
         if _start_of_week is None:
             start_of_week = None
         elif isinstance(_start_of_week, Unset):
             start_of_week = UNSET
         else:
-            start_of_week = WeekDay(_start_of_week)
+            start_of_week = OmitCreatePostgresCredentialsSensitiveCredentialsFieldNamesStartOfWeek.from_dict(
+                _start_of_week
+            )
 
         use_ssh_tunnel = d.pop("useSshTunnel", UNSET)
 
         ssh_tunnel_host = d.pop("sshTunnelHost", UNSET)
 
         ssh_tunnel_port = d.pop("sshTunnelPort", UNSET)
 
@@ -154,41 +166,35 @@
 
         keepalives_idle = d.pop("keepalivesIdle", UNSET)
 
         sslmode = d.pop("sslmode", UNSET)
 
         search_path = d.pop("searchPath", UNSET)
 
-        pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names = (
-            cls(
-                type=type,
-                schema=schema,
-                host=host,
-                port=port,
-                dbname=dbname,
-                role=role,
-                threads=threads,
-                start_of_week=start_of_week,
-                use_ssh_tunnel=use_ssh_tunnel,
-                ssh_tunnel_host=ssh_tunnel_host,
-                ssh_tunnel_port=ssh_tunnel_port,
-                ssh_tunnel_user=ssh_tunnel_user,
-                ssh_tunnel_public_key=ssh_tunnel_public_key,
-                keepalives_idle=keepalives_idle,
-                sslmode=sslmode,
-                search_path=search_path,
-            )
+        omit_create_postgres_credentials_sensitive_credentials_field_names = cls(
+            type=type,
+            schema=schema,
+            host=host,
+            port=port,
+            dbname=dbname,
+            role=role,
+            threads=threads,
+            start_of_week=start_of_week,
+            use_ssh_tunnel=use_ssh_tunnel,
+            ssh_tunnel_host=ssh_tunnel_host,
+            ssh_tunnel_port=ssh_tunnel_port,
+            ssh_tunnel_user=ssh_tunnel_user,
+            ssh_tunnel_public_key=ssh_tunnel_public_key,
+            keepalives_idle=keepalives_idle,
+            sslmode=sslmode,
+            search_path=search_path,
         )
 
-        pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.additional_properties = (
-            d
-        )
-        return (
-            pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names
-        )
+        omit_create_postgres_credentials_sensitive_credentials_field_names.additional_properties = d
+        return omit_create_postgres_credentials_sensitive_credentials_field_names
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.621.0/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,61 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.warehouse_types_redshift import WarehouseTypesREDSHIFT
-from ..models.week_day import WeekDay
+from ..models.omit_create_redshift_credentials_sensitive_credentials_field_names_type import (
+    OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesType,
+)
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar(
-    "T", bound="PickCreateRedshiftCredentialsExcludeKeyofCreateRedshiftCredentialsSensitiveCredentialsFieldNames"
-)
+if TYPE_CHECKING:
+    from ..models.omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week import (
+        OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
+    )
+
+
+T = TypeVar("T", bound="OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNames")
 
 
 @attr.s(auto_attribs=True)
-class PickCreateRedshiftCredentialsExcludeKeyofCreateRedshiftCredentialsSensitiveCredentialsFieldNames:
-    """From T, pick a set of properties whose keys are in the union K
+class OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNames:
+    """Construct a type with the properties of T except for those in type K.
 
     Attributes:
-        type (WarehouseTypesREDSHIFT):
+        type (OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesType):
         schema (str):
         host (str):
         port (float):
         dbname (str):
         threads (Union[Unset, float]):
-        start_of_week (Union[Unset, None, WeekDay]):
+        start_of_week (Union[Unset, None, OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesStartOfWeek]):
         use_ssh_tunnel (Union[Unset, bool]):
         ssh_tunnel_host (Union[Unset, str]):
         ssh_tunnel_port (Union[Unset, float]):
         ssh_tunnel_user (Union[Unset, str]):
         ssh_tunnel_public_key (Union[Unset, str]):
         keepalives_idle (Union[Unset, float]):
         sslmode (Union[Unset, str]):
         ra_3_node (Union[Unset, bool]):
     """
 
-    type: WarehouseTypesREDSHIFT
+    type: OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesType
     schema: str
     host: str
     port: float
     dbname: str
     threads: Union[Unset, float] = UNSET
-    start_of_week: Union[Unset, None, WeekDay] = UNSET
+    start_of_week: Union[Unset, None, "OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesStartOfWeek"] = UNSET
     use_ssh_tunnel: Union[Unset, bool] = UNSET
     ssh_tunnel_host: Union[Unset, str] = UNSET
     ssh_tunnel_port: Union[Unset, float] = UNSET
     ssh_tunnel_user: Union[Unset, str] = UNSET
     ssh_tunnel_public_key: Union[Unset, str] = UNSET
     keepalives_idle: Union[Unset, float] = UNSET
     sslmode: Union[Unset, str] = UNSET
@@ -60,17 +66,17 @@
         type = self.type.value
 
         schema = self.schema
         host = self.host
         port = self.port
         dbname = self.dbname
         threads = self.threads
-        start_of_week: Union[Unset, None, int] = UNSET
+        start_of_week: Union[Unset, None, Dict[str, Any]] = UNSET
         if not isinstance(self.start_of_week, Unset):
-            start_of_week = self.start_of_week.value if self.start_of_week else None
+            start_of_week = self.start_of_week.to_dict() if self.start_of_week else None
 
         use_ssh_tunnel = self.use_ssh_tunnel
         ssh_tunnel_host = self.ssh_tunnel_host
         ssh_tunnel_port = self.ssh_tunnel_port
         ssh_tunnel_user = self.ssh_tunnel_user
         ssh_tunnel_public_key = self.ssh_tunnel_public_key
         keepalives_idle = self.keepalives_idle
@@ -109,35 +115,41 @@
         if ra_3_node is not UNSET:
             field_dict["ra3Node"] = ra_3_node
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week import (
+            OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
+        )
+
         d = src_dict.copy()
-        type = WarehouseTypesREDSHIFT(d.pop("type"))
+        type = OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesType(d.pop("type"))
 
         schema = d.pop("schema")
 
         host = d.pop("host")
 
         port = d.pop("port")
 
         dbname = d.pop("dbname")
 
         threads = d.pop("threads", UNSET)
 
         _start_of_week = d.pop("startOfWeek", UNSET)
-        start_of_week: Union[Unset, None, WeekDay]
+        start_of_week: Union[Unset, None, OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesStartOfWeek]
         if _start_of_week is None:
             start_of_week = None
         elif isinstance(_start_of_week, Unset):
             start_of_week = UNSET
         else:
-            start_of_week = WeekDay(_start_of_week)
+            start_of_week = OmitCreateRedshiftCredentialsSensitiveCredentialsFieldNamesStartOfWeek.from_dict(
+                _start_of_week
+            )
 
         use_ssh_tunnel = d.pop("useSshTunnel", UNSET)
 
         ssh_tunnel_host = d.pop("sshTunnelHost", UNSET)
 
         ssh_tunnel_port = d.pop("sshTunnelPort", UNSET)
 
@@ -147,40 +159,34 @@
 
         keepalives_idle = d.pop("keepalivesIdle", UNSET)
 
         sslmode = d.pop("sslmode", UNSET)
 
         ra_3_node = d.pop("ra3Node", UNSET)
 
-        pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names = (
-            cls(
-                type=type,
-                schema=schema,
-                host=host,
-                port=port,
-                dbname=dbname,
-                threads=threads,
-                start_of_week=start_of_week,
-                use_ssh_tunnel=use_ssh_tunnel,
-                ssh_tunnel_host=ssh_tunnel_host,
-                ssh_tunnel_port=ssh_tunnel_port,
-                ssh_tunnel_user=ssh_tunnel_user,
-                ssh_tunnel_public_key=ssh_tunnel_public_key,
-                keepalives_idle=keepalives_idle,
-                sslmode=sslmode,
-                ra_3_node=ra_3_node,
-            )
+        omit_create_redshift_credentials_sensitive_credentials_field_names = cls(
+            type=type,
+            schema=schema,
+            host=host,
+            port=port,
+            dbname=dbname,
+            threads=threads,
+            start_of_week=start_of_week,
+            use_ssh_tunnel=use_ssh_tunnel,
+            ssh_tunnel_host=ssh_tunnel_host,
+            ssh_tunnel_port=ssh_tunnel_port,
+            ssh_tunnel_user=ssh_tunnel_user,
+            ssh_tunnel_public_key=ssh_tunnel_public_key,
+            keepalives_idle=keepalives_idle,
+            sslmode=sslmode,
+            ra_3_node=ra_3_node,
         )
 
-        pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.additional_properties = (
-            d
-        )
-        return (
-            pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names
-        )
+        omit_create_redshift_credentials_sensitive_credentials_field_names.additional_properties = d
+        return omit_create_redshift_credentials_sensitive_credentials_field_names
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.621.0/lightdash_client/models/snowflake_credentials.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,74 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.warehouse_types_snowflake import WarehouseTypesSNOWFLAKE
-from ..models.week_day import WeekDay
+from ..models.snowflake_credentials_type import SnowflakeCredentialsType
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar(
-    "T", bound="PickCreateSnowflakeCredentialsExcludeKeyofCreateSnowflakeCredentialsSensitiveCredentialsFieldNames"
-)
+if TYPE_CHECKING:
+    from ..models.snowflake_credentials_start_of_week import SnowflakeCredentialsStartOfWeek
+
+
+T = TypeVar("T", bound="SnowflakeCredentials")
 
 
 @attr.s(auto_attribs=True)
-class PickCreateSnowflakeCredentialsExcludeKeyofCreateSnowflakeCredentialsSensitiveCredentialsFieldNames:
-    """From T, pick a set of properties whose keys are in the union K
+class SnowflakeCredentials:
+    """Construct a type with the properties of T except for those in type K.
 
     Attributes:
-        type (WarehouseTypesSNOWFLAKE):
+        type (SnowflakeCredentialsType):
         account (str):
         database (str):
         warehouse (str):
         schema (str):
         role (Union[Unset, str]):
         threads (Union[Unset, float]):
         client_session_keep_alive (Union[Unset, bool]):
         query_tag (Union[Unset, str]):
         access_url (Union[Unset, str]):
-        start_of_week (Union[Unset, None, WeekDay]):
+        start_of_week (Union[Unset, None, SnowflakeCredentialsStartOfWeek]):
     """
 
-    type: WarehouseTypesSNOWFLAKE
+    type: SnowflakeCredentialsType
     account: str
     database: str
     warehouse: str
     schema: str
     role: Union[Unset, str] = UNSET
     threads: Union[Unset, float] = UNSET
     client_session_keep_alive: Union[Unset, bool] = UNSET
     query_tag: Union[Unset, str] = UNSET
     access_url: Union[Unset, str] = UNSET
-    start_of_week: Union[Unset, None, WeekDay] = UNSET
+    start_of_week: Union[Unset, None, "SnowflakeCredentialsStartOfWeek"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         account = self.account
         database = self.database
         warehouse = self.warehouse
         schema = self.schema
         role = self.role
         threads = self.threads
         client_session_keep_alive = self.client_session_keep_alive
         query_tag = self.query_tag
         access_url = self.access_url
-        start_of_week: Union[Unset, None, int] = UNSET
+        start_of_week: Union[Unset, None, Dict[str, Any]] = UNSET
         if not isinstance(self.start_of_week, Unset):
-            start_of_week = self.start_of_week.value if self.start_of_week else None
+            start_of_week = self.start_of_week.to_dict() if self.start_of_week else None
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "type": type,
                 "account": account,
@@ -88,16 +90,18 @@
         if start_of_week is not UNSET:
             field_dict["startOfWeek"] = start_of_week
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.snowflake_credentials_start_of_week import SnowflakeCredentialsStartOfWeek
+
         d = src_dict.copy()
-        type = WarehouseTypesSNOWFLAKE(d.pop("type"))
+        type = SnowflakeCredentialsType(d.pop("type"))
 
         account = d.pop("account")
 
         database = d.pop("database")
 
         warehouse = d.pop("warehouse")
 
@@ -110,40 +114,38 @@
         client_session_keep_alive = d.pop("clientSessionKeepAlive", UNSET)
 
         query_tag = d.pop("queryTag", UNSET)
 
         access_url = d.pop("accessUrl", UNSET)
 
         _start_of_week = d.pop("startOfWeek", UNSET)
-        start_of_week: Union[Unset, None, WeekDay]
+        start_of_week: Union[Unset, None, SnowflakeCredentialsStartOfWeek]
         if _start_of_week is None:
             start_of_week = None
         elif isinstance(_start_of_week, Unset):
             start_of_week = UNSET
         else:
-            start_of_week = WeekDay(_start_of_week)
+            start_of_week = SnowflakeCredentialsStartOfWeek.from_dict(_start_of_week)
 
-        pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names = cls(
+        snowflake_credentials = cls(
             type=type,
             account=account,
             database=database,
             warehouse=warehouse,
             schema=schema,
             role=role,
             threads=threads,
             client_session_keep_alive=client_session_keep_alive,
             query_tag=query_tag,
             access_url=access_url,
             start_of_week=start_of_week,
         )
 
-        pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.additional_properties = (
-            d
-        )
-        return pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names
+        snowflake_credentials.additional_properties = d
+        return snowflake_credentials
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.621.0/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,66 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Type
+from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 
-from ..models.warehouse_types_trino import WarehouseTypesTRINO
-from ..models.week_day import WeekDay
+from ..models.omit_create_trino_credentials_sensitive_credentials_field_names_type import (
+    OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesType,
+)
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="PickCreateTrinoCredentialsExcludeKeyofCreateTrinoCredentialsSensitiveCredentialsFieldNames")
+if TYPE_CHECKING:
+    from ..models.omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week import (
+        OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
+    )
+
+
+T = TypeVar("T", bound="OmitCreateTrinoCredentialsSensitiveCredentialsFieldNames")
 
 
 @attr.s(auto_attribs=True)
-class PickCreateTrinoCredentialsExcludeKeyofCreateTrinoCredentialsSensitiveCredentialsFieldNames:
-    """From T, pick a set of properties whose keys are in the union K
+class OmitCreateTrinoCredentialsSensitiveCredentialsFieldNames:
+    """Construct a type with the properties of T except for those in type K.
 
     Attributes:
-        type (WarehouseTypesTRINO):
+        type (OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesType):
         schema (str):
         host (str):
         port (float):
         dbname (str):
         http_scheme (str):
-        start_of_week (Union[Unset, None, WeekDay]):
+        start_of_week (Union[Unset, None, OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesStartOfWeek]):
     """
 
-    type: WarehouseTypesTRINO
+    type: OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesType
     schema: str
     host: str
     port: float
     dbname: str
     http_scheme: str
-    start_of_week: Union[Unset, None, WeekDay] = UNSET
+    start_of_week: Union[Unset, None, "OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesStartOfWeek"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         type = self.type.value
 
         schema = self.schema
         host = self.host
         port = self.port
         dbname = self.dbname
         http_scheme = self.http_scheme
-        start_of_week: Union[Unset, None, int] = UNSET
+        start_of_week: Union[Unset, None, Dict[str, Any]] = UNSET
         if not isinstance(self.start_of_week, Unset):
-            start_of_week = self.start_of_week.value if self.start_of_week else None
+            start_of_week = self.start_of_week.to_dict() if self.start_of_week else None
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "type": type,
                 "schema": schema,
@@ -65,50 +73,54 @@
         if start_of_week is not UNSET:
             field_dict["startOfWeek"] = start_of_week
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week import (
+            OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesStartOfWeek,
+        )
+
         d = src_dict.copy()
-        type = WarehouseTypesTRINO(d.pop("type"))
+        type = OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesType(d.pop("type"))
 
         schema = d.pop("schema")
 
         host = d.pop("host")
 
         port = d.pop("port")
 
         dbname = d.pop("dbname")
 
         http_scheme = d.pop("http_scheme")
 
         _start_of_week = d.pop("startOfWeek", UNSET)
-        start_of_week: Union[Unset, None, WeekDay]
+        start_of_week: Union[Unset, None, OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesStartOfWeek]
         if _start_of_week is None:
             start_of_week = None
         elif isinstance(_start_of_week, Unset):
             start_of_week = UNSET
         else:
-            start_of_week = WeekDay(_start_of_week)
+            start_of_week = OmitCreateTrinoCredentialsSensitiveCredentialsFieldNamesStartOfWeek.from_dict(
+                _start_of_week
+            )
 
-        pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names = cls(
+        omit_create_trino_credentials_sensitive_credentials_field_names = cls(
             type=type,
             schema=schema,
             host=host,
             port=port,
             dbname=dbname,
             http_scheme=http_scheme,
             start_of_week=start_of_week,
         )
 
-        pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.additional_properties = (
-            d
-        )
-        return pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names
+        omit_create_trino_credentials_sensitive_credentials_field_names.additional_properties = d
+        return omit_create_trino_credentials_sensitive_credentials_field_names
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.621.0/lightdash_client/models/space_dashboard.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,54 +12,53 @@
 import attr
 from dateutil.parser import isoparse
 
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.updated_by_user import UpdatedByUser
+    from ..models.space_dashboard_updated_by_user import SpaceDashboardUpdatedByUser
+    from ..models.space_dashboard_validation_errors_item import SpaceDashboardValidationErrorsItem
 
 
-T = TypeVar(
-    "T",
-    bound="PickDashboardUuidOrNameOrDescriptionOrUpdatedAtOrProjectUuidOrUpdatedByUserOrOrganizationUuidOrSpaceUuidOrViewsOrFirstViewedAtOrPinnedListUuidOrPinnedListOrder",
-)
+T = TypeVar("T", bound="SpaceDashboard")
 
 
 @attr.s(auto_attribs=True)
-class PickDashboardUuidOrNameOrDescriptionOrUpdatedAtOrProjectUuidOrUpdatedByUserOrOrganizationUuidOrSpaceUuidOrViewsOrFirstViewedAtOrPinnedListUuidOrPinnedListOrder:
-    """From T, pick a set of properties whose keys are in the union K
-
+class SpaceDashboard:
+    """
     Attributes:
         name (str):
         organization_uuid (str):
         uuid (str):
         updated_at (datetime.datetime):
         project_uuid (str):
         space_uuid (str):
         views (float):
         description (Union[Unset, str]):
-        updated_by_user (Union[Unset, UpdatedByUser]):
+        updated_by_user (Union[Unset, SpaceDashboardUpdatedByUser]):
         first_viewed_at (Union[None, datetime.datetime, str]):
         pinned_list_uuid (Optional[str]):
         pinned_list_order (Optional[float]):
+        validation_errors (Union[Unset, List['SpaceDashboardValidationErrorsItem']]):
     """
 
     name: str
     organization_uuid: str
     uuid: str
     updated_at: datetime.datetime
     project_uuid: str
     space_uuid: str
     views: float
     first_viewed_at: Union[None, datetime.datetime, str]
     pinned_list_uuid: Optional[str]
     pinned_list_order: Optional[float]
     description: Union[Unset, str] = UNSET
-    updated_by_user: Union[Unset, "UpdatedByUser"] = UNSET
+    updated_by_user: Union[Unset, "SpaceDashboardUpdatedByUser"] = UNSET
+    validation_errors: Union[Unset, List["SpaceDashboardValidationErrorsItem"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
         organization_uuid = self.organization_uuid
         uuid = self.uuid
         updated_at = self.updated_at.isoformat()
@@ -80,14 +79,21 @@
             first_viewed_at = self.first_viewed_at.isoformat()
 
         else:
             first_viewed_at = self.first_viewed_at
 
         pinned_list_uuid = self.pinned_list_uuid
         pinned_list_order = self.pinned_list_order
+        validation_errors: Union[Unset, List[Dict[str, Any]]] = UNSET
+        if not isinstance(self.validation_errors, Unset):
+            validation_errors = []
+            for validation_errors_item_data in self.validation_errors:
+                validation_errors_item = validation_errors_item_data.to_dict()
+
+                validation_errors.append(validation_errors_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "name": name,
                 "organizationUuid": organization_uuid,
@@ -101,20 +107,23 @@
                 "pinnedListOrder": pinned_list_order,
             }
         )
         if description is not UNSET:
             field_dict["description"] = description
         if updated_by_user is not UNSET:
             field_dict["updatedByUser"] = updated_by_user
+        if validation_errors is not UNSET:
+            field_dict["validationErrors"] = validation_errors
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.updated_by_user import UpdatedByUser
+        from ..models.space_dashboard_updated_by_user import SpaceDashboardUpdatedByUser
+        from ..models.space_dashboard_validation_errors_item import SpaceDashboardValidationErrorsItem
 
         d = src_dict.copy()
         name = d.pop("name")
 
         organization_uuid = d.pop("organizationUuid")
 
         uuid = d.pop("uuid")
@@ -126,19 +135,19 @@
         space_uuid = d.pop("spaceUuid")
 
         views = d.pop("views")
 
         description = d.pop("description", UNSET)
 
         _updated_by_user = d.pop("updatedByUser", UNSET)
-        updated_by_user: Union[Unset, UpdatedByUser]
+        updated_by_user: Union[Unset, SpaceDashboardUpdatedByUser]
         if isinstance(_updated_by_user, Unset):
             updated_by_user = UNSET
         else:
-            updated_by_user = UpdatedByUser.from_dict(_updated_by_user)
+            updated_by_user = SpaceDashboardUpdatedByUser.from_dict(_updated_by_user)
 
         def _parse_first_viewed_at(data: object) -> Union[None, datetime.datetime, str]:
             if data is None:
                 return data
             try:
                 if not isinstance(data, str):
                     raise TypeError()
@@ -151,33 +160,39 @@
 
         first_viewed_at = _parse_first_viewed_at(d.pop("firstViewedAt"))
 
         pinned_list_uuid = d.pop("pinnedListUuid")
 
         pinned_list_order = d.pop("pinnedListOrder")
 
-        pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order = cls(
+        validation_errors = []
+        _validation_errors = d.pop("validationErrors", UNSET)
+        for validation_errors_item_data in _validation_errors or []:
+            validation_errors_item = SpaceDashboardValidationErrorsItem.from_dict(validation_errors_item_data)
+
+            validation_errors.append(validation_errors_item)
+
+        space_dashboard = cls(
             name=name,
             organization_uuid=organization_uuid,
             uuid=uuid,
             updated_at=updated_at,
             project_uuid=project_uuid,
             space_uuid=space_uuid,
             views=views,
             description=description,
             updated_by_user=updated_by_user,
             first_viewed_at=first_viewed_at,
             pinned_list_uuid=pinned_list_uuid,
             pinned_list_order=pinned_list_order,
+            validation_errors=validation_errors,
         )
 
-        pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.additional_properties = (
-            d
-        )
-        return pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order
+        space_dashboard.additional_properties = d
+        return space_dashboard
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_group_name.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_organization_name.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_organization_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.621.0/lightdash_client/models/api_pinned_items_results_item_type_2_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,132 +1,125 @@
-import datetime
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
-from dateutil.parser import isoparse
 
-from ..types import UNSET
-from ..types import Unset
-
-if TYPE_CHECKING:
-    from ..models.updated_by_user import UpdatedByUser
-
-
-T = TypeVar(
-    "T",
-    bound="PickSavedChartUuidOrNameOrUpdatedAtOrUpdatedByUserOrDescriptionOrSpaceUuidOrPinnedListUuidOrPinnedListOrder",
-)
+T = TypeVar("T", bound="ApiPinnedItemsResultsItemType2Data")
 
 
 @attr.s(auto_attribs=True)
-class PickSavedChartUuidOrNameOrUpdatedAtOrUpdatedByUserOrDescriptionOrSpaceUuidOrPinnedListUuidOrPinnedListOrder:
-    """From T, pick a set of properties whose keys are in the union K
-
+class ApiPinnedItemsResultsItemType2Data:
+    """
     Attributes:
         name (str):
+        organization_uuid (str):
         uuid (str):
-        updated_at (datetime.datetime):
-        space_uuid (str):
-        description (Union[Unset, str]):
-        updated_by_user (Union[Unset, UpdatedByUser]):
+        project_uuid (str):
+        is_private (bool):
+        chart_count (float):
+        dashboard_count (float):
+        access_list_length (float):
+        access (List[str]):
         pinned_list_uuid (Optional[str]):
         pinned_list_order (Optional[float]):
     """
 
     name: str
+    organization_uuid: str
     uuid: str
-    updated_at: datetime.datetime
-    space_uuid: str
+    project_uuid: str
+    is_private: bool
+    chart_count: float
+    dashboard_count: float
+    access_list_length: float
+    access: List[str]
     pinned_list_uuid: Optional[str]
     pinned_list_order: Optional[float]
-    description: Union[Unset, str] = UNSET
-    updated_by_user: Union[Unset, "UpdatedByUser"] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         name = self.name
+        organization_uuid = self.organization_uuid
         uuid = self.uuid
-        updated_at = self.updated_at.isoformat()
-
-        space_uuid = self.space_uuid
-        description = self.description
-        updated_by_user: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.updated_by_user, Unset):
-            updated_by_user = self.updated_by_user.to_dict()
+        project_uuid = self.project_uuid
+        is_private = self.is_private
+        chart_count = self.chart_count
+        dashboard_count = self.dashboard_count
+        access_list_length = self.access_list_length
+        access = self.access
 
         pinned_list_uuid = self.pinned_list_uuid
         pinned_list_order = self.pinned_list_order
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "name": name,
+                "organizationUuid": organization_uuid,
                 "uuid": uuid,
-                "updatedAt": updated_at,
-                "spaceUuid": space_uuid,
+                "projectUuid": project_uuid,
+                "isPrivate": is_private,
+                "chartCount": chart_count,
+                "dashboardCount": dashboard_count,
+                "accessListLength": access_list_length,
+                "access": access,
                 "pinnedListUuid": pinned_list_uuid,
                 "pinnedListOrder": pinned_list_order,
             }
         )
-        if description is not UNSET:
-            field_dict["description"] = description
-        if updated_by_user is not UNSET:
-            field_dict["updatedByUser"] = updated_by_user
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.updated_by_user import UpdatedByUser
-
         d = src_dict.copy()
         name = d.pop("name")
 
+        organization_uuid = d.pop("organizationUuid")
+
         uuid = d.pop("uuid")
 
-        updated_at = isoparse(d.pop("updatedAt"))
+        project_uuid = d.pop("projectUuid")
+
+        is_private = d.pop("isPrivate")
 
-        space_uuid = d.pop("spaceUuid")
+        chart_count = d.pop("chartCount")
 
-        description = d.pop("description", UNSET)
+        dashboard_count = d.pop("dashboardCount")
 
-        _updated_by_user = d.pop("updatedByUser", UNSET)
-        updated_by_user: Union[Unset, UpdatedByUser]
-        if isinstance(_updated_by_user, Unset):
-            updated_by_user = UNSET
-        else:
-            updated_by_user = UpdatedByUser.from_dict(_updated_by_user)
+        access_list_length = d.pop("accessListLength")
+
+        access = cast(List[str], d.pop("access"))
 
         pinned_list_uuid = d.pop("pinnedListUuid")
 
         pinned_list_order = d.pop("pinnedListOrder")
 
-        pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order = cls(
+        api_pinned_items_results_item_type_2_data = cls(
             name=name,
+            organization_uuid=organization_uuid,
             uuid=uuid,
-            updated_at=updated_at,
-            space_uuid=space_uuid,
-            description=description,
-            updated_by_user=updated_by_user,
+            project_uuid=project_uuid,
+            is_private=is_private,
+            chart_count=chart_count,
+            dashboard_count=dashboard_count,
+            access_list_length=access_list_length,
+            access=access,
             pinned_list_uuid=pinned_list_uuid,
             pinned_list_order=pinned_list_order,
         )
 
-        pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.additional_properties = (
-            d
-        )
-        return pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order
+        api_pinned_items_results_item_type_2_data.additional_properties = d
+        return api_pinned_items_results_item_type_2_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_share_url_path_or_params.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_share_url_path_or_params.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_name.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_space_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_name_or_is_private.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_space_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_space_share_user_uuid.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_space_share_user_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_ssh_key_pair_public_key.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_ssh_key_pair_public_key.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py` & `lightdash_client_python-0.621.0/lightdash_client/models/validation_response_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,110 +5,117 @@
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.validation_error_type import ValidationErrorType
-from ..models.validation_source_type import ValidationSourceType
+from ..models.validation_response_base_error_type import ValidationResponseBaseErrorType
+from ..models.validation_response_base_source import ValidationResponseBaseSource
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="PickValidationResponseBaseExcludeKeyofValidationResponseBaseName")
+T = TypeVar("T", bound="ValidationResponseBase")
 
 
 @attr.s(auto_attribs=True)
-class PickValidationResponseBaseExcludeKeyofValidationResponseBaseName:
-    """From T, pick a set of properties whose keys are in the union K
-
+class ValidationResponseBase:
+    """
     Attributes:
         project_uuid (str):
-        validation_id (float):
-        created_at (datetime.datetime):
+        error_type (ValidationResponseBaseErrorType):
         error (str):
-        error_type (ValidationErrorType):
+        name (str):
+        created_at (datetime.datetime):
+        validation_id (float):
+        source (Union[Unset, ValidationResponseBaseSource]):
         space_uuid (Union[Unset, str]):
-        source (Union[Unset, ValidationSourceType]):
     """
 
     project_uuid: str
-    validation_id: float
-    created_at: datetime.datetime
+    error_type: ValidationResponseBaseErrorType
     error: str
-    error_type: ValidationErrorType
+    name: str
+    created_at: datetime.datetime
+    validation_id: float
+    source: Union[Unset, ValidationResponseBaseSource] = UNSET
     space_uuid: Union[Unset, str] = UNSET
-    source: Union[Unset, ValidationSourceType] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project_uuid = self.project_uuid
-        validation_id = self.validation_id
-        created_at = self.created_at.isoformat()
+        error_type = self.error_type.value
 
         error = self.error
-        error_type = self.error_type.value
+        name = self.name
+        created_at = self.created_at.isoformat()
 
-        space_uuid = self.space_uuid
+        validation_id = self.validation_id
         source: Union[Unset, str] = UNSET
         if not isinstance(self.source, Unset):
             source = self.source.value
 
+        space_uuid = self.space_uuid
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "projectUuid": project_uuid,
-                "validationId": validation_id,
-                "createdAt": created_at,
-                "error": error,
                 "errorType": error_type,
+                "error": error,
+                "name": name,
+                "createdAt": created_at,
+                "validationId": validation_id,
             }
         )
-        if space_uuid is not UNSET:
-            field_dict["spaceUuid"] = space_uuid
         if source is not UNSET:
             field_dict["source"] = source
+        if space_uuid is not UNSET:
+            field_dict["spaceUuid"] = space_uuid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         project_uuid = d.pop("projectUuid")
 
-        validation_id = d.pop("validationId")
-
-        created_at = isoparse(d.pop("createdAt"))
+        error_type = ValidationResponseBaseErrorType(d.pop("errorType"))
 
         error = d.pop("error")
 
-        error_type = ValidationErrorType(d.pop("errorType"))
+        name = d.pop("name")
 
-        space_uuid = d.pop("spaceUuid", UNSET)
+        created_at = isoparse(d.pop("createdAt"))
+
+        validation_id = d.pop("validationId")
 
         _source = d.pop("source", UNSET)
-        source: Union[Unset, ValidationSourceType]
+        source: Union[Unset, ValidationResponseBaseSource]
         if isinstance(_source, Unset):
             source = UNSET
         else:
-            source = ValidationSourceType(_source)
+            source = ValidationResponseBaseSource(_source)
+
+        space_uuid = d.pop("spaceUuid", UNSET)
 
-        pick_validation_response_base_exclude_keyof_validation_response_base_name = cls(
+        validation_response_base = cls(
             project_uuid=project_uuid,
-            validation_id=validation_id,
-            created_at=created_at,
-            error=error,
             error_type=error_type,
-            space_uuid=space_uuid,
+            error=error,
+            name=name,
+            created_at=created_at,
+            validation_id=validation_id,
             source=source,
+            space_uuid=space_uuid,
         )
 
-        pick_validation_response_base_exclude_keyof_validation_response_base_name.additional_properties = d
-        return pick_validation_response_base_exclude_keyof_validation_response_base_name
+        validation_response_base.additional_properties = d
+        return validation_response_base
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py` & `lightdash_client_python-0.621.0/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/post_chart_results_json_body.py` & `lightdash_client_python-0.621.0/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,61 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..types import UNSET
-from ..types import Unset
-
-if TYPE_CHECKING:
-    from ..models.filters import Filters
-
-
-T = TypeVar("T", bound="PostChartResultsJsonBody")
+T = TypeVar("T", bound="PostChartResultsResponse200ResultsMetricQueryFiltersMetricsType0")
 
 
 @attr.s(auto_attribs=True)
-class PostChartResultsJsonBody:
+class PostChartResultsResponse200ResultsMetricQueryFiltersMetricsType0:
     """
     Attributes:
-        filters (Union[Unset, Filters]):
+        or_ (List[Any]):
+        id (str):
     """
 
-    filters: Union[Unset, "Filters"] = UNSET
+    or_: List[Any]
+    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        filters: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.filters, Unset):
-            filters = self.filters.to_dict()
+        or_ = self.or_
+
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if filters is not UNSET:
-            field_dict["filters"] = filters
+        field_dict.update(
+            {
+                "or": or_,
+                "id": id,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.filters import Filters
-
         d = src_dict.copy()
-        _filters = d.pop("filters", UNSET)
-        filters: Union[Unset, Filters]
-        if isinstance(_filters, Unset):
-            filters = UNSET
-        else:
-            filters = Filters.from_dict(_filters)
+        or_ = cast(List[Any], d.pop("or"))
+
+        id = d.pop("id")
 
-        post_chart_results_json_body = cls(
-            filters=filters,
+        post_chart_results_response_200_results_metric_query_filters_metrics_type_0 = cls(
+            or_=or_,
+            id=id,
         )
 
-        post_chart_results_json_body.additional_properties = d
-        return post_chart_results_json_body
+        post_chart_results_response_200_results_metric_query_filters_metrics_type_0.additional_properties = d
+        return post_chart_results_response_200_results_metric_query_filters_metrics_type_0
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/project_member_profile.py` & `lightdash_client_python-0.621.0/lightdash_client/models/project_member_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.project_member_role import ProjectMemberRole
+from ..models.project_member_profile_role import ProjectMemberProfileRole
 
 T = TypeVar("T", bound="ProjectMemberProfile")
 
 
 @attr.s(auto_attribs=True)
 class ProjectMemberProfile:
     """
     Attributes:
         last_name (str):
         first_name (str):
         email (str):
-        role (ProjectMemberRole):
+        role (ProjectMemberProfileRole):
         project_uuid (str):
         user_uuid (str):
     """
 
     last_name: str
     first_name: str
     email: str
-    role: ProjectMemberRole
+    role: ProjectMemberProfileRole
     project_uuid: str
     user_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         last_name = self.last_name
         first_name = self.first_name
@@ -60,15 +60,15 @@
         d = src_dict.copy()
         last_name = d.pop("lastName")
 
         first_name = d.pop("firstName")
 
         email = d.pop("email")
 
-        role = ProjectMemberRole(d.pop("role"))
+        role = ProjectMemberProfileRole(d.pop("role"))
 
         project_uuid = d.pop("projectUuid")
 
         user_uuid = d.pop("userUuid")
 
         project_member_profile = cls(
             last_name=last_name,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/record_string_any.py` & `lightdash_client_python-0.621.0/lightdash_client/models/record_string_any.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/resource_view_space_item.py` & `lightdash_client_python-0.621.0/lightdash_client/models/resource_view_space_item.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 from typing import List
 from typing import Type
 from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
-from ..models.resource_view_item_type_space import ResourceViewItemTypeSPACE
+from ..models.resource_view_space_item_type import ResourceViewSpaceItemType
 
 if TYPE_CHECKING:
     from ..models.resource_view_space_item_data import ResourceViewSpaceItemData
 
 
 T = TypeVar("T", bound="ResourceViewSpaceItem")
 
 
 @attr.s(auto_attribs=True)
 class ResourceViewSpaceItem:
     """
     Attributes:
         data (ResourceViewSpaceItemData):
-        type (ResourceViewItemTypeSPACE):
+        type (ResourceViewSpaceItemType):
     """
 
     data: "ResourceViewSpaceItemData"
-    type: ResourceViewItemTypeSPACE
+    type: ResourceViewSpaceItemType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = self.data.to_dict()
 
         type = self.type.value
 
@@ -47,15 +47,15 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.resource_view_space_item_data import ResourceViewSpaceItemData
 
         d = src_dict.copy()
         data = ResourceViewSpaceItemData.from_dict(d.pop("data"))
 
-        type = ResourceViewItemTypeSPACE(d.pop("type"))
+        type = ResourceViewSpaceItemType(d.pop("type"))
 
         resource_view_space_item = cls(
             data=data,
             type=type,
         )
 
         resource_view_space_item.additional_properties = d
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/resource_view_space_item_data.py` & `lightdash_client_python-0.621.0/lightdash_client/models/resource_view_space_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/run_query_request.py` & `lightdash_client_python-0.621.0/lightdash_client/models/run_query_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,45 +9,45 @@
 
 import attr
 
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.additional_metric import AdditionalMetric
+    from ..models.run_query_request_additional_metrics_item import RunQueryRequestAdditionalMetricsItem
     from ..models.run_query_request_filters import RunQueryRequestFilters
-    from ..models.sort_field import SortField
-    from ..models.table_calculation import TableCalculation
+    from ..models.run_query_request_sorts_item import RunQueryRequestSortsItem
+    from ..models.run_query_request_table_calculations_item import RunQueryRequestTableCalculationsItem
 
 
 T = TypeVar("T", bound="RunQueryRequest")
 
 
 @attr.s(auto_attribs=True)
 class RunQueryRequest:
     """
     Attributes:
-        table_calculations (List['TableCalculation']):
+        table_calculations (List['RunQueryRequestTableCalculationsItem']):
         limit (float):
-        sorts (List['SortField']):
+        sorts (List['RunQueryRequestSortsItem']):
         filters (RunQueryRequestFilters):
         metrics (List[str]):
         dimensions (List[str]):
         csv_limit (Union[Unset, float]):
-        additional_metrics (Union[Unset, List['AdditionalMetric']]):
+        additional_metrics (Union[Unset, List['RunQueryRequestAdditionalMetricsItem']]):
     """
 
-    table_calculations: List["TableCalculation"]
+    table_calculations: List["RunQueryRequestTableCalculationsItem"]
     limit: float
-    sorts: List["SortField"]
+    sorts: List["RunQueryRequestSortsItem"]
     filters: "RunQueryRequestFilters"
     metrics: List[str]
     dimensions: List[str]
     csv_limit: Union[Unset, float] = UNSET
-    additional_metrics: Union[Unset, List["AdditionalMetric"]] = UNSET
+    additional_metrics: Union[Unset, List["RunQueryRequestAdditionalMetricsItem"]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         table_calculations = []
         for table_calculations_item_data in self.table_calculations:
             table_calculations_item = table_calculations_item_data.to_dict()
 
@@ -92,48 +92,48 @@
         if additional_metrics is not UNSET:
             field_dict["additionalMetrics"] = additional_metrics
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.additional_metric import AdditionalMetric
+        from ..models.run_query_request_additional_metrics_item import RunQueryRequestAdditionalMetricsItem
         from ..models.run_query_request_filters import RunQueryRequestFilters
-        from ..models.sort_field import SortField
-        from ..models.table_calculation import TableCalculation
+        from ..models.run_query_request_sorts_item import RunQueryRequestSortsItem
+        from ..models.run_query_request_table_calculations_item import RunQueryRequestTableCalculationsItem
 
         d = src_dict.copy()
         table_calculations = []
         _table_calculations = d.pop("tableCalculations")
         for table_calculations_item_data in _table_calculations:
-            table_calculations_item = TableCalculation.from_dict(table_calculations_item_data)
+            table_calculations_item = RunQueryRequestTableCalculationsItem.from_dict(table_calculations_item_data)
 
             table_calculations.append(table_calculations_item)
 
         limit = d.pop("limit")
 
         sorts = []
         _sorts = d.pop("sorts")
         for sorts_item_data in _sorts:
-            sorts_item = SortField.from_dict(sorts_item_data)
+            sorts_item = RunQueryRequestSortsItem.from_dict(sorts_item_data)
 
             sorts.append(sorts_item)
 
         filters = RunQueryRequestFilters.from_dict(d.pop("filters"))
 
         metrics = cast(List[str], d.pop("metrics"))
 
         dimensions = cast(List[str], d.pop("dimensions"))
 
         csv_limit = d.pop("csvLimit", UNSET)
 
         additional_metrics = []
         _additional_metrics = d.pop("additionalMetrics", UNSET)
         for additional_metrics_item_data in _additional_metrics or []:
-            additional_metrics_item = AdditionalMetric.from_dict(additional_metrics_item_data)
+            additional_metrics_item = RunQueryRequestAdditionalMetricsItem.from_dict(additional_metrics_item_data)
 
             additional_metrics.append(additional_metrics_item)
 
         run_query_request = cls(
             table_calculations=table_calculations,
             limit=limit,
             sorts=sorts,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/run_query_request_filters.py` & `lightdash_client_python-0.621.0/lightdash_client/models/run_query_request_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/scheduled_jobs.py` & `lightdash_client_python-0.621.0/lightdash_client/models/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_base.py` & `lightdash_client_python-0.621.0/lightdash_client/models/scheduler_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,58 +7,58 @@
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.scheduler_format import SchedulerFormat
+from ..models.scheduler_base_format import SchedulerBaseFormat
 
 if TYPE_CHECKING:
-    from ..models.scheduler_csv_options import SchedulerCsvOptions
-    from ..models.scheduler_image_options import SchedulerImageOptions
+    from ..models.scheduler_base_options_type_0 import SchedulerBaseOptionsType0
+    from ..models.scheduler_base_options_type_1 import SchedulerBaseOptionsType1
 
 
 T = TypeVar("T", bound="SchedulerBase")
 
 
 @attr.s(auto_attribs=True)
 class SchedulerBase:
     """
     Attributes:
-        options (Union['SchedulerCsvOptions', 'SchedulerImageOptions']):
+        options (Union['SchedulerBaseOptionsType0', 'SchedulerBaseOptionsType1']):
         cron (str):
-        format_ (SchedulerFormat):
+        format_ (SchedulerBaseFormat):
         created_by (str):
         updated_at (datetime.datetime):
         created_at (datetime.datetime):
         name (str):
         scheduler_uuid (str):
         dashboard_uuid (Optional[str]):
         saved_chart_uuid (Optional[str]):
     """
 
-    options: Union["SchedulerCsvOptions", "SchedulerImageOptions"]
+    options: Union["SchedulerBaseOptionsType0", "SchedulerBaseOptionsType1"]
     cron: str
-    format_: SchedulerFormat
+    format_: SchedulerBaseFormat
     created_by: str
     updated_at: datetime.datetime
     created_at: datetime.datetime
     name: str
     scheduler_uuid: str
     dashboard_uuid: Optional[str]
     saved_chart_uuid: Optional[str]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.scheduler_csv_options import SchedulerCsvOptions
+        from ..models.scheduler_base_options_type_0 import SchedulerBaseOptionsType0
 
         options: Dict[str, Any]
 
-        if isinstance(self.options, SchedulerCsvOptions):
+        if isinstance(self.options, SchedulerBaseOptionsType0):
             options = self.options.to_dict()
 
         else:
             options = self.options.to_dict()
 
         cron = self.cron
         format_ = self.format_.value
@@ -90,39 +90,39 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.scheduler_csv_options import SchedulerCsvOptions
-        from ..models.scheduler_image_options import SchedulerImageOptions
+        from ..models.scheduler_base_options_type_0 import SchedulerBaseOptionsType0
+        from ..models.scheduler_base_options_type_1 import SchedulerBaseOptionsType1
 
         d = src_dict.copy()
 
-        def _parse_options(data: object) -> Union["SchedulerCsvOptions", "SchedulerImageOptions"]:
+        def _parse_options(data: object) -> Union["SchedulerBaseOptionsType0", "SchedulerBaseOptionsType1"]:
             try:
                 if not isinstance(data, dict):
                     raise TypeError()
-                componentsschemas_scheduler_options_type_0 = SchedulerCsvOptions.from_dict(data)
+                options_type_0 = SchedulerBaseOptionsType0.from_dict(data)
 
-                return componentsschemas_scheduler_options_type_0
+                return options_type_0
             except:  # noqa: E722
                 pass
             if not isinstance(data, dict):
                 raise TypeError()
-            componentsschemas_scheduler_options_type_1 = SchedulerImageOptions.from_dict(data)
+            options_type_1 = SchedulerBaseOptionsType1.from_dict(data)
 
-            return componentsschemas_scheduler_options_type_1
+            return options_type_1
 
         options = _parse_options(d.pop("options"))
 
         cron = d.pop("cron")
 
-        format_ = SchedulerFormat(d.pop("format"))
+        format_ = SchedulerBaseFormat(d.pop("format"))
 
         created_by = d.pop("createdBy")
 
         updated_at = isoparse(d.pop("updatedAt"))
 
         created_at = isoparse(d.pop("createdAt"))
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_csv_options.py` & `lightdash_client_python-0.621.0/lightdash_client/models/scheduler_csv_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_email_target.py` & `lightdash_client_python-0.621.0/lightdash_client/models/scheduler_email_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_image_options.py` & `lightdash_client_python-0.621.0/lightdash_client/models/scheduler_image_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_log.py` & `lightdash_client_python-0.621.0/lightdash_client/models/scheduler_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,49 +6,49 @@
 from typing import TYPE_CHECKING
 from typing import TypeVar
 from typing import Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.scheduler_job_status import SchedulerJobStatus
+from ..models.scheduler_log_status import SchedulerLogStatus
 from ..models.scheduler_log_target_type import SchedulerLogTargetType
 from ..models.scheduler_log_task import SchedulerLogTask
 from ..types import UNSET
 from ..types import Unset
 
 if TYPE_CHECKING:
-    from ..models.record_string_any import RecordStringAny
+    from ..models.scheduler_log_details import SchedulerLogDetails
 
 
 T = TypeVar("T", bound="SchedulerLog")
 
 
 @attr.s(auto_attribs=True)
 class SchedulerLog:
     """
     Attributes:
-        status (SchedulerJobStatus):
+        status (SchedulerLogStatus):
         created_at (datetime.datetime):
         scheduled_time (datetime.datetime):
         job_id (str):
         task (SchedulerLogTask):
-        details (Union[Unset, RecordStringAny]): Construct a type with a set of properties K of type T
+        details (Union[Unset, SchedulerLogDetails]): Construct a type with a set of properties K of type T
         target_type (Union[Unset, SchedulerLogTargetType]):
         target (Union[Unset, str]):
         job_group (Union[Unset, str]):
         scheduler_uuid (Union[Unset, str]):
     """
 
-    status: SchedulerJobStatus
+    status: SchedulerLogStatus
     created_at: datetime.datetime
     scheduled_time: datetime.datetime
     job_id: str
     task: SchedulerLogTask
-    details: Union[Unset, "RecordStringAny"] = UNSET
+    details: Union[Unset, "SchedulerLogDetails"] = UNSET
     target_type: Union[Unset, SchedulerLogTargetType] = UNSET
     target: Union[Unset, str] = UNSET
     job_group: Union[Unset, str] = UNSET
     scheduler_uuid: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
@@ -95,33 +95,33 @@
         if scheduler_uuid is not UNSET:
             field_dict["schedulerUuid"] = scheduler_uuid
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.record_string_any import RecordStringAny
+        from ..models.scheduler_log_details import SchedulerLogDetails
 
         d = src_dict.copy()
-        status = SchedulerJobStatus(d.pop("status"))
+        status = SchedulerLogStatus(d.pop("status"))
 
         created_at = isoparse(d.pop("createdAt"))
 
         scheduled_time = isoparse(d.pop("scheduledTime"))
 
         job_id = d.pop("jobId")
 
         task = SchedulerLogTask(d.pop("task"))
 
         _details = d.pop("details", UNSET)
-        details: Union[Unset, RecordStringAny]
+        details: Union[Unset, SchedulerLogDetails]
         if isinstance(_details, Unset):
             details = UNSET
         else:
-            details = RecordStringAny.from_dict(_details)
+            details = SchedulerLogDetails.from_dict(_details)
 
         _target_type = d.pop("targetType", UNSET)
         target_type: Union[Unset, SchedulerLogTargetType]
         if isinstance(_target_type, Unset):
             target_type = UNSET
         else:
             target_type = SchedulerLogTargetType(_target_type)
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/scheduler_slack_target.py` & `lightdash_client_python-0.621.0/lightdash_client/models/scheduler_slack_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/share_url.py` & `lightdash_client_python-0.621.0/lightdash_client/models/share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/slack_channel.py` & `lightdash_client_python-0.621.0/lightdash_client/models/slack_channel.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/sort_field.py` & `lightdash_client_python-0.621.0/lightdash_client/models/sort_field.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/space_share.py` & `lightdash_client_python-0.621.0/lightdash_client/models/create_space_in_project_json_body_access_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.project_member_role import ProjectMemberRole
+from ..models.create_space_in_project_json_body_access_item_role import CreateSpaceInProjectJsonBodyAccessItemRole
 
-T = TypeVar("T", bound="SpaceShare")
+T = TypeVar("T", bound="CreateSpaceInProjectJsonBodyAccessItem")
 
 
 @attr.s(auto_attribs=True)
-class SpaceShare:
+class CreateSpaceInProjectJsonBodyAccessItem:
     """
     Attributes:
-        role (ProjectMemberRole):
+        role (CreateSpaceInProjectJsonBodyAccessItemRole):
         last_name (str):
         first_name (str):
         user_uuid (str):
     """
 
-    role: ProjectMemberRole
+    role: CreateSpaceInProjectJsonBodyAccessItemRole
     last_name: str
     first_name: str
     user_uuid: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         role = self.role.value
@@ -46,31 +46,31 @@
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        role = ProjectMemberRole(d.pop("role"))
+        role = CreateSpaceInProjectJsonBodyAccessItemRole(d.pop("role"))
 
         last_name = d.pop("lastName")
 
         first_name = d.pop("firstName")
 
         user_uuid = d.pop("userUuid")
 
-        space_share = cls(
+        create_space_in_project_json_body_access_item = cls(
             role=role,
             last_name=last_name,
             first_name=first_name,
             user_uuid=user_uuid,
         )
 
-        space_share.additional_properties = d
-        return space_share
+        create_space_in_project_json_body_access_item.additional_properties = d
+        return create_space_in_project_json_body_access_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/space_summary.py` & `lightdash_client_python-0.621.0/lightdash_client/models/space_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/table_calculation.py` & `lightdash_client_python-0.621.0/lightdash_client/models/metric_query_response_filters_metrics_type_1.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,61 @@
 from typing import Any
+from typing import cast
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
-from typing import Union
 
 import attr
 
-from ..types import UNSET
-from ..types import Unset
-
-T = TypeVar("T", bound="TableCalculation")
+T = TypeVar("T", bound="MetricQueryResponseFiltersMetricsType1")
 
 
 @attr.s(auto_attribs=True)
-class TableCalculation:
+class MetricQueryResponseFiltersMetricsType1:
     """
     Attributes:
-        sql (str):
-        display_name (str):
-        name (str):
-        index (Union[Unset, float]):
+        and_ (List[Any]):
+        id (str):
     """
 
-    sql: str
-    display_name: str
-    name: str
-    index: Union[Unset, float] = UNSET
+    and_: List[Any]
+    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        sql = self.sql
-        display_name = self.display_name
-        name = self.name
-        index = self.index
+        and_ = self.and_
+
+        id = self.id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "sql": sql,
-                "displayName": display_name,
-                "name": name,
+                "and": and_,
+                "id": id,
             }
         )
-        if index is not UNSET:
-            field_dict["index"] = index
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        sql = d.pop("sql")
-
-        display_name = d.pop("displayName")
-
-        name = d.pop("name")
+        and_ = cast(List[Any], d.pop("and"))
 
-        index = d.pop("index", UNSET)
+        id = d.pop("id")
 
-        table_calculation = cls(
-            sql=sql,
-            display_name=display_name,
-            name=name,
-            index=index,
+        metric_query_response_filters_metrics_type_1 = cls(
+            and_=and_,
+            id=id,
         )
 
-        table_calculation.additional_properties = d
-        return table_calculation
+        metric_query_response_filters_metrics_type_1.additional_properties = d
+        return metric_query_response_filters_metrics_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/update_pinned_item_order.py` & `lightdash_client_python-0.621.0/lightdash_client/models/update_pinned_item_order_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,74 +1,61 @@
 from typing import Any
 from typing import Dict
 from typing import List
+from typing import Optional
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 
 import attr
 
-from ..models.resource_view_item_type import ResourceViewItemType
-
-if TYPE_CHECKING:
-    from ..models.pick_resource_view_item_at_data_uuid_or_pinned_list_order import (
-        PickResourceViewItemAtDataUuidOrPinnedListOrder,
-    )
-
-
-T = TypeVar("T", bound="UpdatePinnedItemOrder")
+T = TypeVar("T", bound="UpdatePinnedItemOrderData")
 
 
 @attr.s(auto_attribs=True)
-class UpdatePinnedItemOrder:
-    """
+class UpdatePinnedItemOrderData:
+    """From T, pick a set of properties whose keys are in the union K
+
     Attributes:
-        data (PickResourceViewItemAtDataUuidOrPinnedListOrder): From T, pick a set of properties whose keys are in the
-            union K
-        type (ResourceViewItemType):
+        uuid (str):
+        pinned_list_order (Optional[float]):
     """
 
-    data: "PickResourceViewItemAtDataUuidOrPinnedListOrder"
-    type: ResourceViewItemType
+    uuid: str
+    pinned_list_order: Optional[float]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        data = self.data.to_dict()
-
-        type = self.type.value
+        uuid = self.uuid
+        pinned_list_order = self.pinned_list_order
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "data": data,
-                "type": type,
+                "uuid": uuid,
+                "pinnedListOrder": pinned_list_order,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.pick_resource_view_item_at_data_uuid_or_pinned_list_order import (
-            PickResourceViewItemAtDataUuidOrPinnedListOrder,
-        )
-
         d = src_dict.copy()
-        data = PickResourceViewItemAtDataUuidOrPinnedListOrder.from_dict(d.pop("data"))
+        uuid = d.pop("uuid")
 
-        type = ResourceViewItemType(d.pop("type"))
+        pinned_list_order = d.pop("pinnedListOrder")
 
-        update_pinned_item_order = cls(
-            data=data,
-            type=type,
+        update_pinned_item_order_data = cls(
+            uuid=uuid,
+            pinned_list_order=pinned_list_order,
         )
 
-        update_pinned_item_order.additional_properties = d
-        return update_pinned_item_order
+        update_pinned_item_order_data.additional_properties = d
+        return update_pinned_item_order_data
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/update_project_member.py` & `lightdash_client_python-0.621.0/lightdash_client/models/update_project_member.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 from typing import Dict
 from typing import List
 from typing import Type
 from typing import TypeVar
 
 import attr
 
-from ..models.project_member_role import ProjectMemberRole
+from ..models.update_project_member_role import UpdateProjectMemberRole
 
 T = TypeVar("T", bound="UpdateProjectMember")
 
 
 @attr.s(auto_attribs=True)
 class UpdateProjectMember:
     """
     Attributes:
-        role (ProjectMemberRole):
+        role (UpdateProjectMemberRole):
     """
 
-    role: ProjectMemberRole
+    role: UpdateProjectMemberRole
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         role = self.role.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
@@ -33,15 +33,15 @@
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        role = ProjectMemberRole(d.pop("role"))
+        role = UpdateProjectMemberRole(d.pop("role"))
 
         update_project_member = cls(
             role=role,
         )
 
         update_project_member.additional_properties = d
         return update_project_member
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/updated_by_user.py` & `lightdash_client_python-0.621.0/lightdash_client/models/updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/user_allowed_organization.py` & `lightdash_client_python-0.621.0/lightdash_client/models/user_allowed_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/validate_project_json_body.py` & `lightdash_client_python-0.621.0/lightdash_client/models/validate_project_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/validation_error_chart_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/validation_error_chart_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,58 +5,58 @@
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.chart_kind import ChartKind
-from ..models.validation_error_type import ValidationErrorType
-from ..models.validation_source_type import ValidationSourceType
+from ..models.validation_error_chart_response_chart_type import ValidationErrorChartResponseChartType
+from ..models.validation_error_chart_response_error_type import ValidationErrorChartResponseErrorType
+from ..models.validation_error_chart_response_source import ValidationErrorChartResponseSource
 from ..types import UNSET
 from ..types import Unset
 
 T = TypeVar("T", bound="ValidationErrorChartResponse")
 
 
 @attr.s(auto_attribs=True)
 class ValidationErrorChartResponse:
     """
     Attributes:
         project_uuid (str):
-        error_type (ValidationErrorType):
+        error_type (ValidationErrorChartResponseErrorType):
         error (str):
         name (str):
         created_at (datetime.datetime):
         validation_id (float):
         chart_views (float):
-        source (Union[Unset, ValidationSourceType]):
+        source (Union[Unset, ValidationErrorChartResponseSource]):
         space_uuid (Union[Unset, str]):
         chart_name (Union[Unset, str]):
         last_updated_at (Union[Unset, datetime.datetime]):
         last_updated_by (Union[Unset, str]):
         field_name (Union[Unset, str]):
-        chart_type (Union[Unset, ChartKind]):
+        chart_type (Union[Unset, ValidationErrorChartResponseChartType]):
         chart_uuid (Union[Unset, str]):
     """
 
     project_uuid: str
-    error_type: ValidationErrorType
+    error_type: ValidationErrorChartResponseErrorType
     error: str
     name: str
     created_at: datetime.datetime
     validation_id: float
     chart_views: float
-    source: Union[Unset, ValidationSourceType] = UNSET
+    source: Union[Unset, ValidationErrorChartResponseSource] = UNSET
     space_uuid: Union[Unset, str] = UNSET
     chart_name: Union[Unset, str] = UNSET
     last_updated_at: Union[Unset, datetime.datetime] = UNSET
     last_updated_by: Union[Unset, str] = UNSET
     field_name: Union[Unset, str] = UNSET
-    chart_type: Union[Unset, ChartKind] = UNSET
+    chart_type: Union[Unset, ValidationErrorChartResponseChartType] = UNSET
     chart_uuid: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project_uuid = self.project_uuid
         error_type = self.error_type.value
 
@@ -117,32 +117,32 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         project_uuid = d.pop("projectUuid")
 
-        error_type = ValidationErrorType(d.pop("errorType"))
+        error_type = ValidationErrorChartResponseErrorType(d.pop("errorType"))
 
         error = d.pop("error")
 
         name = d.pop("name")
 
         created_at = isoparse(d.pop("createdAt"))
 
         validation_id = d.pop("validationId")
 
         chart_views = d.pop("chartViews")
 
         _source = d.pop("source", UNSET)
-        source: Union[Unset, ValidationSourceType]
+        source: Union[Unset, ValidationErrorChartResponseSource]
         if isinstance(_source, Unset):
             source = UNSET
         else:
-            source = ValidationSourceType(_source)
+            source = ValidationErrorChartResponseSource(_source)
 
         space_uuid = d.pop("spaceUuid", UNSET)
 
         chart_name = d.pop("chartName", UNSET)
 
         _last_updated_at = d.pop("lastUpdatedAt", UNSET)
         last_updated_at: Union[Unset, datetime.datetime]
@@ -152,19 +152,19 @@
             last_updated_at = isoparse(_last_updated_at)
 
         last_updated_by = d.pop("lastUpdatedBy", UNSET)
 
         field_name = d.pop("fieldName", UNSET)
 
         _chart_type = d.pop("chartType", UNSET)
-        chart_type: Union[Unset, ChartKind]
+        chart_type: Union[Unset, ValidationErrorChartResponseChartType]
         if isinstance(_chart_type, Unset):
             chart_type = UNSET
         else:
-            chart_type = ChartKind(_chart_type)
+            chart_type = ValidationErrorChartResponseChartType(_chart_type)
 
         chart_uuid = d.pop("chartUuid", UNSET)
 
         validation_error_chart_response = cls(
             project_uuid=project_uuid,
             error_type=error_type,
             error=error,
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/validation_error_dashboard_response.py` & `lightdash_client_python-0.621.0/lightdash_client/models/validation_response_type_1.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,50 +5,50 @@
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.validation_error_type import ValidationErrorType
-from ..models.validation_source_type import ValidationSourceType
+from ..models.validation_response_type_1_error_type import ValidationResponseType1ErrorType
+from ..models.validation_response_type_1_source import ValidationResponseType1Source
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="ValidationErrorDashboardResponse")
+T = TypeVar("T", bound="ValidationResponseType1")
 
 
 @attr.s(auto_attribs=True)
-class ValidationErrorDashboardResponse:
+class ValidationResponseType1:
     """
     Attributes:
         project_uuid (str):
-        error_type (ValidationErrorType):
+        error_type (ValidationResponseType1ErrorType):
         error (str):
         name (str):
         created_at (datetime.datetime):
         validation_id (float):
         dashboard_views (float):
-        source (Union[Unset, ValidationSourceType]):
+        source (Union[Unset, ValidationResponseType1Source]):
         space_uuid (Union[Unset, str]):
         last_updated_at (Union[Unset, datetime.datetime]):
         last_updated_by (Union[Unset, str]):
         field_name (Union[Unset, str]):
         chart_name (Union[Unset, str]):
         dashboard_uuid (Union[Unset, str]):
     """
 
     project_uuid: str
-    error_type: ValidationErrorType
+    error_type: ValidationResponseType1ErrorType
     error: str
     name: str
     created_at: datetime.datetime
     validation_id: float
     dashboard_views: float
-    source: Union[Unset, ValidationSourceType] = UNSET
+    source: Union[Unset, ValidationResponseType1Source] = UNSET
     space_uuid: Union[Unset, str] = UNSET
     last_updated_at: Union[Unset, datetime.datetime] = UNSET
     last_updated_by: Union[Unset, str] = UNSET
     field_name: Union[Unset, str] = UNSET
     chart_name: Union[Unset, str] = UNSET
     dashboard_uuid: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
@@ -108,32 +108,32 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         project_uuid = d.pop("projectUuid")
 
-        error_type = ValidationErrorType(d.pop("errorType"))
+        error_type = ValidationResponseType1ErrorType(d.pop("errorType"))
 
         error = d.pop("error")
 
         name = d.pop("name")
 
         created_at = isoparse(d.pop("createdAt"))
 
         validation_id = d.pop("validationId")
 
         dashboard_views = d.pop("dashboardViews")
 
         _source = d.pop("source", UNSET)
-        source: Union[Unset, ValidationSourceType]
+        source: Union[Unset, ValidationResponseType1Source]
         if isinstance(_source, Unset):
             source = UNSET
         else:
-            source = ValidationSourceType(_source)
+            source = ValidationResponseType1Source(_source)
 
         space_uuid = d.pop("spaceUuid", UNSET)
 
         _last_updated_at = d.pop("lastUpdatedAt", UNSET)
         last_updated_at: Union[Unset, datetime.datetime]
         if isinstance(_last_updated_at, Unset):
             last_updated_at = UNSET
@@ -144,15 +144,15 @@
 
         field_name = d.pop("fieldName", UNSET)
 
         chart_name = d.pop("chartName", UNSET)
 
         dashboard_uuid = d.pop("dashboardUuid", UNSET)
 
-        validation_error_dashboard_response = cls(
+        validation_response_type_1 = cls(
             project_uuid=project_uuid,
             error_type=error_type,
             error=error,
             name=name,
             created_at=created_at,
             validation_id=validation_id,
             dashboard_views=dashboard_views,
@@ -161,16 +161,16 @@
             last_updated_at=last_updated_at,
             last_updated_by=last_updated_by,
             field_name=field_name,
             chart_name=chart_name,
             dashboard_uuid=dashboard_uuid,
         )
 
-        validation_error_dashboard_response.additional_properties = d
-        return validation_error_dashboard_response
+        validation_response_type_1.additional_properties = d
+        return validation_response_type_1
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/validation_response_base.py` & `lightdash_client_python-0.621.0/lightdash_client/models/validation_error_table_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,117 +5,118 @@
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
 import attr
 from dateutil.parser import isoparse
 
-from ..models.validation_error_type import ValidationErrorType
-from ..models.validation_source_type import ValidationSourceType
+from ..models.validation_error_table_response_error_type import ValidationErrorTableResponseErrorType
+from ..models.validation_error_table_response_source import ValidationErrorTableResponseSource
 from ..types import UNSET
 from ..types import Unset
 
-T = TypeVar("T", bound="ValidationResponseBase")
+T = TypeVar("T", bound="ValidationErrorTableResponse")
 
 
 @attr.s(auto_attribs=True)
-class ValidationResponseBase:
+class ValidationErrorTableResponse:
     """
     Attributes:
         project_uuid (str):
-        error_type (ValidationErrorType):
-        error (str):
-        name (str):
-        created_at (datetime.datetime):
         validation_id (float):
-        source (Union[Unset, ValidationSourceType]):
+        created_at (datetime.datetime):
+        error (str):
+        error_type (ValidationErrorTableResponseErrorType):
         space_uuid (Union[Unset, str]):
+        source (Union[Unset, ValidationErrorTableResponseSource]):
+        name (Union[Unset, str]):
     """
 
     project_uuid: str
-    error_type: ValidationErrorType
-    error: str
-    name: str
-    created_at: datetime.datetime
     validation_id: float
-    source: Union[Unset, ValidationSourceType] = UNSET
+    created_at: datetime.datetime
+    error: str
+    error_type: ValidationErrorTableResponseErrorType
     space_uuid: Union[Unset, str] = UNSET
+    source: Union[Unset, ValidationErrorTableResponseSource] = UNSET
+    name: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project_uuid = self.project_uuid
-        error_type = self.error_type.value
+        validation_id = self.validation_id
+        created_at = self.created_at.isoformat()
 
         error = self.error
-        name = self.name
-        created_at = self.created_at.isoformat()
+        error_type = self.error_type.value
 
-        validation_id = self.validation_id
+        space_uuid = self.space_uuid
         source: Union[Unset, str] = UNSET
         if not isinstance(self.source, Unset):
             source = self.source.value
 
-        space_uuid = self.space_uuid
+        name = self.name
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "projectUuid": project_uuid,
-                "errorType": error_type,
-                "error": error,
-                "name": name,
-                "createdAt": created_at,
                 "validationId": validation_id,
+                "createdAt": created_at,
+                "error": error,
+                "errorType": error_type,
             }
         )
-        if source is not UNSET:
-            field_dict["source"] = source
         if space_uuid is not UNSET:
             field_dict["spaceUuid"] = space_uuid
+        if source is not UNSET:
+            field_dict["source"] = source
+        if name is not UNSET:
+            field_dict["name"] = name
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         project_uuid = d.pop("projectUuid")
 
-        error_type = ValidationErrorType(d.pop("errorType"))
+        validation_id = d.pop("validationId")
+
+        created_at = isoparse(d.pop("createdAt"))
 
         error = d.pop("error")
 
-        name = d.pop("name")
-
-        created_at = isoparse(d.pop("createdAt"))
+        error_type = ValidationErrorTableResponseErrorType(d.pop("errorType"))
 
-        validation_id = d.pop("validationId")
+        space_uuid = d.pop("spaceUuid", UNSET)
 
         _source = d.pop("source", UNSET)
-        source: Union[Unset, ValidationSourceType]
+        source: Union[Unset, ValidationErrorTableResponseSource]
         if isinstance(_source, Unset):
             source = UNSET
         else:
-            source = ValidationSourceType(_source)
+            source = ValidationErrorTableResponseSource(_source)
 
-        space_uuid = d.pop("spaceUuid", UNSET)
+        name = d.pop("name", UNSET)
 
-        validation_response_base = cls(
+        validation_error_table_response = cls(
             project_uuid=project_uuid,
-            error_type=error_type,
-            error=error,
-            name=name,
-            created_at=created_at,
             validation_id=validation_id,
-            source=source,
+            created_at=created_at,
+            error=error,
+            error_type=error_type,
             space_uuid=space_uuid,
+            source=source,
+            name=name,
         )
 
-        validation_response_base.additional_properties = d
-        return validation_response_base
+        validation_error_table_response.additional_properties = d
+        return validation_error_table_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `lightdash_client_python-0.619.1/lightdash_client/models/view_statistics.py` & `lightdash_client_python-0.621.0/lightdash_client/models/view_statistics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/lightdash_client/types.py` & `lightdash_client_python-0.621.0/lightdash_client/types.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/pyproject.toml` & `lightdash_client_python-0.621.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/setup.py` & `lightdash_client_python-0.621.0/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/tests/__init__.py` & `lightdash_client_python-0.621.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/tests/test_dummy.py` & `lightdash_client_python-0.621.0/tests/test_dummy.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.619.1/PKG-INFO` & `lightdash_client_python-0.621.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-client-python
-Version: 0.619.1
+Version: 0.621.0
 Summary: A client library for accessing Lightdash API 
 Author: yu-iskw
 Requires-Python: >=3.8.0,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

