# Comparing `tmp/toucan_connectors-4.5.1.tar.gz` & `tmp/toucan_connectors-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toucan_connectors-4.5.1.tar", max compression
+gzip compressed data, was "toucan_connectors-4.6.0.tar", max compression
```

## Comparing `toucan_connectors-4.5.1.tar` & `toucan_connectors-4.6.0.tar`

### file list

```diff
@@ -1,181 +1,181 @@
--rw-r--r--   0        0        0     1510 2023-04-28 07:36:04.308740 toucan_connectors-4.5.1/LICENSE
--rw-r--r--   0        0        0     9969 2023-04-28 07:36:04.308740 toucan_connectors-4.5.1/README.md
--rw-r--r--   0        0        0     5575 2023-04-28 07:36:04.312739 toucan_connectors-4.5.1/pyproject.toml
--rw-r--r--   0        0        0    10795 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/__init__.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/__init__.py
--rw-r--r--   0        0        0    13648 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/adobe-analytics.png
--rw-r--r--   0        0        0     1740 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/anaplan/__init__.py
--rw-r--r--   0        0        0     7277 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/anaplan/anaplan.png
--rw-r--r--   0        0        0     7005 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/anaplan/anaplan_connector.py
--rw-r--r--   0        0        0     4622 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/auth.py
--rw-r--r--   0        0        0    61900 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/aws/aws.png
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/awsathena/__init__.py
--rw-r--r--   0        0        0     2524 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/awsathena/athena.png
--rw-r--r--   0        0        0     8464 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/awsathena/awsathena_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/azure_mssql/__init__.py
--rw-r--r--   0        0        0     2404 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/azure_mssql/azure_mssql_connector.py
--rw-r--r--   0        0        0    24249 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/azure_mssql/sql-azure.png
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/clickhouse/__init__.py
--rw-r--r--   0        0        0     1780 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/clickhouse/clickhouse.png
--rw-r--r--   0        0        0     4541 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/clickhouse/clickhouse_connector.py
--rw-r--r--   0        0        0    15750 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/common.py
--rw-r--r--   0        0        0     5549 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/condition_translator.py
--rw-r--r--   0        0        0     8162 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/connection_manager.py
--rw-r--r--   0        0        0     3534 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/databricks/databricks.png
--rw-r--r--   0        0        0     5236 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/databricks/databricks_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/dataiku/__init__.py
--rw-r--r--   0        0        0    10971 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/dataiku/dataiku.png
--rw-r--r--   0        0        0     1100 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/dataiku/dataiku_connector.py
--rwxr-xr-x   0        0        0      235 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/default-logo.png
--rw-r--r--   0        0        0     3331 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/denodo/denodo.png
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/elasticsearch/__init__.py
--rw-r--r--   0        0        0    29549 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/elasticsearch/elasticsearch.png
--rw-r--r--   0        0        0     5118 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/elasticsearch/elasticsearch_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/__init__.py
--rw-r--r--   0        0        0      452 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/doc.md
--rw-r--r--   0        0        0      183 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/enums.py
--rw-r--r--   0        0        0     5283 2023-04-28 07:36:04.324740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/facebook_ads_connector.py
--rw-r--r--   0        0        0    27755 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/facebook_logo.png
--rw-r--r--   0        0        0      126 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_ads/helpers.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_insights/__init__.py
--rw-r--r--   0        0        0    38402 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_insights/facebook-insights.png
--rw-r--r--   0        0        0     3985 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/facebook_insights/facebook_insights_connector.py
--rw-r--r--   0        0        0    13001 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/github/GitHub_Logo.png
--rw-r--r--   0        0        0      412 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/github/doc.md
--rw-r--r--   0        0        0    17081 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/github/github_connector.py
--rw-r--r--   0        0        0    15902 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/github/helpers.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/__init__.py
--rw-r--r--   0        0        0      469 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/doc.md
--rw-r--r--   0        0        0    68711 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/google_adwords.jpg
--rw-r--r--   0        0        0     9049 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/google_adwords_connector.py
--rw-r--r--   0        0        0      834 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_adwords/helpers.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_analytics/__init__.py
--rw-r--r--   0        0        0     6243 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_analytics/google-analytics.png
--rw-r--r--   0        0        0     6799 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_analytics/google_analytics_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_big_query/__init__.py
--rw-r--r--   0        0        0    17667 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_big_query/google-bigquery.png
--rw-r--r--   0        0        0    12920 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_big_query/google_big_query_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/__init__.py
--rw-r--r--   0        0        0    24008 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
--rw-r--r--   0        0        0     2488 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
--rw-r--r--   0        0        0     2473 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_credentials.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_my_business/__init__.py
--rw-r--r--   0        0        0     4045 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_my_business/google-my-business.png
--rw-r--r--   0        0        0     3024 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_my_business/google_my_business_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets/__init__.py
--rw-r--r--   0        0        0    14238 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets/google-sheets.png
--rw-r--r--   0        0        0     9061 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets/google_sheets_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets_2/__init__.py
--rw-r--r--   0        0        0      361 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets_2/doc.md
--rw-r--r--   0        0        0     9559 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/__init__.py
--rw-r--r--   0        0        0    14238 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png
--rw-r--r--   0        0        0     2986 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/http_api/__init__.py
--rw-r--r--   0        0        0    19694 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/http_api/http-api.png
--rw-r--r--   0        0        0     7584 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/http_api/http_api_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/__init__.py
--rw-r--r--   0        0        0      380 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/doc.md
--rw-r--r--   0        0        0      294 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/enums.py
--rw-r--r--   0        0        0      173 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/helpers.py
--rw-r--r--   0        0        0    33203 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/hubspot.png
--rw-r--r--   0        0        0     5738 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot/hubspot_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot_private_app/__init__.py
--rw-r--r--   0        0        0     5197 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/hubspot_private_app/hubspot_connector.py
--rw-r--r--   0        0        0      140 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/__init__.py
--rwxr-xr-x   0        0        0      726 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/databricks.sh
--rwxr-xr-x   0        0        0      509 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/mssql.sh
--rwxr-xr-x   0        0        0      926 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
--rwxr-xr-x   0        0        0      908 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/odbc.sh
--rwxr-xr-x   0        0        0      706 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/install_scripts/oracle.sh
--rw-r--r--   0        0        0     3285 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/json_wrapper.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/linkedinads/__init__.py
--rw-r--r--   0        0        0      365 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/linkedinads/doc.md
--rw-r--r--   0        0        0     9990 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/linkedinads/linkedinads.png
--rw-r--r--   0        0        0     7544 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/linkedinads/linkedinads_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/__init__.py
--rw-r--r--   0        0        0     1853 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/client.py
--rw-r--r--   0        0        0     4454 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/data.py
--rw-r--r--   0        0        0     4664 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/micro_strategy_connector.py
--rw-r--r--   0        0        0    13133 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/micro_strategy/microstrategy.png
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/mongo/__init__.py
--rw-r--r--   0        0        0    26880 2023-04-28 07:36:04.328740 toucan_connectors-4.5.1/toucan_connectors/mongo/mongo-db.png
--rw-r--r--   0        0        0    17096 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mongo/mongo_connector.py
--rw-r--r--   0        0        0     1822 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mongo/mongo_translator.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql/__init__.py
--rw-r--r--   0        0        0    26319 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql/mssql.png
--rw-r--r--   0        0        0     4673 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/__init__.py
--rw-r--r--   0        0        0    26319 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/mssql.png
--rw-r--r--   0        0        0     4893 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mysql/__init__.py
--rw-r--r--   0        0        0     3761 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mysql/mysql.png
--rw-r--r--   0        0        0    14656 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/mysql/mysql_connector.py
--rw-r--r--   0        0        0     2401 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/net_explorer/net_explorer.png
--rwxr-xr-x   0        0        0     3536 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/net_explorer/net_explorer_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oauth2_connector/__init__.py
--rw-r--r--   0        0        0     6028 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oauth2_connector/oauth2connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odata/__init__.py
--rw-r--r--   0        0        0    31781 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odata/odata.png
--rw-r--r--   0        0        0     2047 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odata/odata_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odbc/__init__.py
--rw-r--r--   0        0        0     3141 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odbc/odbc.png
--rw-r--r--   0        0        0     1298 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/odbc/odbc_connector.py
--rw-r--r--   0        0        0    10551 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/one_drive/one_drive.png
--rwxr-xr-x   0        0        0    12312 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/one_drive/one_drive_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oracle_sql/__init__.py
--rw-r--r--   0        0        0    12887 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oracle_sql/oracle-sql.png
--rw-r--r--   0        0        0     3375 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/oracle_sql/oracle_sql_connector.py
--rw-r--r--   0        0        0     3948 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/pagination.py
--rw-r--r--   0        0        0     2638 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/pandas_translator.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/peakina/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/peakina/peakina.png
--rw-r--r--   0        0        0      509 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/peakina/peakina_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/postgres/__init__.py
--rw-r--r--   0        0        0    28440 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/postgres/postgres.png
--rw-r--r--   0        0        0    10400 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/postgres/postgresql_connector.py
--rw-r--r--   0        0        0    17824 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/postgres/utils.py
--rw-r--r--   0        0        0     1498 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/query_manager.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/redshift/__init__.py
--rw-r--r--   0        0        0     8867 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/redshift/redshift.png
--rw-r--r--   0        0        0    16551 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/redshift/redshift_database_connector.py
--rw-r--r--   0        0        0     1850 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/redshift/utils.py
--rw-r--r--   0        0        0      410 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce/doc.md
--rw-r--r--   0        0        0   165347 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce.jpg
--rw-r--r--   0        0        0     7429 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce_connector.py
--rw-r--r--   0        0        0      410 2023-04-28 07:36:04.332740 toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/doc.md
--rw-r--r--   0        0        0   165347 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
--rw-r--r--   0        0        0     8536 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce.jpg
--rw-r--r--   0        0        0       84 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/sap_hana/__init__.py
--rw-r--r--   0        0        0    20257 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/sap_hana/sap-hana.png
--rw-r--r--   0        0        0     1264 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/sap_hana/sap_hana_connector.py
--rw-r--r--   0        0        0    20013 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/share_point/share_point.png
--rw-r--r--   0        0        0      143 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake/__init__.py
--rw-r--r--   0        0        0    15417 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake/snowflake.png
--rw-r--r--   0        0        0    18251 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake/snowflake_connector.py
--rw-r--r--   0        0        0    12795 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake_common.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/__init__.py
--rw-r--r--   0        0        0    15417 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/snowflake.png
--rw-r--r--   0        0        0    12246 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/soap/__init__.py
--rw-r--r--   0        0        0      609 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/soap/helpers.py
--rw-r--r--   0        0        0    42145 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/soap/soap.png
--rw-r--r--   0        0        0     4325 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/soap/soap_connector.py
--rw-r--r--   0        0        0     3080 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/sql_query_helper.py
--rw-r--r--   0        0        0    21205 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/toucan_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/toucan_toco/__init__.py
--rwxr-xr-x   0        0        0     4372 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/toucan_toco/toucan.png
--rw-r--r--   0        0        0     1289 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/toucan_toco/toucan_toco_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/trello/__init__.py
--rw-r--r--   0        0        0     3966 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/trello/trello.png
--rw-r--r--   0        0        0     6603 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/trello/trello_connector.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/utils/__init__.py
--rw-r--r--   0        0        0      492 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/utils/datetime.py
--rw-r--r--   0        0        0      629 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/utils/pem.py
--rw-r--r--   0        0        0        0 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/wootric/__init__.py
--rw-r--r--   0        0        0     8734 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/wootric/wootric.png
--rw-r--r--   0        0        0     5228 2023-04-28 07:36:04.336740 toucan_connectors-4.5.1/toucan_connectors/wootric/wootric_connector.py
--rw-r--r--   0        0        0    14616 1970-01-01 00:00:00.000000 toucan_connectors-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1510 2023-06-02 09:26:49.571571 toucan_connectors-4.6.0/LICENSE
+-rw-r--r--   0        0        0     9969 2023-06-02 09:26:49.571571 toucan_connectors-4.6.0/README.md
+-rw-r--r--   0        0        0     5573 2023-06-02 09:26:49.575571 toucan_connectors-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0    10795 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/__init__.py
+-rw-r--r--   0        0        0    13648 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/adobe-analytics.png
+-rw-r--r--   0        0        0     1740 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/anaplan/__init__.py
+-rw-r--r--   0        0        0     7277 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/anaplan/anaplan.png
+-rw-r--r--   0        0        0     7005 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/anaplan/anaplan_connector.py
+-rw-r--r--   0        0        0     4622 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/auth.py
+-rw-r--r--   0        0        0    61900 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/aws/aws.png
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/awsathena/__init__.py
+-rw-r--r--   0        0        0     2524 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/awsathena/athena.png
+-rw-r--r--   0        0        0     8464 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/awsathena/awsathena_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/azure_mssql/__init__.py
+-rw-r--r--   0        0        0     2404 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/azure_mssql/azure_mssql_connector.py
+-rw-r--r--   0        0        0    24249 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/azure_mssql/sql-azure.png
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/clickhouse/__init__.py
+-rw-r--r--   0        0        0     1780 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/clickhouse/clickhouse.png
+-rw-r--r--   0        0        0     4541 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/clickhouse/clickhouse_connector.py
+-rw-r--r--   0        0        0    15322 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/common.py
+-rw-r--r--   0        0        0     5549 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/condition_translator.py
+-rw-r--r--   0        0        0     8162 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/connection_manager.py
+-rw-r--r--   0        0        0     3534 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/databricks/databricks.png
+-rw-r--r--   0        0        0     5236 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/databricks/databricks_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/dataiku/__init__.py
+-rw-r--r--   0        0        0    10971 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/dataiku/dataiku.png
+-rw-r--r--   0        0        0     1100 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/dataiku/dataiku_connector.py
+-rwxr-xr-x   0        0        0      235 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/default-logo.png
+-rw-r--r--   0        0        0     3331 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/denodo/denodo.png
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/elasticsearch/__init__.py
+-rw-r--r--   0        0        0    29549 2023-06-02 09:26:49.587571 toucan_connectors-4.6.0/toucan_connectors/elasticsearch/elasticsearch.png
+-rw-r--r--   0        0        0     5118 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/elasticsearch/elasticsearch_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/__init__.py
+-rw-r--r--   0        0        0      452 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/doc.md
+-rw-r--r--   0        0        0      183 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/enums.py
+-rw-r--r--   0        0        0     5283 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/facebook_ads_connector.py
+-rw-r--r--   0        0        0    27755 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/facebook_logo.png
+-rw-r--r--   0        0        0      126 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_ads/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_insights/__init__.py
+-rw-r--r--   0        0        0    38402 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_insights/facebook-insights.png
+-rw-r--r--   0        0        0     3985 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/facebook_insights/facebook_insights_connector.py
+-rw-r--r--   0        0        0    13001 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/github/GitHub_Logo.png
+-rw-r--r--   0        0        0      412 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/github/doc.md
+-rw-r--r--   0        0        0    17081 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/github/github_connector.py
+-rw-r--r--   0        0        0    15902 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/github/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/__init__.py
+-rw-r--r--   0        0        0      469 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/doc.md
+-rw-r--r--   0        0        0    68711 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/google_adwords.jpg
+-rw-r--r--   0        0        0     9049 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/google_adwords_connector.py
+-rw-r--r--   0        0        0      834 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_adwords/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_analytics/__init__.py
+-rw-r--r--   0        0        0     6243 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_analytics/google-analytics.png
+-rw-r--r--   0        0        0     6799 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_analytics/google_analytics_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_big_query/__init__.py
+-rw-r--r--   0        0        0    17667 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_big_query/google-bigquery.png
+-rw-r--r--   0        0        0    12920 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_big_query/google_big_query_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/__init__.py
+-rw-r--r--   0        0        0    24008 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png
+-rw-r--r--   0        0        0     2488 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py
+-rw-r--r--   0        0        0     2473 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_credentials.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_my_business/__init__.py
+-rw-r--r--   0        0        0     4045 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_my_business/google-my-business.png
+-rw-r--r--   0        0        0     3024 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_my_business/google_my_business_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets/__init__.py
+-rw-r--r--   0        0        0    14238 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets/google-sheets.png
+-rw-r--r--   0        0        0     9061 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets/google_sheets_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets_2/__init__.py
+-rw-r--r--   0        0        0      361 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets_2/doc.md
+-rw-r--r--   0        0        0     9559 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/__init__.py
+-rw-r--r--   0        0        0    14238 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png
+-rw-r--r--   0        0        0     2986 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/http_api/__init__.py
+-rw-r--r--   0        0        0    19694 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/http_api/http-api.png
+-rw-r--r--   0        0        0     7584 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/http_api/http_api_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/__init__.py
+-rw-r--r--   0        0        0      380 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/doc.md
+-rw-r--r--   0        0        0      294 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/enums.py
+-rw-r--r--   0        0        0      173 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/helpers.py
+-rw-r--r--   0        0        0    33203 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/hubspot.png
+-rw-r--r--   0        0        0     5738 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot/hubspot_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot_private_app/__init__.py
+-rw-r--r--   0        0        0     5197 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/hubspot_private_app/hubspot_connector.py
+-rw-r--r--   0        0        0      140 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/__init__.py
+-rwxr-xr-x   0        0        0      726 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/databricks.sh
+-rwxr-xr-x   0        0        0      509 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/mssql.sh
+-rwxr-xr-x   0        0        0      926 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh
+-rwxr-xr-x   0        0        0      908 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/odbc.sh
+-rwxr-xr-x   0        0        0      706 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/install_scripts/oracle.sh
+-rw-r--r--   0        0        0     3285 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/json_wrapper.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.591571 toucan_connectors-4.6.0/toucan_connectors/linkedinads/__init__.py
+-rw-r--r--   0        0        0      365 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/linkedinads/doc.md
+-rw-r--r--   0        0        0     9990 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/linkedinads/linkedinads.png
+-rw-r--r--   0        0        0     7544 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/linkedinads/linkedinads_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/__init__.py
+-rw-r--r--   0        0        0     1853 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/client.py
+-rw-r--r--   0        0        0     4454 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/data.py
+-rw-r--r--   0        0        0     4664 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/micro_strategy_connector.py
+-rw-r--r--   0        0        0    13133 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/micro_strategy/microstrategy.png
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mongo/__init__.py
+-rw-r--r--   0        0        0    26880 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mongo/mongo-db.png
+-rw-r--r--   0        0        0    17096 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mongo/mongo_connector.py
+-rw-r--r--   0        0        0     1822 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mongo/mongo_translator.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql/__init__.py
+-rw-r--r--   0        0        0    26319 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql/mssql.png
+-rw-r--r--   0        0        0     4673 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/__init__.py
+-rw-r--r--   0        0        0    26319 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/mssql.png
+-rw-r--r--   0        0        0     4893 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mysql/__init__.py
+-rw-r--r--   0        0        0     3761 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mysql/mysql.png
+-rw-r--r--   0        0        0    14656 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/mysql/mysql_connector.py
+-rw-r--r--   0        0        0     2401 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/net_explorer/net_explorer.png
+-rwxr-xr-x   0        0        0     3536 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/net_explorer/net_explorer_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oauth2_connector/__init__.py
+-rw-r--r--   0        0        0     6028 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oauth2_connector/oauth2connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odata/__init__.py
+-rw-r--r--   0        0        0    31781 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odata/odata.png
+-rw-r--r--   0        0        0     2047 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odata/odata_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odbc/__init__.py
+-rw-r--r--   0        0        0     3141 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odbc/odbc.png
+-rw-r--r--   0        0        0     1298 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/odbc/odbc_connector.py
+-rw-r--r--   0        0        0    10551 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/one_drive/one_drive.png
+-rwxr-xr-x   0        0        0    12312 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/one_drive/one_drive_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oracle_sql/__init__.py
+-rw-r--r--   0        0        0    12887 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oracle_sql/oracle-sql.png
+-rw-r--r--   0        0        0     3375 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/oracle_sql/oracle_sql_connector.py
+-rw-r--r--   0        0        0     3948 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/pagination.py
+-rw-r--r--   0        0        0     2638 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/pandas_translator.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/peakina/__init__.py
+-rw-r--r--   0        0        0     1377 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/peakina/peakina.png
+-rw-r--r--   0        0        0      509 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/peakina/peakina_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/postgres/__init__.py
+-rw-r--r--   0        0        0    28440 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/postgres/postgres.png
+-rw-r--r--   0        0        0    10400 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/postgres/postgresql_connector.py
+-rw-r--r--   0        0        0    17824 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/postgres/utils.py
+-rw-r--r--   0        0        0     1498 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/query_manager.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/redshift/__init__.py
+-rw-r--r--   0        0        0     8867 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/redshift/redshift.png
+-rw-r--r--   0        0        0    16551 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/redshift/redshift_database_connector.py
+-rw-r--r--   0        0        0     1850 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/redshift/utils.py
+-rw-r--r--   0        0        0      410 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/salesforce/doc.md
+-rw-r--r--   0        0        0   165347 2023-06-02 09:26:49.595571 toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce.jpg
+-rw-r--r--   0        0        0     7429 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce_connector.py
+-rw-r--r--   0        0        0      410 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/doc.md
+-rw-r--r--   0        0        0   165347 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png
+-rw-r--r--   0        0        0     8536 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce.jpg
+-rw-r--r--   0        0        0       84 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce_sandbox_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/sap_hana/__init__.py
+-rw-r--r--   0        0        0    20257 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/sap_hana/sap-hana.png
+-rw-r--r--   0        0        0     1264 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/sap_hana/sap_hana_connector.py
+-rw-r--r--   0        0        0    20013 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/share_point/share_point.png
+-rw-r--r--   0        0        0      143 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake/__init__.py
+-rw-r--r--   0        0        0    15417 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake/snowflake.png
+-rw-r--r--   0        0        0    18251 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake/snowflake_connector.py
+-rw-r--r--   0        0        0    12795 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake_common.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/__init__.py
+-rw-r--r--   0        0        0    15417 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/snowflake.png
+-rw-r--r--   0        0        0    12246 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/soap/__init__.py
+-rw-r--r--   0        0        0      609 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/soap/helpers.py
+-rw-r--r--   0        0        0    42145 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/soap/soap.png
+-rw-r--r--   0        0        0     4325 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/soap/soap_connector.py
+-rw-r--r--   0        0        0     3080 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/sql_query_helper.py
+-rw-r--r--   0        0        0    21205 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/toucan_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/toucan_toco/__init__.py
+-rwxr-xr-x   0        0        0     4372 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/toucan_toco/toucan.png
+-rw-r--r--   0        0        0     1289 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/toucan_toco/toucan_toco_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/trello/__init__.py
+-rw-r--r--   0        0        0     3966 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/trello/trello.png
+-rw-r--r--   0        0        0     6603 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/trello/trello_connector.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/utils/__init__.py
+-rw-r--r--   0        0        0      492 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/utils/datetime.py
+-rw-r--r--   0        0        0      629 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/utils/pem.py
+-rw-r--r--   0        0        0        0 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/wootric/__init__.py
+-rw-r--r--   0        0        0     8734 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/wootric/wootric.png
+-rw-r--r--   0        0        0     5228 2023-06-02 09:26:49.599572 toucan_connectors-4.6.0/toucan_connectors/wootric/wootric_connector.py
+-rw-r--r--   0        0        0    14616 1970-01-01 00:00:00.000000 toucan_connectors-4.6.0/PKG-INFO
```

### Comparing `toucan_connectors-4.5.1/LICENSE` & `toucan_connectors-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/README.md` & `toucan_connectors-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/pyproject.toml` & `toucan_connectors-4.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 profile = "black"
 include_trailing_comma = true
 line_length = 100
 multi_line_output = 3
 
 [tool.poetry]
 name = "toucan-connectors"
-version = "4.5.1"
+version = "4.6.0"
 description = "Toucan Toco Connectors"
 authors = ["Toucan Toco <dev@toucantoco.com>"]
 license = "BSD"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
@@ -67,40 +67,40 @@
 
 [tool.poetry.dev-dependencies]
 Authlib = "^1.0.1"
 aioresponses = ">=0.7.3,<1.0"
 black = "^23.3.0"
 click = "^8.1.3"
 cryptography = ">=40.0.2"
-docker = "^6.0.1"
+docker = "^6.1.3"
 flake8 = "^6.0.0"
 flake8-quotes = "^3.3.2"
 isort = "^5.12.0"
 mock = "^5.0.2"
 pytest-aiohttp = "^1.0.4"
 pytest-asyncio = ">=0.19.0,<1"
-pytest-cov = "^4.0.0"
+pytest-cov = "^4.1.0"
 pytest = "^7.3.1"
 pytest-mock = "^3.10.0"
 pytest-rerunfailures = "^11.1"
 python-slugify = "<7"
 PyYAML = "<6"
 responses = ">=0.21.0,<1"
 psycopg2 = "^2.9.3"
 xmltodict = ">=0.13.0,<1"
 python-graphql-client = ">=0.4.3,<1"
 clickhouse-driver = ">=0.2.3,<1"
 lxml = "4.9.1"
 zeep = "^4.1.0"
-mypy = "^1.2"
-pandas-stubs = "^2.0.0.230412"
-types-requests = "^2.28.11.17"
-types-simplejson = "^3.19.0.0"
+mypy = "^1.3"
+pandas-stubs = "^2.0.1.230501"
+types-requests = "^2.31.0.1"
+types-simplejson = "^3.19.0.1"
 types-python-slugify = "^8.0.0.2"
-types-pyopenssl = "^23.1.0.2"
+types-pyopenssl = "^23.2.0.0"
 
 [tool.poetry.extras]
 adobe = ["adobe-analytics"]
 awsathena = ["awswrangler"]
 azure_mssql = ["pyodbc"]
 clickhouse = ["clickhouse-driver"]
 dataiku = ["dataiku-api-client"]
```

### Comparing `toucan_connectors-4.5.1/toucan_connectors/__init__.py` & `toucan_connectors-4.6.0/toucan_connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/adobe-analytics.png` & `toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/adobe-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/adobe_analytics/adobe_analytics_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/adobe_analytics/adobe_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/anaplan/anaplan.png` & `toucan_connectors-4.6.0/toucan_connectors/anaplan/anaplan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/anaplan/anaplan_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/anaplan/anaplan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/auth.py` & `toucan_connectors-4.6.0/toucan_connectors/auth.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/aws/aws.png` & `toucan_connectors-4.6.0/toucan_connectors/aws/aws.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/awsathena/athena.png` & `toucan_connectors-4.6.0/toucan_connectors/awsathena/athena.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/awsathena/awsathena_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/awsathena/awsathena_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/azure_mssql/azure_mssql_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/azure_mssql/azure_mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/azure_mssql/sql-azure.png` & `toucan_connectors-4.6.0/toucan_connectors/azure_mssql/sql-azure.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/clickhouse/clickhouse.png` & `toucan_connectors-4.6.0/toucan_connectors/clickhouse/clickhouse.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/clickhouse/clickhouse_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/clickhouse/clickhouse_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/common.py` & `toucan_connectors-4.6.0/toucan_connectors/common.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from contextlib import suppress
 from copy import deepcopy
 from typing import Any, Callable
 
 import jq
 import pandas as pd
 from aiohttp import ClientSession
-from jinja2 import Environment, StrictUndefined, Template, meta
+from jinja2 import Environment, Template, Undefined, UndefinedError, meta
 from jinja2.nativetypes import NativeEnvironment
 from pydantic import Field
 from toucan_data_sdk.utils.helpers import slugify
 
 # Query interpolation
 
 RE_PARAM = r'%\(([^(%\()]*)\)s'
@@ -27,21 +27,14 @@
 # Identify jinja params with no quotes around or complex condition
 RE_JINJA_ALONE_IN_STRING = [RE_JINJA + r'([ )])', RE_JINJA + r'()$']
 
 RE_SET_KEEP_TYPE = r'{{__keep_type__\1}}\2'
 RE_GET_KEEP_TYPE = r'{{(__keep_type__[^({{)}]*)}}'
 RE_NAMED_PARAM = r'\'?%\([a-zA-Z0-9_]*\)s\'?'
 
-# If a parameter has one of these values, it'll be removed from a query
-_PARAMETER_VALUES_TO_ELIMINATE = ('__VOID__',)
-
-
-class NonValidVariable(Exception):
-    """Error thrown for a non valid variable in endpoint"""
-
 
 class ClusterStartException(Exception):
     """Raised when start cluster fails"""
 
 
 def is_jinja_alone(s: str) -> bool:
     """
@@ -99,27 +92,64 @@
             # a list has been rendered: flatten the result
             result += rendered_elem
         else:
             result.append(rendered_elem)
     return result
 
 
-def _render_query(query: dict | list[dict] | tuple | str, parameters: dict):
+class UndefinedVariableError(Exception):
+    def __init__(self, message: str | None, var_name: str | None) -> None:
+        self.var_name = var_name
+        super().__init__(message)
+
+
+def _raise_or_return_undefined(res: Undefined | None, handle_errors: bool) -> Undefined:
+    var_name = None if res is None or res._undefined_name is None else res._undefined_name
+    if not handle_errors:
+        return res or Undefined(name=var_name)
+    # This is publicly documented, so we can safely access it:
+    # https://jinja.palletsprojects.com/en/3.0.x/api/#jinja2.Undefined._undefined_name
+    raise UndefinedVariableError(var_name=var_name, message=f'Undefined variable: {var_name}')
+
+
+def _is_defined(value: Any) -> bool:
+    return not isinstance(value, Undefined)
+
+
+def _render_query(
+    query: dict | list[dict] | tuple | str, parameters: dict | None, handle_errors: bool = False
+):
     """
     Render both jinja or %()s templates in query
     while keeping type of parameters
     """
+
+    if parameters is None:
+        return query
+
     if isinstance(query, dict):
-        return {key: _render_query(value, parameters) for key, value in deepcopy(query).items()}
+        return {
+            key: rendered
+            for key, value in deepcopy(query).items()
+            if _is_defined(rendered := _render_query(value, parameters, handle_errors))
+        }
     elif isinstance(query, list):
-        rendered_query = [_render_query(elt, parameters) for elt in deepcopy(query)]
+        rendered_query = [
+            rendered
+            for value in deepcopy(query)
+            if _is_defined(rendered := _render_query(value, parameters, handle_errors))
+        ]
         rendered_query = _flatten_rendered_nested_list(query, rendered_query)
         return rendered_query
     elif isinstance(query, tuple):
-        return tuple(_render_query(value, parameters) for value in deepcopy(query))
+        return tuple(
+            rendered
+            for value in deepcopy(query)
+            if _is_defined(rendered := _render_query(value, parameters, handle_errors))
+        )
     elif isinstance(query, str):
         if not _has_parameters(query):
             return query
 
         # Replace param templating with jinja templating:
         query = re.sub(RE_PARAM, r'{{ \g<1> }}', query)
 
@@ -129,81 +159,42 @@
             clean_p = _prepare_parameters(clean_p)
 
         if is_jinja_alone(query):
             env = NativeEnvironment()
         else:
             env = Environment()
 
-        res = env.from_string(query).render(clean_p)
+        try:
+            res = env.from_string(query).render(clean_p)
+        # This happens if we try to access an attribute of an undefined var, i.e nope['nein']
+        except UndefinedError:
+            return _raise_or_return_undefined(None, handle_errors)
+
+        if isinstance(res, Undefined):
+            return _raise_or_return_undefined(res, handle_errors)
         # NativeEnvironment's render() isn't recursive, so we need to
         # apply recursively the literal_eval by hand for lists and dicts:
         if isinstance(res, (list, dict)):
             return _prepare_result(res)
         return res
     else:
         return query
 
 
-def _handle_missing_params(elt: dict | list[dict] | tuple | str, params: dict, handle_errors: bool):
-    """
-    Remove a dictionary key if its value has a missing parameter.
-    This is used to support the __VOID__ syntax, specific at Toucan Toco :
-        cf. https://bit.ly/2Ln6rcf
-    """
-    if isinstance(elt, dict):
-        e = {}
-        for k, v in elt.items():
-            if isinstance(v, str):
-                missing_params = []
-                # In case the query was interpolated before being passed to the connector
-                if v.strip() in _PARAMETER_VALUES_TO_ELIMINATE:
-                    continue
-                matches = re.findall(RE_PARAM, v) + re.findall(RE_JINJA, v)
-
-                for m in matches:
-                    try:
-                        rendered = Template('{{ %s }}' % m, undefined=StrictUndefined).render(
-                            params
-                        )
-                        if rendered in _PARAMETER_VALUES_TO_ELIMINATE:
-                            missing_params.append(m)
-                    except Exception:
-                        if handle_errors:
-                            raise NonValidVariable(f'Non valid variable {m}')
-                        missing_params.append(m)
-                if any(missing_params):
-                    continue
-                else:
-                    e[k] = v
-            else:
-                e[k] = _handle_missing_params(v, params, handle_errors)
-        return e
-    elif isinstance(elt, list):
-        # Not filtering out empty dicts here because they may have a meaning in some backends
-        return [_handle_missing_params(e, params, handle_errors) for e in elt]
-    else:
-        return elt
-
-
 def nosql_apply_parameters_to_query(
     query: dict | list[dict] | tuple | str, parameters: dict | None, handle_errors: bool = False
 ):
     """
     WARNING : DO NOT USE THIS WITH VARIANTS OF SQL
     Instead use your client library parameter substitution method.
     https://www.owasp.org/index.php/Query_Parameterization_Cheat_Sheet
     """
-
-    query = _handle_missing_params(query, parameters, handle_errors)
-
-    if parameters is None:
-        return query
-
-    query = _render_query(query, parameters)
-    return query
+    rendered = _render_query(query, parameters, handle_errors)
+    # If we have undefined, return the default value for the given type
+    return rendered if _is_defined(rendered) else type(query)()
 
 
 def apply_query_parameters(query: str, parameters: dict) -> str:
     """
     Apply parameters to query
 
     Interpolate the query, which is a Jinja templates, with the provided parameters.
```

### Comparing `toucan_connectors-4.5.1/toucan_connectors/condition_translator.py` & `toucan_connectors-4.6.0/toucan_connectors/condition_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/connection_manager.py` & `toucan_connectors-4.6.0/toucan_connectors/connection_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/databricks/databricks.png` & `toucan_connectors-4.6.0/toucan_connectors/databricks/databricks.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/databricks/databricks_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/databricks/databricks_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/dataiku/dataiku.png` & `toucan_connectors-4.6.0/toucan_connectors/dataiku/dataiku.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/dataiku/dataiku_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/dataiku/dataiku_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/denodo/denodo.png` & `toucan_connectors-4.6.0/toucan_connectors/denodo/denodo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/elasticsearch/elasticsearch.png` & `toucan_connectors-4.6.0/toucan_connectors/elasticsearch/elasticsearch.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/elasticsearch/elasticsearch_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/elasticsearch/elasticsearch_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/facebook_ads/facebook_ads_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/facebook_ads/facebook_ads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/facebook_ads/facebook_logo.png` & `toucan_connectors-4.6.0/toucan_connectors/facebook_ads/facebook_logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/facebook_insights/facebook-insights.png` & `toucan_connectors-4.6.0/toucan_connectors/facebook_insights/facebook-insights.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/facebook_insights/facebook_insights_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/facebook_insights/facebook_insights_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/github/GitHub_Logo.png` & `toucan_connectors-4.6.0/toucan_connectors/github/GitHub_Logo.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/github/github_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/github/github_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/github/helpers.py` & `toucan_connectors-4.6.0/toucan_connectors/github/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_adwords/google_adwords.jpg` & `toucan_connectors-4.6.0/toucan_connectors/google_adwords/google_adwords.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_adwords/google_adwords_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/google_adwords/google_adwords_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_adwords/helpers.py` & `toucan_connectors-4.6.0/toucan_connectors/google_adwords/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_analytics/google-analytics.png` & `toucan_connectors-4.6.0/toucan_connectors/google_analytics/google-analytics.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_analytics/google_analytics_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/google_analytics/google_analytics_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_big_query/google-bigquery.png` & `toucan_connectors-4.6.0/toucan_connectors/google_big_query/google-bigquery.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_big_query/google_big_query_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/google_big_query/google_big_query_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png` & `toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/google-cloud-mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/google_cloud_mysql/google_cloud_mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_credentials.py` & `toucan_connectors-4.6.0/toucan_connectors/google_credentials.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_my_business/google-my-business.png` & `toucan_connectors-4.6.0/toucan_connectors/google_my_business/google-my-business.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_my_business/google_my_business_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/google_my_business/google_my_business_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_sheets/google-sheets.png` & `toucan_connectors-4.6.0/toucan_connectors/google_sheets/google-sheets.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_sheets/google_sheets_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/google_sheets/google_sheets_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_sheets_2/google_sheets_2_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/google_sheets_2/google_sheets_2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/google-spreadsheet.png` & `toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/google-spreadsheet.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/google_spreadsheet/google_spreadsheet_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/http_api/http-api.png` & `toucan_connectors-4.6.0/toucan_connectors/http_api/http-api.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/http_api/http_api_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/http_api/http_api_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/hubspot/hubspot.png` & `toucan_connectors-4.6.0/toucan_connectors/hubspot/hubspot.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/hubspot/hubspot_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/hubspot/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/hubspot_private_app/hubspot_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/hubspot_private_app/hubspot_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/install_scripts/databricks.sh` & `toucan_connectors-4.6.0/toucan_connectors/install_scripts/databricks.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/install_scripts/mssql_TLSv1_0.sh` & `toucan_connectors-4.6.0/toucan_connectors/install_scripts/mssql_TLSv1_0.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/install_scripts/odbc.sh` & `toucan_connectors-4.6.0/toucan_connectors/install_scripts/odbc.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/install_scripts/oracle.sh` & `toucan_connectors-4.6.0/toucan_connectors/install_scripts/oracle.sh`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/json_wrapper.py` & `toucan_connectors-4.6.0/toucan_connectors/json_wrapper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/linkedinads/linkedinads.png` & `toucan_connectors-4.6.0/toucan_connectors/linkedinads/linkedinads.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/linkedinads/linkedinads_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/linkedinads/linkedinads_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/micro_strategy/client.py` & `toucan_connectors-4.6.0/toucan_connectors/micro_strategy/client.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/micro_strategy/data.py` & `toucan_connectors-4.6.0/toucan_connectors/micro_strategy/data.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/micro_strategy/micro_strategy_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/micro_strategy/micro_strategy_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/micro_strategy/microstrategy.png` & `toucan_connectors-4.6.0/toucan_connectors/micro_strategy/microstrategy.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mongo/mongo-db.png` & `toucan_connectors-4.6.0/toucan_connectors/mongo/mongo-db.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mongo/mongo_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/mongo/mongo_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mongo/mongo_translator.py` & `toucan_connectors-4.6.0/toucan_connectors/mongo/mongo_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mssql/mssql.png` & `toucan_connectors-4.6.0/toucan_connectors/mssql/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mssql/mssql_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/mssql/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/mssql.png` & `toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/mssql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mssql_TLSv1_0/mssql_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/mssql_TLSv1_0/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mysql/mysql.png` & `toucan_connectors-4.6.0/toucan_connectors/mysql/mysql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/mysql/mysql_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/mysql/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/net_explorer/net_explorer.png` & `toucan_connectors-4.6.0/toucan_connectors/net_explorer/net_explorer.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/net_explorer/net_explorer_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/net_explorer/net_explorer_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/oauth2_connector/oauth2connector.py` & `toucan_connectors-4.6.0/toucan_connectors/oauth2_connector/oauth2connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/odata/odata.png` & `toucan_connectors-4.6.0/toucan_connectors/odata/odata.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/odata/odata_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/odata/odata_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/odbc/odbc.png` & `toucan_connectors-4.6.0/toucan_connectors/odbc/odbc.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/odbc/odbc_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/odbc/odbc_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/one_drive/one_drive.png` & `toucan_connectors-4.6.0/toucan_connectors/one_drive/one_drive.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/one_drive/one_drive_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/one_drive/one_drive_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/oracle_sql/oracle-sql.png` & `toucan_connectors-4.6.0/toucan_connectors/oracle_sql/oracle-sql.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/oracle_sql/oracle_sql_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/oracle_sql/oracle_sql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/pagination.py` & `toucan_connectors-4.6.0/toucan_connectors/pagination.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/pandas_translator.py` & `toucan_connectors-4.6.0/toucan_connectors/pandas_translator.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/peakina/peakina.png` & `toucan_connectors-4.6.0/toucan_connectors/peakina/peakina.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/postgres/postgres.png` & `toucan_connectors-4.6.0/toucan_connectors/postgres/postgres.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/postgres/postgresql_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/postgres/postgresql_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/postgres/utils.py` & `toucan_connectors-4.6.0/toucan_connectors/postgres/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/query_manager.py` & `toucan_connectors-4.6.0/toucan_connectors/query_manager.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/redshift/redshift.png` & `toucan_connectors-4.6.0/toucan_connectors/redshift/redshift.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/redshift/redshift_database_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/redshift/redshift_database_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/redshift/utils.py` & `toucan_connectors-4.6.0/toucan_connectors/redshift/utils.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce-service-cloud.png` & `toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce.jpg` & `toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/salesforce/salesforce_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/salesforce/salesforce_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png` & `toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce-service-cloud.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/salesforce_sandbox/salesforce.jpg` & `toucan_connectors-4.6.0/toucan_connectors/salesforce_sandbox/salesforce.jpg`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/sap_hana/sap-hana.png` & `toucan_connectors-4.6.0/toucan_connectors/sap_hana/sap-hana.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/sap_hana/sap_hana_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/sap_hana/sap_hana_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/share_point/share_point.png` & `toucan_connectors-4.6.0/toucan_connectors/share_point/share_point.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/snowflake/snowflake.png` & `toucan_connectors-4.6.0/toucan_connectors/snowflake/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/snowflake/snowflake_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/snowflake/snowflake_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/snowflake_common.py` & `toucan_connectors-4.6.0/toucan_connectors/snowflake_common.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/snowflake.png` & `toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/snowflake.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/snowflake_oauth2/snowflake_oauth2_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/soap/helpers.py` & `toucan_connectors-4.6.0/toucan_connectors/soap/helpers.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/soap/soap.png` & `toucan_connectors-4.6.0/toucan_connectors/soap/soap.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/soap/soap_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/soap/soap_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/sql_query_helper.py` & `toucan_connectors-4.6.0/toucan_connectors/sql_query_helper.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/toucan_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/toucan_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/toucan_toco/toucan.png` & `toucan_connectors-4.6.0/toucan_connectors/toucan_toco/toucan.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/toucan_toco/toucan_toco_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/toucan_toco/toucan_toco_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/trello/trello.png` & `toucan_connectors-4.6.0/toucan_connectors/trello/trello.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/trello/trello_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/trello/trello_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/utils/pem.py` & `toucan_connectors-4.6.0/toucan_connectors/utils/pem.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/wootric/wootric.png` & `toucan_connectors-4.6.0/toucan_connectors/wootric/wootric.png`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/toucan_connectors/wootric/wootric_connector.py` & `toucan_connectors-4.6.0/toucan_connectors/wootric/wootric_connector.py`

 * *Files identical despite different names*

### Comparing `toucan_connectors-4.5.1/PKG-INFO` & `toucan_connectors-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toucan-connectors
-Version: 4.5.1
+Version: 4.6.0
 Summary: Toucan Toco Connectors
 License: BSD
 Author: Toucan Toco
 Author-email: dev@toucantoco.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

