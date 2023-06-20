# Comparing `tmp/gencove-2.5.0.tar.gz` & `tmp/gencove-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gencove-2.5.0.tar", last modified: Fri Jun 16 14:34:43 2023, max compression
+gzip compressed data, was "dist/gencove-2.5.1.tar", last modified: Tue Jun 20 17:40:45 2023, max compression
```

## Comparing `gencove-2.5.0.tar` & `gencove-2.5.1.tar`

### file list

```diff
@@ -1,301 +1,301 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-06-16 14:34:43.000000 gencove-2.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2085 2023-06-16 14:34:08.000000 gencove-2.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    32627 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6009 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       92 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2398 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/autoimports/create/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/biosamples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2212 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/biosamples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/projects/
--rw-rw-rw-   0 root         (0) root         (0)       86 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2031 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      235 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2151 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/basespace_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/basespace/projects/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/common_cli_options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/download/
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2104 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    14731 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/main.py
--rw-rw-rw-   0 root         (0) root         (0)    10579 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/download/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/files/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/files/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/files/main.py
--rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/files/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1682 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1439 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/create_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/create_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1316 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/create_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/create_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      687 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/create_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/delete_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/delete_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/delete_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/delete_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/get_batch/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/get_batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/get_batch/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/get_batch/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/get_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/get_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/get_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/get_merged_vcf/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2191 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      442 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/import_existing_samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      469 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2859 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      688 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/main.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batch_types/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list_batches/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list_batches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batches/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2182 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batches/main.py
--rw-rw-rw-   0 root         (0) root         (0)      499 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_batches/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1668 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/main.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/main.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/list_pipelines/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/restore_samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/restore_samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/restore_samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1823 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/restore_samples/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/run_prefix/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/run_prefix/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1953 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/run_prefix/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/run_prefix/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4918 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/run_prefix/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1603 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/samples/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/samples/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2454 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/samples/main.py
--rw-rw-rw-   0 root         (0) root         (0)      735 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/samples/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      705 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1813 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/main.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/projects/status_merged_vcf/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2314 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/autoimports/create/main.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1434 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/s3_imports/s3_import/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/samples/
--rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/samples/download_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/samples/download_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2911 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/download_file/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/download_file/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     4930 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/download_file/main.py
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/download_file/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/samples/get_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/samples/get_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/get_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     2348 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/get_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/samples/set_metadata/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/samples/set_metadata/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/set_metadata/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1981 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/samples/set_metadata/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/upload/
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    16788 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/main.py
--rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/multi_file_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     8819 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/upload/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/uploads/
--rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/uploads/list/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/uploads/list/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/list/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/list/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/list/main.py
--rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/uploads/list/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/webhook/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/webhook/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/command/webhook/verify/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/command/webhook/verify/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/webhook/verify/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      999 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/command/webhook/verify/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3731 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/description/
--rw-rw-rw-   0 root         (0) root         (0)     1811 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/description/pypi_readme.md
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3205 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/logger.py
--rw-rw-rw-   0 root         (0) root         (0)     7984 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/basespace/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/basespace/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6374 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4249 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7257 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_biosamples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6334 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_projects_import.py
--rw-rw-rw-   0 root         (0) root         (0)     5955 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/basespace/test_basespace_projects_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/basespace/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/basespace/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3328 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/download/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/download/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    36754 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/download/test_cli_download.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/download/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/download/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/download/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/files/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/files/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4371 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/files/test_file_types_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/files/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/files/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4519 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/projects/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/projects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6781 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_batch_get.py
--rw-rw-rw-   0 root         (0) root         (0)     4502 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_batch_types_list.py
--rw-rw-rw-   0 root         (0) root         (0)     8945 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_batches_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4601 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_batches_list.py
--rw-rw-rw-   0 root         (0) root         (0)     4380 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_create.py
--rw-rw-rw-   0 root         (0) root         (0)     9108 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_create_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     8901 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_delete_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    12016 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_get_merged_vcf.py
--rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_import_existing_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    10605 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6511 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
--rw-rw-rw-   0 root         (0) root         (0)     3899 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_pipelines_list.py
--rw-rw-rw-   0 root         (0) root         (0)     7212 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_restore_samples.py
--rw-rw-rw-   0 root         (0) root         (0)    13390 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_run_prefix.py
--rw-rw-rw-   0 root         (0) root         (0)     7184 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_samples_list.py
--rw-rw-rw-   0 root         (0) root         (0)     6468 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/test_projects_status_merged_vcf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/projects/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/projects/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11910 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/projects/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/s3_imports/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/s3_imports/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6422 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/s3_imports/test_s3_autoimports_create.py
--rw-rw-rw-   0 root         (0) root         (0)     4163 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/s3_imports/test_s3_autoimports_list.py
--rw-rw-rw-   0 root         (0) root         (0)     5269 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/s3_imports/test_s3_uri_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/s3_imports/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/s3_imports/vcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/samples/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/samples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8865 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/samples/test_samples_download_file.py
--rw-rw-rw-   0 root         (0) root         (0)     7024 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/samples/test_samples_get_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/samples/test_samples_set_metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/samples/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/samples/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/samples/vcr/filters.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/test_logger.py
--rw-rw-rw-   0 root         (0) root         (0)    22425 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/upload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/upload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    42140 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/upload/test_cli_upload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/upload/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/upload/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5281 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/upload/vcr/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/uploads/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/uploads/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4357 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/uploads/test_uploads_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/uploads/vcr/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/uploads/vcr/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      971 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/tests/webhook/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-16 14:34:09.000000 gencove-2.5.0/gencove/tests/webhook/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/tests/webhook/test_webhook_verify.py
--rw-rw-rw-   0 root         (0) root         (0)     5174 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove/version/
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/version/A-major
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/version/B-minor
--rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/version/C-patch
--rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-16 14:34:08.000000 gencove-2.5.0/gencove/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2387 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10251 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-16 14:34:43.000000 gencove-2.5.0/gencove.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-16 14:34:43.000000 gencove-2.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1866 2023-06-16 14:34:08.000000 gencove-2.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-06-20 17:40:45.000000 gencove-2.5.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2085 2023-06-20 17:40:11.000000 gencove-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    32627 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6009 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2398 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/autoimports/create/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/biosamples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/biosamples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/biosamples/biosamples_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/biosamples/biosamples_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/biosamples/biosamples_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2212 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/biosamples/biosamples_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      547 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/biosamples/biosamples_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/biosamples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      235 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2151 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      571 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/basespace_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      358 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/basespace/projects/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1548 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/common_cli_options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/download/
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4611 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/download/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2104 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/download/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/download/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    14731 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/download/main.py
+-rw-rw-rw-   0 root         (0) root         (0)    10579 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/download/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/files/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/files/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1888 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/files/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/files/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1682 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      793 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1439 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/create_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/create_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/create_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/delete_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/delete_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/delete_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1931 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/delete_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/get_batch/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/get_batch/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      936 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/get_batch/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2769 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/get_batch/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/get_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/get_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/get_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/get_merged_vcf/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/import_existing_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/import_existing_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/import_existing_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/import_existing_samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2191 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/import_existing_samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      442 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/import_existing_samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      469 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2859 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/list_batch_types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_batch_types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      688 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_batch_types/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2264 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_batch_types/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_batch_types/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/list_batches/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_batches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_batches/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_batches/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      499 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_batches/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/list_pipeline_capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_pipeline_capabilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_pipeline_capabilities/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_pipeline_capabilities/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_pipeline_capabilities/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/list_pipelines/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_pipelines/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_pipelines/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_pipelines/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/list_pipelines/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/restore_samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/restore_samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/restore_samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1823 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/restore_samples/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/run_prefix/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/run_prefix/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/run_prefix/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/run_prefix/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4918 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/run_prefix/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1603 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/samples/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/samples/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2454 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/samples/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/samples/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/projects/status_merged_vcf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/status_merged_vcf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      705 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/status_merged_vcf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1813 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/status_merged_vcf/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/projects/status_merged_vcf/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/autoimport_list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/autoimport_list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/autoimport_list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/autoimport_list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/autoimport_list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/create/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/create/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/create/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/create/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2314 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/autoimports/create/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/s3_imports/s3_import/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/s3_import/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1434 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/s3_import/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/s3_import/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/s3_imports/s3_import/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/samples/
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/samples/download_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/download_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2911 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/download_file/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/download_file/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     4930 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/download_file/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/download_file/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/samples/get_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/get_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/get_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     2348 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/get_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/samples/set_metadata/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/set_metadata/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      758 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/set_metadata/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/samples/set_metadata/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/upload/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2760 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/upload/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/upload/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/upload/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    17222 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/upload/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     3028 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/upload/multi_file_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     9443 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/upload/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/uploads/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/uploads/list/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/uploads/list/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/uploads/list/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      277 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/uploads/list/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/uploads/list/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      573 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/uploads/list/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3462 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/webhook/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/command/webhook/verify/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/webhook/verify/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1011 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/webhook/verify/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      999 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/command/webhook/verify/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3731 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/description/
+-rw-rw-rw-   0 root         (0) root         (0)     1811 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/description/pypi_readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3205 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/basespace/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/basespace/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6374 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/basespace/test_basespace_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4249 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/basespace/test_basespace_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7257 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/basespace/test_basespace_biosamples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6334 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/basespace/test_basespace_projects_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     5955 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/basespace/test_basespace_projects_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/basespace/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/basespace/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4675 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3328 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/download/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/download/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    36754 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/download/test_cli_download.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/download/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/download/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/download/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/files/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/files/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4371 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/files/test_file_types_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/files/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/files/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4519 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/projects/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_batch_get.py
+-rw-rw-rw-   0 root         (0) root         (0)     4502 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_batch_types_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     8945 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_batches_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4601 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_batches_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     4380 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     9108 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_create_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     8901 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_delete_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    12016 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_get_merged_vcf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6286 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_import_existing_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    10605 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6511 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_pipeline_capabilities_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     3899 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_pipelines_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     7212 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_restore_samples.py
+-rw-rw-rw-   0 root         (0) root         (0)    13390 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_run_prefix.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_samples_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     6468 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/test_projects_status_merged_vcf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/projects/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11910 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/projects/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/s3_imports/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/s3_imports/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/s3_imports/test_s3_autoimports_create.py
+-rw-rw-rw-   0 root         (0) root         (0)     4163 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/s3_imports/test_s3_autoimports_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     5269 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/s3_imports/test_s3_uri_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/s3_imports/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/s3_imports/vcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/samples/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/samples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8865 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/samples/test_samples_download_file.py
+-rw-rw-rw-   0 root         (0) root         (0)     7024 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/samples/test_samples_get_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/samples/test_samples_set_metadata.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/samples/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/samples/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/samples/vcr/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/test_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    24076 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/upload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/upload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    44376 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/upload/test_cli_upload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/upload/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/upload/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5281 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/upload/vcr/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/uploads/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/uploads/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4357 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/uploads/test_uploads_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/uploads/vcr/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/uploads/vcr/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      971 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/tests/webhook/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/webhook/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3430 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/tests/webhook/test_webhook_verify.py
+-rw-rw-rw-   0 root         (0) root         (0)     5174 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove/version/
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/version/A-major
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/version/B-minor
+-rw-rw-rw-   0 root         (0) root         (0)        2 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/version/C-patch
+-rw-rw-rw-   0 root         (0) root         (0)      400 2023-06-20 17:40:11.000000 gencove-2.5.1/gencove/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10251 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-20 17:40:45.000000 gencove-2.5.1/gencove.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-20 17:40:45.000000 gencove-2.5.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1866 2023-06-20 17:40:11.000000 gencove-2.5.1/setup.py
```

### Comparing `gencove-2.5.0/PKG-INFO` & `gencove-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.5.0
+Version: 2.5.1
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.5.0/README.md` & `gencove-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/cli.py` & `gencove-2.5.1/gencove/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/client.py` & `gencove-2.5.1/gencove/client.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/base.py` & `gencove-2.5.1/gencove/command/base.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/cli.py` & `gencove-2.5.1/gencove/command/basespace/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/main.py` & `gencove-2.5.1/gencove/command/basespace/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/autoimports/autoimport_list/utils.py` & `gencove-2.5.1/gencove/command/basespace/autoimports/autoimport_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/autoimports/create/cli.py` & `gencove-2.5.1/gencove/command/basespace/autoimports/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/autoimports/create/main.py` & `gencove-2.5.1/gencove/command/basespace/autoimports/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/cli.py` & `gencove-2.5.1/gencove/command/basespace/biosamples/biosamples_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/main.py` & `gencove-2.5.1/gencove/command/basespace/biosamples/biosamples_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/biosamples/biosamples_list/utils.py` & `gencove-2.5.1/gencove/command/basespace/biosamples/biosamples_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/projects/basespace_import/cli.py` & `gencove-2.5.1/gencove/command/basespace/projects/basespace_import/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/projects/basespace_import/main.py` & `gencove-2.5.1/gencove/command/basespace/projects/basespace_import/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/projects/basespace_list/cli.py` & `gencove-2.5.1/gencove/command/basespace/projects/basespace_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/projects/basespace_list/main.py` & `gencove-2.5.1/gencove/command/basespace/projects/basespace_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/basespace/projects/basespace_list/utils.py` & `gencove-2.5.1/gencove/command/basespace/projects/basespace_list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/common_cli_options.py` & `gencove-2.5.1/gencove/command/common_cli_options.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/download/cli.py` & `gencove-2.5.1/gencove/command/download/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/download/constants.py` & `gencove-2.5.1/gencove/command/download/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/download/main.py` & `gencove-2.5.1/gencove/command/download/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/download/utils.py` & `gencove-2.5.1/gencove/command/download/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/files/cli.py` & `gencove-2.5.1/gencove/command/files/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/files/main.py` & `gencove-2.5.1/gencove/command/files/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/cli.py` & `gencove-2.5.1/gencove/command/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/create/cli.py` & `gencove-2.5.1/gencove/command/projects/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/create/main.py` & `gencove-2.5.1/gencove/command/projects/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/create_batch/cli.py` & `gencove-2.5.1/gencove/command/projects/create_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/create_batch/main.py` & `gencove-2.5.1/gencove/command/projects/create_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/create_merged_vcf/cli.py` & `gencove-2.5.1/gencove/command/projects/create_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/create_merged_vcf/main.py` & `gencove-2.5.1/gencove/command/projects/create_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/delete_samples/cli.py` & `gencove-2.5.1/gencove/command/projects/delete_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/delete_samples/main.py` & `gencove-2.5.1/gencove/command/projects/delete_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/get_batch/cli.py` & `gencove-2.5.1/gencove/command/projects/get_batch/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/get_batch/main.py` & `gencove-2.5.1/gencove/command/projects/get_batch/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/get_merged_vcf/cli.py` & `gencove-2.5.1/gencove/command/projects/get_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/get_merged_vcf/main.py` & `gencove-2.5.1/gencove/command/projects/get_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/import_existing_samples/cli.py` & `gencove-2.5.1/gencove/command/projects/import_existing_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/import_existing_samples/main.py` & `gencove-2.5.1/gencove/command/projects/import_existing_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list/main.py` & `gencove-2.5.1/gencove/command/projects/list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list/utils.py` & `gencove-2.5.1/gencove/command/projects/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list_batch_types/cli.py` & `gencove-2.5.1/gencove/command/projects/list_batch_types/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list_batch_types/main.py` & `gencove-2.5.1/gencove/command/projects/list_batch_types/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list_batches/cli.py` & `gencove-2.5.1/gencove/command/projects/list_batches/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list_batches/main.py` & `gencove-2.5.1/gencove/command/projects/list_batches/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/cli.py` & `gencove-2.5.1/gencove/command/projects/list_pipeline_capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list_pipeline_capabilities/main.py` & `gencove-2.5.1/gencove/command/projects/list_pipeline_capabilities/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list_pipelines/cli.py` & `gencove-2.5.1/gencove/command/projects/list_pipelines/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/list_pipelines/main.py` & `gencove-2.5.1/gencove/command/projects/list_pipelines/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/restore_samples/cli.py` & `gencove-2.5.1/gencove/command/projects/restore_samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/restore_samples/main.py` & `gencove-2.5.1/gencove/command/projects/restore_samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/run_prefix/cli.py` & `gencove-2.5.1/gencove/command/projects/run_prefix/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/run_prefix/main.py` & `gencove-2.5.1/gencove/command/projects/run_prefix/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/samples/cli.py` & `gencove-2.5.1/gencove/command/projects/samples/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/samples/main.py` & `gencove-2.5.1/gencove/command/projects/samples/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/samples/utils.py` & `gencove-2.5.1/gencove/command/projects/samples/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/status_merged_vcf/cli.py` & `gencove-2.5.1/gencove/command/projects/status_merged_vcf/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/projects/status_merged_vcf/main.py` & `gencove-2.5.1/gencove/command/projects/status_merged_vcf/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/cli.py` & `gencove-2.5.1/gencove/command/s3_imports/autoimports/autoimport_list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/s3_imports/autoimports/autoimport_list/main.py` & `gencove-2.5.1/gencove/command/s3_imports/autoimports/autoimport_list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/s3_imports/autoimports/create/cli.py` & `gencove-2.5.1/gencove/command/s3_imports/autoimports/create/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/s3_imports/autoimports/create/main.py` & `gencove-2.5.1/gencove/command/s3_imports/autoimports/create/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/s3_imports/s3_import/cli.py` & `gencove-2.5.1/gencove/command/s3_imports/s3_import/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/s3_imports/s3_import/main.py` & `gencove-2.5.1/gencove/command/s3_imports/s3_import/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/samples/download_file/cli.py` & `gencove-2.5.1/gencove/command/samples/download_file/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/samples/download_file/main.py` & `gencove-2.5.1/gencove/command/samples/download_file/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/samples/download_file/utils.py` & `gencove-2.5.1/gencove/command/samples/download_file/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/samples/get_metadata/cli.py` & `gencove-2.5.1/gencove/command/samples/get_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/samples/get_metadata/main.py` & `gencove-2.5.1/gencove/command/samples/get_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/samples/set_metadata/cli.py` & `gencove-2.5.1/gencove/command/samples/set_metadata/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/samples/set_metadata/main.py` & `gencove-2.5.1/gencove/command/samples/set_metadata/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/upload/cli.py` & `gencove-2.5.1/gencove/command/upload/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/upload/constants.py` & `gencove-2.5.1/gencove/command/upload/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/upload/main.py` & `gencove-2.5.1/gencove/command/upload/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,38 +64,47 @@
         self.upload_ids = set()
         self.output = output
         self.assigned_samples = []
         self.no_progress = no_progress
         self.metadata = options.metadata
 
     @staticmethod
-    def generate_gncv_destination():
+    def generate_gncv_destination(fastq_source: str = "cli"):
         """Autogenerate gencove destination path."""
         return (
-            f"{UPLOAD_PREFIX}cli-"
+            f"{UPLOAD_PREFIX}{fastq_source}-"
             f"{datetime.utcnow().strftime('%Y%m%d%H%M%S')}-"
             f"{uuid.uuid4().hex}"
         )
 
+    @staticmethod
+    def map_paths_are_urls(fastq_map: dict) -> bool:
+        """If all path values for fastq_map look like URLs,
+        return True, otherwise False"""
+        return all(looks_like_url(next(iter(path))) for path in fastq_map.values())
+
     def initialize(self):
         """Initialize upload command parameters from provided arguments."""
         self.echo_debug(f"Host is {self.options.host}")
         self.echo_warning(TMP_UPLOADS_WARNING)
 
         # fmt: off
+        fastqs_source = "cli"
         if os.path.isfile(self.source) and self.source.endswith(FASTQ_MAP_EXTENSION):  # noqa: E501  # pylint: disable=line-too-long
             self.echo_debug("Scanning fastqs map file")
             self.fastqs_map = parse_fastqs_map_file(self.source)
+            if self.map_paths_are_urls(self.fastqs_map):
+                fastqs_source = "cli-url"
             self.echo_debug(f"got fastq pairs: {self.fastqs_map}")
         else:
             self.echo_debug("Seeking files to upload")
             self.fastqs = list(seek_files_to_upload(self.source))
 
         if not self.destination:
-            self.destination = self.generate_gncv_destination()
+            self.destination = self.generate_gncv_destination(fastqs_source)
             self.echo_info(
                 f"Files will be uploaded to: {self.destination}"
             )
         # fmt: on
 
         # Make sure there is just one trailing slash. Only exception is
         # UPLOAD_PREFIX itself, which can have two trailing slashes.
```

### Comparing `gencove-2.5.0/gencove/command/upload/multi_file_reader.py` & `gencove-2.5.1/gencove/command/upload/multi_file_reader.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/upload/utils.py` & `gencove-2.5.1/gencove/command/upload/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,14 +209,29 @@
     for column in FastQ.__fields__:
         if column not in header_columns:
             raise ValidationError(
                 f"Unexpected CSV header. Expected: {', '.join(FastQ.__fields__)}"
             )
 
 
+def _validate_parsed_map(fastqs: dict):
+    """Validates contents of fastqs dict to ensure path
+    column contains homogenous values, i.e. all local paths
+     or all URLs"""
+    paths = [next(iter(x)) for x in fastqs.values()]
+    all_urls = all(looks_like_url(p) for p in paths)
+    all_paths = all(not looks_like_url(p) for p in paths)
+    if not all_urls and not all_paths:
+        raise ValidationError(
+            "Detected both URLs and file paths in 'path' column. "
+            "Please only supply one type of path (URL or local path)"
+            " in the map file."
+        )
+
+
 def parse_fastqs_map_file(fastqs_map_path):
     """Parse fastq map file.
 
     Map file has to have following columns/headers:
         client_id, r_notation, path
 
     Note this map file also supports URLs under the path column
@@ -244,14 +259,15 @@
         _validate_header(header)
         for row in reader:
             fastq = FastQ(**row)
             _validate_fastq(fastq)
             fastqs[(fastq.client_id, R_NOTATION_MAP[fastq.r_notation])].append(
                 fastq.path
             )
+    _validate_parsed_map(fastqs)
     return fastqs
 
 
 def get_gncv_path(client_id, r_notation):
     """Build gncv upload path.
 
     Args:
```

### Comparing `gencove-2.5.0/gencove/command/uploads/list/cli.py` & `gencove-2.5.1/gencove/command/uploads/list/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/uploads/list/main.py` & `gencove-2.5.1/gencove/command/uploads/list/main.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/uploads/list/utils.py` & `gencove-2.5.1/gencove/command/uploads/list/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/utils.py` & `gencove-2.5.1/gencove/command/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/webhook/verify/cli.py` & `gencove-2.5.1/gencove/command/webhook/verify/cli.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/command/webhook/verify/utils.py` & `gencove-2.5.1/gencove/command/webhook/verify/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/constants.py` & `gencove-2.5.1/gencove/constants.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/description/pypi_readme.md` & `gencove-2.5.1/gencove/description/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/logger.py` & `gencove-2.5.1/gencove/logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/models.py` & `gencove-2.5.1/gencove/models.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/basespace/test_basespace_autoimports_create.py` & `gencove-2.5.1/gencove/tests/basespace/test_basespace_autoimports_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/basespace/test_basespace_autoimports_list.py` & `gencove-2.5.1/gencove/tests/basespace/test_basespace_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/basespace/test_basespace_biosamples_list.py` & `gencove-2.5.1/gencove/tests/basespace/test_basespace_biosamples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/basespace/test_basespace_projects_import.py` & `gencove-2.5.1/gencove/tests/basespace/test_basespace_projects_import.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/basespace/test_basespace_projects_list.py` & `gencove-2.5.1/gencove/tests/basespace/test_basespace_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/conftest.py` & `gencove-2.5.1/gencove/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/decorators.py` & `gencove-2.5.1/gencove/tests/decorators.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/download/test_cli_download.py` & `gencove-2.5.1/gencove/tests/download/test_cli_download.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/download/vcr/filters.py` & `gencove-2.5.1/gencove/tests/download/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/files/test_file_types_list.py` & `gencove-2.5.1/gencove/tests/files/test_file_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/filters.py` & `gencove-2.5.1/gencove/tests/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_batch_get.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_batch_get.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_batch_types_list.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_batch_types_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_batches_create.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_batches_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_batches_list.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_batches_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_create.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_create_merged_vcf.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_create_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_delete_samples.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_delete_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_get_merged_vcf.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_get_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_import_existing_samples.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_import_existing_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_list.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_pipeline_capabilities_list.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_pipeline_capabilities_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_pipelines_list.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_pipelines_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_restore_samples.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_restore_samples.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_run_prefix.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_run_prefix.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_samples_list.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_samples_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/test_projects_status_merged_vcf.py` & `gencove-2.5.1/gencove/tests/projects/test_projects_status_merged_vcf.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/projects/vcr/filters.py` & `gencove-2.5.1/gencove/tests/projects/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/s3_imports/test_s3_autoimports_create.py` & `gencove-2.5.1/gencove/tests/s3_imports/test_s3_autoimports_create.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/s3_imports/test_s3_autoimports_list.py` & `gencove-2.5.1/gencove/tests/s3_imports/test_s3_autoimports_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/s3_imports/test_s3_uri_import.py` & `gencove-2.5.1/gencove/tests/s3_imports/test_s3_uri_import.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/samples/test_samples_download_file.py` & `gencove-2.5.1/gencove/tests/samples/test_samples_download_file.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/samples/test_samples_get_metadata.py` & `gencove-2.5.1/gencove/tests/samples/test_samples_get_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/samples/test_samples_set_metadata.py` & `gencove-2.5.1/gencove/tests/samples/test_samples_set_metadata.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/samples/vcr/filters.py` & `gencove-2.5.1/gencove/tests/samples/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/test_logger.py` & `gencove-2.5.1/gencove/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/test_utils.py` & `gencove-2.5.1/gencove/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from gencove.command.download.utils import (
     _get_prefix_parts,
     build_file_path,
     get_download_template_format_params,
 )
 from gencove.command.upload.utils import (
     _validate_header,
+    _validate_parsed_map,
     looks_like_url,
     parse_fastqs_map_file,
     upload_file,
     valid_fastq_file_name_in_url,
 )
 from gencove.command.utils import is_valid_uuid, validate_uuid, validate_uuid_list
 from gencove.constants import (
@@ -324,48 +325,14 @@
         )
         assert (
             fastqs[("barid", "R1")][1]
             == "https://storage.googleapis.com/samples/2/R1.fastq.gz"
         )
 
 
-def test_parse_fastqs_map_file_with_urls_and_s3():
-    """Test parsing of map file with URLs into dict"""
-    runner = CliRunner()
-    fastq_file_path = "barid-R2.fastq.gz"
-    with runner.isolated_filesystem():
-        with open(fastq_file_path, "w", encoding="utf-8") as fastq_file:
-            fastq_file.write("AAABBB")
-
-        with open("test_url_map.fastq-map.csv", "w", encoding="utf-8") as map_file:
-            writer = csv.writer(map_file)
-            writer.writerows(
-                [
-                    ["client_id", "r_notation", "path"],
-                    [
-                        "barid",
-                        "r1",
-                        "https://s3.amazonaws.com/samples/1/barid-R1.fastq.gz",
-                    ],
-                    ["barid", "r2", fastq_file_path],
-                ]
-            )
-
-        fastqs = parse_fastqs_map_file("test_url_map.fastq-map.csv")
-        assert len(fastqs) == 2
-        assert ("barid", "R1") in fastqs
-        assert ("barid", "R2") in fastqs
-        assert len(fastqs[("barid", "R1")]) == 1
-        assert (
-            fastqs[("barid", "R1")][0]
-            == "https://s3.amazonaws.com/samples/1/barid-R1.fastq.gz"
-        )
-        assert fastqs[("barid", "R2")][0] == fastq_file_path
-
-
 def test_parse_fastqs_map_file_with_urls_invalid():
     """Test parsing of map file with URLs into dict, invalid URLs"""
     runner = CliRunner()
     with runner.isolated_filesystem():
         with open("test_url_map.fastq-map.csv", "w", encoding="utf-8") as map_file:
             writer = csv.writer(map_file)
             writer.writerows(
@@ -403,14 +370,83 @@
     assert _validate_header(header_row) is None
 
     # with uppercase
     header_row = dict(client_id="client_id", r_notation="R_notation", path="path")
     assert _validate_header(header_row) is None
 
 
+def test_validate_parsed_map__all_urls():
+    """Test validation of parsed map, all URLs OK"""
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        with open("test_url_map.fastq-map.csv", "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    ["url", "r1", "https://s3.amazonaws.com/samples/1/R1.fastq.gz"],
+                    ["url", "r2", "https://s3.amazonaws.com/samples/1/R2.fastq.gz"],
+                ]
+            )
+        fastqs = parse_fastqs_map_file("test_url_map.fastq-map.csv")
+    assert _validate_parsed_map(fastqs) is None
+
+
+def test_validate_parsed_map__all_paths():
+    """Test validation of parsed map, all paths OK"""
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        os.mkdir("test_dir")
+        with open("test_dir/file_r1.fastq.gz", "w", encoding="utf-8") as fastq_file1:
+            fastq_file1.write("AAABBB")
+
+        with open("test_dir/file_r2.fastq.gz", "w", encoding="utf-8") as fastq_file2:
+            fastq_file2.write("AAABBB")
+
+        with open("test_file_map.fastq-map.csv", "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    ["file", "r1", "test_dir/file_r1.fastq.gz"],
+                    ["file", "r2", "test_dir/file_r2.fastq.gz"],
+                ]
+            )
+        fastqs = parse_fastqs_map_file("test_file_map.fastq-map.csv")
+    assert _validate_parsed_map(fastqs) is None
+
+
+def test_validate_parsed_map__mixed():
+    """Test validation of parsed map to prevent heterogeneous path values"""
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        os.mkdir("test_dir")
+        with open("test_dir/file_r1.fastq.gz", "w", encoding="utf-8") as fastq_file1:
+            fastq_file1.write("AAABBB")
+
+        with open("test_dir/file_r2.fastq.gz", "w", encoding="utf-8") as fastq_file2:
+            fastq_file2.write("AAABBB")
+
+        with open("test_mixed_map.fastq-map.csv", "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    ["url", "r1", "https://s3.amazonaws.com/samples/1/R1.fastq.gz"],
+                    ["url", "r2", "https://s3.amazonaws.com/samples/1/R1.fastq.gz"],
+                    ["file", "r1", "test_dir/file_r1.fastq.gz"],
+                    ["file", "r2", "test_dir/file_r2.fastq.gz"],
+                ]
+            )
+        try:
+            parse_fastqs_map_file("test_mixed_map.fastq-map.csv")
+        except ValidationError as err:
+            assert "Detected both URLs and file paths" in err.args[0]
+
+
 def test_is_valid_uuid__is_valid():
     """Test that a UUID is a valid UUID"""
     assert is_valid_uuid("11111111-1111-1111-1111-111111111111")
 
 
 def test_is_valid_uuid__is_not_valid__too_long():
     """Test that UUID with extra chars is not a valid UUID"""
```

### Comparing `gencove-2.5.0/gencove/tests/upload/test_cli_upload.py` & `gencove-2.5.1/gencove/tests/upload/test_cli_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -1014,18 +1014,16 @@
         assert res.exit_code == 0
         if not recording:
             mocked_import_fastqs_from_url.assert_called_once()
         mocked_get_credentials.assert_called_once()
         assert "All files were successfully processed" in res.output
 
 
-@pytest.mark.vcr
-@assert_authorization
-def test_upload_url_with_local(credentials, vcr, recording, mocker):
-    """Basic check of uploading URL"""
+def test_upload_url_with_local(credentials):
+    """Confirm this case raises error, cannot mix URL and path"""
     # pylint: disable=too-many-locals
 
     runner = CliRunner()
     with runner.isolated_filesystem():
         os.mkdir("cli_test_data")
         map_file_path = "cli_test_data/test_url_map.fastq-map.csv"
 
@@ -1048,45 +1046,21 @@
                         "bar",
                         "r1",
                         fastq_file_path,
                     ],
                 ]
             )
 
-        mocked_get_credentials = mocker.patch(
-            "gencove.command.upload.main.get_s3_client_refreshable",
-            side_effect=get_s3_client_refreshable,
-        )
-
-        if not recording:
-            url_response = get_vcr_response("/api/v2/uploads-url/", vcr)
-            mocked_import_fastqs_from_url = mocker.patch.object(
-                APIClient,
-                "import_fastqs_from_url",
-                return_value=UploadURLImport(**url_response),
-            )
-
-            upload_response = get_vcr_response("/api/v2/uploads-post-data/", vcr)
-            mocked_get_upload_details = mocker.patch.object(
-                APIClient,
-                "get_upload_details",
-                return_value=UploadsPostData(**upload_response),
-            )
-
         res = runner.invoke(
             upload,
             [map_file_path, *credentials],
         )
-        assert not res.exception
-        assert res.exit_code == 0
-        if not recording:
-            mocked_import_fastqs_from_url.assert_called_once()
-            mocked_get_upload_details.assert_called_once()
-        mocked_get_credentials.assert_called_once()
-        assert "All files were successfully processed" in res.output
+        assert res.exception
+        assert res.exit_code == 1
+        assert "Please only supply one type of path" in res.output
 
 
 @pytest.mark.vcr
 @assert_authorization
 def test_upload_url_and_run_immediately(
     credentials, vcr, recording, mocker, project_id
 ):
@@ -1146,7 +1120,104 @@
         assert "All files were successfully processed" in res.output
         if not recording:
             mocked_import_fastqs_from_url.assert_called_once()
             mocked_get_sample_sheet.assert_called()
             mocked_assign_sample.assert_called_once()
 
         mocked_regular_progress_bar.assert_called_once()
+
+
+@pytest.mark.vcr
+@assert_authorization
+def test_upload_default_destination(credentials, vcr, recording, mocker):
+    """Test to confirm default destination is gncv://cli-*"""
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        os.mkdir("cli_test_data")
+        map_file_path = "cli_test_data/test_map.fastq-map.csv"
+        fastq_file_path = "cli_test_data/test.fastq.gz"
+
+        with open(fastq_file_path, "w", encoding="utf-8") as fastq_file:
+            fastq_file.write("AAABBB")
+
+        with open(map_file_path, "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    [
+                        "bar",
+                        "r1",
+                        fastq_file_path,
+                    ],
+                ]
+            )
+        mocked_get_credentials = mocker.patch(
+            "gencove.command.upload.main.get_s3_client_refreshable",
+            side_effect=get_s3_client_refreshable,
+        )
+        if not recording:
+            response = get_vcr_response("/api/v2/uploads-post-data/", vcr)
+            mocker.patch.object(
+                APIClient,
+                "get_upload_details",
+                return_value=UploadsPostData(**response),
+            )
+        mocker.patch("gencove.command.upload.main.upload_file", side_effect=upload_file)
+
+        res = runner.invoke(
+            upload,
+            [map_file_path, *credentials],
+        )
+
+    mocked_get_credentials.assert_called_once()
+
+    assert not res.exception
+    assert res.exit_code == 0
+    assert "uploaded to: gncv://cli-" in res.output
+    assert "uploaded to: gncv://cli-url-" not in res.output
+
+
+@pytest.mark.vcr
+@assert_authorization
+def test_upload_url_destination(credentials, vcr, recording, mocker):
+    """Test to confirm default destination is gncv://cli-url-*"""
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        os.mkdir("cli_test_data")
+        map_file_path = "cli_test_data/test_map.fastq-map.csv"
+
+        with open(map_file_path, "w", encoding="utf-8") as map_file:
+            writer = csv.writer(map_file)
+            writer.writerows(
+                [
+                    ["client_id", "r_notation", "path"],
+                    [
+                        "bar",
+                        "r1",
+                        "https://s3.amazonaws.com/example/client-id_R1.fastq.gz",
+                    ],
+                ]
+            )
+
+        mocked_get_credentials = mocker.patch(
+            "gencove.command.upload.main.get_s3_client_refreshable",
+            side_effect=get_s3_client_refreshable,
+        )
+
+        if not recording:
+            response = get_vcr_response("/api/v2/uploads-url/", vcr)
+            mocker.patch.object(
+                APIClient,
+                "import_fastqs_from_url",
+                return_value=UploadURLImport(**response),
+            )
+
+        res = runner.invoke(
+            upload,
+            [map_file_path, *credentials],
+        )
+
+    mocked_get_credentials.assert_called_once()
+    assert not res.exception
+    assert res.exit_code == 0
+    assert "uploaded to: gncv://cli-url-" in res.output
```

### Comparing `gencove-2.5.0/gencove/tests/upload/vcr/filters.py` & `gencove-2.5.1/gencove/tests/upload/vcr/filters.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/uploads/test_uploads_list.py` & `gencove-2.5.1/gencove/tests/uploads/test_uploads_list.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/utils.py` & `gencove-2.5.1/gencove/tests/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/tests/webhook/test_webhook_verify.py` & `gencove-2.5.1/gencove/tests/webhook/test_webhook_verify.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove/utils.py` & `gencove-2.5.1/gencove/utils.py`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/gencove.egg-info/PKG-INFO` & `gencove-2.5.1/gencove.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gencove
-Version: 2.5.0
+Version: 2.5.1
 Summary: Gencove API and CLI tool
 Home-page: http://docs.gencove.com
 Author: Tomaz Berisa
 License: Apache 2.0
 Description: # The Gencove CLI
         
         [![PyPI Latest Release](https://img.shields.io/pypi/v/gencove.svg)](https://pypi.org/project/gencove/)
```

### Comparing `gencove-2.5.0/gencove.egg-info/SOURCES.txt` & `gencove-2.5.1/gencove.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gencove-2.5.0/setup.py` & `gencove-2.5.1/setup.py`

 * *Files identical despite different names*

