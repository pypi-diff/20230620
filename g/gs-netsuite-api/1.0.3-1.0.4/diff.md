# Comparing `tmp/gs-netsuite-api-1.0.3.tar.gz` & `tmp/gs-netsuite-api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs-netsuite-api-1.0.3.tar", last modified: Tue Jun 20 20:04:58 2023, max compression
+gzip compressed data, was "gs-netsuite-api-1.0.4.tar", last modified: Tue Jun 20 21:09:42 2023, max compression
```

## Comparing `gs-netsuite-api-1.0.3.tar` & `gs-netsuite-api-1.0.4.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.666028 gs-netsuite-api-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     1910 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.idea/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.idea/GitlabLint.xml
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.idea/vcs.xml
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.local-antora-playbook.yml
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:30:08.000000 gs-netsuite-api-1.0.3/.ruff
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-20 20:04:58.666028 gs-netsuite-api-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/README.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/docs/
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/docs/antora.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.646028 gs-netsuite-api-1.0.3/docs/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/docs/modules/ROOT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.646028 gs-netsuite-api-1.0.3/docs/modules/ROOT/examples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/docs/modules/ROOT/nav.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/
--rw-rw-rw-   0 root         (0) root         (0)     3361 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/api.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2996 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/convertion.adoc
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/index.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2206 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/types.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/example/
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/example/sample_item_fulfillment_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/example/sample_item_receipt_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-20 19:51:18.000000 gs-netsuite-api-1.0.3/example/sample_product_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/example/sample_purchase_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/example/sample_sale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      582 2023-06-20 12:28:34.000000 gs-netsuite-api-1.0.3/netsuite-api.iml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.646028 gs-netsuite-api-1.0.3/output/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.646028 gs-netsuite-api-1.0.3/output/wsdl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/output/wsdl/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   133803 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/wsdl/v2022_2_0/netsuite.wsdl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/output/xsd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/output/xsd/activities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/output/xsd/activities/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    38231 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/activities/v2022_2_0/scheduling.xsd
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/activities/v2022_2_0/schedulingTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/output/xsd/documents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/output/xsd/documents/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)     8963 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/documents/v2022_2_0/fileCabinet.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4282 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/output/xsd/general/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.654028 gs-netsuite-api-1.0.3/output/xsd/general/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    14530 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/general/v2022_2_0/communication.xsd
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/general/v2022_2_0/communicationTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/output/xsd/lists/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.658028 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   424972 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/accounting.xsd
--rw-rw-rw-   0 root         (0) root         (0)    40848 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/accountingTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    11949 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/employeeTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    31010 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/employees.xsd
--rw-rw-rw-   0 root         (0) root         (0)    27949 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/marketing.xsd
--rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/marketingTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/relationshipTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)   102099 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/relationships.xsd
--rw-rw-rw-   0 root         (0) root         (0)    16989 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/supplyChain.xsd
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    29653 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/support.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2906 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/supportTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/website.xsd
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/websiteTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/output/xsd/platform/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.662028 gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   744517 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/common.xsd
--rw-rw-rw-   0 root         (0) root         (0)    59244 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/commonTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    47859 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/core.xsd
--rw-rw-rw-   0 root         (0) root         (0)    37883 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/coreTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    72361 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/faultTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     3764 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/faults.xsd
--rw-rw-rw-   0 root         (0) root         (0)    28339 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/messages.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/output/xsd/setup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.662028 gs-netsuite-api-1.0.3/output/xsd/setup/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   102180 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/setup/v2022_2_0/customization.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4880 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/setup/v2022_2_0/customizationTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/output/xsd/transactions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.662028 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    13345 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/bank.xsd
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/bankTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/customerTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    75538 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/customers.xsd
--rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/demandPlanning.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/employeeTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    43650 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/employees.xsd
--rw-rw-rw-   0 root         (0) root         (0)     5844 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/financial.xsd
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/financialTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    23444 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/general.xsd
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/inventory.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    64002 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/purchases.xsd
--rw-rw-rw-   0 root         (0) root         (0)    32740 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/saleTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)   141383 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/sales.xsd
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-20 10:28:15.000000 gs-netsuite-api-1.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 20:04:58.666028 gs-netsuite-api-1.0.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.650028 gs-netsuite-api-1.0.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.666028 gs-netsuite-api-1.0.3/src/gs_netsuite_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-20 20:04:58.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    26185 2023-06-20 19:52:27.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api/api.py.adoc
--rw-rw-rw-   0 root         (0) root         (0)     4184 2023-06-20 19:46:27.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)     4296 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api/ns_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:04:58.666028 gs-netsuite-api-1.0.3/src/gs_netsuite_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-20 20:04:58.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3252 2023-06-20 20:04:58.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:04:58.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-20 20:04:58.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-20 20:04:58.000000 gs-netsuite-api-1.0.3/src/gs_netsuite_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3862 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.3/wsdldownloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.793536 gs-netsuite-api-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.idea/GitlabLint.xml
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.local-antora-playbook.yml
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 10:30:08.000000 gs-netsuite-api-1.0.4/.ruff
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-20 21:09:42.793536 gs-netsuite-api-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/README.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/docs/antora.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/docs/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/docs/modules/ROOT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/docs/modules/ROOT/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.785536 gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/
+-rw-rw-rw-   0 root         (0) root         (0)     3361 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/api.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/convertion.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/index.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2206 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/types.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.785536 gs-netsuite-api-1.0.4/example/
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/example/sample_item_fulfillment_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/example/sample_item_receipt_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-20 19:51:18.000000 gs-netsuite-api-1.0.4/example/sample_product_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/example/sample_purchase_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/example/sample_sale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      582 2023-06-20 12:28:34.000000 gs-netsuite-api-1.0.4/netsuite-api.iml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/wsdl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.785536 gs-netsuite-api-1.0.4/output/wsdl/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   133803 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/wsdl/v2022_2_0/netsuite.wsdl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/xsd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/xsd/activities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.785536 gs-netsuite-api-1.0.4/output/xsd/activities/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    38231 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/activities/v2022_2_0/scheduling.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/activities/v2022_2_0/schedulingTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/xsd/documents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.785536 gs-netsuite-api-1.0.4/output/xsd/documents/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)     8963 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/documents/v2022_2_0/fileCabinet.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4282 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/xsd/general/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.785536 gs-netsuite-api-1.0.4/output/xsd/general/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    14530 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/general/v2022_2_0/communication.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/general/v2022_2_0/communicationTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/xsd/lists/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.785536 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   424972 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/accounting.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    40848 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/accountingTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/employeeTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    31010 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/employees.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    27949 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/marketing.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/marketingTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/relationshipTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)   102099 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/relationships.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    16989 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/supplyChain.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    29653 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/support.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2906 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/supportTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/website.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/websiteTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/xsd/platform/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.789536 gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   744517 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/common.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    59244 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/commonTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    47859 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/core.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    37883 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/coreTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    72361 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/faultTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     3764 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/faults.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    28339 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/messages.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/xsd/setup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.789536 gs-netsuite-api-1.0.4/output/xsd/setup/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   102180 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/setup/v2022_2_0/customization.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4880 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/setup/v2022_2_0/customizationTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/output/xsd/transactions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.789536 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    13345 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/bank.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/bankTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/customerTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    75538 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/customers.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/demandPlanning.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/employeeTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    43650 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/employees.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5844 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/financial.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/financialTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    23444 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/general.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/inventory.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    64002 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/purchases.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    32740 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/saleTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)   141383 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/sales.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-20 10:28:15.000000 gs-netsuite-api-1.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 21:09:42.793536 gs-netsuite-api-1.0.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.781536 gs-netsuite-api-1.0.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.793536 gs-netsuite-api-1.0.4/src/gs_netsuite_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-20 21:09:42.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    26213 2023-06-20 21:06:34.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api/api.py.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     4184 2023-06-20 19:46:27.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     4296 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api/ns_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 21:09:42.793536 gs-netsuite-api-1.0.4/src/gs_netsuite_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-20 21:09:42.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3252 2023-06-20 21:09:42.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 21:09:42.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-20 21:09:42.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-20 21:09:42.000000 gs-netsuite-api-1.0.4/src/gs_netsuite_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3862 2023-06-20 07:51:29.000000 gs-netsuite-api-1.0.4/wsdldownloader.py
```

### Comparing `gs-netsuite-api-1.0.3/.gitignore` & `gs-netsuite-api-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/.pre-commit-config.yaml` & `gs-netsuite-api-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/README.adoc` & `gs-netsuite-api-1.0.4/README.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/api.adoc` & `gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/api.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/convertion.adoc` & `gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/convertion.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/index.adoc` & `gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/index.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/docs/modules/ROOT/pages/types.adoc` & `gs-netsuite-api-1.0.4/docs/modules/ROOT/pages/types.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/example/sample_item_fulfillment_api.py` & `gs-netsuite-api-1.0.4/example/sample_item_fulfillment_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/example/sample_item_receipt_api.py` & `gs-netsuite-api-1.0.4/example/sample_item_receipt_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/example/sample_product_api.py` & `gs-netsuite-api-1.0.4/example/sample_product_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/example/sample_purchase_api.py` & `gs-netsuite-api-1.0.4/example/sample_purchase_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/example/sample_sale_api.py` & `gs-netsuite-api-1.0.4/example/sample_sale_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/mkdocs.yml` & `gs-netsuite-api-1.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/netsuite-api.iml` & `gs-netsuite-api-1.0.4/netsuite-api.iml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/wsdl/v2022_2_0/netsuite.wsdl` & `gs-netsuite-api-1.0.4/output/wsdl/v2022_2_0/netsuite.wsdl`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/activities/v2022_2_0/scheduling.xsd` & `gs-netsuite-api-1.0.4/output/xsd/activities/v2022_2_0/scheduling.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/activities/v2022_2_0/schedulingTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/activities/v2022_2_0/schedulingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/documents/v2022_2_0/fileCabinet.xsd` & `gs-netsuite-api-1.0.4/output/xsd/documents/v2022_2_0/fileCabinet.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/general/v2022_2_0/communication.xsd` & `gs-netsuite-api-1.0.4/output/xsd/general/v2022_2_0/communication.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/general/v2022_2_0/communicationTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/general/v2022_2_0/communicationTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/accounting.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/accounting.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/accountingTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/accountingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/employeeTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/employeeTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/employees.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/employees.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/marketing.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/marketing.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/marketingTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/marketingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/relationshipTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/relationshipTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/relationships.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/relationships.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/supplyChain.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/supplyChain.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/support.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/support.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/supportTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/supportTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/lists/v2022_2_0/website.xsd` & `gs-netsuite-api-1.0.4/output/xsd/lists/v2022_2_0/website.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/common.xsd` & `gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/common.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/commonTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/commonTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/core.xsd` & `gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/core.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/coreTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/coreTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/faultTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/faultTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/faults.xsd` & `gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/faults.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/platform/v2022_2_0/messages.xsd` & `gs-netsuite-api-1.0.4/output/xsd/platform/v2022_2_0/messages.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/setup/v2022_2_0/customization.xsd` & `gs-netsuite-api-1.0.4/output/xsd/setup/v2022_2_0/customization.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/setup/v2022_2_0/customizationTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/setup/v2022_2_0/customizationTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/bank.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/bank.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/customerTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/customerTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/customers.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/customers.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/demandPlanning.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/demandPlanning.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/employeeTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/employeeTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/employees.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/employees.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/financial.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/financial.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/financialTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/financialTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/general.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/general.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/inventory.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/inventory.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/purchases.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/purchases.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/saleTypes.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/saleTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/output/xsd/transactions/v2022_2_0/sales.xsd` & `gs-netsuite-api-1.0.4/output/xsd/transactions/v2022_2_0/sales.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/pyproject.toml` & `gs-netsuite-api-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/src/gs_netsuite_api/api.py` & `gs-netsuite-api-1.0.4/src/gs_netsuite_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -495,15 +495,15 @@
 
     def _convert_to_data(self, record) -> PurchaseOrderData:
         purchase = PurchaseOrderData(
             name=record.tranId,
             internalId=int(record.internalId),
             currency=RecordRef.from_rec_named(record.currency),
             supplier=RecordRef.from_rec_named(record.entity),
-            employee=RecordRef.from_rec_named(record.employee),
+            employee=record.employee and RecordRef.from_rec_named(record.employee) or None,
             total_tax_excluded=record.subTotal,
             total_tax=record.taxTotal,
             total_tax_included=record.total,
             order_date=record.tranDate,
             state=record.status,
         )
         for sub_el in record.itemList.item:
```

### Comparing `gs-netsuite-api-1.0.3/src/gs_netsuite_api/data_types.py` & `gs-netsuite-api-1.0.4/src/gs_netsuite_api/data_types.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/src/gs_netsuite_api/ns_utils.py` & `gs-netsuite-api-1.0.4/src/gs_netsuite_api/ns_utils.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/src/gs_netsuite_api.egg-info/SOURCES.txt` & `gs-netsuite-api-1.0.4/src/gs_netsuite_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.0.3/wsdldownloader.py` & `gs-netsuite-api-1.0.4/wsdldownloader.py`

 * *Files identical despite different names*

