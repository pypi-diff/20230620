# Comparing `tmp/lino-welfare-23.1.0.tar.gz` & `tmp/lino-welfare-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-welfare-23.1.0.tar", last modified: Sun Jan  1 07:50:30 2023, max compression
+gzip compressed data, was "lino-welfare-23.6.0.tar", last modified: Tue Jun 20 12:11:07 2023, max compression
```

## Comparing `lino-welfare-23.1.0.tar` & `lino-welfare-23.6.0.tar`

### file list

```diff
@@ -1,529 +1,521 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:53.000000 lino-welfare-23.1.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      244 2022-12-15 17:33:14.000000 lino-welfare-23.1.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     2074 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1130 2022-12-16 10:31:01.000000 lino-welfare-23.1.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      653 2021-04-28 06:36:41.000000 lino-welfare-23.1.0/lino_welfare/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    21270 2022-09-05 22:58:50.000000 lino-welfare-23.1.0/lino_welfare/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)   193321 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/migrate_old.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      659 2017-06-14 02:24:21.000000 lino-welfare-23.1.0/lino_welfare/modlib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      562 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      984 2021-04-15 06:04:24.000000 lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2329 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:02.000000 lino-welfare-23.1.0/lino_welfare/modlib/active_job_search__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/aids/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1538 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2458 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1142 2020-07-22 09:24:05.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      890 2019-08-01 14:29:04.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       65 2015-09-19 03:53:59.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/default.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      713 2015-09-19 03:53:59.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      872 2021-02-18 14:09:18.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      774 2015-09-19 03:54:00.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      575 2015-09-19 03:54:00.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      564 2018-05-25 10:09:23.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      763 2015-09-19 03:53:59.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4798 2015-12-16 12:20:46.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      745 2015-09-19 03:54:00.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/aids/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:00.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6723 2021-04-17 00:36:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6340 2021-04-11 05:44:50.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    11507 2022-10-30 00:46:13.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    27336 2022-04-23 09:53:58.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      366 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/aids/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/art60/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1138 2022-10-07 01:12:03.000000 lino-welfare-23.1.0/lino_welfare/modlib/art60/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/art60/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/art60/config/art60/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/art60/config/art60/Contract/
--rw-rw-r--   0 luc       (1000) www-data    (33)    46358 2022-10-05 09:08:36.000000 lino-welfare-23.1.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/art60/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-23.1.0/lino_welfare/modlib/art60/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      806 2022-10-05 09:04:45.000000 lino-welfare-23.1.0/lino_welfare/modlib/art60/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10769 2022-12-15 10:10:20.000000 lino-welfare-23.1.0/lino_welfare/modlib/art60/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/art61/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      983 2022-10-01 01:36:58.000000 lino-welfare-23.1.0/lino_welfare/modlib/art61/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1739 2022-10-17 02:01:30.000000 lino-welfare-23.1.0/lino_welfare/modlib/art61/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/art61/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/art61/config/art61/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/art61/config/art61/Contract/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8721 2015-09-19 03:53:45.000000 lino-welfare-23.1.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/art61/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-23.1.0/lino_welfare/modlib/art61/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      347 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/art61/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7238 2022-12-15 10:10:32.000000 lino-welfare-23.1.0/lino_welfare/modlib/art61/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/badges/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1244 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/badges/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1693 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/badges/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/cal/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      472 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cal/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cal/config/cal/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/cal/config/cal/Guest/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1249 2015-09-19 03:53:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      248 2015-09-19 03:53:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/config/cal/Guest/Visitor.eml.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1700 2016-03-11 22:32:06.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/cal/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       44 2016-02-22 08:52:32.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      607 2021-04-14 07:25:37.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       43 2016-02-22 08:52:32.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    14055 2022-09-29 18:34:19.000000 lino-welfare-23.1.0/lino_welfare/modlib/cal/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8464 2016-11-17 14:00:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/2013HealthCareInsurance.wsdl
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4120 2017-04-21 06:04:21.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3740 2019-10-02 18:54:22.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2846 2015-09-19 03:53:40.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    23800 2016-07-01 08:28:52.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    15771 2016-05-18 07:19:58.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.wsdl
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3353 2016-05-18 07:19:58.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2075 2015-09-19 03:53:40.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.813554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.817554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/20190612/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11616 2016-09-30 09:59:39.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)   139908 2016-09-30 09:59:26.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    16746 2013-12-23 11:43:40.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceTypesV1.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1639 2013-11-06 13:08:24.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/HealthCareInsuranceV1.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)      154 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/README.txt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.817554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8507 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)      777 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)      933 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4198 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.817554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9867 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7931 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1042 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.817554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5622 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13874 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2435 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5569 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5699 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9421 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    19800 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1361 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.817554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1600 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4063 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5074 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1146 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.817554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3334 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2591 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1460 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3450 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3938 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11981 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5436 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6504 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3332 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1119 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1969 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1044 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4562 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3627 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6440 2015-09-19 03:53:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3491 2019-03-22 11:35:44.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2902 2019-03-22 11:35:44.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    26504 2019-03-22 11:35:44.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/
--rw-rw-rw-   0 luc       (1000) www-data    (33)   121083 2019-03-22 11:35:44.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2715 2022-12-16 07:03:40.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3241 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/config/cbss/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    21764 2015-09-19 03:53:40.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    15865 2015-09-19 03:53:40.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      538 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/cbss.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3295 2021-04-09 12:30:52.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1961 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2109 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2579 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4542 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1826 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11618 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    24155 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    26292 2015-11-29 20:09:07.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)      619 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/democfg.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6081 2021-04-14 07:25:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    20869 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9170 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/purposes.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2401 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/sectors.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    16822 2016-09-29 13:14:34.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    23231 2016-09-30 11:44:50.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml
--rw-rw-rw-   0 luc       (1000) www-data    (33)    25160 2016-09-30 11:41:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/management/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/management/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/cbss/management/commands/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/management/commands/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1895 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    23598 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    26644 2022-12-16 07:04:27.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      401 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/roles.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    37959 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/tx25.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9036 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/ui.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2468 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cbss/utils.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/client_vouchers/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      656 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/client_vouchers/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3449 2022-12-27 18:33:44.000000 lino-welfare-23.1.0/lino_welfare/modlib/client_vouchers/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1764 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/client_vouchers/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.821554 lino-welfare-23.1.0/lino_welfare/modlib/contacts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      870 2021-07-09 11:56:17.000000 lino-welfare-23.1.0/lino_welfare/modlib/contacts/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/contacts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:52.000000 lino-welfare-23.1.0/lino_welfare/modlib/contacts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       49 2016-07-06 14:59:14.000000 lino-welfare-23.1.0/lino_welfare/modlib/contacts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2016-07-06 14:59:14.000000 lino-welfare-23.1.0/lino_welfare/modlib/contacts/fixtures/std.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/contacts/management/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-12 00:26:17.000000 lino-welfare-23.1.0/lino_welfare/modlib/contacts/management/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/contacts/management/commands/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-12 00:27:23.000000 lino-welfare-23.1.0/lino_welfare/modlib/contacts/management/commands/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       70 2016-07-06 14:59:13.000000 lino-welfare-23.1.0/lino_welfare/modlib/contacts/management/commands/garble_persons.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9487 2022-10-16 03:27:14.000000 lino-welfare-23.1.0/lino_welfare/modlib/contacts/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/cv/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      479 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cv/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/cv/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:58.000000 lino-welfare-23.1.0/lino_welfare/modlib/cv/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      945 2021-04-14 07:26:02.000000 lino-welfare-23.1.0/lino_welfare/modlib/cv/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7690 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/cv/fixtures/props.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2016-02-22 08:56:29.000000 lino-welfare-23.1.0/lino_welfare/modlib/cv/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5142 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/cv/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/debts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1729 2021-04-09 10:55:15.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4424 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/debts/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/debts/config/debts/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/debts/config/debts/Budget/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    17514 2018-09-28 15:27:47.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    24679 2015-09-19 03:53:44.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    19964 2015-09-19 03:53:43.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1636 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/fields.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/debts/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:44.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4587 2021-04-16 13:14:18.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    20553 2021-04-09 10:55:49.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/fixtures/minimal.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      577 2021-04-09 10:56:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2136 2021-04-16 02:09:56.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    22270 2022-08-24 20:49:31.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      352 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/roles.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    21324 2022-09-29 18:34:19.000000 lino-welfare-23.1.0/lino_welfare/modlib/debts/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      824 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:03.000000 lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      420 2021-04-14 07:26:11.000000 lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1924 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1679 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/esf/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      852 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6282 2021-04-16 13:12:12.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/esf/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/Client/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      742 2020-11-20 03:16:25.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/ClientSummary/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      905 2016-06-07 02:40:58.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      620 2018-03-08 12:32:06.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/esf/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-01-19 01:49:31.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      360 2018-05-25 08:15:58.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      482 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     5631 2022-10-17 13:39:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/esf/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/finan/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      381 2021-04-09 10:56:41.000000 lino-welfare-23.1.0/lino_welfare/modlib/finan/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/finan/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-12-12 21:53:36.000000 lino-welfare-23.1.0/lino_welfare/modlib/finan/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      467 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/finan/fixtures/payments.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1969 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/finan/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/households/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      306 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/households/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/households/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:45.000000 lino-welfare-23.1.0/lino_welfare/modlib/households/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-02-22 08:57:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/households/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       50 2016-02-22 08:57:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/households/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3807 2021-12-14 02:24:13.000000 lino-welfare-23.1.0/lino_welfare/modlib/households/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/immersion/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1107 2021-04-10 14:05:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/immersion/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/immersion/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/immersion/config/immersion/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.825554 lino-welfare-23.1.0/lino_welfare/modlib/immersion/config/immersion/Contract/
--rw-rw-rw-   0 luc       (1000) www-data    (33)   667935 2018-05-10 19:37:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5587 2016-02-11 13:18:18.000000 lino-welfare-23.1.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/immersion/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:47.000000 lino-welfare-23.1.0/lino_welfare/modlib/immersion/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1446 2021-04-09 13:17:47.000000 lino-welfare-23.1.0/lino_welfare/modlib/immersion/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3463 2022-10-17 19:12:30.000000 lino-welfare-23.1.0/lino_welfare/modlib/immersion/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3921 2022-12-15 10:10:45.000000 lino-welfare-23.1.0/lino_welfare/modlib/immersion/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/integ/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2406 2022-10-16 06:00:46.000000 lino-welfare-23.1.0/lino_welfare/modlib/integ/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/integ/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:46.000000 lino-welfare-23.1.0/lino_welfare/modlib/integ/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     8565 2022-10-17 13:22:39.000000 lino-welfare-23.1.0/lino_welfare/modlib/integ/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2425 2021-04-09 10:57:30.000000 lino-welfare-23.1.0/lino_welfare/modlib/integ/fixtures/std.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    23997 2022-11-08 12:30:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/integ/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      377 2021-04-09 10:57:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/integ/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/isip/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      351 2022-10-07 00:51:22.000000 lino-welfare-23.1.0/lino_welfare/modlib/isip/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      722 2021-04-09 10:57:53.000000 lino-welfare-23.1.0/lino_welfare/modlib/isip/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/isip/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.805554 lino-welfare-23.1.0/lino_welfare/modlib/isip/config/isip/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/isip/config/isip/Contract/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    55172 2016-08-02 05:50:22.000000 lino-welfare-23.1.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    17687 2022-11-22 09:04:17.000000 lino-welfare-23.1.0/lino_welfare/modlib/isip/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11358 2022-12-15 10:09:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/isip/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/jobs/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      903 2022-10-16 05:44:50.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/Contract/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    94813 2015-09-19 03:54:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9896 2015-09-19 03:54:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9876 2015-09-19 03:54:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/jobs/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:54:02.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      935 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2927 2022-10-17 19:19:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/mixins.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13181 2022-10-17 19:28:42.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      327 2015-09-19 03:54:02.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/template_messages.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    17073 2022-12-15 10:11:11.000000 lino-welfare-23.1.0/lino_welfare/modlib/jobs/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/ledger/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      419 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/ledger/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/ledger/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-23.1.0/lino_welfare/modlib/ledger/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      531 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/ledger/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2758 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/ledger/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3082 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/ledger/fixtures/std_journals.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2438 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/ledger/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/newcomers/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      996 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/newcomers/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/newcomers/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-23.1.0/lino_welfare/modlib/newcomers/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3181 2021-04-14 07:26:29.000000 lino-welfare-23.1.0/lino_welfare/modlib/newcomers/fixtures/demo.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    16680 2022-11-08 12:30:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/newcomers/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      416 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/newcomers/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/notes/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      282 2018-11-22 22:34:11.000000 lino-welfare-23.1.0/lino_welfare/modlib/notes/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/notes/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:57.000000 lino-welfare-23.1.0/lino_welfare/modlib/notes/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      889 2021-04-14 07:26:37.000000 lino-welfare-23.1.0/lino_welfare/modlib/notes/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       45 2016-02-22 09:05:22.000000 lino-welfare-23.1.0/lino_welfare/modlib/notes/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2462 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/notes/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1516 2022-10-25 08:21:59.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     4422 2022-10-30 00:46:13.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/actions.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2558 2021-04-09 10:58:06.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/choicelists.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      366 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/client_address.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.829554 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/Client/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    32053 2015-09-19 03:53:51.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)   157223 2015-09-19 03:53:51.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    31905 2015-09-19 03:53:51.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      373 2015-09-19 03:53:51.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/Client/pac.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      487 2015-09-19 03:53:51.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/welcome.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:52.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2287 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1595 2021-04-09 10:58:22.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    36531 2022-10-25 02:47:29.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      509 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/pcsw/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/polls/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      335 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/polls/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/polls/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:39.000000 lino-welfare-23.1.0/lino_welfare/modlib/polls/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5736 2021-04-14 07:26:52.000000 lino-welfare-23.1.0/lino_welfare/modlib/polls/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      328 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/polls/fixtures/jobsearch.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       51 2016-07-06 15:15:32.000000 lino-welfare-23.1.0/lino_welfare/modlib/polls/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      214 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/polls/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/projects/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      619 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/projects/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2069 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/projects/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/reception/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      532 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/reception/__init__.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    14430 2022-11-08 12:30:48.000000 lino-welfare-23.1.0/lino_welfare/modlib/reception/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/sales/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:50.000000 lino-welfare-23.1.0/lino_welfare/modlib/sales/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      466 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/sales/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/sepa/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      308 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/sepa/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/sepa/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:58.000000 lino-welfare-23.1.0/lino_welfare/modlib/sepa/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4013 2021-04-14 07:27:02.000000 lino-welfare-23.1.0/lino_welfare/modlib/sepa/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1603 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/sepa/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/system/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      216 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/system/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4074 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/system/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/users/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      345 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/users/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/users/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:53.000000 lino-welfare-23.1.0/lino_welfare/modlib/users/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       46 2017-06-13 23:57:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/users/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       48 2017-06-13 23:57:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/users/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       52 2017-06-13 23:57:01.000000 lino-welfare-23.1.0/lino_welfare/modlib/users/fixtures/demo_users.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2777 2022-11-08 12:29:27.000000 lino-welfare-23.1.0/lino_welfare/modlib/users/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1050 2022-11-08 12:29:57.000000 lino-welfare-23.1.0/lino_welfare/modlib/users/ui.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      407 2021-04-15 05:57:45.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.833554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)   672907 2021-02-18 17:59:31.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      511 2015-09-19 03:53:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/TasksByClient.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1221 2015-09-19 03:53:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1146 2015-09-19 03:53:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      533 2015-10-21 13:33:32.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)       40 2015-09-19 03:53:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/default.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      624 2015-09-19 03:53:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)      800 2021-02-03 10:12:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/integ/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    11787 2015-09-19 03:53:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      585 2021-02-18 18:02:26.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/notes/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/notes/Note/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    50685 2015-09-19 03:53:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    43435 2022-10-22 20:04:19.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1040 2021-04-14 07:27:52.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    29832 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4212 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3232 2022-10-03 06:09:37.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/std2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    25860 2022-12-28 23:23:37.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/help_texts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    38280 2022-10-22 20:07:00.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo
--rw-rw-r--   0 luc       (1000) www-data    (33)   131375 2022-11-22 09:25:02.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    35602 2022-11-22 09:25:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo
--rw-rw-r--   0 luc       (1000) www-data    (33)   130350 2022-11-22 09:25:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/nl/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:56.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    18127 2020-01-29 15:42:45.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4743 2018-11-22 22:34:07.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/garble.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4518 2018-11-22 22:34:12.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    14642 2018-11-22 22:34:09.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    35429 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5859 2021-04-15 05:57:38.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     6303 2022-10-16 05:44:21.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7580 2022-10-15 08:03:38.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/user_types.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1635 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/welfare/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1055 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/config/courses/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/config/courses/Course/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    12127 2015-09-19 03:53:49.000000 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)    12100 2015-09-19 03:53:49.000000 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:49.000000 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3037 2021-04-14 07:28:00.000000 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    20702 2021-05-12 14:10:36.000000 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/models.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      363 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/modlib/xcourses/roles.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/projects/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      206 2019-03-26 11:55:25.000000 lino-welfare-23.1.0/lino_welfare/projects/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/projects/gerd/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      297 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      415 2019-02-06 12:35:36.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/django110_isnull.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      280 2020-07-24 14:51:22.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/manage.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1388 2022-11-06 03:59:24.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/print_tx25.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.837554 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      342 2021-04-16 02:21:20.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      763 2022-08-15 07:53:16.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      388 2019-02-06 12:35:36.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/doctests.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/beid/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3046 2019-02-06 20:01:51.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7615 2019-02-06 20:01:50.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg
--rw-rw-r--   0 luc       (1000) www-data    (33)     3068 2022-12-05 15:59:46.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/beid/592382784616.jpg
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/webdav/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/
--rw-rw-r--   0 luc       (1000) www-data    (33)    13379 2022-12-31 09:42:01.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       85 2019-02-06 12:35:36.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/memory.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1038 2019-03-26 11:59:36.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/mysql.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2459 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_aids.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2765 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7909 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_cbss.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3017 2022-08-02 12:20:26.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_clients.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4214 2021-02-15 07:59:43.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_debts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      253 2021-02-15 14:17:17.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_restore.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    35630 2021-04-07 10:22:55.000000 lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_watchtim.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/lino_welfare/projects/mathieu/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      365 2021-04-07 10:22:54.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      282 2019-03-26 11:59:10.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/manage.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      281 2022-10-05 18:42:47.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      512 2022-10-23 11:48:19.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      347 2019-02-06 12:35:36.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/doctests.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/media/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/media/beid/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3046 2022-10-23 06:31:52.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7615 2022-10-23 06:31:52.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg
--rw-rw-rw-   0 luc       (1000) www-data    (33)       85 2019-02-06 12:35:36.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/memory.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/lino_welfare/projects/mathieu/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2019-02-06 12:35:36.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7008 2022-06-16 10:20:24.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/tests/test_chatelet.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)    18271 2022-08-15 07:53:16.000000 lino-welfare-23.1.0/lino_welfare/projects/mathieu/tests/test_notify.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/lino_welfare/scripts/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:30.000000 lino-welfare-23.1.0/lino_welfare/scripts/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7346 2018-11-22 22:34:35.000000 lino-welfare-23.1.0/lino_welfare/scripts/load_plp.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     7750 2023-01-01 07:47:33.000000 lino-welfare-23.1.0/lino_welfare/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.809554 lino-welfare-23.1.0/lino_welfare.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2074 2023-01-01 07:50:30.000000 lino-welfare-23.1.0/lino_welfare.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)    18180 2023-01-01 07:50:30.000000 lino-welfare-23.1.0/lino_welfare.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-01-01 07:50:30.000000 lino-welfare-23.1.0/lino_welfare.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2016-09-02 10:20:26.000000 lino-welfare-23.1.0/lino_welfare.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2023-01-01 07:50:30.000000 lino-welfare-23.1.0/lino_welfare.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       13 2023-01-01 07:50:30.000000 lino-welfare-23.1.0/lino_welfare.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      150 2022-08-24 23:22:25.000000 lino-welfare-23.1.0/requirements-install.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      362 2022-05-25 04:06:50.000000 lino-welfare-23.1.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      164 2017-01-04 05:50:59.000000 lino-welfare-23.1.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      619 2022-10-22 23:43:43.000000 lino-welfare-23.1.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-01-01 07:50:30.841554 lino-welfare-23.1.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      559 2021-04-07 10:22:53.000000 lino-welfare-23.1.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2021-03-07 17:52:34.000000 lino-welfare-23.1.0/tests/test_demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      172 2018-05-03 15:32:38.000000 lino-welfare-23.1.0/tests/test_docs.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/COPYING
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      244 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/MANIFEST.in
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2037 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1130 2023-03-18 07:37:29.000000 lino-welfare-23.6.0/README.rst
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      653 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    21221 2023-04-02 10:55:01.000000 lino-welfare-23.6.0/lino_welfare/migrate.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   193321 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/migrate_old.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/modlib/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      659 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      562 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      984 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2329 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/active_job_search__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare/modlib/aids/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1538 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2458 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/choicelists.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1142 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      890 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       65 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/default.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      713 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      872 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      774 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      575 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      564 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      763 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4798 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      745 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6723 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6340 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    11507 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/mixins.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    27336 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      366 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/aids/roles.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art60/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1138 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/art60/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/art60/config/art60/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art60/config/art60/Contract/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    46358 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art60/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      806 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10776 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art60/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art61/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      983 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1739 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/choicelists.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/art61/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/art61/config/art61/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art61/config/art61/Contract/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     8721 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/art61/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      347 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7238 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/art61/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.058802 lino-welfare-23.6.0/lino_welfare/modlib/badges/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1244 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/badges/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1693 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/badges/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.062801 lino-welfare-23.6.0/lino_welfare/modlib/cal/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      472 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.062801 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1249 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      248 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/Visitor.eml.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1700 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.062801 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       44 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      825 2023-04-27 06:29:51.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/demo2.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       43 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    14042 2023-04-27 06:29:51.000000 lino-welfare-23.6.0/lino_welfare/modlib/cal/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.062801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4120 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3740 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2846 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2075 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    11616 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   139908 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      154 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/README.txt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     8507 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      777 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      933 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4198 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.066801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     9867 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7931 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1042 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.070802 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5622 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13874 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2435 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5569 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5699 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     9421 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    19800 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1361 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.070802 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1600 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4063 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5074 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1146 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.074802 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3334 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2591 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1460 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3450 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3938 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    11981 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.074802 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5436 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6504 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3332 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1119 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1969 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1044 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4562 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3627 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6440 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3491 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2902 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    26504 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.042801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   121083 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2715 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3241 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/choicelists.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    21764 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.078801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    15865 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.082801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      538 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/cbss.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3295 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1961 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2109 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2579 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4542 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1826 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    11618 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    24155 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    26292 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      619 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/democfg.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6081 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20869 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     9170 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/purposes.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2401 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/sectors.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    16822 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    23231 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    25160 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.082801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.082801 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/commands/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/commands/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1895 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    23598 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/mixins.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    26644 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      401 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/roles.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    37959 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/tx25.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     9036 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/ui.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2468 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cbss/utils.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      656 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3449 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1764 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/ui.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/contacts/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      872 2023-03-30 05:52:14.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/contacts/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       49 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       48 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/fixtures/std.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/commands/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/commands/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       70 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/management/commands/garble_persons.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     9487 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/contacts/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/cv/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      479 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.086802 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      945 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7545 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/props.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       48 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5673 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/cv/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/debts/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1551 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4424 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/choicelists.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    17514 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    24679 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    19964 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      661 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fields.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4587 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20553 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/minimal.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      577 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1866 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/mixins.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    22106 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      352 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/roles.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    21350 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/debts/ui.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      824 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.090802 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      420 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/fixtures/demo2.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1924 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/mixins.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1679 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/esf/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      852 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6282 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/choicelists.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/Client/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      742 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      905 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      620 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/esf/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      360 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      482 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5631 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/esf/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/finan/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      381 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/finan/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/finan/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/finan/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      467 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/finan/fixtures/payments.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1969 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/finan/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/households/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      306 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/households/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       51 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       50 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3807 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/households/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.094802 lino-welfare-23.6.0/lino_welfare/modlib/immersion/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1107 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.098802 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   667935 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5587 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.098802 lino-welfare-23.6.0/lino_welfare/modlib/immersion/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1446 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3463 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3921 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/immersion/ui.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.098802 lino-welfare-23.6.0/lino_welfare/modlib/integ/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2406 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.098802 lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     8565 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2470 2023-04-02 10:54:19.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    23997 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      377 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/integ/roles.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/isip/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      351 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      722 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/choicelists.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/isip/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/isip/config/isip/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/isip/config/isip/Contract/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    55172 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    17714 2023-04-02 09:54:45.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/mixins.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    11361 2023-04-02 09:44:08.000000 lino-welfare-23.6.0/lino_welfare/modlib/isip/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      903 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/Contract/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    94813 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     9896 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     9876 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/jobs/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      935 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2930 2023-04-02 09:55:26.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/mixins.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13181 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      327 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/template_messages.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    17073 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/jobs/ui.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.102802 lino-welfare-23.6.0/lino_welfare/modlib/ledger/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      419 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      531 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2758 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3082 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/std_journals.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2438 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/ledger/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      996 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3181 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    16680 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      416 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/newcomers/roles.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/notes/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      282 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.106802 lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      889 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       45 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2462 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/notes/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.110802 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1516 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4420 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/actions.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2558 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/choicelists.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      366 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/client_address.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.110802 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.110802 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    32053 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   157223 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    31905 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      373 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/pac.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      487 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/welcome.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.110802 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2287 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/demo2.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1595 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    36618 2023-04-02 09:58:50.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      509 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/pcsw/roles.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/polls/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      335 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5736 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      328 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/jobsearch.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       51 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      214 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/polls/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/projects/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      619 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/projects/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2069 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/projects/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/reception/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      532 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/reception/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    14505 2023-03-22 06:06:32.000000 lino-welfare-23.6.0/lino_welfare/modlib/reception/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/sales/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sales/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      466 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sales/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/sepa/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      308 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sepa/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/sepa/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sepa/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4013 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sepa/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1603 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/sepa/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/system/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      216 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/system/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4076 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/system/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/users/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      345 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.114802 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       46 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       48 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/demo2.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       52 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/fixtures/demo_users.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2777 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1050 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/users/ui.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.118802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      407 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.118802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.118802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   672907 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      511 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/TasksByClient.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1221 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1146 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      533 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       40 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/default.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      624 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      800 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/integ/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    11787 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      585 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/notes/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/notes/Note/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    50685 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    43393 2023-04-02 10:53:58.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1040 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/demo2.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    29832 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4243 2023-03-05 11:09:30.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3232 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/std2.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    26073 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/help_texts.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.122802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    38241 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   131485 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.126802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    35602 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   130979 2023-04-02 08:02:31.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.046801 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.126802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      409 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    93297 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.126802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4743 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/garble.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4518 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    14642 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    35429 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     5859 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6296 2023-03-31 11:56:45.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/settings.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7612 2023-04-27 06:29:51.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/user_types.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1635 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/welfare/workflows.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1055 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    12127 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    12100 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3037 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20702 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      363 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/modlib/xcourses/roles.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/projects/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      206 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/projects/gerd/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      297 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      415 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/django110_isnull.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      278 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/manage.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1388 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/print_tx25.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.130802 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      342 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      763 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      388 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/doctests.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3046 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7615 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/webdav/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13377 2023-04-05 09:05:00.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       85 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/memory.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1038 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/mysql.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2459 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_aids.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2765 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7909 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_cbss.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2948 2023-04-02 10:54:08.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_clients.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4214 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_debts.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      253 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_restore.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    35630 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_watchtim.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/mathieu/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      365 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      280 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/manage.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      281 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      512 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      347 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/doctests.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.050801 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.134802 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3046 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7615 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       85 2023-02-28 05:23:16.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/memory.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     6890 2023-04-29 06:46:42.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/test_chatelet.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18271 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/test_notify.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/lino_welfare/scripts/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/scripts/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7346 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare/scripts/load_plp.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7750 2023-06-20 12:09:45.000000 lino-welfare-23.6.0/lino_welfare/setup_info.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.054801 lino-welfare-23.6.0/lino_welfare.egg-info/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2037 2023-06-20 12:11:06.000000 lino-welfare-23.6.0/lino_welfare.egg-info/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    17726 2023-06-20 12:11:07.000000 lino-welfare-23.6.0/lino_welfare.egg-info/SOURCES.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-06-20 12:11:06.000000 lino-welfare-23.6.0/lino_welfare.egg-info/dependency_links.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/lino_welfare.egg-info/not-zip-safe
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       60 2023-06-20 12:11:06.000000 lino-welfare-23.6.0/lino_welfare.egg-info/requires.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       13 2023-06-20 12:11:06.000000 lino-welfare-23.6.0/lino_welfare.egg-info/top_level.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      141 2023-03-31 12:17:48.000000 lino-welfare-23.6.0/requirements-install.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      362 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/requirements.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/setup.cfg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      164 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/setup.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      619 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/tasks.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:11:07.138802 lino-welfare-23.6.0/tests/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      559 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/tests/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      457 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/tests/test_demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      172 2023-02-28 05:23:17.000000 lino-welfare-23.6.0/tests/test_docs.py
```

### Comparing `lino-welfare-23.1.0/COPYING` & `lino-welfare-23.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/PKG-INFO` & `lino-welfare-23.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino-welfare
-Version: 23.1.0
+Version: 23.6.0
 Summary: A Lino plugin library for Belgian PCSWs
 Home-page: https://gitlab.com/lino-framework/welfare
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -57,9 +55,7 @@
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
-
-
```

### Comparing `lino-welfare-23.1.0/README.rst` & `lino-welfare-23.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/__init__.py` & `lino-welfare-23.6.0/lino_welfare/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/migrate.py` & `lino-welfare-23.6.0/lino_welfare/migrate.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import datetime
 from decimal import Decimal
 from django.conf import settings
 from lino.utils.dpy import Migrator, override
 from lino.core.utils import resolve_model
 from lino.api import dd, rt
 from lino_xl.lib.sepa.utils import belgian_nban_to_iban_bic
-from lino_xl.lib.cal.choicelists import WORKDAYS
 
 
 SINCE_ALWAYS = datetime.date(1990, 1, 1)
 
 
 def noop(*args):
     return None
```

### Comparing `lino-welfare-23.1.0/lino_welfare/migrate_old.py` & `lino-welfare-23.6.0/lino_welfare/migrate_old.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/active_job_search/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/active_job_search/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/choicelists.py` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/clothing_bank.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/fixed_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/food_bank.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/foreigner_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/furniture.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/heating_refund.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/integ_income.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/medical_refund.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/config/aids/Confirmation/urgent_medical_care.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/mixins.py` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/aids/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/aids/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/art60/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/art60/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/art60/config/art60/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/art60/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/art60/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/art60/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/art60/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -252,16 +252,16 @@
         return qs
 
 
 class ContractsByClient(Contracts):
     required_roles = dd.login_required((SocialUser, SocialCoordinator))
     master_key = 'client'
     auto_fit_column_widths = True
-    no_phantom_row = False  # set back to default behaviour
-    column_names = "applies_from applies_until date_ended duration type user *"
+    no_phantom_row = False  # override ContractBaseTable
+    column_names = "applies_from applies_until date_ended duration type user remark:30 *"
     # hidden_columns = """
     # language contact_person contact_role
     # printed regime schedule hourly_rate
     # date_decided date_issued user_asd exam_policy ending date_ended
     # duration reference_person responsibilities remark
     # """
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/art61/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/art61/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/art61/choicelists.py` & `lino-welfare-23.6.0/lino_welfare/modlib/art61/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/art61/config/art61/Contract/contract.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/art61/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/art61/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/badges/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/badges/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/badges/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/badges/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html` & `lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/Colleague.eml.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/cal/config/cal/Guest/presence_certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cal/fixtures/demo2.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cal/fixtures/demo2.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,18 +2,28 @@
 # Copyright 2013-2021 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 from lino_xl.lib.cal.fixtures.demo2 import objects as lino_objects
 from lino.api import rt
 from lino.utils import Cycler
 
+def walk(obj):
+    if obj is None:
+        pass  # ignore None values
+    elif hasattr(obj, '__iter__'):
+        for o in obj:
+            for so in walk(o):
+                yield so
+    else:
+        yield obj
+
 
 def objects():
     ses = rt.login()
     Client = rt.models.pcsw.Client
     CLIENTS = Cycler(Client.objects.all())
-    for obj in lino_objects():
+    for obj in walk(lino_objects()):
         if obj.__class__.__name__ == 'Event':
             if obj.event_type.invite_client:
                 obj.project = CLIENTS.pop()
         yield obj
         obj.update_guests.run_from_code(ses)
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cal/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cal/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,15 +324,15 @@
     # waiting_since busy_since gone_since
     # outbox.MailsByController
     # """)
     site.modules.cal.Events.set_detail_layout("general more")
     site.modules.cal.Events.add_detail_panel("general", """
     event_type summary project
     start end user assigned_to
-    room priority access_class transparent #rset
+    room priority transparent #rset
     owner workflow_buttons
     description GuestsByEvent
     """, _("General"))
     site.modules.cal.Events.add_detail_panel("more", """
     id created:20 modified:20 state
     outbox.MailsByController #postings.PostingsByController
     """, _("More"))
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd`

 * *Files 11% similar despite different names*

#### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/common/CommonV3.xsd`

```diff
@@ -1,580 +1,601 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- edited with XMLSpy v2008 rel. 2 sp2 (http://www.altova.com) by USER (KSZ-BCSS) -->
-<!-- ============================================================================================================
-         * File Name :   			UnemployementDataV2.xsd
-         * Author :        			Groenveldt Choukri
-         * Owner :            	  	KSZ / CBSS
-         * Creation date :     	22/04/2015
-         * Status :                  Planned
-         * Description :             A service to consult the allowance for a people
-         * Current version :         0.4
-         * Revision History : 
-		                 - 0.2 Update of an enumeration for the family situation (before EMPLOYEE_WITH_DEPENDANTS, now HOUSEHOLDER)
-						 - 0.3 Added new legal context and more data for the payment in the operation consultSituation
-						 - 0.4 Update paidAmount with minimal value 0 in place of 1 and comment cleaning
-						 - 0.5 Suppress enumeration restriction for the legalContext
-						 - 0.6 SanctionType - the sanction period choice become optional
+<!--
+====================================================================================================================================
+	* File Name				: CommonV3.xsd
+	* Author					: Johan Kumps - Peter Van den Bosch
+	* Owner					: Crossroad Bank for Social Security (CBSS)
+	* Domain					: CBSS Registries Public Services
+	* Creation Date			: 31-05-2010
+	* Description				: This XML schema document contains a set of Common XML  type definition and content model fragments for use in CBSS webservices and batch file schema definitions within the CBSS domain. 
+	* Revision History		: 09-03-2011  	String2Type added
+	*														LegalContext added
+	*														DescriptionType refactored + lenght constraint 50 changed to 100
+	*														InformationCustomerType.ticket length constraint 32 changed to 36
+	*														LegalContext + IntegrationContext concepts added
+	*														RuntimeFaultType refactored to CBSSFaultType
+	*														Parameters added to BaseRequestType
+	*                                18-10-2011 		removed String100Type 
+   *                                         				Added InformationNotificationCBSS/InformationNotified
+   *                                         				Increased the max number of occurences of Information in CBSSFaultType from 5 to 15
+	*									25-10-2011	Refactored unbounded business errors to 25
+	*														Refactored SSINType to SsinType
+   *                          09-11-2011 Changed namespace to v3
+   *                                         thorough validation leading to modifications: see CBSS common XSD types.doc
+   *                           18-01-2011          informationNotified: identification renamed to notifiedIdentification (consistency)
+   *                                                          CbeNumberType: changed from 9 or 10 digits, to mandatory 10 digits
+  *                                                          added types for euro amounts, enterprise numbers and business unit numbers
+ *                                                          Removed status and business anomalies from BaseResponseType, as the request fields should be copied in the same order in the response
+*                                20-03-2012        Renamed BaseDescriptionType to DescriptionType, removed old DescriptionType
+*                                                        Removed DescriptionStyleParametersType
+*                                                        Removed RegisterCharacterSetType
+*                                 29-05-2012           Really remove RegisterCharacterSetType
+*								  14-11-2013		Added InformationCBSSBatchType
+*								  04-09-2014		Added SenderReceiverType
+*								  07-01-2015		Added SequenceNumberType
+*								  03-07-2015		Added NssoRegistrationNumberType
+*                                 11-09-2015      Modified NssoRegistrationNumberType to allow both 9 long as temporary 10 long numbers starting with 51.
+*                                 16-09-2015      Modified NssoRegistrationNumberType to 10 long numbers starting with 51 or with 0.
+*                                 08-02-2016      Added StatusOkType
+*                                 27-09-2016      Added YearQuarterType format yyyyQx, QuarterPeriodType and OpenQuarterPeriodType
+*                                 04-04-2018      Added DataFiltersType
+*                                 27-11-2018      Added LocalizedDescription(s)Type
+*                                 04-01-2019      Added SsinWithCanceledAndReplacesStatusType and SsinWithCanceledAndReplacedByStatusType
+====================================================================================================================================
 -->
-<xsd:schema xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://kszbcss.fgov.be/types/UnemploymentData/v2" xmlns:tns="http://kszbcss.fgov.be/types/UnemploymentData/v2" xmlns:common="http://kszbcss.fgov.be/types/common/v3" targetNamespace="http://kszbcss.fgov.be/types/UnemploymentData/v2" elementFormDefault="unqualified" attributeFormDefault="unqualified" version="2016-03-02">
-  <xsd:import namespace="http://kszbcss.fgov.be/types/common/v3" schemaLocation="be/fgov/kszbcss/types/common/CommonV3.xsd"/>
-  <!--=== Provide a detail of the paid allowance by month for a person ===-->
-  <xsd:complexType name="ConsultPaidSumsRequestType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractRequestCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByPeriod"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <xsd:complexType name="ConsultPaidSumsResponseType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractResponseCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByPeriod"/>
-          <xsd:element name="status" type="common:StatusType"/>
-          <xsd:element name="paidSums" type="PaidSumsResponseType" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <!--=== Operation especialy defined in Unemployment - Usually used by PCSA and SPP-IS. ===-->
-  <!--=== It provides more options than the L035 like the concatenation of this rights and payment.  ===-->
-  <xsd:complexType name="ConsultSituationRequestType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractRequestCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByDateType"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <xsd:complexType name="ConsultSituationResponseType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractResponseCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByDateType"/>
-          <xsd:element name="status" type="common:StatusType"/>
-          <xsd:element name="situation" type="SituationType" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <!--=== Provides all information about the rights for a people ===-->
-  <xsd:complexType name="ConsultRightsRequestType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractRequestCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByDateType"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <xsd:complexType name="ConsultRightsResponseType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractResponseCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByDateType"/>
-          <xsd:element name="status" type="common:StatusType"/>
-          <xsd:element name="rights" type="RightsType" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <!--=== Provides all information about the payments for a people === -->
-  <xsd:complexType name="ConsultPaymentsRequestType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractRequestCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByDateType"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <xsd:complexType name="ConsultPaymentsResponseType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractResponseCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByDateType"/>
-          <xsd:element name="status" type="common:StatusType"/>
-          <xsd:element name="payment" type="PaymentType" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <!--=== Provides all information about activation payments  ===-->
-  <xsd:complexType name="ConsultActivationPaidSumsRequestType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractRequestCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByQuarterForActivationPaidExtentedType"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <xsd:complexType name="ConsultActivationPaidSumsResponseType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractResponseCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByQuarterForActivationPaidExtentedType"/>
-          <xsd:element name="status" type="common:StatusType"/>
-          <xsd:element name="activationAllowances" type="ActivationAllowancesType" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <!--=== Provides a grid than contains the detail of allowance by allowance paid day ===-->
-  <xsd:complexType name="ConsultScheduledPaymentRequestType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractRequestCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByQuarterBaseType"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <xsd:complexType name="ConsultScheduledPaymentResponseType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractResponseCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByQuarterBaseType"/>
-          <xsd:element name="status" type="common:StatusType"/>
-          <xsd:element name="scheduledPayment" type="ScheduledPaymentType" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <!--=== Provides a all information about carreer interruptions ===-->
-  <xsd:complexType name="ConsultCareerBreakRequestType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractRequestCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByPeriodForCareerInterruptionAndCreditTimeType"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <xsd:complexType name="ConsultCareerBreakResponseType">
-    <xsd:complexContent>
-      <xsd:extension base="AbstractResponseCustomerType">
-        <xsd:sequence>
-          <xsd:element name="searchCriteria" type="SearchCriteriaByPeriodForCareerInterruptionAndCreditTimeType"/>
-          <xsd:element name="status" type="common:StatusType"/>
-          <xsd:element name="careerBreaks" type="CareerBreaksType" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <!--=== Redefined common type  ===-->
-  <xsd:complexType name="AbstractRequestCustomerType" abstract="true">
+<xsd:schema xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:tns="http://kszbcss.fgov.be/types/common/v3" targetNamespace="http://kszbcss.fgov.be/types/common/v3" elementFormDefault="unqualified" attributeFormDefault="unqualified" version="3.3-45">
+  <!-- Request / response meta data -->
+  <xsd:simpleType name="SeverityType">
+    <xsd:restriction base="xsd:string">
+      <xsd:enumeration value="INFORMATION"/>
+      <xsd:enumeration value="WARNING"/>
+      <xsd:enumeration value="FATAL"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="UUIDType">
+    <xsd:restriction base="xsd:string">
+      <xsd:pattern value="[\da-fA-F]{8}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{4}-[\da-fA-F]{12}"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="TicketType">
+    <xsd:restriction base="xsd:string">
+      <xsd:maxLength value="36"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="CbeNumberType">
     <xsd:annotation>
-      <xsd:documentation>Base complex type for all request messages.</xsd:documentation>
+      <xsd:documentation>CBE number identifying an enterprise or business unit</xsd:documentation>
     </xsd:annotation>
-    <xsd:sequence>
-      <xsd:element name="informationCustomer" type="common:InformationCustomerType"/>
-      <xsd:element name="informationCBSS" type="common:InformationCBSSType" minOccurs="0"/>
-      <xsd:element name="legalContext" type="UnemploymentDataLegalContextType"/>
-    </xsd:sequence>
-  </xsd:complexType>
-  <xsd:complexType name="AbstractResponseCustomerType" abstract="true">
+    <xsd:restriction base="xsd:string">
+      <xsd:pattern value="\d{10}"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="EnterpriseNumberType">
+    <xsd:annotation>
+      <xsd:documentation>CBE enterprise number (starting with 0 or 1)</xsd:documentation>
+    </xsd:annotation>
+    <xsd:restriction base="xsd:string">
+      <xsd:pattern value="[0-1]\d{9}"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="BusinessUnitNumberType">
+    <xsd:annotation>
+      <xsd:documentation>CBE business unit number (starting with 2-8)</xsd:documentation>
+    </xsd:annotation>
+    <xsd:restriction base="xsd:string">
+      <xsd:pattern value="[2-8]\d{9}"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="SsinType">
+    <xsd:restriction base="xsd:string">
+      <xsd:pattern value="[0-9][0-9](([0][0-9])|([1][0-2]))(([0-2][0-9])|([3][0-1]))(([0-9]{2}[1-9])|([0-9][1-9][0-9])|([1-9][0-9]{2}))(([0-8][0-9])|([9][0-7]))">
+        <xsd:annotation>
+          <xsd:documentation xml:lang="FR">Registre National</xsd:documentation>
+          <xsd:documentation xml:lang="NL">Rijksregister</xsd:documentation>
+        </xsd:annotation>
+      </xsd:pattern>
+      <xsd:pattern value="[0-9][0-9](([2][0-9])|([3][0-2]))(([0-2][0-9])|([3][0-1]))[0-9]{3}(([0-8][0-9])|([9][0-7]))">
+        <xsd:annotation>
+          <xsd:documentation xml:lang="FR">Registre Bis : numero Bis</xsd:documentation>
+          <xsd:documentation xml:lang="NL">Bis register : Bisnummer</xsd:documentation>
+        </xsd:annotation>
+      </xsd:pattern>
+      <xsd:pattern value="[0-9][0-9](([4][0-9])|([5][0-2]))(([0-2][0-9])|([3][0-1]))[0-9]{3}(([0-8][0-9])|([9][0-7]))">
+        <xsd:annotation>
+          <xsd:documentation xml:lang="FR">Registre Bis : numero TER</xsd:documentation>
+          <xsd:documentation xml:lang="NL">Bisregister : Ternummer</xsd:documentation>
+        </xsd:annotation>
+      </xsd:pattern>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="LegalContextType">
+    <xsd:restriction base="xsd:string">
+      <xsd:maxLength value="64"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="IntegrationContextType">
     <xsd:annotation>
-      <xsd:documentation>Base complex type for all request messages.</xsd:documentation>
+      <xsd:documentation>deprecated type. Use InscriptionContextType instead in new XSDs</xsd:documentation>
+    </xsd:annotation>
+    <xsd:restriction base="xsd:string">
+      <xsd:maxLength value="64"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="InscriptionContextType">
+    <xsd:annotation>
+      <xsd:documentation>The way in which an organization knows a person (textual equivalent of former numerical quality code)</xsd:documentation>
+    </xsd:annotation>
+    <xsd:restriction base="xsd:string">
+      <xsd:maxLength value="64"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="SequenceNumberType">
+    <xsd:restriction base="xsd:long">
+      <xsd:minInclusive value="1"/>
+      <xsd:totalDigits value="15"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:complexType name="InformationCBSSType">
+    <xsd:annotation>
+      <xsd:documentation>Information block from CBSS.</xsd:documentation>
     </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="informationCustomer" type="common:InformationCustomerType"/>
-      <xsd:element name="informationCBSS" type="common:InformationCBSSType"/>
-      <xsd:element name="legalContext" type="UnemploymentDataLegalContextType"/>
+      <xsd:element name="ticketCBSS" type="tns:UUIDType"/>
+      <xsd:element name="timestampReceive" type="xsd:dateTime">
+        <xsd:annotation>
+          <xsd:documentation>Time request was received by CBSS.</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
+      <xsd:element name="timestampReply" type="xsd:dateTime">
+        <xsd:annotation>
+          <xsd:documentation>Time reply was sent by CBSS.</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
     </xsd:sequence>
   </xsd:complexType>
-  <!--=== Redefined searchCriteriaType - Different time criteria are needed for all the operations ===-->
-  <xsd:complexType name="SearchCriteriaByDateType">
+  <xsd:complexType name="InformationCustomerType">
+    <xsd:annotation>
+      <xsd:documentation>Information block that can be used by the customer for diagnostic use.</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="ssin" type="common:SsinType"/>
-      <xsd:element name="date" type="xsd:date" minOccurs="0">
+      <xsd:element name="ticket" type="tns:TicketType" minOccurs="0">
         <xsd:annotation>
-          <xsd:documentation>In the case where the date is not defined the last situation found is searched</xsd:documentation>
+          <xsd:documentation>Client can assign their own ticket reference for the request. Not mandatory. For non-UUID tickets only the first 32 chars are stored at CBSS.</xsd:documentation>
         </xsd:annotation>
       </xsd:element>
+      <xsd:element name="timestampSent" type="xsd:dateTime" minOccurs="0">
+        <xsd:annotation>
+          <xsd:documentation>Timestamp when client sent request.</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
+      <xsd:element name="customerIdentification" type="tns:OrganizationIdentificationType"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="SearchCriteriaByQuarterBaseType">
+  <xsd:complexType name="InformationSupplierType">
+    <xsd:annotation>
+      <xsd:documentation>Information block for supplier of a service</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="ssin" type="common:SsinType"/>
-      <xsd:element name="quarterCriteria" type="QuarterCriteriaType"/>
+      <xsd:element name="ticket" type="tns:TicketType" minOccurs="0">
+        <xsd:annotation>
+          <xsd:documentation>UUID generated by Customer or Supplier</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
+      <xsd:element name="timestampReceive" type="xsd:dateTime" minOccurs="0">
+        <xsd:annotation>
+          <xsd:documentation>Time of request</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
+      <xsd:element name="timestampReply" type="xsd:dateTime" minOccurs="0">
+        <xsd:annotation>
+          <xsd:documentation>Time of request</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
+      <xsd:element name="supplierIdentification" type="tns:OrganizationIdentificationType"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="SearchCriteriaByQuarterForActivationPaidExtentedType">
-    <xsd:complexContent>
-      <xsd:extension base="SearchCriteriaByQuarterBaseType">
-        <xsd:sequence>
-          <xsd:element name="allAllowance" type="AllAllowanceType" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
-  </xsd:complexType>
-  <xsd:complexType name="SearchCriteriaByPeriod">
+  <xsd:complexType name="InformationNotificationCBSSType">
+    <xsd:annotation>
+      <xsd:documentation>Deprecated type. Use SenderReceiverType in new batch XSDs. Information block for CBSS info when CBSS notifies partner</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="ssin" type="common:SsinType"/>
-      <xsd:element name="period" type="common:PeriodType"/>
-      <xsd:element name="allAllowance" type="AllAllowanceType" minOccurs="0"/>
+      <xsd:element name="ticketCBSS" type="tns:UUIDType">
+        <xsd:annotation>
+          <xsd:documentation>UUID generated by Customer or Supplier</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
+      <xsd:element name="timestampSent" type="xsd:dateTime">
+        <xsd:annotation>
+          <xsd:documentation>Time of request</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="SearchCriteriaByPeriodForCareerInterruptionAndCreditTimeType">
+  <xsd:complexType name="InformationNotifiedType">
+    <xsd:annotation>
+      <xsd:documentation>Deprecated type. Use SenderReceiverType in new batch XSDs. Information block for partner info when CBSS notifies partner</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="ssin" type="common:SsinType"/>
-      <xsd:element name="period" type="common:PeriodType"/>
+      <xsd:element name="ticket" type="tns:TicketType" minOccurs="0"/>
+      <xsd:element name="timestampReply" type="xsd:dateTime" minOccurs="0"/>
+      <xsd:element name="notifiedIdentification" type="tns:OrganizationIdentificationType"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="QuarterCriteriaType">
+  <xsd:complexType name="InformationCBSSBatchType">
+    <xsd:annotation>
+      <xsd:documentation>Deprecated type. Use SenderReceiverType in new batch XSDs</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="quarter" type="QuarterType"/>
-      <xsd:element name="year" type="xsd:gYear"/>
+      <xsd:element name="fileId" type="xsd:unsignedLong"/>
+      <xsd:element name="fileCreationTimestamp" type="xsd:dateTime"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="PaidSumsResponseType">
+  <xsd:complexType name="SenderReceiverType">
+    <xsd:annotation>
+      <xsd:documentation>Information block containing info about the sender or receiver of a message.</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="paidSum" type="PaidSumType" maxOccurs="48">
+      <xsd:element name="ticket" type="tns:TicketType" minOccurs="0">
         <xsd:annotation>
-          <xsd:documentation>If any the paidAmount is lower than 1 the tag is skipped</xsd:documentation>
+          <xsd:documentation>The partner can assign a ticket reference to the message. Not mandatory.</xsd:documentation>
         </xsd:annotation>
       </xsd:element>
-    </xsd:sequence>
-  </xsd:complexType>
-  <xsd:complexType name="SanctionType">
-    <xsd:sequence>
-      <xsd:element name="beginDate" type="xsd:date"/>
-      <xsd:choice minOccurs="0">
+      <xsd:element name="timestampSent" type="xsd:dateTime" minOccurs="0">
         <xsd:annotation>
-          <xsd:documentation>Only one of these fields may be filled</xsd:documentation>
+          <xsd:documentation>Timestamp when message was sent. In the receiver block of response messages the timestampSent is the timestamp when the request was created by the organization that receives the response.</xsd:documentation>
         </xsd:annotation>
-        <xsd:element name="endDate" type="xsd:date"/>
-        <xsd:element name="nbrOfWeeksSanction">
+      </xsd:element>
+      <xsd:element name="organizationIdentification" type="tns:OrganizationIdentificationType"/>
+    </xsd:sequence>
+  </xsd:complexType>
+  <xsd:complexType name="OrganizationIdentificationType">
+    <xsd:choice>
+      <xsd:element name="cbeNumber" type="tns:CbeNumberType"/>
+      <xsd:sequence>
+        <xsd:element name="sector">
           <xsd:simpleType>
-            <xsd:restriction base="xsd:int">
-              <xsd:minInclusive value="1"/>
+            <xsd:restriction base="xsd:unsignedShort">
               <xsd:maxInclusive value="999"/>
             </xsd:restriction>
           </xsd:simpleType>
         </xsd:element>
-      </xsd:choice>
-      <xsd:element name="article" type="ArticleCode" minOccurs="0"/>
-    </xsd:sequence>
+        <xsd:element name="institution">
+          <xsd:simpleType>
+            <xsd:restriction base="xsd:unsignedShort">
+              <xsd:maxInclusive value="999"/>
+            </xsd:restriction>
+          </xsd:simpleType>
+        </xsd:element>
+      </xsd:sequence>
+    </xsd:choice>
   </xsd:complexType>
-  <xsd:complexType name="ExclusionType">
+  <xsd:complexType name="OpenPeriodType">
+    <xsd:annotation>
+      <xsd:documentation>Period containing a begin date and an optional end date.</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="beginDate" type="xsd:date"/>
+      <xsd:element name="endDate" type="xsd:date" minOccurs="0"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="RightsEndType">
+  <xsd:complexType name="PeriodType">
+    <xsd:annotation>
+      <xsd:documentation>Period containing a begin date and an end date.</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="beginDate" type="xsd:date"/>
+      <xsd:element name="endDate" type="xsd:date"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="NoRightType">
-    <xsd:complexContent>
-      <xsd:extension base="NoRightBaseType">
-        <xsd:sequence>
-          <xsd:element name="admissibilityArticle" minOccurs="0" maxOccurs="6">
-            <xsd:simpleType>
-              <xsd:restriction base="xsd:string">
-                <xsd:minLength value="1"/>
-                <xsd:maxLength value="8"/>
-              </xsd:restriction>
-            </xsd:simpleType>
-          </xsd:element>
-          <xsd:element name="indemnisabilityArticle" minOccurs="0" maxOccurs="6">
-            <xsd:simpleType>
-              <xsd:restriction base="xsd:string">
-                <xsd:minLength value="1"/>
-                <xsd:maxLength value="8"/>
-              </xsd:restriction>
-            </xsd:simpleType>
-          </xsd:element>
-          <xsd:element name="triggerDate" type="xsd:date" minOccurs="0"/>
-        </xsd:sequence>
-      </xsd:extension>
-    </xsd:complexContent>
+  <xsd:complexType name="OpenQuarterPeriodType">
+    <xsd:annotation>
+      <xsd:documentation>Quarter period containing a quarter begin date and an optional quarter end date.</xsd:documentation>
+    </xsd:annotation>
+    <xsd:sequence>
+      <xsd:element name="beginQuarter" type="tns:YearQuarterType"/>
+      <xsd:element name="endQuarter" type="tns:YearQuarterType" minOccurs="0"/>
+    </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="NoRightBaseType">
-    <xsd:choice>
-      <xsd:annotation>
-        <xsd:documentation>Only one of these fields may be filled</xsd:documentation>
-      </xsd:annotation>
-      <xsd:element name="sanction" type="SanctionType"/>
-      <xsd:element name="exclusion" type="ExclusionType"/>
-      <xsd:element name="rightsEnd" type="RightsEndType"/>
-    </xsd:choice>
+  <xsd:complexType name="QuarterPeriodType">
+    <xsd:annotation>
+      <xsd:documentation>Quarter period containing a quarter begin date and a quarter end date.</xsd:documentation>
+    </xsd:annotation>
+    <xsd:sequence>
+      <xsd:element name="beginQuarter" type="tns:YearQuarterType"/>
+      <xsd:element name="endQuarter" type="tns:YearQuarterType"/>
+    </xsd:sequence>
+  </xsd:complexType>
+  <xsd:simpleType name="YearQuarterType">
+    <xsd:restriction base="xsd:string">
+      <xsd:length value="6"/>
+      <xsd:whiteSpace value="collapse"/>
+      <xsd:pattern value="[1-2]\d{3}Q(1|2|3|4)"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="IncompleteDateType">
+    <xsd:annotation>
+      <xsd:documentation>A possibly incomplete date. Format yyyy-mm-dd, yyyy-mm-00 or yyyy-00-00</xsd:documentation>
+    </xsd:annotation>
+    <xsd:restriction base="xsd:string">
+      <xsd:length value="10"/>
+      <xsd:whiteSpace value="collapse"/>
+      <xsd:pattern value="[0-2][0-9]{3}\-[0-1][0-9]\-[0-3][0-9]"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="DescriptionType">
+    <xsd:restriction base="xsd:string">
+      <xsd:maxLength value="100"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:simpleType name="LanguageType">
+    <xsd:annotation>
+      <xsd:documentation>Type specifying the language of a given value</xsd:documentation>
+    </xsd:annotation>
+    <xsd:restriction base="xsd:string">
+      <xsd:enumeration value="NL"/>
+      <xsd:enumeration value="FR"/>
+      <xsd:enumeration value="DE"/>
+    </xsd:restriction>
+  </xsd:simpleType>
+  <xsd:complexType name="LocalizedDescriptionType">
+    <xsd:simpleContent>
+      <xsd:extension base="tns:DescriptionType">
+        <xsd:attribute name="language" type="tns:LanguageType" use="optional"/>
+      </xsd:extension>
+    </xsd:simpleContent>
   </xsd:complexType>
-  <xsd:complexType name="RightType">
+  <xsd:complexType name="LocalizedDescriptionsType">
     <xsd:sequence>
-      <xsd:element name="theoricDailyAllowanceAmount" type="EurocentGreaterEqualZeroAmountType"/>
-      <xsd:element name="rightStartingDate" type="xsd:date"/>
-      <xsd:element name="unemploymentCode">
-        <xsd:simpleType>
-          <xsd:restriction base="xsd:int">
-            <xsd:minInclusive value="0"/>
-            <xsd:maxInclusive value="99"/>
-          </xsd:restriction>
-        </xsd:simpleType>
-      </xsd:element>
-      <xsd:element name="familyState" minOccurs="0">
-        <xsd:simpleType>
-          <xsd:restriction base="xsd:string">
-            <xsd:enumeration value="SOLITARY"/>
-            <xsd:enumeration value="COHABITING"/>
-            <xsd:enumeration value="HOUSEHOLDER"/>
-          </xsd:restriction>
-        </xsd:simpleType>
-      </xsd:element>
-      <xsd:element name="indemnificationRegime" type="IndemnificationRegimeType" minOccurs="0"/>
-      <xsd:element name="unemployedWorkerStatus" type="UnemployedWorkerStatus" minOccurs="0"/>
-      <xsd:element name="theoricRightsEndingDate" type="xsd:date" minOccurs="0"/>
-      <xsd:element name="selfEmploymentSupplement" type="xsd:boolean" minOccurs="0"/>
+      <xsd:element name="description" type="tns:LocalizedDescriptionType" maxOccurs="3"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="PaymentType">
+  <xsd:complexType name="DataFiltersType">
+    <xsd:annotation>
+      <xsd:documentation>Type indicating which data elements have been filtered</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="paidMonth" type="xsd:gYearMonth"/>
-      <xsd:element name="theoricDailyAllowanceAmount" type="EurocentGreaterEqualZeroAmountType"/>
-      <xsd:element name="nbrOfAllowances" type="NbrOfAllowanceType" minOccurs="0"/>
-      <xsd:element name="unemploymentCode">
-        <xsd:simpleType>
-          <xsd:restriction base="xsd:int">
-            <xsd:minInclusive value="0"/>
-            <xsd:maxInclusive value="99"/>
-          </xsd:restriction>
-        </xsd:simpleType>
-      </xsd:element>
-      <xsd:element name="indemnificationRegime" type="IndemnificationRegimeType" minOccurs="0"/>
+      <xsd:element name="filteredElement" type="xsd:string" maxOccurs="unbounded"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="SituationType">
+  <!-- Errors and warnings structures -->
+  <xsd:group name="BusinessAnomaliesContentFragment">
+    <xsd:annotation>
+      <xsd:documentation>Structure reporting business errors to the consumer</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="payment" type="PaymentType" minOccurs="0"/>
-      <xsd:element name="rights" type="RightsType" minOccurs="0"/>
+      <xsd:element name="businessAnomalies" type="tns:BusinessAnomaliesType" minOccurs="0"/>
+    </xsd:sequence>
+  </xsd:group>
+  <xsd:complexType name="BusinessAnomaliesType">
+    <xsd:annotation>
+      <xsd:documentation>Type defining the structure of the part of the response containing business Faults</xsd:documentation>
+    </xsd:annotation>
+    <xsd:sequence>
+      <xsd:element name="businessAnomaly" type="tns:BusinessAnomalyType" maxOccurs="25"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="PaidSumType">
+  <xsd:complexType name="BusinessAnomalyType">
+    <xsd:annotation>
+      <xsd:documentation>Type defining the structure of one business Faults</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="relatedMonth" type="xsd:gYearMonth"/>
-      <xsd:element name="paidAmount" type="EurocentGreaterEqualZeroAmountType"/>
-      <xsd:element name="acceptedAmount" type="EurocentGreaterEqualZeroAmountType" minOccurs="0">
+      <xsd:element name="code" type="xsd:string">
         <xsd:annotation>
-          <xsd:documentation>Defined only when the dossierStatus has the value 1 or 2</xsd:documentation>
+          <xsd:documentation>Unique code referring to a description of this Fault</xsd:documentation>
         </xsd:annotation>
       </xsd:element>
-      <xsd:element name="dossierStatus" type="DossierStatusType"/>
-      <xsd:element name="nbrOfAllowances" type="NbrOfAllowanceType" minOccurs="0"/>
-    </xsd:sequence>
-  </xsd:complexType>
-  <xsd:complexType name="RightsType">
-    <xsd:choice>
-      <xsd:annotation>
-        <xsd:documentation>Only one of these fields may be filled</xsd:documentation>
-      </xsd:annotation>
-      <xsd:element name="right" type="RightType" maxOccurs="2"/>
-      <xsd:element name="noRight" type="NoRightType"/>
-    </xsd:choice>
-  </xsd:complexType>
-  <xsd:complexType name="ActivationAllowanceType">
-    <xsd:sequence>
-      <xsd:element name="paymentMonth" type="xsd:gYearMonth"/>
-      <xsd:element name="activationAllowanceAmount" type="EurocentGreaterEqualZeroAmountType"/>
-      <xsd:element name="activationAllowanceCode" minOccurs="0">
+      <xsd:element name="severity" type="tns:SeverityType"/>
+      <xsd:element name="description">
+        <xsd:annotation>
+          <xsd:documentation>Some description of this Fault</xsd:documentation>
+        </xsd:annotation>
         <xsd:simpleType>
           <xsd:restriction base="xsd:string">
-            <xsd:maxLength value="10"/>
-            <xsd:minLength value="1"/>
+            <xsd:maxLength value="256"/>
           </xsd:restriction>
         </xsd:simpleType>
       </xsd:element>
+      <xsd:element name="information" type="tns:InformationType" minOccurs="0" maxOccurs="15"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="EmployersType">
-    <xsd:sequence maxOccurs="5">
-      <xsd:element name="cbeNumber" type="common:CbeNumberType"/>
-    </xsd:sequence>
-  </xsd:complexType>
-  <xsd:complexType name="ActivationAllowancesType">
+  <xsd:complexType name="CBSSFaultType">
     <xsd:sequence>
-      <xsd:element name="activationAllowance" type="ActivationAllowanceType" maxOccurs="3"/>
-      <xsd:element name="employers" type="EmployersType"/>
+      <xsd:element name="informationCustomer" type="tns:InformationCustomerType" minOccurs="0"/>
+      <xsd:element name="informationCBSS" type="tns:InformationCBSSType"/>
+      <xsd:element name="detail" type="tns:MessageType" maxOccurs="30"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="CareerBreakType">
+  <xsd:complexType name="MessageType">
     <xsd:sequence>
-      <xsd:element name="beginDate" type="xsd:date"/>
-      <xsd:element name="endDate" type="xsd:date"/>
-      <xsd:element name="complementaryActivityCode" type="ComplementaryActivityType" minOccurs="0"/>
-      <xsd:element name="careerBreakCode" minOccurs="0">
+      <xsd:element name="severity" type="tns:SeverityType"/>
+      <xsd:element name="reasonCode">
         <xsd:simpleType>
           <xsd:restriction base="xsd:string">
-            <xsd:maxLength value="2"/>
-            <xsd:minLength value="1"/>
+            <xsd:maxLength value="16"/>
           </xsd:restriction>
         </xsd:simpleType>
       </xsd:element>
-      <xsd:element name="allowanceAmount" type="EurocentGreaterEqualZeroAmountType" minOccurs="0"/>
-      <xsd:element name="careerBreakType" minOccurs="0">
+      <xsd:element name="diagnostic">
         <xsd:simpleType>
           <xsd:restriction base="xsd:string">
-            <xsd:length value="1"/>
+            <xsd:maxLength value="256"/>
           </xsd:restriction>
         </xsd:simpleType>
       </xsd:element>
-      <xsd:element name="careerBreakReason" minOccurs="0">
+      <xsd:element name="authorCode">
         <xsd:simpleType>
           <xsd:restriction base="xsd:string">
-            <xsd:length value="1"/>
+            <xsd:maxLength value="64"/>
           </xsd:restriction>
         </xsd:simpleType>
       </xsd:element>
+      <xsd:element name="information" type="tns:InformationType" minOccurs="0" maxOccurs="15"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="CareerBreaksType">
+  <xsd:complexType name="InformationType">
+    <xsd:sequence>
+      <xsd:element name="fieldName">
+        <xsd:simpleType>
+          <xsd:restriction base="xsd:string">
+            <xsd:maxLength value="64"/>
+          </xsd:restriction>
+        </xsd:simpleType>
+      </xsd:element>
+      <xsd:element name="fieldValue" minOccurs="0">
+        <xsd:simpleType>
+          <xsd:restriction base="xsd:string">
+            <xsd:maxLength value="256"/>
+          </xsd:restriction>
+        </xsd:simpleType>
+      </xsd:element>
+    </xsd:sequence>
+  </xsd:complexType>
+  <!--Base types for most common request/response format for consultation type operations. Can be used to define request and response types with extension type inheritance. Don't use if it doesn't fit the requirements.  -->
+  <xsd:complexType name="BaseRequestType" abstract="true">
+    <xsd:annotation>
+      <xsd:documentation>Type defining the base structure for all service requests</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="benifitiaryInformation" type="BenifitiaryInformationType"/>
-      <xsd:element name="careerBreak" type="CareerBreakType" minOccurs="0" maxOccurs="50"/>
+      <xsd:element name="informationCustomer" type="tns:InformationCustomerType"/>
+      <xsd:element name="informationCBSS" type="tns:InformationCBSSType" minOccurs="0"/>
+      <xsd:element name="legalContext" type="tns:LegalContextType">
+        <xsd:annotation>
+          <xsd:documentation>legal context under which the request was made</xsd:documentation>
+        </xsd:annotation>
+      </xsd:element>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="BenifitiaryInformationType">
+  <xsd:complexType name="BaseResponseType" abstract="true">
+    <xsd:annotation>
+      <xsd:documentation>Type defining the base structure for all service responses</xsd:documentation>
+    </xsd:annotation>
     <xsd:sequence>
-      <xsd:element name="ssin" type="common:SsinType"/>
-      <xsd:element name="creationDate" type="xsd:date"/>
+      <xsd:element name="informationCustomer" type="tns:InformationCustomerType"/>
+      <xsd:element name="informationCBSS" type="tns:InformationCBSSType"/>
+      <xsd:element name="legalContext" type="tns:LegalContextType"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="DailyDataType">
+  <!-- Commonly used status type for consultation type operations. Define another if it doesn't fit requirements.-->
+  <xsd:complexType name="StatusType">
     <xsd:sequence>
-      <xsd:element name="day">
+      <xsd:element name="value">
+        <xsd:annotation>
+          <xsd:documentation>global status of the result</xsd:documentation>
+        </xsd:annotation>
         <xsd:simpleType>
-          <xsd:restriction base="xsd:int">
-            <xsd:maxInclusive value="31"/>
-            <xsd:minInclusive value="1"/>
+          <xsd:restriction base="xsd:string">
+            <xsd:enumeration value="DATA_FOUND"/>
+            <xsd:enumeration value="NO_DATA_FOUND"/>
+            <xsd:enumeration value="NO_RESULT"/>
           </xsd:restriction>
         </xsd:simpleType>
       </xsd:element>
-      <xsd:element name="unemploymentCode">
+      <xsd:element name="code">
+        <xsd:annotation>
+          <xsd:documentation>the code of the status</xsd:documentation>
+        </xsd:annotation>
         <xsd:simpleType>
-          <xsd:restriction base="xsd:int">
-            <xsd:minInclusive value="0"/>
-            <xsd:maxInclusive value="99"/>
+          <xsd:restriction base="xsd:string">
+            <xsd:maxLength value="16"/>
           </xsd:restriction>
         </xsd:simpleType>
       </xsd:element>
-    </xsd:sequence>
-  </xsd:complexType>
-  <xsd:complexType name="MonthlyDataType">
-    <xsd:sequence>
-      <xsd:element name="month">
+      <xsd:element name="description" minOccurs="0">
+        <xsd:annotation>
+          <xsd:documentation>the description of the status</xsd:documentation>
+        </xsd:annotation>
         <xsd:simpleType>
-          <xsd:restriction base="xsd:int">
-            <xsd:minInclusive value="1"/>
-            <xsd:maxInclusive value="12"/>
+          <xsd:restriction base="xsd:string">
+            <xsd:maxLength value="256"/>
           </xsd:restriction>
         </xsd:simpleType>
       </xsd:element>
-      <xsd:element name="dailyData" type="DailyDataType" maxOccurs="31"/>
+      <xsd:element name="information" type="tns:InformationType" minOccurs="0" maxOccurs="15"/>
     </xsd:sequence>
   </xsd:complexType>
-  <xsd:complexType name="ScaleDataType">
+  <!-- Commonly used status type for ok/nok type operations like notifications. Don't use if it doesn't fit requirements.-->
+  <xsd:complexType name="StatusOkType">
     <xsd:sequence>
-      <xsd:element name="scaleCode">
+      <xsd:element name="value">
+        <xsd:annotation>
+          <xsd:documentation>global status of the result</xsd:documentation>
+        </xsd:annotation>
         <xsd:simpleType>
           <xsd:restriction base="xsd:string">
-            <xsd:maxLength value="10"/>
+            <xsd:enumeration value="OK"/>
+            <xsd:enumeration value="NOK"/>
           </xsd:restriction>
         </xsd:simpleType>
       </xsd:element>
-      <xsd:element name="validityDate" type="xsd:date"/>
-    </xsd:sequence>
-  </xsd:complexType>
-  <xsd:complexType name="ScheduledPaymentType">
-    <xsd:sequence>
-      <xsd:element name="monthlyData" type="MonthlyDataType" maxOccurs="3"/>
-      <xsd:element name="scaleData" type="ScaleDataType" maxOccurs="12"/>
+      <xsd:element name="code">
+        <xsd:annotation>
+          <xsd:documentation>the code of the status</xsd:documentation>
+        </xsd:annotation>
+        <xsd:simpleType>
+          <xsd:restriction base="xsd:string">
+            <xsd:maxLength value="16"/>
+          </xsd:restriction>
+        </xsd:simpleType>
+      </xsd:element>
+      <xsd:element name="description" minOccurs="0">
+        <xsd:annotation>
+          <xsd:documentation>the description of the status</xsd:documentation>
+        </xsd:annotation>
+        <xsd:simpleType>
+          <xsd:restriction base="xsd:string">
+            <xsd:maxLength value="256"/>
+          </xsd:restriction>
+        </xsd:simpleType>
+      </xsd:element>
+      <xsd:element name="information" type="tns:InformationType" minOccurs="0" maxOccurs="15"/>
     </xsd:sequence>
   </xsd:complexType>
-  <!--=== Simple with all the legal context usable for this service ===-->
-  <xsd:simpleType name="UnemploymentDataLegalContextType">
-    <xsd:restriction base="xsd:string">
-      <xsd:minLength value="1"/>
-    </xsd:restriction>
-  </xsd:simpleType>
-  <!--=== Boolean than defined if the client want all the allowance ===-->
-  <xsd:simpleType name="AllAllowanceType">
-    <xsd:restriction base="xsd:int">
-      <xsd:minInclusive value="0"/>
-      <xsd:maxInclusive value="1"/>
-    </xsd:restriction>
-  </xsd:simpleType>
-  <xsd:simpleType name="EurocentGreaterThanZeroAmountType">
-    <xsd:annotation>
-      <xsd:documentation>Eurocent Amount in interval [1,9999999]</xsd:documentation>
-    </xsd:annotation>
-    <xsd:restriction base="common:EurocentPositiveAmountType">
-      <xsd:minInclusive value="1"/>
-      <xsd:maxExclusive value="10000000"/>
-    </xsd:restriction>
-  </xsd:simpleType>
-  <xsd:simpleType name="EurocentGreaterEqualZeroAmountType">
-    <xsd:annotation>
-      <xsd:documentation>Eurocent Amount in interval [0,9999999]</xsd:documentation>
-    </xsd:annotation>
-    <xsd:restriction base="common:EurocentPositiveAmountType">
-      <xsd:minInclusive value="0"/>
-      <xsd:maxExclusive value="10000000"/>
-    </xsd:restriction>
-  </xsd:simpleType>
-  <xsd:simpleType name="DossierStatusType">
-    <xsd:annotation>
-      <xsd:documentation>Type defining the status of the payment concerning the month</xsd:documentation>
-    </xsd:annotation>
-    <xsd:restriction base="xsd:string">
-      <xsd:enumeration value="COMPLETED"/>
-      <xsd:enumeration value="PROVISIONAL"/>
-      <xsd:enumeration value="NOT_STARTED"/>
-    </xsd:restriction>
-  </xsd:simpleType>
-  <xsd:simpleType name="NbrOfAllowanceType">
-    <xsd:annotation>
-      <xsd:documentation>Type defining the number of benefits received [0,99.5]. Is an integer or integer+0.5</xsd:documentation>
-    </xsd:annotation>
+  <xsd:simpleType name="EuroPositiveAmountType">
     <xsd:restriction base="xsd:decimal">
-      <xsd:minInclusive value="0"/>
-      <xsd:maxInclusive value="99.5"/>
-      <xsd:pattern value="[\d]*([\.]5|.0)?"/>
+      <xsd:fractionDigits value="2"/>
+      <xsd:maxExclusive value="1000000000000000"/>
     </xsd:restriction>
   </xsd:simpleType>
-  <xsd:simpleType name="IndemnificationRegimeType">
-    <xsd:annotation>
-      <xsd:documentation>Type defining the regime of benefits [0.5,6] and with a decimal value rounded to 0.0 or 0.5</xsd:documentation>
-    </xsd:annotation>
+  <xsd:simpleType name="EuroAmountType">
     <xsd:restriction base="xsd:decimal">
-      <xsd:pattern value="[\d]*([\.]5|.0)?"/>
+      <xsd:fractionDigits value="2"/>
+      <xsd:maxExclusive value="1000000000000000"/>
+      <xsd:minExclusive value="-1000000000000000"/>
     </xsd:restriction>
   </xsd:simpleType>
-  <xsd:simpleType name="ComplementaryActivityType">
-    <xsd:restriction base="xsd:string">
-      <xsd:enumeration value="INDEPENDENT"/>
-      <xsd:enumeration value="EMPLOYEE"/>
+  <xsd:simpleType name="EurocentPositiveAmountType">
+    <xsd:restriction base="xsd:unsignedLong">
+      <xsd:maxExclusive value="100000000000000000"/>
     </xsd:restriction>
   </xsd:simpleType>
-  <xsd:simpleType name="QuarterType">
-    <xsd:restriction base="xsd:int">
-      <xsd:minInclusive value="1"/>
-      <xsd:maxInclusive value="4"/>
+  <xsd:simpleType name="EurocentAmountType">
+    <xsd:restriction base="xsd:long">
+      <xsd:minExclusive value="-100000000000000000"/>
+      <xsd:maxExclusive value="100000000000000000"/>
     </xsd:restriction>
   </xsd:simpleType>
-  <xsd:simpleType name="UnemployedWorkerStatus">
-    <xsd:restriction base="xsd:string">
-      <xsd:enumeration value="UNEMPLOYMENT_ALLOCATION"/>
-      <xsd:enumeration value="INSERTION_ALLOCATION"/>
-    </xsd:restriction>
-  </xsd:simpleType>
-  <xsd:simpleType name="ArticleCode">
+  <xsd:simpleType name="NssoRegistrationNumberType">
+    <xsd:annotation>
+      <xsd:documentation>Identification number of an enterprise at NSSO (= RSZ/ONSS). Numbers starting with 51 and length 10 are always temporary numbers.</xsd:documentation>
+    </xsd:annotation>
     <xsd:restriction base="xsd:string">
-      <xsd:minLength value="1"/>
-      <xsd:maxLength value="9"/>
+      <xsd:pattern value="0\d{9}"/>
+      <xsd:pattern value="51\d{8}"/>
     </xsd:restriction>
   </xsd:simpleType>
+  <xsd:complexType name="SsinWithCanceledAndReplacesStatusType">
+    <xsd:simpleContent>
+      <xsd:extension base="tns:SsinType">
+        <xsd:attribute name="canceled" type="xsd:boolean"/>
+        <xsd:attribute name="replaces" type="tns:SsinType"/>
+      </xsd:extension>
+    </xsd:simpleContent>
+  </xsd:complexType>
+  <xsd:complexType name="SsinWithCanceledAndReplacedByStatusType">
+    <xsd:simpleContent>
+      <xsd:extension base="tns:SsinType">
+        <xsd:attribute name="canceled" type="xsd:boolean"/>
+        <xsd:attribute name="replacedBy" type="tns:SsinType"/>
+      </xsd:extension>
+    </xsd:simpleContent>
+  </xsd:complexType>
 </xsd:schema>
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Common/ResultSummary.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/IdentifyPersonRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/IdentifyPerson/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_AB_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_C_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_Common.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Reply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/LoiWet65_DF_decision_Request.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/Loi65Wet65/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/ManageAccessRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/ManageAccess/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/AddressHistory.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/FamilyComposition.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvestigationRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/PerformInvetigationReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/OCMW_CPAS/PerformInvestigation/WaitRegister.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/AddressInformation.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/Citizen.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Person/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/CommonDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/NamespaceRoot.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNReply.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/SSDN/Service/SSDNRequest.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/intf/RetrieveTIGroupsService/RetrieveTIGroupsV2.wsdl`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/kszbcss/types/RetrieveTIGroups/RetrieveTIGroupsV2.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/XSD/be/fgov/rrn/ibz/xsd/xm25/xm25.xsd`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/choicelists.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/IdentifyPersonRequest/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/config/cbss/RetrieveTIGroupsRequest/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/cbss.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/cbss.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/cbss_demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_1.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_2.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_3.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_4.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_ipr_5.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_1.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_2.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/demo_tx25_3.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/democfg.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/democfg.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/garble_tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/lijst_van_sectoren_liste_des_secteurs.csv`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/purposes.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/purposes.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/sectors.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/sectors.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1107.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1358.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/fixtures/tx25_1373.xml`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/management/commands/cbss_validate_request.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/mixins.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/tx25.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/ui.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cbss/utils.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cbss/utils.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/client_vouchers/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/client_vouchers/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/client_vouchers/ui.py` & `lino-welfare-23.6.0/lino_welfare/modlib/client_vouchers/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/contacts/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/contacts/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from django.utils.text import format_lazy
 from django.utils.translation import gettext_lazy as _
 
 
 class Plugin(Plugin):
 
-    use_vcard_export = False
+    # use_vcard_export = False
 
     extends_models = ['Partner', 'Person', 'Company']
 
     def setup_main_menu(self, site, user_type, main):
         m = main.add_menu(self.app_label, self.verbose_name)
         m.add_action('contacts.Persons')
         m.add_action(
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/contacts/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/contacts/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cv/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cv/fixtures/props.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cv/fixtures/props.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2008-2013 Rumma & Ko Ltd
+# Copyright 2008-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 """
-Installs a set of property types and property groups specific to 
+Installs a set of property types and property groups specific to
 :mod:`lino_welfare.modlib.pcsw`.
 
 """
 
 
 from django.utils.translation import gettext as _
 from django.conf import settings
@@ -18,42 +18,37 @@
 from lino_xl.lib.properties.models import PropType
 
 
 def objects():
     onoff = PropType.objects.get(pk=1)  # created in std fixture
     appraisal = PropType.objects.get(pk=2)  # created in std fixture
 
-    pgroup = Instantiator('properties.PropGroup').build
+    pgroup = Instantiator('properties.PropGroup', 'property_area').build
 
-    skills = pgroup(**babel_values('name', **dict(
-        en="Skills", de=u"Fachkompetenzen",
-        fr=u"Compétences professionnelles")))
+    skills = pgroup('skills', **babel_values('name',
+        en="Skills", de="Fachkompetenzen",
+        fr="Compétences professionnelles"))
     skills.save()
     yield skills
-    softskills = pgroup(**babel_values('name', **dict(
+    softskills = pgroup('softskills', **babel_values('name',
         en="Soft skills",
-        de=u"Sozialkompetenzen",
-        fr=u"Compétences sociales")))
+        de="Sozialkompetenzen",
+        fr="Compétences sociales"))
     softskills.save()
     yield softskills
-    obstacles = pgroup(**babel_values('name', **dict(
-        en="Obstacles", de=u"Hindernisse",
-        fr="Obstacles")))
+    obstacles = pgroup('obstacles', **babel_values('name',
+        en="Obstacles", de="Hindernisse",
+        fr="Obstacles"))
     obstacles.save()
     yield obstacles
 
-    #~ settings.SITE.update_site_config(
-      #~ propgroup_skills = skills,
-      #~ propgroup_softskills = softskills,
-      #~ propgroup_obstacles = obstacles,
-      #~ )
-    settings.SITE.site_config.propgroup_skills = skills
-    settings.SITE.site_config.propgroup_softskills = softskills
-    settings.SITE.site_config.propgroup_obstacles = obstacles
-    yield settings.SITE.site_config
+    # settings.SITE.site_config.propgroup_skills = skills
+    # settings.SITE.site_config.propgroup_softskills = softskills
+    # settings.SITE.site_config.propgroup_obstacles = obstacles
+    # yield settings.SITE.site_config
 
     skill = Instantiator('properties.Property', group=skills, type=onoff).build
     softskill = Instantiator(
         'properties.Property', group=softskills, type=appraisal).build
     obstacle = Instantiator(
         'properties.Property', group=obstacles, type=onoff).build
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/cv/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/cv/models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2008-2015 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
-# License: GNU Affero General Public License v3 (see file COPYING for details)
 """
 The :xfile:`models.py` file for :mod:`lino_welfare.modlib.cv`.
 """
 
-import logging
-logger = logging.getLogger(__name__)
+import logging ; logger = logging.getLogger(__name__)
 
 from django.db import models
 from django.conf import settings
-from django.utils.translation import gettext_lazy as _
-
-from lino.api import dd, rt
 
+from lino.api import dd, rt, _
 from lino_xl.lib.cv.models import *
-
 from lino_welfare.modlib.integ.roles import IntegUser
 from lino_welfare.modlib.pcsw.roles import SocialStaff
-
-from lino_xl.lib.properties import models as properties
+# from lino_xl.lib.properties import models as properties
+from lino_xl.lib.properties.choicelists import PropertyAreas
+from lino_xl.lib.properties.mixins import PropertyOccurence
+
+add = PropertyAreas.add_item
+
+add("010", _("Skills"), 'skills')
+add("020", _("Soft skills"), 'softskills')
+add("030", _("Obstacles"), 'obstacles')
 
 
 #
 # PROPERTIES
 #
 
-
-class PersonProperty(properties.PropertyOccurence):
+class PersonProperty(PropertyOccurence):
 
     """The occurrence of a given property on a given client. """
 
     allow_cascaded_delete = ['person']
 
     class Meta:
         app_label = 'cv'
@@ -78,84 +79,93 @@
 class ConfiguredPropsByPerson(PropsByPerson):
 
     """Base class for :class`SkillsByPerson`, :class`SoftSkillsByPerson`
     and :class`ObstaclesByPerson`.
 
     """
 
-    propgroup_config_name = None
+    property_area = None
+
+    # propgroup_config_name = None
 
-    typo_check = False  # to avoid warning "ConfiguredPropsByPerson
-                       # defines new attribute(s) propgroup_config_name"
+    # typo_check = False  # to avoid warning "ConfiguredPropsByPerson
+    #                    # defines new attribute(s) propgroup_config_name"
 
     @classmethod
     def get_known_values(self):
-        pg = getattr(settings.SITE.site_config, self.propgroup_config_name)
+        # pg = getattr(settings.SITE.site_config, self.propgroup_config_name)
+        pg = self.property_area.get_object()
         return dict(group=pg)
 
     @classmethod
     def get_actor_label(self):
-        if self.propgroup_config_name is None:
+        # if self.propgroup_config_name is None:
+        if self.property_area is None:
             return self.__name__
-        pg = getattr(settings.SITE.site_config, self.propgroup_config_name)
-        if pg is None:
-            return _("(SiteConfig %s is empty)" % self.propgroup_config_name)
-        return dd.babelattr(pg, 'name')
+        # pg = getattr(settings.SITE.site_config, self.propgroup_config_name)
+        pg = self.property_area.get_object()
+        return str(pg)
+        # if pg is None:
+        #     return _("(SiteConfig %s is empty)" % self.propgroup_config_name)
+        # return dd.babelattr(pg, 'name')
 
 
 class SkillsByPerson(ConfiguredPropsByPerson):
-    propgroup_config_name = 'propgroup_skills'
+    property_area = PropertyAreas.skills
+    # propgroup_config_name = 'propgroup_skills'
 
 
 class SoftSkillsByPerson(ConfiguredPropsByPerson):
-    propgroup_config_name = 'propgroup_softskills'
+    property_area = PropertyAreas.softskills
+    # propgroup_config_name = 'propgroup_softskills'
 
 
 class ObstaclesByPerson(ConfiguredPropsByPerson):
-    propgroup_config_name = 'propgroup_obstacles'
-
+    property_area = PropertyAreas.obstacles
+    # propgroup_config_name = 'propgroup_obstacles'
 
-def customize_siteconfig():
 
-    dd.inject_field(
-        'system.SiteConfig',
-        'propgroup_skills',
-        dd.ForeignKey(
-            'properties.PropGroup',
-            blank=True, null=True,
-            verbose_name=_("Skills Property Group"),
-            related_name='skills_sites',
-            help_text=_(
-                "The property group to be used as master "
-                "for the SkillsByPerson table.")))
-    dd.inject_field(
-        'system.SiteConfig',
-        'propgroup_softskills',
-        dd.ForeignKey(
-            'properties.PropGroup',
-            blank=True, null=True,
-            verbose_name=_("Soft Skills Property Group"),
-            related_name='softskills_sites',
-            help_text=_(
-                "The property group to be used as master "
-                "for the SoftSkillsByPerson table.")))
-    dd.inject_field(
-        'system.SiteConfig',
-        'propgroup_obstacles',
-        dd.ForeignKey(
-            'properties.PropGroup',
-            blank=True, null=True,
-            verbose_name=_("Obstacles Property Group"),
-            related_name='obstacles_sites',
-            help_text=_(
-                "The property group to be used as master "
-                "for the ObstaclesByPerson table.")))
-
-
-customize_siteconfig()
+# def customize_siteconfig():
+#
+#     dd.inject_field(
+#         'system.SiteConfig',
+#         'propgroup_skills',
+#         dd.ForeignKey(
+#             'properties.PropGroup',
+#             blank=True, null=True,
+#             verbose_name=_("Skills Property Group"),
+#             related_name='skills_sites',
+#             help_text=_(
+#                 "The property group to be used as master "
+#                 "for the SkillsByPerson table.")))
+#     dd.inject_field(
+#         'system.SiteConfig',
+#         'propgroup_softskills',
+#         dd.ForeignKey(
+#             'properties.PropGroup',
+#             blank=True, null=True,
+#             verbose_name=_("Soft Skills Property Group"),
+#             related_name='softskills_sites',
+#             help_text=_(
+#                 "The property group to be used as master "
+#                 "for the SoftSkillsByPerson table.")))
+#     dd.inject_field(
+#         'system.SiteConfig',
+#         'propgroup_obstacles',
+#         dd.ForeignKey(
+#             'properties.PropGroup',
+#             blank=True, null=True,
+#             verbose_name=_("Obstacles Property Group"),
+#             related_name='obstacles_sites',
+#             help_text=_(
+#                 "The property group to be used as master "
+#                 "for the ObstaclesByPerson table.")))
+#
+#
+# customize_siteconfig()
 
 
 @dd.receiver(dd.post_analyze)
 def set_detail_layouts(sender=None, **kwargs):
     rt.models.properties.Properties.set_detail_layout("""
     id group type
     name
@@ -177,8 +187,7 @@
 
 def properties_list(owner, *prop_ids):
     for pk in prop_ids:
         try:
             yield owner.personproperty_set.get(property__id=pk)
         except PersonProperty.DoesNotExist:
             pass
-
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-# Copyright 2014-2021 Rumma & Ko Ltd
+# Copyright 2014-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
-"""Functionality for doing "debts mediation".
-
-.. autosummary::
-   :toctree:
-
-   mixins
-   fields
-   fixtures.std
-   fixtures.minimal
-   fixtures.demo
-
-
+"""See :doc:`/specs/debts`.
 
 """
 
-from lino import ad
-
-from django.utils.translation import gettext_lazy as _
+from lino import ad, _
 
 
 class Plugin(ad.Plugin):
     verbose_name = _("Debts mediation")
 
     ref_length = 20
     """The `max_length` of the `Reference` field of an account.
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/choicelists.py` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default_2.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/config/debts/Budget/Default_new.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/fixtures/minimal.py` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/minimal.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/mixins.py` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/mixins.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2012-2021 Rumma & Ko Ltd
+# Copyright 2012-2023 Rumma & Ko Ltd
 
-"""
-Database models for `lino_welfare.modlib.debts`.
-
-"""
 
 from django.db import models
 
 from lino import mixins
 from lino.api import dd, _
 from lino_xl.lib.notes.choicelists import SpecialTypes
 
@@ -30,18 +26,14 @@
             return False
         return super(
             SequencedBudgetComponent, self).get_row_permission(user, state, ba)
 
 
 
 class ActorBase:
-    """Base class for both the volatile :class:`MainActor` and the
-    :class:`Actor <lino_welfare.modlib.debts.models.Actor>` model.
-
-    """
 
     def get_first_meeting(self):
         obj = self.client
         if obj:
             return obj.get_first_meeting(self.budget.date)
 
     def get_first_meeting_text(self, *args):
@@ -67,15 +59,13 @@
 
     def __str__(self):
         return self.header
 
 
 class MainActor(ActorBase):
 
-    "A volatile object that represents the budget partner as actor"
-
     def __init__(self, budget, header):
         self.budget = budget
         self.header = header
         self.remark = ''
         if budget.partner_id:
             self.partner = budget.partner
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,15 +395,15 @@
     partner = dd.ForeignKey('contacts.Partner', blank=True)
     header = models.CharField(_("Header"), max_length=20, blank=True)
     remark = dd.RichTextField(_("Remark"), format="html", blank=True)
 
     def save(self, *args, **kw):
         if not self.header:
             self.header = gettext("Actor") + " " + str(self.seqno)
-        super(Actor, self).save(*args, **kw)
+        super().save(*args, **kw)
 
 
 class Entry(SequencedBudgetComponent):
     class Meta:
         verbose_name = _("Budget Entry")
         verbose_name_plural = _("Budget Entries")
         # unique_together = ['budget','account','name']
@@ -414,19 +414,15 @@
     # group = dd.ForeignKey(AccountGroup)
     account_type = AccountTypes.field(blank=True)
     account = dd.ForeignKey('debts.Account')
     partner = dd.ForeignKey('contacts.Partner', blank=True, null=True)
     # name = models.CharField(_("Remark"),max_length=200,blank=True)
     # amount = dd.PriceField(_("Amount"),default=0)
     amount = dd.PriceField(_("Amount"), blank=True, null=True)
-    actor = dd.ForeignKey(Actor,
-                              blank=True, null=True,
-        help_text="""\
-Hier optional einen Akteur angeben, wenn der Eintrag
-sich nicht auf den Gesamthaushalt bezieht.""")
+    actor = dd.ForeignKey(Actor, blank=True, null=True)
     # amount = dd.PriceField(_("Amount"),default=0)
     circa = models.BooleanField(_("Circa"),
         default=False)
     distribute = models.BooleanField(
         _("Distribute"),
         default=False,
         help_text=u"""\
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/debts/ui.py` & `lino-welfare-23.6.0/lino_welfare/modlib/debts/ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,37 +255,37 @@
 class AssetsByBudget(EntriesByBudget, EntriesByType):
     _account_type = AccountTypes.assets
     column_names = "account remark amount actor move_buttons:8 todo seqno id"
 
 
 ## PrintEntriesByBudget
 
+from lino.core.fields import TableRow
 
-class EntryGroup(object):
+class EntryGroup(TableRow):
     """Volatile object used to encapsulate the account groups that have
     some data in a given budget.  Entry groups are instantiated and
     yielded by :meth:`Budget.entry_groups
     <lino_welfare.modlib.debts.models.Budget.entry_groups>`, and they
     are used as the master instance for all
     :class:`PrintEntriesByBudget` tables.
 
     """
 
-    pk = None
-
     def __init__(self, budget, group, ar):
         self.budget = budget
         self.group = group
         self.action_request = ar.spawn(
             PrintEntriesByBudget, master_instance=self)
 
     def has_data(self):
         return self.action_request.get_total_count() > 0
 
 
+
 class PrintEntriesByBudget(dd.VirtualTable):
     """Base class for the printable tables of entries by budget
 (:class:`PrintExpensesByBudget`, :class:`PrintIncomesByBudget`,
 :class:`PrintLiabilitiesByBudget` and :class:`PrintAssetsByBudget`).
 
 This is historically the first table that uses Lino's per-request
 dynamic columns feature.
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/mixins.py` & `lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/mixins.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/dupable_clients/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/dupable_clients/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/esf/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/esf/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/esf/choicelists.py` & `lino-welfare-23.6.0/lino_welfare/modlib/esf/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html` & `lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/Client/esf_file.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html` & `lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/base.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html` & `lino-welfare-23.6.0/lino_welfare/modlib/esf/config/esf/ClientSummary/default.weasy.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/esf/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/esf/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/finan/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/finan/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/households/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/households/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/immersion/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/immersion/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/StageForem.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/immersion/config/immersion/Contract/immersion.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/immersion/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/immersion/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/immersion/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/immersion/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/immersion/ui.py` & `lino-welfare-23.6.0/lino_welfare/modlib/immersion/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/integ/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/integ/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/integ/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/integ/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/integ/fixtures/std.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 ONE_DAY = datetime.timedelta(days=1)
 
 from django.conf import settings
 
 from lino.api import dd, _
 from lino.utils.instantiator import Instantiator
 
-from lino_xl.lib.cal.choicelists import DurationUnits, WORKDAYS
+from lino.modlib.system.choicelists import DurationUnits
+from lino.modlib.system.choicelists import WORKDAYS
 
 
 def objects():
     """
     Lino Welfare does not use time slots when generating evaluation
     meetings because the exact planning is done by the user. But we
     define a limit of 4 client meetings per day per user.
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/integ/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/integ/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/isip/choicelists.py` & `lino-welfare-23.6.0/lino_welfare/modlib/isip/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/isip/config/isip/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/isip/mixins.py` & `lino-welfare-23.6.0/lino_welfare/modlib/isip/mixins.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from lino.modlib.users.mixins import UserAuthored
 from lino.utils import mti
 from lino.utils.ranges import isrange
 from lino.utils.ranges import overlap2, encompass
 from lino_welfare.modlib.integ.roles import IntegUser
 from lino_xl.lib.coachings.mixins import ClientChecker
 from lino_welfare.modlib.system.models import Signers
-from lino_xl.lib.cal.choicelists import DurationUnits
+from lino.modlib.system.choicelists import DurationUnits
 from lino_xl.lib.cal.mixins import EventGenerator
 from lino_xl.lib.cal.utils import update_auto_task
 from lino_xl.lib.contacts.mixins import AbstractContactRelated
 from lino_xl.lib.excerpts.mixins import Certifiable
 from lino_welfare.modlib.pcsw.roles import SocialUser
 from lino_welfare.modlib.integ.roles import IntegUser
 from .choicelists import ContractEvents, OverlapGroups
@@ -61,15 +61,16 @@
     @dd.chooser(simple_values=True)
     def template_choices(cls):
         bm = rt.models.printing.BuildMethods.get_system_default()
         return rt.find_template_config_files(
             bm.template_ext, cls.templates_group)
 
 
-class ContractBase(Signers, Certifiable, EventGenerator, UserAuthored):
+class ContractBase(Signers, Certifiable, EventGenerator, UserAuthored,
+    UploadController):
 
     manager_roles_required = dd.login_required(IntegUser)
 
     TASKTYPE_CONTRACT_APPLIES_UNTIL = 1
 
     class Meta:
         abstract = True
@@ -437,15 +438,15 @@
     params_panel_hidden = True
     no_phantom_row = True
 
     @classmethod
     def param_defaults(cls, ar, **kw):
         kw = super().param_defaults(ar, **kw)
         kw.update(start_date=dd.today())
-        kw.update(end_date=dd.today())
+        # kw.update(end_date=dd.today())
         return kw
 
     @classmethod
     def get_request_queryset(cls, ar):
         qs = super().get_request_queryset(ar)
         pv = ar.param_values
         #~ logger.info("20120608.get_request_queryset param_values = %r", pv)
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/isip/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/isip/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from django.conf import settings
 from django.db import models
 from django.utils.translation import gettext_lazy as _
 
 from lino import mixins
-from lino_xl.lib.cal.mixins import RecurrenceSet
+from lino.modlib.system.mixins import RecurrenceSet
 from .choicelists import *
 from .mixins import (ContractTypeBase,
                      ContractPartnerBase, ContractBase,
                      ContractBaseTable)
 
 config = dd.plugins.isip
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/jobs/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/Contract/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/ContractsSituation/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/jobs/config/jobs/OldJobsOverview/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/jobs/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/jobs/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/jobs/mixins.py` & `lino-welfare-23.6.0/lino_welfare/modlib/jobs/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ONE_DAY = datetime.timedelta(days=1)
 
 from django.db import models
 from django.utils.translation import pgettext_lazy as pgettext
 
 from lino.api import dd, rt, _
 
-from lino_xl.lib.cal.choicelists import DurationUnits
+from lino.modlib.system.choicelists import DurationUnits
 from lino_welfare.modlib.isip.mixins import (ContractPartnerBase,
                                              ContractBase)
 
 
 class CandidatureStates(dd.ChoiceList):
     help_text = _("The possible states of a candidature.")
     verbose_name = _("Candidature state")
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/jobs/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/jobs/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/jobs/ui.py` & `lino-welfare-23.6.0/lino_welfare/modlib/jobs/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/ledger/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/ledger/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/ledger/fixtures/std_journals.py` & `lino-welfare-23.6.0/lino_welfare/modlib/ledger/fixtures/std_journals.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/ledger/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/ledger/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/newcomers/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/newcomers/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/newcomers/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/newcomers/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/newcomers/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/newcomers/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/notes/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/notes/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/notes/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/notes/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/actions.py` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         obj.client_state = ClientStates.refused
         obj.full_clean()
         obj.save()
 
         ctx = dict(
             client=obj, user=ar.get_user(), state=self.target_state)
         subject = self.done_msg.format(**ctx)
-        ctx.update(client=ar.obj2memo(obj))
+        ctx.update(client=obj.obj2memo())
         body = self.done_msg.format(**ctx)
         body += '\n{}: {}'.format(
             RefusalReasons.verbose_name, ar.action_param_values.reason)
         if ar.action_param_values.remark:
             body += '\n' + str(ar.action_param_values.remark)
         # dd.logger.info("20170412 %r", ar.action_param_values)
         # 20170412 seems that mysql does not support newstr:
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/choicelists.py` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/choicelists.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/cv.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/eid-content.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/config/pcsw/Client/file_sheet.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/fixtures/demo2.py` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/demo2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/pcsw/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/pcsw/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from lino.utils import join_elems
 from etgen.html import E
 
 from lino.api import dd, rt, _
 from lino.core.utils import get_field
 
 from lino_xl.lib.cal.utils import update_reminder
-from lino_xl.lib.cal.choicelists import DurationUnits
+from lino.modlib.system.choicelists import DurationUnits
 from lino_xl.lib.coachings.mixins import ClientChecker
 from lino.modlib.uploads.choicelists import Shortcuts
 from lino.modlib.uploads.mixins import UploadController
 
 from lino_xl.lib.notes.choicelists import SpecialTypes
 from lino_xl.lib.notes.mixins import Notable
 from lino_welfare.modlib.dupable_clients.mixins import DupableClient
@@ -72,14 +72,15 @@
         verbose_name = _("Client")
         verbose_name_plural = _("Clients")
         abstract = dd.is_abstract_model(__name__, 'Client')
         ordering = ['id']  # required because Django 3.2 otherwise inherits it from Person
 
     # quick_search_fields = "prefix name phone gsm street national_id"
     quick_search_fields = "prefix name phone gsm national_id"
+    memo_command = "client"
 
     group = dd.ForeignKey("pcsw.PersonGroup", blank=True, null=True,
                           verbose_name=_("Integration phase"))
 
     civil_state = CivilStates.field(blank=True)
 
     residence_type = ResidenceTypes.field(blank=True)
@@ -282,15 +283,16 @@
     #         yield o
     #     for o in find_them('coached_until', today, datetime.timedelta(days=30),
     #                        _("coaching ends"), tab=1):
     #         yield o
 
     def get_skills_set(self):
         return self.personproperty_set.filter(
-            group=settings.SITE.site_config.propgroup_skills)
+            group=PropertyAreas.skills.get_object())
+            # group=settings.SITE.site_config.propgroup_skills)
     skills_set = property(get_skills_set)
 
     def properties_list(self, *prop_ids):
         """Yields a list of the :class:`PersonProperty
         <lino_welfare.modlib.cv.models.PersonProperty>` properties of
         this person in the specified order.  If this person has no
         entry for a requested :class:`Property`, it is simply skipped.
@@ -402,15 +404,15 @@
             return ''
         cbss = dd.resolve_app('cbss')
         SLAVE = cbss.RetrieveTIGroupsRequestsByPerson
         elems = []
         sar = ar.spawn(
             SLAVE, master_instance=self,
             filter=models.Q(status__in=OK_STATES))
-        btn = SLAVE.insert_action.request_from(ar).ar2button()
+        btn = SLAVE.insert_action.request_from(sar).ar2button()
         n = sar.get_total_count()
         if n > 0:
             items = []
             SHOWN_TYPES = ('110', '120', '140', '141')
             obj = sar.data_iterator[n - 1]
             res = obj.Result(ar)
             for row in res:
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/polls/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/polls/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/projects/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/projects/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/projects/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/reception/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/reception/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/reception/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/reception/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,23 +346,24 @@
                     client.create_visit,
                     _("Visit"),
                     request_kwargs=dict(action_param_values=apv),
                     icon_name=CreateClientVisit.icon_name)
             elems += [btn, ' ']
 
         if client.client_state == ClientStates.coached \
-           or user.newcomer_appointments:
-           # or user.newcomer_quota > 0:
-            sar = extensible.CalendarPanel.request(
-                subst_user=user,
-                current_project=client.pk)
-            elems += [ar.href_to_request(
-                sar, _("Find date"),
-                title=_("Find date"),
-                icon_name=FindDateByClientTable.icon_name), ' ']
+                or user.newcomer_appointments:
+                # or user.newcomer_quota > 0:
+            if extensible is not None:
+                sar = extensible.CalendarPanel.request(
+                    subst_user=user,
+                    current_project=client.pk)
+                elems += [ar.href_to_request(
+                    sar, _("Find date"),
+                    title=_("Find date"),
+                    icon_name=FindDateByClientTable.icon_name), ' ']
             #~ icon_name = 'x-tbar-calendar'
             #~ icon_file = 'calendar.png'
 
         return E.div(*elems)
 
 
 class CoachingsByClient(CoachingsByClient):
@@ -410,9 +411,9 @@
 for T in MyWaitingVisitors, GoneVisitors, BusyVisitors:
     T.column_names = T.column_names.replace('partner', 'client')
 
 WaitingVisitors.column_names = ('since:15 client event__user:10 event__user__coaching_type:10 waiting_number:5 '
                 'event__summary workflow_buttons')
 
 WaitingVisitors._editable = True
-WaitingVisitors.no_phantom_row = True  
+WaitingVisitors.no_phantom_row = True
 # reception clerk can modify waiting number and remark of a visitor.
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/sepa/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/sepa/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/sepa/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/sepa/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/system/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/system/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         signer1 signer2
         signer1_function signer2_function
         """, label=_("General"))
 
     constants = dd.Panel(
         """
         system_note_type default_build_method
-        propgroup_skills propgroup_softskills propgroup_obstacles
+        # propgroup_skills propgroup_softskills propgroup_obstacles
         residence_permit_upload_type \
         work_permit_upload_type \
         driving_licence_upload_type
         # client_calendar
         default_event_type prompt_calendar hide_events_before
         client_guestrole team_guestrole
         """, label=_("Constants"))
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/users/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/users/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/users/ui.py` & `lino-welfare-23.6.0/lino_welfare/modlib/users/ui.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/anw.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/aus.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/certificate.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/Excerpt/summary.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/excerpts/base.body.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/integ/ActivityReport/Default.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/letter_margin_bottom.html`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/config/notes/Note/Letter.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,16 +20,15 @@
 from lino.utils import i2d, Cycler
 from lino_xl.lib.beid.mixins import BeIdCardTypes
 from lino.utils.instantiator import Instantiator
 from lino.core.utils import resolve_model
 from lino.utils import mti
 from lino.utils.ssin import generate_ssin
 
-from lino_xl.lib.cal.choicelists import DurationUnits
-# from lino_xl.lib.cal.utils import WORKDAYS
+from lino.modlib.system.choicelists import DurationUnits
 
 isip = dd.resolve_app('isip')
 jobs = dd.resolve_app('jobs')
 pcsw = dd.resolve_app('pcsw')
 # uploads = dd.resolve_app('uploads')
 contacts = dd.resolve_app('contacts')
 countries = dd.resolve_app('countries')
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/demo2.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/demo2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/pp2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/std.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/std.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2008-2020 Rumma & Ko Ltd
+# Copyright 2008-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 
 from django.contrib.contenttypes.models import ContentType
 from lino.utils.instantiator import Instantiator
 from lino_xl.lib.notes.choicelists import SpecialTypes
 
@@ -68,33 +68,33 @@
 
     ContractEnding = dd.resolve_model('isip.ContractEnding')
     yield ContractEnding(name=_("Normal"))
     yield ContractEnding(name=_("Alcohol"), needs_date_ended=True)
     yield ContractEnding(name=_("Health"), needs_date_ended=True)
     yield ContractEnding(name=_("Force majeure"), needs_date_ended=True)
 
-    I = Instantiator(
-        'gfks.HelpText', 'content_type field help_text').build
-
-    Client = dd.resolve_model('pcsw.Client')
-    t = ContentType.objects.get_for_model(Client)
-    yield I(t, 'in_belgium_since', u"""\
-Since when this person in Belgium lives.
-<b>Important:</b> help_text can be formatted.""")
-    yield I(t, 'noble_condition', u"""\
-The eventual noble condition of this person. Imported from TIM.
-""")
+#     I = Instantiator(
+#         'gfks.HelpText', 'content_type field help_text').build
+#
+#     Client = dd.resolve_model('pcsw.Client')
+#     t = ContentType.objects.get_for_model(Client)
+#     yield I(t, 'in_belgium_since', u"""\
+# Since when this person in Belgium lives.
+# <b>Important:</b> help_text can be formatted.""")
+#     yield I(t, 'noble_condition', u"""\
+# The eventual noble condition of this person. Imported from TIM.
+# """)
     #~ t = ContentType.objects.get_for_model(Person)
     #~ yield I(t,'birth_date',u"""\
 #~ Unkomplette Geburtsdaten sind erlaubt, z.B.
 #~ <ul>
 #~ <li>00.00.1980 : irgendwann in 1980</li>
 #~ <li>00.07.1980 : im Juli 1980</li>
 #~ <li>23.07.0000 : Geburtstag am 23. Juli, Alter unbekannt</li>
 #~ </ul>
 #~ """)
 
-    Partner = dd.resolve_model('contacts.Partner')
-    t = ContentType.objects.get_for_model(Partner)
-    yield I(t, 'language', u"""\
-    Die Sprache, in der Dokumente ausgestellt werden sollen.
-""")
+    # Partner = dd.resolve_model('contacts.Partner')
+    # t = ContentType.objects.get_for_model(Partner)
+#     yield I(t, 'language', u"""\
+#     Die Sprache, in der Dokumente ausgestellt werden sollen.
+# """)
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/fixtures/std2.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/fixtures/std2.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/help_texts.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/help_texts.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,14 @@
     'lino_welfare.modlib.cbss.NewStyleRequest.on_cbss_ok' : _("""Called when a successful reply has been received."""),
     'lino_welfare.modlib.cbss.SSIN' : _("""Abstract base for Requests that have a field national_id and a method
 get_ssin()."""),
     'lino_welfare.modlib.cbss.WithPerson' : _("""Mixin for models that have certain fields"""),
     'lino_welfare.modlib.cbss.WithPerson.first_name' : _("""Space-separated list of all first names."""),
     'lino_welfare.modlib.cbss.WithPerson.last_name' : _("""Last name (family name)."""),
     'lino_welfare.modlib.client_vouchers.Plugin' : _("""See lino.core.plugin.Plugin."""),
-    'lino_welfare.modlib.debts.fields.PeriodsField' : _("""Used for Entry.periods and Account.periods
-(the latter holds simply the default value for the former).
-It means: for how many months the entered amount counts.
-Default value is 1. For yearly amounts set it to 12."""),
-    'lino_welfare.modlib.debts.ActorBase' : _("""Base class for both the volatile MainActor and the
-Actor model."""),
-    'lino_welfare.modlib.debts.MainActor' : _("""A volatile object that represents the budget partner as actor"""),
     'lino_welfare.modlib.dupable_clients.Plugin' : _("""See lino.core.plugin.Plugin."""),
     'lino_welfare.modlib.dupable_clients.DupableClient' : _("""Model mixin to add to the base classes of your application’s
 pcsw.Client model."""),
     'lino_welfare.modlib.dupable_clients.DupableClient.find_similar_instances' : _("""Overrides
 lino.mixins.dupable.Dupable.find_similar_instances(),
 adding some additional rules."""),
     'lino_welfare.modlib.esf.Plugin' : _("""See lino.core.plugin.Plugin."""),
@@ -162,36 +155,45 @@
     'lino_welfare.modlib.cbss.ManageAccessRequest.purpose' : _("""Pointer to Purpose."""),
     'lino_welfare.modlib.cbss.ManageAccessRequest.action' : _("""The action to perform.  This must be one of the values in
 lino_welfare.modlib.cbss.choicelists.ManageActions"""),
     'lino_welfare.modlib.cbss.ManageAccessRequest.query_register' : _("""The register to be query.
 This must be one of the values in
 lino_welfare.modlib.cbss.choicelists.QueryRegisters"""),
     'lino_welfare.modlib.cbss.RetrieveTIGroupsRequest' : _("""A request to the RetrieveTIGroups service (aka Tx25)"""),
+    'lino_welfare.modlib.debts.Budget.print_empty_rows' : _("""Whether to print empty rows."""),
+    'lino_welfare.modlib.debts.Budget.ignore_yearly_incomes' : _("""Whether to ignore yearly incomes."""),
+    'lino_welfare.modlib.debts.Budget.entry_groups' : _("""Yield the entry groups for this budget, i.e. one item for each
+account group for which this budget has some data."""),
+    'lino_welfare.modlib.debts.Actor' : _("""The database model used to represent a budget actor."""),
+    'lino_welfare.modlib.debts.Entry' : _("""A detail row of a Budget."""),
+    'lino_welfare.modlib.debts.Entry.actor' : _("""Optionally specify a budget actor who contributes this entry.
+Leave empty when the entry refers to the entire household."""),
+    'lino_welfare.modlib.debts.Entry.amount' : _("""The amount of money. An empty amount is different from a zero
+amount in that the latter will be printed while the former
+not."""),
+    'lino_welfare.modlib.debts.Entry.account' : _("""The related Account."""),
     'lino_welfare.modlib.debts.Account' : _("""An account is an item of an account chart used to collect
 ledger transactions or other accountable items."""),
     'lino_welfare.modlib.debts.Account.name' : _("""The multilingual designation of this account, as the users see
 it."""),
     'lino_welfare.modlib.debts.Account.group' : _("""The account group to which this account belongs.  This must
 point to an instance of Group."""),
     'lino_welfare.modlib.debts.Account.seqno' : _("""The sequence number of this account within its group."""),
     'lino_welfare.modlib.debts.Account.ref' : _("""An optional unique name which can be used to reference a given
 account."""),
     'lino_welfare.modlib.debts.Account.type' : _("""The account type of this account.  This must
 point to an item of
 lino_welfare.modlib.debts.AccountTypes."""),
-    'lino_welfare.modlib.debts.Budget' : _("""Django model used to represent a debts mediation budget."""),
-    'lino_welfare.modlib.debts.Budget.entry_groups' : _("""Yield the entry groups for this budget, i.e. one item for each
-account group for which this budget has some data."""),
-    'lino_welfare.modlib.debts.Actor' : _("""An actor of a budget is a partner who is part of the household
-for which the budget has been established."""),
-    'lino_welfare.modlib.debts.Entry' : _("""A detail row of a Budget."""),
-    'lino_welfare.modlib.debts.Entry.amount' : _("""The amount of money. An empty amount is different from a zero
-amount in that the latter will be printed while the former
-not."""),
-    'lino_welfare.modlib.debts.Entry.account' : _("""The related Account."""),
+    'lino_welfare.modlib.debts.ActorBase' : _("""Base class for both the volatile MainActor and the
+Actor model."""),
+    'lino_welfare.modlib.debts.MainActor' : _("""A volatile object that represents the budget partner as actor"""),
+    'lino_welfare.modlib.debts.PeriodsField' : _("""Used for Entry.periods and Account.periods
+(the latter holds simply the default value for the former).
+It means: for how many months the entered amount counts.
+Default value is 1. For yearly amounts set it to 12."""),
     'lino_welfare.modlib.esf.ClientSummary' : _("""The Django model that represents a client summary."""),
     'lino_welfare.modlib.esf.Summaries' : _("""Base class for all tables on ClientSummary."""),
     'lino_welfare.modlib.esf.AllSummaries' : _("""Lists all ESF summaries for all clients."""),
     'lino_welfare.modlib.esf.SummariesByClient' : _("""Lists the ESF summaries for a given client."""),
     'lino_welfare.modlib.esf.StatisticalField' : _("""Base class for all statistical fields."""),
     'lino_welfare.modlib.esf.StatisticalField.short_name' : _("""Used as the verbose_name of field."""),
     'lino_welfare.modlib.esf.StatisticalField.field_name' : _("""The internal field name."""),
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.mo`

 * *Files 9% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: Lino-DSBE\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-10-22 23:07+0300\n"
+"PO-Revision-Date: 2023-04-01 18:28+0200\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
 "Language-Team: de <luc.saffre@gmail.com>\n"
 "Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 "X-Generator: Poedit 3.0.1\n"
 
 msgid " and "
 msgstr " und "
 
 msgid " born "
 msgstr " geboren "
@@ -55,17 +55,14 @@
 
 msgid "%s (distributable)"
 msgstr "%s (verteilbar)"
 
 msgid "(%d candidatures have been marked inactive)"
 msgstr "( %d Kandidaturen wurden als inaktiv markiert)"
 
-msgid "(SiteConfig %s is empty)"
-msgstr "(Site-Parameter %s ist leer)"
-
 msgctxt "(place)"
 msgid " at "
 msgstr " bei "
 
 msgctxt "(time)"
 msgid "at"
 msgstr "um"
@@ -1237,17 +1234,14 @@
 
 msgid "Observed event"
 msgstr "Beobachtungskriterium"
 
 msgid "Observed events"
 msgstr "Beobachtungskriterium"
 
-msgid "Obstacles Property Group"
-msgstr "Eigenschaftsgruppe Hindernisse"
-
 msgid "Occupations"
 msgstr "Beschäftigungen"
 
 msgid "Once after 10 days"
 msgstr "Einmalig nach 10 Tagen"
 
 msgid "Only active clients"
@@ -1258,14 +1252,21 @@
 
 msgid "Only primary clients"
 msgstr "Nur primäre Begleitungen"
 
 msgid "Open/Close"
 msgstr "Offen/Abgeschlossen"
 
+msgid ""
+"Optionally specify a budget actor who contributes this entry.\n"
+"Leave empty when the entry refers to the entire household."
+msgstr ""
+"Hier optional den Akteur angeben, der diesen Eintrag beiträgt. \n"
+"Leer lassen, wenn der Eintrag sich auf den Gesamthaushalt bezieht."
+
 msgid "Organ Donations"
 msgstr "Organspenden"
 
 msgid "Organization"
 msgstr "Organisation"
 
 msgid "Organizations in charge"
@@ -1612,17 +1613,14 @@
 
 msgid "Since"
 msgstr "Seit"
 
 msgid "Situation financière"
 msgstr "Finanzielle Situation"
 
-msgid "Skills Property Group"
-msgstr "Eigenschaftsgruppe Fähigkeiten"
-
 msgid "Social Board (SB)"
 msgstr "Sozialhilferat (SHR)"
 
 msgid "Social Commission (SC)"
 msgstr "Sozialhilfeausschuss (SAS)"
 
 msgid "Social Welfare Centre"
@@ -1636,17 +1634,14 @@
 
 msgid "Social agent (Manager)"
 msgstr "Sozialarbeiter (Verwalter)"
 
 msgid "Social economy"
 msgstr "Sozialökonomie"
 
-msgid "Soft Skills Property Group"
-msgstr "Eigenschaftsgruppe Sozialkompetenzen"
-
 msgid "Special Infos"
 msgstr "Zusätzliche Informationen"
 
 msgid "Special Retirement Certificates"
 msgstr "Sonder-Pensionszertifikate"
 
 msgid "Standby"
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/de/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 # Copyright (C) 2016 ORGANIZATION
 # This file is distributed under the same license as the lino-welfare
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version:  Lino-DSBE\n"
+"Project-Id-Version: Lino-DSBE\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-11-22 10:25+0100\n"
-"PO-Revision-Date: 2022-10-22 23:07+0300\n"
+"POT-Creation-Date: 2023-04-01 18:26+0200\n"
+"PO-Revision-Date: 2023-04-01 18:28+0200\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
-"Language: de\n"
 "Language-Team: de <luc.saffre@gmail.com>\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Generated-By: Babel 2.12.1\n"
+"X-Generator: Poedit 3.0.1\n"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:19
 #, fuzzy
 msgid "Active Job Search"
 msgstr "Arbeitssuche"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:20
@@ -36,21 +37,21 @@
 
 #: lino_welfare/modlib/active_job_search/models.py:24
 #, fuzzy
 msgid "Proofs of search"
 msgstr "Arbeitssuche"
 
 #: lino_welfare/modlib/active_job_search/models.py:28
-#: lino_welfare/modlib/badges/models.py:45
-#: lino_welfare/modlib/cal/models.py:357 lino_welfare/modlib/cbss/tx25.py:316
-#: lino_welfare/modlib/cbss/tx25.py:363 lino_welfare/modlib/cbss/tx25.py:372
-#: lino_welfare/modlib/cbss/tx25.py:384 lino_welfare/modlib/cbss/tx25.py:475
-#: lino_welfare/modlib/cbss/tx25.py:487 lino_welfare/modlib/debts/models.py:108
-#: lino_welfare/modlib/isip/models.py:363 lino_welfare/modlib/jobs/ui.py:427
-#: lino_welfare/modlib/jobs/ui.py:548 lino_welfare/modlib/pcsw/models.py:1002
+#: lino_welfare/modlib/badges/models.py:45 lino_welfare/modlib/cal/models.py:357
+#: lino_welfare/modlib/cbss/tx25.py:316 lino_welfare/modlib/cbss/tx25.py:363
+#: lino_welfare/modlib/cbss/tx25.py:372 lino_welfare/modlib/cbss/tx25.py:384
+#: lino_welfare/modlib/cbss/tx25.py:475 lino_welfare/modlib/cbss/tx25.py:487
+#: lino_welfare/modlib/debts/models.py:108
+#: lino_welfare/modlib/isip/models.py:365 lino_welfare/modlib/jobs/ui.py:427
+#: lino_welfare/modlib/jobs/ui.py:548 lino_welfare/modlib/pcsw/models.py:1004
 msgid "Date"
 msgstr "Datum"
 
 #: lino_welfare/modlib/active_job_search/models.py:30
 #, fuzzy
 msgid "Spontaneous"
 msgstr "Kontakte"
@@ -78,15 +79,15 @@
 
 #: lino_welfare/modlib/active_job_search/models.py:75
 msgid "Notes concerning child custody."
 msgstr ""
 
 #: lino_welfare/modlib/aids/__init__.py:14
 #: lino_welfare/modlib/ledger/models.py:54
-#: lino_welfare/modlib/pcsw/models.py:506
+#: lino_welfare/modlib/pcsw/models.py:508
 msgid "Aids"
 msgstr "Hilfen"
 
 #: lino_welfare/modlib/aids/choicelists.py:50
 msgid "Aid confirmation type"
 msgstr "Hilfebescheinigungsart"
 
@@ -148,57 +149,50 @@
 msgstr "Entstätigen"
 
 #: lino_welfare/modlib/aids/mixins.py:97
 #, python-format
 msgid "You revoke your confirmation that %(client)s %(text)s"
 msgstr "Sie annulieren Ihre Bestätigung, dass %(client)s %(text)s"
 
-#: lino_welfare/modlib/aids/mixins.py:111
-#: lino_welfare/modlib/aids/mixins.py:137
+#: lino_welfare/modlib/aids/mixins.py:111 lino_welfare/modlib/aids/mixins.py:137
 msgctxt "aids"
 msgid "Signer"
 msgstr "Bestätiger"
 
 #: lino_welfare/modlib/aids/mixins.py:181
 #, python-format
 msgid "receives %(what)s %(when)s."
 msgstr "%(when)s %(what)s erhält."
 
 #: lino_welfare/modlib/aids/mixins.py:213
-#: lino_welfare/modlib/badges/models.py:50 lino_welfare/modlib/cv/models.py:45
+#: lino_welfare/modlib/badges/models.py:50 lino_welfare/modlib/cv/models.py:46
 #: lino_welfare/modlib/debts/models.py:397
 #: lino_welfare/modlib/debts/models.py:437 lino_welfare/modlib/esf/models.py:37
 #: lino_welfare/modlib/immersion/models.py:100
 #: lino_welfare/modlib/jobs/mixins.py:44 lino_welfare/modlib/jobs/models.py:236
-#: lino_welfare/modlib/jobs/models.py:266
-#: lino_welfare/modlib/jobs/models.py:336
-#: lino_welfare/modlib/jobs/models.py:406
-#: lino_welfare/modlib/pcsw/actions.py:40
-#: lino_welfare/modlib/pcsw/models.py:906
-#: lino_welfare/modlib/pcsw/models.py:967
+#: lino_welfare/modlib/jobs/models.py:266 lino_welfare/modlib/jobs/models.py:336
+#: lino_welfare/modlib/jobs/models.py:406 lino_welfare/modlib/pcsw/actions.py:40
+#: lino_welfare/modlib/pcsw/models.py:908 lino_welfare/modlib/pcsw/models.py:969
 #: lino_welfare/modlib/projects/models.py:44
 #: lino_welfare/modlib/xcourses/models.py:186
 #: lino_welfare/modlib/xcourses/models.py:363
 msgid "Remark"
 msgstr "Bemerkung"
 
 #: lino_welfare/modlib/aids/mixins.py:245
 #, python-format
 msgid "Date range %(p1)s lies outside of granted period %(p2)s."
 msgstr "Datumsbereich %(p1)s außerhalb der Laufzeit des Beschlusses %(p2)s."
 
-#: lino_welfare/modlib/aids/mixins.py:317
-#: lino_welfare/modlib/cbss/models.py:284
+#: lino_welfare/modlib/aids/mixins.py:317 lino_welfare/modlib/cbss/models.py:279
 msgid "Period from"
 msgstr "Periode vom"
 
-#: lino_welfare/modlib/aids/mixins.py:319
-#: lino_welfare/modlib/aids/models.py:210
-#: lino_welfare/modlib/pcsw/models.py:912
-#: lino_welfare/modlib/pcsw/models.py:966
+#: lino_welfare/modlib/aids/mixins.py:319 lino_welfare/modlib/aids/models.py:210
+#: lino_welfare/modlib/pcsw/models.py:914 lino_welfare/modlib/pcsw/models.py:968
 msgid "until"
 msgstr "bis"
 
 #: lino_welfare/modlib/aids/mixins.py:322
 msgid "Recipient (Organization)"
 msgstr "Empfänger (Organisation)"
 
@@ -236,16 +230,16 @@
 
 #: lino_welfare/modlib/aids/models.py:72
 msgid "Integration duty"
 msgstr "Verpflichtung DSBE"
 
 #: lino_welfare/modlib/aids/models.py:73
 msgid ""
-"Whether aid grantings of this type are considered as duty for integration"
-" contract."
+"Whether aid grantings of this type are considered as duty for integration "
+"contract."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:77
 msgid "Urgent"
 msgstr "Dringend"
 
 #: lino_welfare/modlib/aids/models.py:78
@@ -254,22 +248,22 @@
 
 #: lino_welfare/modlib/aids/models.py:82
 msgid "Confirmed by primary coach"
 msgstr "Primärbegleiter bestätigt"
 
 #: lino_welfare/modlib/aids/models.py:83
 msgid ""
-"Whether grantings for this aid type are to be signed by the client's "
-"primary coach."
+"Whether grantings for this aid type are to be signed by the client's primary "
+"coach."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:90
 msgid ""
-"Which client address to print on confirmations. If this is empty, Lino "
-"will use the primary address."
+"Which client address to print on confirmations. If this is empty, Lino will "
+"use the primary address."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:95
 msgid "Body template"
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:149
@@ -282,33 +276,31 @@
 
 #: lino_welfare/modlib/aids/models.py:158
 msgid "Date of request"
 msgstr "Antragsdatum"
 
 #: lino_welfare/modlib/aids/models.py:189
 #: lino_welfare/modlib/reception/models.py:323
-#: lino_welfare/modlib/reception/models.py:381
+#: lino_welfare/modlib/reception/models.py:382
 msgid "Actions"
 msgstr "Aktionen"
 
 #: lino_welfare/modlib/aids/models.py:200
 msgid "Create confirmation"
 msgstr "Bescheinigung ausstellen"
 
 #: lino_welfare/modlib/aids/models.py:207
 msgid "Applies from"
 msgstr "Laufzeit von"
 
-#: lino_welfare/modlib/aids/models.py:238
-#: lino_welfare/modlib/aids/models.py:360
+#: lino_welfare/modlib/aids/models.py:238 lino_welfare/modlib/aids/models.py:360
 msgid "Only rows decided by this board."
 msgstr ""
 
-#: lino_welfare/modlib/aids/models.py:242
-#: lino_welfare/modlib/aids/models.py:369
+#: lino_welfare/modlib/aids/models.py:242 lino_welfare/modlib/aids/models.py:369
 msgid "Only confirmations about this aid type."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:299
 msgid "Grantings to confirm"
 msgstr "Zu bestätigende Hilfebeschlüsse"
 
@@ -367,16 +359,15 @@
 
 #: lino_welfare/modlib/aids/models.py:666
 msgid "Can refund"
 msgstr "Kostenrückerstattung"
 
 #: lino_welfare/modlib/aids/models.py:667
 msgid ""
-"Whether persons of this type can be used as doctor of a refund "
-"confirmation."
+"Whether persons of this type can be used as doctor of a refund confirmation."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:703
 msgid "Refund confirmation"
 msgstr "Kostenübernahmeschein"
 
 #: lino_welfare/modlib/aids/models.py:704
@@ -455,26 +446,24 @@
 msgstr "Art.61-Konvention"
 
 #: lino_welfare/modlib/art60/models.py:36
 #, fuzzy
 msgid "Art60 job supplyment"
 msgstr "Art.60§7-Konvention"
 
-#: lino_welfare/modlib/art60/models.py:50
-#: lino_welfare/modlib/jobs/models.py:118 lino_welfare/modlib/jobs/ui.py:38
+#: lino_welfare/modlib/art60/models.py:50 lino_welfare/modlib/jobs/models.py:118
+#: lino_welfare/modlib/jobs/ui.py:38
 msgid "Art60§7 job supplyment"
 msgstr "Art.60§7-Konvention"
 
-#: lino_welfare/modlib/art60/models.py:51
-#: lino_welfare/modlib/jobs/models.py:119
+#: lino_welfare/modlib/art60/models.py:51 lino_welfare/modlib/jobs/models.py:119
 msgid "Art60§7 job supplyments"
 msgstr "Art.60§7-Konventionen"
 
-#: lino_welfare/modlib/art60/models.py:58
-#: lino_welfare/modlib/art61/models.py:77
+#: lino_welfare/modlib/art60/models.py:58 lino_welfare/modlib/art61/models.py:77
 #: lino_welfare/modlib/jobs/models.py:132
 #, fuzzy
 msgid "Type"
 msgstr "Typ "
 
 #: lino_welfare/modlib/art60/models.py:98
 #, fuzzy
@@ -494,16 +483,15 @@
 #: lino_welfare/modlib/art60/models.py:114
 #: lino_welfare/modlib/art60/models.py:222
 #, fuzzy
 msgid "Monthly refund"
 msgstr "Monatsrate"
 
 #: lino_welfare/modlib/art60/models.py:115
-#: lino_welfare/modlib/jobs/models.py:141
-#: lino_welfare/modlib/jobs/models.py:264
+#: lino_welfare/modlib/jobs/models.py:141 lino_welfare/modlib/jobs/models.py:264
 msgid "hourly rate"
 msgstr "Stundensatz"
 
 #: lino_welfare/modlib/art60/models.py:116
 #: lino_welfare/modlib/jobs/models.py:142
 msgid "refund rate"
 msgstr "Rückzahlung"
@@ -511,35 +499,34 @@
 #: lino_welfare/modlib/art60/models.py:167
 #: lino_welfare/modlib/jobs/models.py:184
 #, python-format
 msgid "(%d candidatures have been marked inactive)"
 msgstr "( %d Kandidaturen wurden als inaktiv markiert)"
 
 #: lino_welfare/modlib/art60/models.py:168
-#: lino_welfare/modlib/isip/models.py:116
-#: lino_welfare/modlib/jobs/models.py:185
+#: lino_welfare/modlib/isip/models.py:116 lino_welfare/modlib/jobs/models.py:185
 #: lino_welfare/modlib/pcsw/actions.py:84
 #: lino_welfare/modlib/pcsw/actions.py:115
 msgid "Success"
 msgstr "Abschluss"
 
-#: lino_welfare/modlib/art60/models.py:225 lino_welfare/modlib/jobs/ui.py:172
+#: lino_welfare/modlib/art60/models.py:225 lino_welfare/modlib/jobs/ui.py:171
 msgid "Only contracts of type"
 msgstr "Vertragsart"
 
-#: lino_welfare/modlib/art60/models.py:276
+#: lino_welfare/modlib/art60/models.py:277
 #: lino_welfare/modlib/isip/choicelists.py:24
 msgid "Conventions"
 msgstr "Vorstrafen"
 
-#: lino_welfare/modlib/art60/models.py:322
+#: lino_welfare/modlib/art60/models.py:323
 msgid "My art60§7 contracts (IS)"
 msgstr ""
 
-#: lino_welfare/modlib/art60/models.py:335
+#: lino_welfare/modlib/art60/models.py:336
 msgid "My art60§7 contracts (GSS)"
 msgstr ""
 
 #: lino_welfare/modlib/art61/__init__.py:14
 msgid "Art61 job supplying"
 msgstr "Art.61-Konvention"
 
@@ -570,16 +557,15 @@
 msgid "Tutorate"
 msgstr ""
 
 #: lino_welfare/modlib/art61/choicelists.py:48
 msgid "Walloon Region"
 msgstr ""
 
-#: lino_welfare/modlib/art61/models.py:30
-#: lino_welfare/modlib/art61/models.py:66
+#: lino_welfare/modlib/art61/models.py:30 lino_welfare/modlib/art61/models.py:66
 msgid "Art61 job supplyment"
 msgstr "Art.61-Konvention"
 
 #: lino_welfare/modlib/art61/models.py:48
 msgid "Art61 job supplyment type"
 msgstr "Art.61-Konventionsart"
 
@@ -743,15 +729,15 @@
 msgstr ""
 
 #: lino_welfare/modlib/cal/models.py:416
 msgid "Delegated to client"
 msgstr ""
 
 #: lino_welfare/modlib/cbss/__init__.py:34
-#: lino_welfare/modlib/pcsw/models.py:399
+#: lino_welfare/modlib/pcsw/models.py:401
 msgid "CBSS"
 msgstr "ZDSS"
 
 #: lino_welfare/modlib/cbss/choicelists.py:20
 #: lino_welfare/modlib/cbss/mixins.py:85
 msgid "Sent"
 msgstr "Abgeschickt"
@@ -877,104 +863,103 @@
 msgid "First name"
 msgstr "Vorname"
 
 #: lino_welfare/modlib/cbss/mixins.py:684 lino_welfare/modlib/cbss/ui.py:185
 msgid "Last name"
 msgstr "Familienname"
 
-#: lino_welfare/modlib/cbss/models.py:40 lino_welfare/modlib/cbss/models.py:64
+#: lino_welfare/modlib/cbss/models.py:35 lino_welfare/modlib/cbss/models.py:59
 msgid "Sector"
 msgstr "Sektor"
 
-#: lino_welfare/modlib/cbss/models.py:41
+#: lino_welfare/modlib/cbss/models.py:36
 msgid "Sectors"
 msgstr "Sektoren"
 
-#: lino_welfare/modlib/cbss/models.py:45 lino_welfare/modlib/cbss/models.py:68
+#: lino_welfare/modlib/cbss/models.py:40 lino_welfare/modlib/cbss/models.py:63
 msgid "Code"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:46
+#: lino_welfare/modlib/cbss/models.py:41
 msgid "Subcode"
 msgstr "Unter-Code"
 
-#: lino_welfare/modlib/cbss/models.py:47
+#: lino_welfare/modlib/cbss/models.py:42
 msgid "Abbreviation"
 msgstr "Abkürzung"
 
-#: lino_welfare/modlib/cbss/models.py:61
+#: lino_welfare/modlib/cbss/models.py:56
 msgid "Purpose"
 msgstr "Eigenschafts-Code"
 
-#: lino_welfare/modlib/cbss/models.py:62
+#: lino_welfare/modlib/cbss/models.py:57
 msgid "Purposes"
 msgstr "Eigenschafts-Codes"
 
-#: lino_welfare/modlib/cbss/models.py:91
+#: lino_welfare/modlib/cbss/models.py:86
 msgid "IdentifyPerson Request"
 msgstr "IdentifyPerson-Anfrage"
 
-#: lino_welfare/modlib/cbss/models.py:92
+#: lino_welfare/modlib/cbss/models.py:87
 msgid "IdentifyPerson Requests"
 msgstr "IdentifyPerson-Anfragen"
 
-#: lino_welfare/modlib/cbss/models.py:96
+#: lino_welfare/modlib/cbss/models.py:91
 msgid "Middle name"
 msgstr "Zwischenname"
 
-#: lino_welfare/modlib/cbss/models.py:101
+#: lino_welfare/modlib/cbss/models.py:96
 msgid "Tolerance"
 msgstr "Toleranz"
 
-#: lino_welfare/modlib/cbss/models.py:250
+#: lino_welfare/modlib/cbss/models.py:245
 msgid "ManageAccess Request"
 msgstr "ManageAccess-Anfrage"
 
-#: lino_welfare/modlib/cbss/models.py:251
+#: lino_welfare/modlib/cbss/models.py:246
 msgid "ManageAccess Requests"
 msgstr "ManageAccess-Anfragen"
 
-#: lino_welfare/modlib/cbss/models.py:287
+#: lino_welfare/modlib/cbss/models.py:282
 msgid "Period until"
 msgstr "Periode bis"
 
-#: lino_welfare/modlib/cbss/models.py:411
+#: lino_welfare/modlib/cbss/models.py:406
 msgid "Tx25 Request"
 msgstr "Tx25-Anfrage"
 
-#: lino_welfare/modlib/cbss/models.py:412
+#: lino_welfare/modlib/cbss/models.py:407
 msgid "Tx25 Requests"
 msgstr "Tx25-Anfragen"
 
-#: lino_welfare/modlib/cbss/models.py:420
-#: lino_welfare/modlib/pcsw/models.py:513
+#: lino_welfare/modlib/cbss/models.py:415 lino_welfare/modlib/pcsw/models.py:515
 msgid "History"
 msgstr "Historie"
 
-#: lino_welfare/modlib/cbss/models.py:563
+#: lino_welfare/modlib/cbss/models.py:558
 msgid "Requesting organisation"
 msgstr "Anfragende Organisation"
 
-#: lino_welfare/modlib/cbss/models.py:576
+#: lino_welfare/modlib/cbss/models.py:571
 msgid "SSDN User Id"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:582
+#: lino_welfare/modlib/cbss/models.py:577
 msgid "SSDN email address"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:589
+#: lino_welfare/modlib/cbss/models.py:584
 msgid "HTTP username"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:596
+#: lino_welfare/modlib/cbss/models.py:591
 msgid "HTTP password"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:631
+#: lino_welfare/modlib/cbss/models.py:626
 msgid "CBSS summary"
 msgstr "Zusammenfassung ZDSS"
 
 #: lino_welfare/modlib/cbss/tx25.py:42
 msgid "until "
 msgstr "bis "
 
@@ -1112,16 +1097,15 @@
 
 #: lino_welfare/modlib/cbss/tx25.py:709 lino_welfare/modlib/cbss/tx25.py:751
 msgid "SSIN "
 msgstr "NR-Nr. "
 
 #: lino_welfare/modlib/cbss/tx25.py:729
 #: lino_welfare/modlib/immersion/models.py:87
-#: lino_welfare/modlib/isip/models.py:149
-#: lino_welfare/modlib/jobs/models.py:127
+#: lino_welfare/modlib/isip/models.py:149 lino_welfare/modlib/jobs/models.py:127
 msgid "Organization"
 msgstr "Organisation"
 
 #: lino_welfare/modlib/cbss/tx25.py:810 lino_welfare/modlib/isip/models.py:56
 msgid "Reference"
 msgstr "Referenz"
 
@@ -1362,17 +1346,16 @@
 msgid "Driving Licenses"
 msgstr "Führerscheine"
 
 #: lino_welfare/modlib/cbss/tx25.py:1217
 msgid "Identity Cards"
 msgstr "Personalausweise"
 
-#: lino_welfare/modlib/cbss/tx25.py:1233 lino_welfare/modlib/pcsw/models.py:116
-#: lino_welfare/modlib/pcsw/models.py:905
-#: lino_welfare/modlib/pcsw/models.py:961
+#: lino_welfare/modlib/cbss/tx25.py:1233 lino_welfare/modlib/pcsw/models.py:117
+#: lino_welfare/modlib/pcsw/models.py:907 lino_welfare/modlib/pcsw/models.py:963
 #: lino_welfare/modlib/reception/models.py:108
 #: lino_welfare/modlib/reception/models.py:136
 msgid "Reason"
 msgstr "Begründung"
 
 #: lino_welfare/modlib/cbss/tx25.py:1246
 msgid "Legal cohabitations"
@@ -1447,16 +1430,15 @@
 msgid "Birth location"
 msgstr "Geburtsort"
 
 #: lino_welfare/modlib/cbss/ui.py:205
 msgid "Civil state"
 msgstr "Zivilstand"
 
-#: lino_welfare/modlib/cbss/ui.py:209
-#: lino_welfare/modlib/xcourses/models.py:612
+#: lino_welfare/modlib/cbss/ui.py:209 lino_welfare/modlib/xcourses/models.py:612
 msgid "Address"
 msgstr "Adresse"
 
 #: lino_welfare/modlib/cbss/ui.py:219 lino_welfare/modlib/cbss/ui.py:239
 msgid "Requested action"
 msgstr "Angefragte Aktion"
 
@@ -1507,21 +1489,21 @@
 #: lino_welfare/modlib/contacts/models.py:313
 msgid "Contact"
 msgstr "Kontakt"
 
 #: lino_welfare/modlib/contacts/models.py:149
 #: lino_welfare/modlib/contacts/models.py:237
 #: lino_welfare/modlib/contacts/models.py:328
-#: lino_welfare/modlib/pcsw/models.py:533
+#: lino_welfare/modlib/pcsw/models.py:535
 msgid "Miscellaneous"
 msgstr "Sonstiges"
 
 #: lino_welfare/modlib/contacts/models.py:158
 #: lino_welfare/modlib/households/models.py:81
-#: lino_welfare/modlib/pcsw/models.py:449
+#: lino_welfare/modlib/pcsw/models.py:451
 msgid "Person"
 msgstr ""
 
 #: lino_welfare/modlib/contacts/models.py:159
 msgid "Persons"
 msgstr "Personen"
 
@@ -1542,51 +1524,37 @@
 msgid "Show also obsolete records."
 msgstr "Auch veraltete Daten"
 
 #: lino_welfare/modlib/contacts/models.py:276
 msgid "VAT id"
 msgstr "MWSt-Nr"
 
-#: lino_welfare/modlib/cv/models.py:39
+#: lino_welfare/modlib/cv/models.py:23
+#, fuzzy
+msgid "Skills"
+msgstr "Sonstige Fähigkeiten"
+
+#: lino_welfare/modlib/cv/models.py:24
+#, fuzzy
+msgid "Soft skills"
+msgstr "Sonstige Fähigkeiten"
+
+#: lino_welfare/modlib/cv/models.py:25
+#, fuzzy
+msgid "Obstacles"
+msgstr "Sonstige Hindernisse"
+
+#: lino_welfare/modlib/cv/models.py:40
 msgid "Property"
 msgstr "Eigenschaft"
 
-#: lino_welfare/modlib/cv/models.py:40
+#: lino_welfare/modlib/cv/models.py:41
 msgid "Properties"
 msgstr "Eigenschaften"
 
-#: lino_welfare/modlib/cv/models.py:101
-#, python-format
-msgid "(SiteConfig %s is empty)"
-msgstr "(Site-Parameter %s ist leer)"
-
-#: lino_welfare/modlib/cv/models.py:125
-msgid "Skills Property Group"
-msgstr "Eigenschaftsgruppe Fähigkeiten"
-
-#: lino_welfare/modlib/cv/models.py:127
-msgid "The property group to be used as master for the SkillsByPerson table."
-msgstr ""
-
-#: lino_welfare/modlib/cv/models.py:136
-msgid "Soft Skills Property Group"
-msgstr "Eigenschaftsgruppe Sozialkompetenzen"
-
-#: lino_welfare/modlib/cv/models.py:138
-msgid "The property group to be used as master for the SoftSkillsByPerson table."
-msgstr ""
-
-#: lino_welfare/modlib/cv/models.py:147
-msgid "Obstacles Property Group"
-msgstr "Eigenschaftsgruppe Hindernisse"
-
-#: lino_welfare/modlib/cv/models.py:149
-msgid "The property group to be used as master for the ObstaclesByPerson table."
-msgstr ""
-
 #: lino_welfare/modlib/debts/__init__.py:25
 msgid "Debts mediation"
 msgstr "Schuldnerberatung"
 
 #: lino_welfare/modlib/debts/choicelists.py:23
 #, fuzzy
 msgid "Financial statement"
@@ -1871,16 +1839,16 @@
 #: lino_welfare/modlib/debts/models.py:462
 #: lino_welfare/modlib/debts/models.py:576 lino_welfare/modlib/debts/ui.py:473
 msgid "Debt collection agency"
 msgstr "Schuldeneintreiber"
 
 #: lino_welfare/modlib/debts/models.py:463
 msgid ""
-"Leave empty for simple debts, otherwise select         here the "
-"responsible bailiff or collection agency"
+"Leave empty for simple debts, otherwise select         here the responsible "
+"bailiff or collection agency"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:529
 msgid "Periods must be > 0"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:533
@@ -2002,20 +1970,19 @@
 
 #: lino_welfare/modlib/debts/ui.py:641
 #, fuzzy
 msgid ""
 "Répartition au marc-le-franc.\n"
 "A table with one row per entry in Liabilities which has \"distribute\" "
 "checked,\n"
-"proportionally distributing the `Distributable amount` among the debtors."
-"\n"
+"proportionally distributing the `Distributable amount` among the debtors.\n"
 msgstr ""
 "Répartition au marc-le-franc.\n"
-"Tabelle mit einer Zeile pro Eintrag in \"Verpflichtungen\", dessen Option"
-" \"verteilen\" angekreuzt ist. \n"
+"Tabelle mit einer Zeile pro Eintrag in \"Verpflichtungen\", dessen Option "
+"\"verteilen\" angekreuzt ist. \n"
 "Der verfügbare Betrag wird dabei proportional zum geschuldeten Betrag "
 "aufgeteilt.\n"
 
 #: lino_welfare/modlib/debts/ui.py:679
 msgid "%"
 msgstr ""
 
@@ -2192,16 +2159,15 @@
 msgid "Disbursement orders"
 msgstr "Ausgabeanweisungen"
 
 #: lino_welfare/modlib/finan/models.py:59
 msgid "Internal reference"
 msgstr "Interne Referenz"
 
-#: lino_welfare/modlib/finan/models.py:61
-#: lino_welfare/modlib/finan/models.py:66
+#: lino_welfare/modlib/finan/models.py:61 lino_welfare/modlib/finan/models.py:66
 msgid "External reference"
 msgstr "Externe Referenz"
 
 #: lino_welfare/modlib/households/models.py:133
 #, python-format
 msgid "%(count)d adult"
 msgid_plural "%(count)d adults"
@@ -2244,26 +2210,25 @@
 msgstr ""
 
 #: lino_welfare/modlib/immersion/models.py:70
 msgid "Immersion training goals"
 msgstr ""
 
 #: lino_welfare/modlib/immersion/models.py:97
-#: lino_welfare/modlib/isip/mixins.py:325
+#: lino_welfare/modlib/isip/mixins.py:326
 msgid "reference person"
 msgstr "Referenzperson"
 
 #: lino_welfare/modlib/immersion/models.py:99
-#: lino_welfare/modlib/isip/mixins.py:327
+#: lino_welfare/modlib/isip/mixins.py:328
 msgid "responsibilities"
 msgstr "Aufgabenbereich"
 
 #: lino_welfare/modlib/immersion/models.py:117
-#: lino_welfare/modlib/isip/mixins.py:317
-#: lino_welfare/modlib/isip/mixins.py:415
+#: lino_welfare/modlib/isip/mixins.py:318 lino_welfare/modlib/isip/mixins.py:416
 #: lino_welfare/modlib/isip/models.py:214
 msgid "Responsible (IS)"
 msgstr "Verantwortlicher (DSBE)"
 
 #: lino_welfare/modlib/immersion/ui.py:99
 #, fuzzy
 msgid "Only immersion trainings of type"
@@ -2305,15 +2270,15 @@
 msgid "Available"
 msgstr "Verfügbar"
 
 #: lino_welfare/modlib/integ/models.py:78
 msgid "Integration Clients"
 msgstr "DSBE-Klienten"
 
-#: lino_welfare/modlib/integ/models.py:95 lino_welfare/modlib/pcsw/models.py:81
+#: lino_welfare/modlib/integ/models.py:95 lino_welfare/modlib/pcsw/models.py:82
 msgid "Integration phase"
 msgstr "Integrationsphase"
 
 #: lino_welfare/modlib/integ/models.py:97
 msgid "Language knowledge"
 msgstr "Sprachkenntnis"
 
@@ -2411,16 +2376,15 @@
 
 #: lino_welfare/modlib/integ/models.py:599
 msgid "Activity Report"
 msgstr "Tätigkeitsbericht"
 
 #: lino_welfare/modlib/integ/models.py:606
 #: lino_welfare/modlib/isip/__init__.py:14
-#: lino_welfare/modlib/isip/models.py:183
-#: lino_welfare/modlib/isip/models.py:258
+#: lino_welfare/modlib/isip/models.py:183 lino_welfare/modlib/isip/models.py:258
 msgid "ISIP"
 msgstr "VSE"
 
 #: lino_welfare/modlib/integ/models.py:630
 msgid "Indicateurs généraux"
 msgstr "Allgemeine Indikatoren"
 
@@ -2504,79 +2468,79 @@
 msgid "Trainings"
 msgstr "Ausbildungen"
 
 #: lino_welfare/modlib/isip/mixins.py:51
 msgid "Full name"
 msgstr "Voller Name"
 
-#: lino_welfare/modlib/isip/mixins.py:82
+#: lino_welfare/modlib/isip/mixins.py:83
 msgid "applies from"
 msgstr "Laufzeit von"
 
-#: lino_welfare/modlib/isip/mixins.py:83
+#: lino_welfare/modlib/isip/mixins.py:84
 msgid "applies until"
 msgstr "Laufzeit bis"
 
-#: lino_welfare/modlib/isip/mixins.py:85
+#: lino_welfare/modlib/isip/mixins.py:86
 msgid "date decided"
 msgstr "Beschlossen am"
 
-#: lino_welfare/modlib/isip/mixins.py:87
+#: lino_welfare/modlib/isip/mixins.py:88
 msgid "date issued"
 msgstr "Ausgestellt am"
 
-#: lino_welfare/modlib/isip/mixins.py:91 lino_welfare/modlib/isip/mixins.py:417
+#: lino_welfare/modlib/isip/mixins.py:92 lino_welfare/modlib/isip/mixins.py:418
 msgid "Responsible (GSS)"
 msgstr "Verantwortlicher (ASD)"
 
-#: lino_welfare/modlib/isip/mixins.py:105
+#: lino_welfare/modlib/isip/mixins.py:106
 #: lino_welfare/modlib/xcourses/models.py:369
 msgid "date ended"
 msgstr "Enddatum"
 
-#: lino_welfare/modlib/isip/mixins.py:194
+#: lino_welfare/modlib/isip/mixins.py:195
 msgid "Contract ends before it started."
 msgstr "Vertrag endet bevor er startet."
 
-#: lino_welfare/modlib/isip/mixins.py:210
+#: lino_welfare/modlib/isip/mixins.py:211
 msgid "You must specify a contract type."
 msgstr ""
 
-#: lino_welfare/modlib/isip/mixins.py:242
+#: lino_welfare/modlib/isip/mixins.py:243
 #, python-format
 msgid "Evaluation %d"
 msgstr "Auswertung %d"
 
-#: lino_welfare/modlib/isip/mixins.py:253
+#: lino_welfare/modlib/isip/mixins.py:254
 msgid "Contract ends in a month"
 msgstr "Vertrag endet in einem Monat"
 
-#: lino_welfare/modlib/isip/mixins.py:373
+#: lino_welfare/modlib/isip/mixins.py:374
 #, python-format
 msgid "Date range %(p1)s lies outside of coached period %(p2)s."
 msgstr "Datumsbereich %(p1)s außerhalb Begleitungsperiode %(p2)s."
 
-#: lino_welfare/modlib/isip/mixins.py:379
+#: lino_welfare/modlib/isip/mixins.py:380
 msgid "Date range overlaps with {ctype} #{id}."
 msgstr "Datumsbereich überschneidet sich mit {ctype} #{id}"
 
-#: lino_welfare/modlib/isip/mixins.py:392
+#: lino_welfare/modlib/isip/mixins.py:393
 #, python-format
 msgid "%(ctype)s #%(id)s : %(msg)s"
 msgstr ""
 
-#: lino_welfare/modlib/isip/mixins.py:400
+#: lino_welfare/modlib/isip/mixins.py:401
 msgid "Check for overlapping contracts"
 msgstr "Auf Vertragsüberschneidungen prüfen"
 
-#: lino_welfare/modlib/isip/mixins.py:420
+#: lino_welfare/modlib/isip/mixins.py:421
 msgid "Successfully ended"
 msgstr "Erfolgreich abgeschlossen"
 
-#: lino_welfare/modlib/isip/mixins.py:430
+#: lino_welfare/modlib/isip/mixins.py:431
 msgid "Only contracts with this company as partner."
 msgstr ""
 
 #: lino_welfare/modlib/isip/models.py:53
 msgid "ISIP Type"
 msgstr "VSE-Art"
 
@@ -2604,18 +2568,17 @@
 msgid "Reason of termination"
 msgstr "Beendigungsgrund"
 
 #: lino_welfare/modlib/isip/models.py:111
 msgid "Contract termination reasons"
 msgstr "Vertragsbeendigungsgründe"
 
-#: lino_welfare/modlib/isip/models.py:113
-#: lino_welfare/modlib/jobs/models.py:404
-#: lino_welfare/modlib/pcsw/models.py:825
-#: lino_welfare/modlib/pcsw/models.py:1005
+#: lino_welfare/modlib/isip/models.py:113 lino_welfare/modlib/jobs/models.py:404
+#: lino_welfare/modlib/pcsw/models.py:827
+#: lino_welfare/modlib/pcsw/models.py:1007
 msgid "Designation"
 msgstr "Bezeichnung"
 
 #: lino_welfare/modlib/isip/models.py:118
 msgid "Require date ended"
 msgstr "erfordert Enddatum"
 
@@ -2631,16 +2594,15 @@
 msgid "duties company"
 msgstr "Verpflichtungen Firma"
 
 #: lino_welfare/modlib/isip/models.py:184
 msgid "ISIPs"
 msgstr "VSEs"
 
-#: lino_welfare/modlib/isip/models.py:189
-#: lino_welfare/modlib/jobs/models.py:263
+#: lino_welfare/modlib/isip/models.py:189 lino_welfare/modlib/jobs/models.py:263
 msgid "Contract Type"
 msgstr "Vertragsart"
 
 #: lino_welfare/modlib/isip/models.py:194
 msgid "stages"
 msgstr "Etappen"
 
@@ -2662,21 +2624,21 @@
 
 #: lino_welfare/modlib/isip/models.py:209
 msgid "duties person"
 msgstr "Verpflichtungen Person"
 
 #: lino_welfare/modlib/isip/models.py:238
 msgid ""
-"Cannot print {} because there is no active aid confirmation and Duties "
-"(PCSW) is empty."
+"Cannot print {} because there is no active aid confirmation and Duties (PCSW) "
+"is empty."
 msgstr ""
 "Kann {} nicht drucken, weil es keine aktive Hilfebestätigung gibt und "
 "Verpflichtungen ÖSHZ leer ist."
 
-#: lino_welfare/modlib/isip/models.py:352
+#: lino_welfare/modlib/isip/models.py:354
 #, fuzzy
 msgid "Proceedings"
 msgstr "prodziert"
 
 #: lino_welfare/modlib/jobs/__init__.py:18
 msgid "Job supplying"
 msgstr "Art. 60§7"
@@ -2761,16 +2723,15 @@
 msgid "Job Offer"
 msgstr "Stellenangebot"
 
 #: lino_welfare/modlib/jobs/models.py:217
 msgid "Job Offers"
 msgstr "Stellenangebote"
 
-#: lino_welfare/modlib/jobs/models.py:222
-#: lino_welfare/modlib/jobs/models.py:258
+#: lino_welfare/modlib/jobs/models.py:222 lino_welfare/modlib/jobs/models.py:258
 #: lino_welfare/modlib/xcourses/models.py:78
 #: lino_welfare/modlib/xcourses/models.py:108
 #: lino_welfare/modlib/xcourses/models.py:179
 msgid "Name"
 msgstr ""
 
 #: lino_welfare/modlib/jobs/models.py:227
@@ -2787,20 +2748,19 @@
 msgstr "Beginndatum"
 
 #: lino_welfare/modlib/jobs/models.py:254 lino_welfare/modlib/jobs/ui.py:434
 msgid "Job"
 msgstr "Stelle"
 
 #: lino_welfare/modlib/jobs/models.py:255 lino_welfare/modlib/jobs/ui.py:83
-#: lino_welfare/modlib/jobs/ui.py:102
+#: lino_welfare/modlib/jobs/ui.py:101
 msgid "Jobs"
 msgstr "Stellen"
 
-#: lino_welfare/modlib/jobs/models.py:259
-#: lino_welfare/modlib/jobs/models.py:399
+#: lino_welfare/modlib/jobs/models.py:259 lino_welfare/modlib/jobs/models.py:399
 msgid "Job Type"
 msgstr "Stellenart"
 
 #: lino_welfare/modlib/jobs/models.py:265
 msgid "capacity"
 msgstr "Kapazität"
 
@@ -3056,15 +3016,15 @@
 msgstr "Aufwand"
 
 #: lino_welfare/modlib/newcomers/models.py:124
 msgid "Competence"
 msgstr "Kompetenz"
 
 #: lino_welfare/modlib/newcomers/models.py:125
-#: lino_welfare/modlib/pcsw/models.py:550
+#: lino_welfare/modlib/pcsw/models.py:552
 msgid "Competences"
 msgstr "Kompetenzen"
 
 #: lino_welfare/modlib/newcomers/models.py:143
 #, fuzzy
 msgid "User"
 msgstr "Ablehnen"
@@ -3179,15 +3139,15 @@
 
 #: lino_welfare/modlib/pcsw/actions.py:140
 #, python-format
 msgid "This will end %(count)d coachings of %(client)s."
 msgstr "Hierdurch werden %(count)d Begleitungen von %(client)s beendet."
 
 #: lino_welfare/modlib/pcsw/choicelists.py:15
-#: lino_welfare/modlib/pcsw/models.py:901
+#: lino_welfare/modlib/pcsw/models.py:903
 msgid "Dispense"
 msgstr "Dispenz"
 
 #: lino_welfare/modlib/pcsw/choicelists.py:27
 msgid "Penalty"
 msgstr "AG-Sperre"
 
@@ -3211,297 +3171,297 @@
 msgid "Client did not return"
 msgstr "Antragsteller ist nicht zurück gekommen"
 
 #: lino_welfare/modlib/pcsw/models.py:73
 msgid "Clients"
 msgstr "Klienten"
 
-#: lino_welfare/modlib/pcsw/models.py:88
+#: lino_welfare/modlib/pcsw/models.py:89
 msgid "Lives in Belgium since"
 msgstr "Lebt in Belgien seit"
 
-#: lino_welfare/modlib/pcsw/models.py:90
+#: lino_welfare/modlib/pcsw/models.py:91
 #, fuzzy
 msgid "Residence until"
 msgstr "Register"
 
-#: lino_welfare/modlib/pcsw/models.py:92
+#: lino_welfare/modlib/pcsw/models.py:93
 msgid "Unemployed since"
 msgstr "Arbeitslos seit"
 
-#: lino_welfare/modlib/pcsw/models.py:93
+#: lino_welfare/modlib/pcsw/models.py:94
 msgid "Since when the client has not been employed in any regular job."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:96
+#: lino_welfare/modlib/pcsw/models.py:97
 msgid "Seeking work since"
 msgstr "Sucht Arbeit seit"
 
-#: lino_welfare/modlib/pcsw/models.py:97
+#: lino_welfare/modlib/pcsw/models.py:98
 msgid "Since when the client is seeking for a job."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:99
+#: lino_welfare/modlib/pcsw/models.py:100
 msgid "Needs residence permit"
 msgstr "Braucht Aufenthaltserlaubnis"
 
-#: lino_welfare/modlib/pcsw/models.py:101
+#: lino_welfare/modlib/pcsw/models.py:102
 msgid "Needs work permit"
 msgstr "Braucht Arb.Erl."
 
-#: lino_welfare/modlib/pcsw/models.py:103
+#: lino_welfare/modlib/pcsw/models.py:104
 msgid "suspended until"
 msgstr "Wartezeit bis"
 
-#: lino_welfare/modlib/pcsw/models.py:107
+#: lino_welfare/modlib/pcsw/models.py:108
 msgid "Declared name"
 msgstr "Deklarierter Name"
 
-#: lino_welfare/modlib/pcsw/models.py:109
+#: lino_welfare/modlib/pcsw/models.py:110
 msgid "is seeking work"
 msgstr "Arbeit suchend"
 
-#: lino_welfare/modlib/pcsw/models.py:113
+#: lino_welfare/modlib/pcsw/models.py:114
 msgid "Unavailable until"
 msgstr "Nicht verfügbar bis"
 
-#: lino_welfare/modlib/pcsw/models.py:118
+#: lino_welfare/modlib/pcsw/models.py:119
 msgid "Other obstacles"
 msgstr "Sonstige Hindernisse"
 
-#: lino_welfare/modlib/pcsw/models.py:119
+#: lino_welfare/modlib/pcsw/models.py:120
 msgid "Other skills"
 msgstr "Sonstige Fähigkeiten"
 
-#: lino_welfare/modlib/pcsw/models.py:124
+#: lino_welfare/modlib/pcsw/models.py:125
 msgid "Contact person at local job office"
 msgstr "Kontaktperson ADG"
 
-#: lino_welfare/modlib/pcsw/models.py:216
+#: lino_welfare/modlib/pcsw/models.py:217
 msgid "Circular reference"
 msgstr "Redundanter RÜckbezug"
 
-#: lino_welfare/modlib/pcsw/models.py:243
+#: lino_welfare/modlib/pcsw/models.py:244
 msgid "eID card expires in 2 months"
 msgstr "eID-Karte läuft in 2 Monaten ab"
 
-#: lino_welfare/modlib/pcsw/models.py:247
+#: lino_welfare/modlib/pcsw/models.py:248
 msgid "becomes available again in 1 month"
 msgstr "wird wieder verfügbar in 1 Monat"
 
-#: lino_welfare/modlib/pcsw/models.py:250
+#: lino_welfare/modlib/pcsw/models.py:251
 msgid "work permit suspension ends in 1 month"
 msgstr "Arbeitslosen-Wartezeit endet in 1 Monat"
 
-#: lino_welfare/modlib/pcsw/models.py:330
+#: lino_welfare/modlib/pcsw/models.py:332
 msgid "Contract starts"
 msgstr "Vertrag beginnt"
 
-#: lino_welfare/modlib/pcsw/models.py:336
+#: lino_welfare/modlib/pcsw/models.py:338
 msgid "Contract ends"
 msgstr "Vertrag endet"
 
-#: lino_welfare/modlib/pcsw/models.py:344
+#: lino_welfare/modlib/pcsw/models.py:346
 msgid "Working at "
 msgstr "Arbeitet bei"
 
-#: lino_welfare/modlib/pcsw/models.py:351
+#: lino_welfare/modlib/pcsw/models.py:353
 #, fuzzy
 msgid "Active contract"
 msgstr "erlaubt in Verträgen"
 
-#: lino_welfare/modlib/pcsw/models.py:471
+#: lino_welfare/modlib/pcsw/models.py:473
 msgid "Human Links"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:476
+#: lino_welfare/modlib/pcsw/models.py:478
 msgid "Coaches"
 msgstr "Begleiter"
 
-#: lino_welfare/modlib/pcsw/models.py:499
+#: lino_welfare/modlib/pcsw/models.py:501
 msgid "Job search"
 msgstr "Arbeitssuche"
 
-#: lino_welfare/modlib/pcsw/models.py:525
+#: lino_welfare/modlib/pcsw/models.py:527
 msgid "Calendar"
 msgstr "Kalender"
 
-#: lino_welfare/modlib/pcsw/models.py:540
+#: lino_welfare/modlib/pcsw/models.py:542
 msgid "Career"
 msgstr "Lebenslauf"
 
-#: lino_welfare/modlib/pcsw/models.py:545
+#: lino_welfare/modlib/pcsw/models.py:547
 msgid "Languages"
 msgstr "Sprachen"
 
-#: lino_welfare/modlib/pcsw/models.py:556
+#: lino_welfare/modlib/pcsw/models.py:558
 msgid "Contracts"
 msgstr "Verträge"
 
-#: lino_welfare/modlib/pcsw/models.py:589
+#: lino_welfare/modlib/pcsw/models.py:591
 msgid "Coached by"
 msgstr "Begleitet durch"
 
-#: lino_welfare/modlib/pcsw/models.py:593
+#: lino_welfare/modlib/pcsw/models.py:595
 msgid "and by"
 msgstr "und durch"
 
-#: lino_welfare/modlib/pcsw/models.py:597
+#: lino_welfare/modlib/pcsw/models.py:599
 msgid "Nationality"
 msgstr "Staatsangehörigkeit"
 
-#: lino_welfare/modlib/pcsw/models.py:600
+#: lino_welfare/modlib/pcsw/models.py:602
 msgid "Extended filter criteria, e.g.:"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:602
+#: lino_welfare/modlib/pcsw/models.py:604
 msgid "Active: All those who have some active coaching."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:604
+#: lino_welfare/modlib/pcsw/models.py:606
 msgid "Only primary clients"
 msgstr "Nur primäre Begleitungen"
 
-#: lino_welfare/modlib/pcsw/models.py:743
+#: lino_welfare/modlib/pcsw/models.py:745
 msgid "and"
 msgstr "und"
 
-#: lino_welfare/modlib/pcsw/models.py:748
+#: lino_welfare/modlib/pcsw/models.py:750
 #, python-format
 msgid " on %(date)s"
 msgstr " am %(date)s"
 
-#: lino_welfare/modlib/pcsw/models.py:752
+#: lino_welfare/modlib/pcsw/models.py:754
 #, python-format
 msgid "Coached on %s"
 msgstr "Begleitet am %s"
 
-#: lino_welfare/modlib/pcsw/models.py:801
+#: lino_welfare/modlib/pcsw/models.py:803
 msgid "Check for valid identification"
 msgstr "Auf gültige Identifizierungsangaben prüfen"
 
-#: lino_welfare/modlib/pcsw/models.py:810
+#: lino_welfare/modlib/pcsw/models.py:812
 msgid "Neither valid eId data nor alternative identifying document."
 msgstr "Weder gültige eID-Daten noch identifizierendes Dokument."
 
-#: lino_welfare/modlib/pcsw/models.py:826
+#: lino_welfare/modlib/pcsw/models.py:828
 msgid "Reference name"
 msgstr "Referenzname"
 
-#: lino_welfare/modlib/pcsw/models.py:827
+#: lino_welfare/modlib/pcsw/models.py:829
 msgid "Considered active"
 msgstr "aktive Phase"
 
-#: lino_welfare/modlib/pcsw/models.py:832
+#: lino_welfare/modlib/pcsw/models.py:834
 msgid "Integration Phase"
 msgstr "Integrationsphase"
 
-#: lino_welfare/modlib/pcsw/models.py:833
+#: lino_welfare/modlib/pcsw/models.py:835
 msgid "Integration Phases"
 msgstr "Integrationsphasen"
 
-#: lino_welfare/modlib/pcsw/models.py:840
+#: lino_welfare/modlib/pcsw/models.py:842
 msgid "Liste des phases d'intégration possibles."
 msgstr "Liste der möglichen Integrationsphasen."
 
-#: lino_welfare/modlib/pcsw/models.py:855
+#: lino_welfare/modlib/pcsw/models.py:857
 msgid "activity"
 msgstr "Beruf"
 
-#: lino_welfare/modlib/pcsw/models.py:856
+#: lino_welfare/modlib/pcsw/models.py:858
 msgid "activities"
 msgstr "Berufe"
 
-#: lino_welfare/modlib/pcsw/models.py:858
+#: lino_welfare/modlib/pcsw/models.py:860
 msgid "Appears in Listing 104"
 msgstr "Listing 104"
 
-#: lino_welfare/modlib/pcsw/models.py:865
+#: lino_welfare/modlib/pcsw/models.py:867
 msgid "Liste des \"activités\" ou \"codes profession\"."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:880
+#: lino_welfare/modlib/pcsw/models.py:882
 msgid "Dispense reason"
 msgstr "Dispenzgrund"
 
-#: lino_welfare/modlib/pcsw/models.py:881
+#: lino_welfare/modlib/pcsw/models.py:883
 msgid "Dispense reasons"
 msgstr "Dispenzgründe"
 
-#: lino_welfare/modlib/pcsw/models.py:890
+#: lino_welfare/modlib/pcsw/models.py:892
 msgid "A list of reasons for being dispensed"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:902
+#: lino_welfare/modlib/pcsw/models.py:904
 msgid "Dispenses"
 msgstr "Dispenzen"
 
-#: lino_welfare/modlib/pcsw/models.py:909
+#: lino_welfare/modlib/pcsw/models.py:911
 msgid "Dispensed from"
 msgstr "Dispenziert seit"
 
-#: lino_welfare/modlib/pcsw/models.py:917
+#: lino_welfare/modlib/pcsw/models.py:919
 msgid "Liste de dispenses"
 msgstr "Liste aller Dispenzen"
 
-#: lino_welfare/modlib/pcsw/models.py:935
+#: lino_welfare/modlib/pcsw/models.py:937
 msgid "Unemployment exclusion type"
 msgstr "AG-Sperrgrund"
 
-#: lino_welfare/modlib/pcsw/models.py:936
+#: lino_welfare/modlib/pcsw/models.py:938
 msgid "Unemployment exclusion types"
 msgstr "AG-Sperrgründe"
 
-#: lino_welfare/modlib/pcsw/models.py:945
+#: lino_welfare/modlib/pcsw/models.py:947
 msgid ""
 "Liste des raisons possibles d'arrêter temporairement\n"
 "    le paiement d'une aide financière prévue."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:956
+#: lino_welfare/modlib/pcsw/models.py:958
 msgid "Exclusion from unemployment"
 msgstr "AG-Sperre"
 
-#: lino_welfare/modlib/pcsw/models.py:957
+#: lino_welfare/modlib/pcsw/models.py:959
 msgid "Exclusions from unemployment"
 msgstr "AG-Sperren"
 
-#: lino_welfare/modlib/pcsw/models.py:964
+#: lino_welfare/modlib/pcsw/models.py:966
 msgid "Excluded from"
 msgstr "AG-Sperre seit"
 
-#: lino_welfare/modlib/pcsw/models.py:980
+#: lino_welfare/modlib/pcsw/models.py:982
 msgid "Liste des exclusions."
 msgstr "Liste der Arbeitslosengeld-Sperren"
 
-#: lino_welfare/modlib/pcsw/models.py:986
+#: lino_welfare/modlib/pcsw/models.py:988
 msgid "Unemployment situation"
 msgstr "AG-Sperren"
 
-#: lino_welfare/modlib/pcsw/models.py:998
+#: lino_welfare/modlib/pcsw/models.py:1000
 msgid "Conviction"
 msgstr "Vorstrafe"
 
-#: lino_welfare/modlib/pcsw/models.py:999
+#: lino_welfare/modlib/pcsw/models.py:1001
 msgid "Convictions"
 msgstr "Vorstrafen"
 
-#: lino_welfare/modlib/pcsw/models.py:1003
+#: lino_welfare/modlib/pcsw/models.py:1005
 msgid "Prejudicial"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:1038
+#: lino_welfare/modlib/pcsw/models.py:1040
 msgid "aid type"
 msgstr "Sozialhilfeart"
 
-#: lino_welfare/modlib/pcsw/models.py:1039
+#: lino_welfare/modlib/pcsw/models.py:1041
 msgid "aid types"
 msgstr "Sozialhilfearten"
 
-#: lino_welfare/modlib/pcsw/models.py:1043
+#: lino_welfare/modlib/pcsw/models.py:1045
 msgid "Liste des types d'aide financière."
 msgstr ""
 
 #: lino_welfare/modlib/pcsw/fixtures/std.py:26
 msgid "Formation"
 msgstr "Ausbildung"
 
@@ -3605,36 +3565,36 @@
 msgstr "Klient muss eID-Karte einlesen!"
 
 #: lino_welfare/modlib/reception/models.py:228
 msgid "Do you still want to issue an excerpt?"
 msgstr ""
 
 #: lino_welfare/modlib/reception/models.py:286
-#: lino_welfare/modlib/reception/models.py:370
+#: lino_welfare/modlib/reception/models.py:371
 msgid "Create appointment with"
 msgstr "Termin machen mit"
 
 #: lino_welfare/modlib/reception/models.py:315
 msgid "Agent"
 msgstr "Sozi"
 
 #: lino_welfare/modlib/reception/models.py:319
 msgid "Coaching type"
 msgstr "Dienst"
 
 #: lino_welfare/modlib/reception/models.py:343
 #: lino_welfare/modlib/reception/models.py:347
-#: lino_welfare/modlib/reception/models.py:389
+#: lino_welfare/modlib/reception/models.py:390
 msgid "Visit"
 msgstr "Visite"
 
-#: lino_welfare/modlib/reception/models.py:359
 #: lino_welfare/modlib/reception/models.py:360
-#: lino_welfare/modlib/reception/models.py:396
+#: lino_welfare/modlib/reception/models.py:361
 #: lino_welfare/modlib/reception/models.py:397
+#: lino_welfare/modlib/reception/models.py:398
 msgid "Find date"
 msgstr "Termin finden"
 
 #: lino_welfare/modlib/sepa/models.py:21
 msgid "Giro"
 msgstr ""
 
@@ -3714,18 +3674,16 @@
 #: lino_welfare/modlib/welfare/help_texts.py:7
 msgid "The plugin."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:8
 msgid ""
 "Optionally specify the primary key (an integer) of the last granting for\n"
-"which you want to deactivate date range validation in confirmations.  "
-"This\n"
-"is useful for keeping legacy confirmations that have been issued before "
-"the\n"
+"which you want to deactivate date range validation in confirmations.  This\n"
+"is useful for keeping legacy confirmations that have been issued before the\n"
 "rule was activated."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:12
 #: lino_welfare/modlib/welfare/help_texts.py:15
 #: lino_welfare/modlib/welfare/help_texts.py:76
 #: lino_welfare/modlib/welfare/help_texts.py:84
@@ -3863,16 +3821,15 @@
 "requests."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:60
 msgid ""
 "Validates the generated XML against the XSD files.\n"
 "Used by test suite.\n"
-"It is not necessary to validate each real request before actually sending"
-" it."
+"It is not necessary to validate each real request before actually sending it."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:63
 msgid "SSDN specific part of a request."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:64
@@ -4165,507 +4122,518 @@
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:168
 msgid "A request to the RetrieveTIGroups service (aka Tx25)"
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:169
-msgid ""
-"An account is an item of an account chart used to collect\n"
-"ledger transactions or other accountable items."
-msgstr ""
+#, fuzzy
+msgid "Whether to print empty rows."
+msgstr "Auch leere Einträge drucken"
+
+#: lino_welfare/modlib/welfare/help_texts.py:170
+#, fuzzy
+msgid "Whether to ignore yearly incomes."
+msgstr "Jährliche Einkommen berücksichtigen"
 
 #: lino_welfare/modlib/welfare/help_texts.py:171
 msgid ""
-"The multilingual designation of this account, as the users see\n"
-"it."
+"Yield the entry groups for this budget, i.e. one item for each\n"
+"account group for which this budget has some data."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:173
-msgid ""
-"The account group to which this account belongs.  This must\n"
-"point to an instance of Group."
+msgid "The database model used to represent a budget actor."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:175
-msgid "The sequence number of this account within its group."
+#: lino_welfare/modlib/welfare/help_texts.py:174
+msgid "A detail row of a Budget."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:176
+#: lino_welfare/modlib/welfare/help_texts.py:175
 msgid ""
-"An optional unique name which can be used to reference a given\n"
-"account."
+"Optionally specify a budget actor who contributes this entry.\n"
+"Leave empty when the entry refers to the entire household."
 msgstr ""
+"Hier optional den Akteur angeben, der diesen Eintrag beiträgt. \n"
+"Leer lassen, wenn der Eintrag sich auf den Gesamthaushalt bezieht."
 
-#: lino_welfare/modlib/welfare/help_texts.py:178
+#: lino_welfare/modlib/welfare/help_texts.py:177
 msgid ""
-"The account type of this account.  This must\n"
-"point to an item of\n"
-"lino_welfare.modlib.debts.AccountTypes."
+"The amount of money. An empty amount is different from a zero\n"
+"amount in that the latter will be printed while the former\n"
+"not."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:181
-msgid "Django model used to represent a debts mediation budget."
+#: lino_welfare/modlib/welfare/help_texts.py:180
+msgid "The related Account."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:182
+#: lino_welfare/modlib/welfare/help_texts.py:181
 msgid ""
-"Yield the entry groups for this budget, i.e. one item for each\n"
-"account group for which this budget has some data."
+"An account is an item of an account chart used to collect\n"
+"ledger transactions or other accountable items."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:184
+#: lino_welfare/modlib/welfare/help_texts.py:183
 msgid ""
-"An actor of a budget is a partner who is part of the household\n"
-"for which the budget has been established."
+"The multilingual designation of this account, as the users see\n"
+"it."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:186
-msgid "A detail row of a Budget."
+#: lino_welfare/modlib/welfare/help_texts.py:185
+msgid ""
+"The account group to which this account belongs.  This must\n"
+"point to an instance of Group."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:187
+msgid "The sequence number of this account within its group."
+msgstr ""
+
+#: lino_welfare/modlib/welfare/help_texts.py:188
 msgid ""
-"The amount of money. An empty amount is different from a zero\n"
-"amount in that the latter will be printed while the former\n"
-"not."
+"An optional unique name which can be used to reference a given\n"
+"account."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:190
-msgid "The related Account."
+msgid ""
+"The account type of this account.  This must\n"
+"point to an item of\n"
+"lino_welfare.modlib.debts.AccountTypes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:191
+#: lino_welfare/modlib/welfare/help_texts.py:193
 msgid "The Django model that represents a client summary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:192
+#: lino_welfare/modlib/welfare/help_texts.py:194
 msgid "Base class for all tables on ClientSummary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:193
+#: lino_welfare/modlib/welfare/help_texts.py:195
 msgid "Lists all ESF summaries for all clients."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:194
+#: lino_welfare/modlib/welfare/help_texts.py:196
 msgid "Lists the ESF summaries for a given client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:195
+#: lino_welfare/modlib/welfare/help_texts.py:197
 msgid "Base class for all statistical fields."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:196
+#: lino_welfare/modlib/welfare/help_texts.py:198
 msgid "Used as the verbose_name of field."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:197
+#: lino_welfare/modlib/welfare/help_texts.py:199
 msgid "The internal field name."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:198
+#: lino_welfare/modlib/welfare/help_texts.py:200
 msgid "The field descriptor (an instance of a Django Field)"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:199
+#: lino_welfare/modlib/welfare/help_texts.py:201
 msgid "Count the number of presences."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:200
+#: lino_welfare/modlib/welfare/help_texts.py:202
 msgid "Count the real hours of presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:201
+#: lino_welfare/modlib/welfare/help_texts.py:203
 msgid "Count the event’s duration for each presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:202
+#: lino_welfare/modlib/welfare/help_texts.py:204
 msgid "Count a fixed time for each presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:203
+#: lino_welfare/modlib/welfare/help_texts.py:205
 msgid ""
-"Shows the members of the primary household of this person together with "
-"an\n"
+"Shows the members of the primary household of this person together with an\n"
 "amount which depends on whether that member is adult or not."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:205
+#: lino_welfare/modlib/welfare/help_texts.py:207
 msgid ""
 "The amount to refund for children (household members less than\n"
 "lino_xl.lib.households.Plugin.adult_age years old)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:207
+#: lino_welfare/modlib/welfare/help_texts.py:209
 msgid ""
 "The amount to refund for children (household members who are\n"
 "lino_xl.lib.households.Plugin.adult_age years or older)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:209
+#: lino_welfare/modlib/welfare/help_texts.py:211
 msgid "The full name of the household member."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:210
+#: lino_welfare/modlib/welfare/help_texts.py:212
 msgid ""
 "The amount to pay. This is either child_tariff or\n"
 "adult_tarif depending on the age of the household member."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:212
+#: lino_welfare/modlib/welfare/help_texts.py:214
 msgid "Model mixin for all integration contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:213
+#: lino_welfare/modlib/welfare/help_texts.py:215
 msgid "The person who created this contract."
 msgstr "Die Person, die diesen Vertrag erstellt hat."
 
-#: lino_welfare/modlib/welfare/help_texts.py:214
+#: lino_welfare/modlib/welfare/help_texts.py:216
 msgid "The responsible person at the general social service."
 msgstr "Die verantwortliche Person im allgemeinen Sozialdienst."
 
-#: lino_welfare/modlib/welfare/help_texts.py:215
+#: lino_welfare/modlib/welfare/help_texts.py:217
 msgid "The client for whom this contract is done."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:216
+#: lino_welfare/modlib/welfare/help_texts.py:218
 msgid "The start date of the contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:217
+#: lino_welfare/modlib/welfare/help_texts.py:219
 msgid "The planned end date of this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:218
+#: lino_welfare/modlib/welfare/help_texts.py:220
 msgid ""
 "The date when this contract was effectively ended.\n"
 "This field is set to the same value as applies_until."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:220
+#: lino_welfare/modlib/welfare/help_texts.py:222
 msgid ""
 "The reason of prematured ending.  Pointer to\n"
 "ContractEnding"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:222
+#: lino_welfare/modlib/welfare/help_texts.py:224
 msgid "When the contract was issued to the client and signed by them."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:223
+#: lino_welfare/modlib/welfare/help_texts.py:225
 msgid "When the contract was ratified by the responsible board."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:224
+#: lino_welfare/modlib/welfare/help_texts.py:226
 msgid ""
 "The language of this contract. Default value is the client’s\n"
 "language."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:226
+#: lino_welfare/modlib/welfare/help_texts.py:228
 msgid ""
 "The type of this contract. Pointer to a subclass of\n"
 "ContractTypeBase."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:228
+#: lino_welfare/modlib/welfare/help_texts.py:230
 msgid ""
 "The printed title of a contract specifies just the contract type\n"
 "(not the number and name of client)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:230
+#: lino_welfare/modlib/welfare/help_texts.py:232
 msgid ""
 "Overrides\n"
 "lino_xl.lib.excerpts.Certifiable.get_excerpt_templates()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:232
+#: lino_welfare/modlib/welfare/help_texts.py:234
 msgid ""
 "If the contract’s author is the client’s primary coach, then set\n"
 "user_asd to None, otherwise set user_asd to the primary coach.\n"
 "We no longer suppose that only integration agents write\n"
 "contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:236
+#: lino_welfare/modlib/welfare/help_texts.py:238
 msgid "Checks for the following error conditions:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:237
+#: lino_welfare/modlib/welfare/help_texts.py:239
 msgid ""
 "Returns the last aid confirmation that has been issued for this\n"
 "contract. May be used in .odt template."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:239
+#: lino_welfare/modlib/welfare/help_texts.py:241
 msgid ""
 "Automatic evaluation events have the client as mandatory\n"
 "participant, plus possibly some other coach."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:241
+#: lino_welfare/modlib/welfare/help_texts.py:243
 msgid ""
 "All contracts of a demo project (not only one) are being printed.\n"
 "Overrides\n"
 "lino.modlib.printing.Printable.get_printable_demo_objects()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:244
+#: lino_welfare/modlib/welfare/help_texts.py:246
 msgid ""
 "Model mixin for integration contracts\n"
 "that have a single partner."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:246
+#: lino_welfare/modlib/welfare/help_texts.py:248
 msgid "Base for contract tables. Defines the following parameter fields:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:247
+#: lino_welfare/modlib/welfare/help_texts.py:249
 #, fuzzy
 msgid "See ContractEvents."
 msgstr "erlaubt in Verträgen"
 
-#: lino_welfare/modlib/welfare/help_texts.py:248
+#: lino_welfare/modlib/welfare/help_texts.py:250
 msgid ""
 "Show only contracts with the specified\n"
 "ContractEnding."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:250
+#: lino_welfare/modlib/welfare/help_texts.py:252
 msgid ""
 "Select “Yes” to show only contracts whose ending\n"
 "ContractEnding has\n"
 "is_success\n"
 "checked."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:254
+#: lino_welfare/modlib/welfare/help_texts.py:256
 msgid "The Django model representing an ISIP."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:255
+#: lino_welfare/modlib/welfare/help_texts.py:257
 msgid ""
 "The type of this contract.\n"
 "Pointer to ContractType."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:257
+#: lino_welfare/modlib/welfare/help_texts.py:259
 msgid ""
 "The type of study that is going to be followed during this\n"
 "contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:259
+#: lino_welfare/modlib/welfare/help_texts.py:261
 msgid "The table of all ISIP contract types."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:260
+#: lino_welfare/modlib/welfare/help_texts.py:262
 msgid "The type of a Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:261
+#: lino_welfare/modlib/welfare/help_texts.py:263
 msgid ""
 "Whether contracts of this type need their study_type\n"
 "field filled in."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:263
+#: lino_welfare/modlib/welfare/help_texts.py:265
 msgid "Django model to represent an examination policy."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:264
+#: lino_welfare/modlib/welfare/help_texts.py:266
 msgid "A possible reason for premature termination of a contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:265
+#: lino_welfare/modlib/welfare/help_texts.py:267
 msgid ""
 "Represents a third-party external partner who participates in this\n"
 "contract. For every partner there is a rich text field describing\n"
 "their duties."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:268
+#: lino_welfare/modlib/welfare/help_texts.py:270
 msgid ""
 "A list of observable events for filtering contracts\n"
 "(ContractBaseTable.observed_event)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:270
+#: lino_welfare/modlib/welfare/help_texts.py:272
 msgid ""
 "Whether the client has at least one ISIP contact during the\n"
 "observed date range."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:272
+#: lino_welfare/modlib/welfare/help_texts.py:274
 msgid ""
 "To see this table you need either IntegrationAgent or\n"
 "SocialCoordinator."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:274
+#: lino_welfare/modlib/welfare/help_texts.py:276
 msgid "Base class for all ContractType models."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:275
+#: lino_welfare/modlib/welfare/help_texts.py:277
 msgid ""
 "The full description of this contract type as used in printed\n"
 "documents."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:277
+#: lino_welfare/modlib/welfare/help_texts.py:279
 msgid ""
 "The default examination policy to be used for contracts of\n"
 "this type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:279
+#: lino_welfare/modlib/welfare/help_texts.py:281
 msgid ""
 "The overlap group to use when checking whether two contracts are\n"
 "overlapping or not. If this field is empty, Lino does not check at all\n"
 "for overlapping contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:282
+#: lino_welfare/modlib/welfare/help_texts.py:284
 msgid ""
 "The main template to use instead of the default template\n"
 "defined on the excerpt type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:284
+#: lino_welfare/modlib/welfare/help_texts.py:286
 msgid ""
 "The list of all known overlap groups to be selected for the\n"
 "overlap_group\n"
 "of a contract type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:287
+#: lino_welfare/modlib/welfare/help_texts.py:289
 msgid ""
 "Volatile object used to test for overlapping contracts.  It is\n"
 "responsible for issuing the following error messages:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:289
+#: lino_welfare/modlib/welfare/help_texts.py:291
 msgid "A given client cannot have two active contracts at the same time."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:290
+#: lino_welfare/modlib/welfare/help_texts.py:292
 msgid ""
 "Organisation bénéficiant de l’agrément « Initiative d’économie sociale »\n"
 "octroyé par la Wallonie."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:292
+#: lino_welfare/modlib/welfare/help_texts.py:294
 #, fuzzy
 msgid "Shows all Art60 job supplyments."
 msgstr "Art.60§7-Konvention"
 
-#: lino_welfare/modlib/welfare/help_texts.py:293
+#: lino_welfare/modlib/welfare/help_texts.py:295
 #, fuzzy
 msgid "Shows the Art60 job supplyments for this client."
 msgstr "Art.61-Konventionsart"
 
-#: lino_welfare/modlib/welfare/help_texts.py:294
+#: lino_welfare/modlib/welfare/help_texts.py:296
 msgid ""
 "Model mixin for jobs.Contract\n"
 "and art61.Contract. And also\n"
 "for art60.Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:297
+#: lino_welfare/modlib/welfare/help_texts.py:299
 msgid "The duration of this job supplyment (number of working days)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:298
+#: lino_welfare/modlib/welfare/help_texts.py:300
 msgid "Django model used to represent a beneficiary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:299
+#: lino_welfare/modlib/welfare/help_texts.py:301
 msgid "Whether Lino should make ESF summaries for this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:300
+#: lino_welfare/modlib/welfare/help_texts.py:302
 msgid "A panel with general information about this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:301
+#: lino_welfare/modlib/welfare/help_texts.py:303
 msgid ""
 "A virtual field displaying a group of shortcut links for managing CVs\n"
 "(Curriculum Vitaes)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:303
+#: lino_welfare/modlib/welfare/help_texts.py:305
 msgid ""
 "A virtual field displaying a group of buttons for managing the\n"
 "“identifying document”, i.e. an uploaded document which has been\n"
 "used as alternative to the eID card."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:306
+#: lino_welfare/modlib/welfare/help_texts.py:308
 msgid ""
 "Pointer to PersonGroup.\n"
 "The intergration phase of this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:308
+#: lino_welfare/modlib/welfare/help_texts.py:310
 msgid ""
 "The civil state of this client. Allowed choices are defined in\n"
 "CivilState."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:310
+#: lino_welfare/modlib/welfare/help_texts.py:312
 #, fuzzy
 msgid "Pointer to ClientStates."
 msgstr "DSBE-Klienten"
 
-#: lino_welfare/modlib/welfare/help_texts.py:311
+#: lino_welfare/modlib/welfare/help_texts.py:313
 msgid ""
 "The date when this client got unemployed and stopped to have a\n"
 "regular work."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:313
+#: lino_welfare/modlib/welfare/help_texts.py:315
 msgid ""
 "The date when this client registered as unemployed and started\n"
 "to look for a new job."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:315
+#: lino_welfare/modlib/welfare/help_texts.py:317
 msgid ""
 "Return the last note of type “First meeting” for this client.\n"
 "Usage example see debts and\n"
 "notes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:318
+#: lino_welfare/modlib/welfare/help_texts.py:320
 #, fuzzy
 msgid "The list that opens by Contacts ‣ Clients."
 msgstr "Liste der Klientenkontakte"
 
-#: lino_welfare/modlib/welfare/help_texts.py:319
+#: lino_welfare/modlib/welfare/help_texts.py:321
 msgid ""
 "If not empty, show only Clients whose client_state equals\n"
 "the specified value."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:321
+#: lino_welfare/modlib/welfare/help_texts.py:323
 msgid ""
 "Displays the response of an RetrieveTIGroupsRequest\n"
 "as a table."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:323
+#: lino_welfare/modlib/welfare/help_texts.py:325
 msgid "The Django database model."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:324
+#: lino_welfare/modlib/welfare/help_texts.py:326
 msgid "Yield a list of all subsidizations activated for this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:325
+#: lino_welfare/modlib/welfare/help_texts.py:327
 #, fuzzy
 msgid "Shows the Art61 job supplyments for this client."
 msgstr "Art.61-Konventionsart"
 
 #: lino_welfare/modlib/welfare/models.py:34
 msgid "Local job office"
 msgstr "Lokales Arbeitsamt"
@@ -4684,16 +4652,15 @@
 
 #: lino_welfare/modlib/welfare/models.py:71
 msgid "usable in contracts"
 msgstr "erlaubt in Verträgen"
 
 #: lino_welfare/modlib/welfare/models.py:73
 msgid ""
-"Whether Links of this type can be used as contact person of a job "
-"contract."
+"Whether Links of this type can be used as contact person of a job contract."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/user_types.py:173
 msgid "Anonymous"
 msgstr "Anonym"
 
 #: lino_welfare/modlib/welfare/user_types.py:175
@@ -5121,7 +5088,18 @@
 
 #~ msgid "SINE"
 #~ msgstr "Seit"
 
 #~ msgid "responsible (IS)"
 #~ msgstr "Verantwortlicher (DSBE)"
 
+#~ msgid "(SiteConfig %s is empty)"
+#~ msgstr "(Site-Parameter %s ist leer)"
+
+#~ msgid "Skills Property Group"
+#~ msgstr "Eigenschaftsgruppe Fähigkeiten"
+
+#~ msgid "Soft Skills Property Group"
+#~ msgstr "Eigenschaftsgruppe Sozialkompetenzen"
+
+#~ msgid "Obstacles Property Group"
+#~ msgstr "Eigenschaftsgruppe Hindernisse"
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 # Copyright (C) 2016 ORGANIZATION
 # This file is distributed under the same license as the lino-welfare
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2016.
 #
 msgid ""
 msgstr ""
-"Project-Id-Version: lino_welfare\n"
+"Project-Id-Version:  lino_welfare\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-11-22 10:25+0100\n"
+"POT-Creation-Date: 2023-04-01 18:26+0200\n"
 "PO-Revision-Date: 2022-11-22 10:25+0100\n"
 "Last-Translator: Luc Saffre <luc.saffre@gmail.com>\n"
-"Language-Team: fr <info@lino-framework.org>\n"
 "Language: fr\n"
+"Language-Team: fr <info@lino-framework.org>\n"
+"Plural-Forms: nplurals=2; plural=n>1;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=n>1;\n"
-"Generated-By: Babel 2.10.3\n"
-"X-Generator: Poedit 3.0.1\n"
+"Generated-By: Babel 2.12.1\n"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:19
 msgid "Active Job Search"
 msgstr "Recherche active d'emploi"
 
 #: lino_welfare/modlib/active_job_search/__init__.py:20
 msgid "AJS"
@@ -33,21 +32,21 @@
 msgstr "Preuve de recherche"
 
 #: lino_welfare/modlib/active_job_search/models.py:24
 msgid "Proofs of search"
 msgstr "Preuves de recherche"
 
 #: lino_welfare/modlib/active_job_search/models.py:28
-#: lino_welfare/modlib/badges/models.py:45 lino_welfare/modlib/cal/models.py:357
-#: lino_welfare/modlib/cbss/tx25.py:316 lino_welfare/modlib/cbss/tx25.py:363
-#: lino_welfare/modlib/cbss/tx25.py:372 lino_welfare/modlib/cbss/tx25.py:384
-#: lino_welfare/modlib/cbss/tx25.py:475 lino_welfare/modlib/cbss/tx25.py:487
-#: lino_welfare/modlib/debts/models.py:108 lino_welfare/modlib/isip/models.py:363
-#: lino_welfare/modlib/jobs/ui.py:427 lino_welfare/modlib/jobs/ui.py:548
-#: lino_welfare/modlib/pcsw/models.py:1002
+#: lino_welfare/modlib/badges/models.py:45
+#: lino_welfare/modlib/cal/models.py:357 lino_welfare/modlib/cbss/tx25.py:316
+#: lino_welfare/modlib/cbss/tx25.py:363 lino_welfare/modlib/cbss/tx25.py:372
+#: lino_welfare/modlib/cbss/tx25.py:384 lino_welfare/modlib/cbss/tx25.py:475
+#: lino_welfare/modlib/cbss/tx25.py:487 lino_welfare/modlib/debts/models.py:108
+#: lino_welfare/modlib/isip/models.py:365 lino_welfare/modlib/jobs/ui.py:427
+#: lino_welfare/modlib/jobs/ui.py:548 lino_welfare/modlib/pcsw/models.py:1004
 msgid "Date"
 msgstr ""
 
 #: lino_welfare/modlib/active_job_search/models.py:30
 msgid "Spontaneous"
 msgstr "Spontanée"
 
@@ -73,15 +72,16 @@
 msgstr "Garde d'enfant"
 
 #: lino_welfare/modlib/active_job_search/models.py:75
 msgid "Notes concerning child custody."
 msgstr ""
 
 #: lino_welfare/modlib/aids/__init__.py:14
-#: lino_welfare/modlib/ledger/models.py:54 lino_welfare/modlib/pcsw/models.py:506
+#: lino_welfare/modlib/ledger/models.py:54
+#: lino_welfare/modlib/pcsw/models.py:508
 msgid "Aids"
 msgstr "Aides"
 
 #: lino_welfare/modlib/aids/choicelists.py:50
 msgid "Aid confirmation type"
 msgstr "Type de confirmation d'aide"
 
@@ -144,49 +144,57 @@
 msgstr "Révoquer"
 
 #: lino_welfare/modlib/aids/mixins.py:97
 #, python-format
 msgid "You revoke your confirmation that %(client)s %(text)s"
 msgstr "Vous annullez votre confirmation que %(client)s %(text)s"
 
-#: lino_welfare/modlib/aids/mixins.py:111 lino_welfare/modlib/aids/mixins.py:137
+#: lino_welfare/modlib/aids/mixins.py:111
+#: lino_welfare/modlib/aids/mixins.py:137
 msgctxt "aids"
 msgid "Signer"
 msgstr "Signataire"
 
 #: lino_welfare/modlib/aids/mixins.py:181
 #, python-format
 msgid "receives %(what)s %(when)s."
 msgstr "béneficie d'une aide %(what)s %(when)s."
 
-#: lino_welfare/modlib/aids/mixins.py:213 lino_welfare/modlib/badges/models.py:50
-#: lino_welfare/modlib/cv/models.py:45 lino_welfare/modlib/debts/models.py:397
+#: lino_welfare/modlib/aids/mixins.py:213
+#: lino_welfare/modlib/badges/models.py:50 lino_welfare/modlib/cv/models.py:46
+#: lino_welfare/modlib/debts/models.py:397
 #: lino_welfare/modlib/debts/models.py:437 lino_welfare/modlib/esf/models.py:37
 #: lino_welfare/modlib/immersion/models.py:100
 #: lino_welfare/modlib/jobs/mixins.py:44 lino_welfare/modlib/jobs/models.py:236
-#: lino_welfare/modlib/jobs/models.py:266 lino_welfare/modlib/jobs/models.py:336
-#: lino_welfare/modlib/jobs/models.py:406 lino_welfare/modlib/pcsw/actions.py:40
-#: lino_welfare/modlib/pcsw/models.py:906 lino_welfare/modlib/pcsw/models.py:967
+#: lino_welfare/modlib/jobs/models.py:266
+#: lino_welfare/modlib/jobs/models.py:336
+#: lino_welfare/modlib/jobs/models.py:406
+#: lino_welfare/modlib/pcsw/actions.py:40
+#: lino_welfare/modlib/pcsw/models.py:908
+#: lino_welfare/modlib/pcsw/models.py:969
 #: lino_welfare/modlib/projects/models.py:44
 #: lino_welfare/modlib/xcourses/models.py:186
 #: lino_welfare/modlib/xcourses/models.py:363
 msgid "Remark"
 msgstr "Remarque"
 
 #: lino_welfare/modlib/aids/mixins.py:245
 #, python-format
 msgid "Date range %(p1)s lies outside of granted period %(p2)s."
 msgstr "Période %(p1)s hors de la période d'ocroi %(p2)s."
 
-#: lino_welfare/modlib/aids/mixins.py:317 lino_welfare/modlib/cbss/models.py:284
+#: lino_welfare/modlib/aids/mixins.py:317
+#: lino_welfare/modlib/cbss/models.py:279
 msgid "Period from"
 msgstr "Période du"
 
-#: lino_welfare/modlib/aids/mixins.py:319 lino_welfare/modlib/aids/models.py:210
-#: lino_welfare/modlib/pcsw/models.py:912 lino_welfare/modlib/pcsw/models.py:966
+#: lino_welfare/modlib/aids/mixins.py:319
+#: lino_welfare/modlib/aids/models.py:210
+#: lino_welfare/modlib/pcsw/models.py:914
+#: lino_welfare/modlib/pcsw/models.py:968
 msgid "until"
 msgstr "jusque"
 
 #: lino_welfare/modlib/aids/mixins.py:322
 msgid "Recipient (Organization)"
 msgstr "Destinataire (Organisation)"
 
@@ -226,16 +234,16 @@
 #: lino_welfare/modlib/aids/models.py:72
 #, fuzzy
 msgid "Integration duty"
 msgstr "Intégration"
 
 #: lino_welfare/modlib/aids/models.py:73
 msgid ""
-"Whether aid grantings of this type are considered as duty for integration "
-"contract."
+"Whether aid grantings of this type are considered as duty for integration"
+" contract."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:77
 #, fuzzy
 msgid "Urgent"
 msgstr "Budget"
 
@@ -245,22 +253,22 @@
 
 #: lino_welfare/modlib/aids/models.py:82
 msgid "Confirmed by primary coach"
 msgstr "Confirmé par le titulaire"
 
 #: lino_welfare/modlib/aids/models.py:83
 msgid ""
-"Whether grantings for this aid type are to be signed by the client's primary "
-"coach."
+"Whether grantings for this aid type are to be signed by the client's "
+"primary coach."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:90
 msgid ""
-"Which client address to print on confirmations. If this is empty, Lino will "
-"use the primary address."
+"Which client address to print on confirmations. If this is empty, Lino "
+"will use the primary address."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:95
 msgid "Body template"
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:149
@@ -273,32 +281,34 @@
 
 #: lino_welfare/modlib/aids/models.py:158
 msgid "Date of request"
 msgstr "Date de la demande"
 
 #: lino_welfare/modlib/aids/models.py:189
 #: lino_welfare/modlib/reception/models.py:323
-#: lino_welfare/modlib/reception/models.py:381
+#: lino_welfare/modlib/reception/models.py:382
 #, fuzzy
 msgid "Actions"
 msgstr "Occupations"
 
 #: lino_welfare/modlib/aids/models.py:200
 msgid "Create confirmation"
 msgstr "Créer attestation"
 
 #: lino_welfare/modlib/aids/models.py:207
 msgid "Applies from"
 msgstr "Date de début"
 
-#: lino_welfare/modlib/aids/models.py:238 lino_welfare/modlib/aids/models.py:360
+#: lino_welfare/modlib/aids/models.py:238
+#: lino_welfare/modlib/aids/models.py:360
 msgid "Only rows decided by this board."
 msgstr ""
 
-#: lino_welfare/modlib/aids/models.py:242 lino_welfare/modlib/aids/models.py:369
+#: lino_welfare/modlib/aids/models.py:242
+#: lino_welfare/modlib/aids/models.py:369
 msgid "Only confirmations about this aid type."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:299
 msgid "Grantings to confirm"
 msgstr "Octrois à confirmer"
 
@@ -361,15 +371,16 @@
 #: lino_welfare/modlib/aids/models.py:666
 #, fuzzy
 msgid "Can refund"
 msgstr "Fin de l'accompagnement"
 
 #: lino_welfare/modlib/aids/models.py:667
 msgid ""
-"Whether persons of this type can be used as doctor of a refund confirmation."
+"Whether persons of this type can be used as doctor of a refund "
+"confirmation."
 msgstr ""
 
 #: lino_welfare/modlib/aids/models.py:703
 #, fuzzy
 msgid "Refund confirmation"
 msgstr "Certificat de revenu"
 
@@ -448,24 +459,26 @@
 msgid "Art60 job supplying"
 msgstr "Mise à l'emploi art60"
 
 #: lino_welfare/modlib/art60/models.py:36
 msgid "Art60 job supplyment"
 msgstr "Mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/art60/models.py:50 lino_welfare/modlib/jobs/models.py:118
-#: lino_welfare/modlib/jobs/ui.py:38
+#: lino_welfare/modlib/art60/models.py:50
+#: lino_welfare/modlib/jobs/models.py:118 lino_welfare/modlib/jobs/ui.py:38
 msgid "Art60§7 job supplyment"
 msgstr "Mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/art60/models.py:51 lino_welfare/modlib/jobs/models.py:119
+#: lino_welfare/modlib/art60/models.py:51
+#: lino_welfare/modlib/jobs/models.py:119
 msgid "Art60§7 job supplyments"
 msgstr "Mises à l'emploi art60§7"
 
-#: lino_welfare/modlib/art60/models.py:58 lino_welfare/modlib/art61/models.py:77
+#: lino_welfare/modlib/art60/models.py:58
+#: lino_welfare/modlib/art61/models.py:77
 #: lino_welfare/modlib/jobs/models.py:132
 #, fuzzy
 msgid "Type"
 msgstr "Type d'aide sociale"
 
 #: lino_welfare/modlib/art60/models.py:98
 msgid "Art60§7 convention"
@@ -480,48 +493,53 @@
 msgstr "Date de début"
 
 #: lino_welfare/modlib/art60/models.py:114
 #: lino_welfare/modlib/art60/models.py:222
 msgid "Monthly refund"
 msgstr "Rétrocession mensuelle"
 
-#: lino_welfare/modlib/art60/models.py:115 lino_welfare/modlib/jobs/models.py:141
+#: lino_welfare/modlib/art60/models.py:115
+#: lino_welfare/modlib/jobs/models.py:141
 #: lino_welfare/modlib/jobs/models.py:264
 msgid "hourly rate"
 msgstr "coût horaire"
 
-#: lino_welfare/modlib/art60/models.py:116 lino_welfare/modlib/jobs/models.py:142
+#: lino_welfare/modlib/art60/models.py:116
+#: lino_welfare/modlib/jobs/models.py:142
 msgid "refund rate"
 msgstr "tarif de remboursement"
 
-#: lino_welfare/modlib/art60/models.py:167 lino_welfare/modlib/jobs/models.py:184
+#: lino_welfare/modlib/art60/models.py:167
+#: lino_welfare/modlib/jobs/models.py:184
 #, python-format
 msgid "(%d candidatures have been marked inactive)"
 msgstr ""
 
-#: lino_welfare/modlib/art60/models.py:168 lino_welfare/modlib/isip/models.py:116
-#: lino_welfare/modlib/jobs/models.py:185 lino_welfare/modlib/pcsw/actions.py:84
+#: lino_welfare/modlib/art60/models.py:168
+#: lino_welfare/modlib/isip/models.py:116
+#: lino_welfare/modlib/jobs/models.py:185
+#: lino_welfare/modlib/pcsw/actions.py:84
 #: lino_welfare/modlib/pcsw/actions.py:115
 msgid "Success"
 msgstr "Réussi"
 
-#: lino_welfare/modlib/art60/models.py:225 lino_welfare/modlib/jobs/ui.py:172
+#: lino_welfare/modlib/art60/models.py:225 lino_welfare/modlib/jobs/ui.py:171
 msgid "Only contracts of type"
 msgstr "Uniquement contrats de type"
 
-#: lino_welfare/modlib/art60/models.py:276
+#: lino_welfare/modlib/art60/models.py:277
 #: lino_welfare/modlib/isip/choicelists.py:24
 msgid "Conventions"
 msgstr "Conventions"
 
-#: lino_welfare/modlib/art60/models.py:322
+#: lino_welfare/modlib/art60/models.py:323
 msgid "My art60§7 contracts (IS)"
 msgstr "Mes contrats art60§7 (SI)"
 
-#: lino_welfare/modlib/art60/models.py:335
+#: lino_welfare/modlib/art60/models.py:336
 msgid "My art60§7 contracts (GSS)"
 msgstr "Mes contrats art60§7 (SSG)"
 
 #: lino_welfare/modlib/art61/__init__.py:14
 msgid "Art61 job supplying"
 msgstr "Mise à l'emploi art61"
 
@@ -549,15 +567,16 @@
 msgid "Tutorate"
 msgstr "Tutorat"
 
 #: lino_welfare/modlib/art61/choicelists.py:48
 msgid "Walloon Region"
 msgstr "Région Wallonne"
 
-#: lino_welfare/modlib/art61/models.py:30 lino_welfare/modlib/art61/models.py:66
+#: lino_welfare/modlib/art61/models.py:30
+#: lino_welfare/modlib/art61/models.py:66
 msgid "Art61 job supplyment"
 msgstr "Mise à l'emploi art.61"
 
 #: lino_welfare/modlib/art61/models.py:48
 msgid "Art61 job supplyment type"
 msgstr "Type de mise à l'emploi art.61"
 
@@ -598,15 +617,16 @@
 msgid "Badge Awards"
 msgstr "Tests de niveau"
 
 #: lino_welfare/modlib/badges/models.py:42
 msgid "Holder"
 msgstr ""
 
-#: lino_welfare/modlib/badges/models.py:47 lino_welfare/modlib/cbss/mixins.py:286
+#: lino_welfare/modlib/badges/models.py:47
+#: lino_welfare/modlib/cbss/mixins.py:286
 #: lino_welfare/modlib/projects/models.py:45
 msgid "Result"
 msgstr "Résultat"
 
 #: lino_welfare/modlib/badges/models.py:60
 #: lino_welfare/modlib/badges/models.py:68
 msgid "Awards"
@@ -675,16 +695,17 @@
 msgid "Notes"
 msgstr ""
 
 #: lino_welfare/modlib/cal/models.py:334
 #: lino_welfare/modlib/client_vouchers/ui.py:38
 #: lino_welfare/modlib/contacts/models.py:118
 #: lino_welfare/modlib/contacts/models.py:204
-#: lino_welfare/modlib/contacts/models.py:294 lino_welfare/modlib/debts/ui.py:125
-#: lino_welfare/modlib/finan/models.py:19 lino_welfare/modlib/isip/models.py:253
+#: lino_welfare/modlib/contacts/models.py:294
+#: lino_welfare/modlib/debts/ui.py:125 lino_welfare/modlib/finan/models.py:19
+#: lino_welfare/modlib/isip/models.py:253
 #: lino_welfare/modlib/system/models.py:106 lino_welfare/modlib/users/ui.py:23
 #: lino_welfare/modlib/welfare/workflows.py:48
 msgid "General"
 msgstr "Général"
 
 #: lino_welfare/modlib/cal/models.py:338 lino_welfare/modlib/finan/models.py:24
 msgid "More"
@@ -713,15 +734,16 @@
 msgid "Tasks"
 msgstr ""
 
 #: lino_welfare/modlib/cal/models.py:416
 msgid "Delegated to client"
 msgstr "à faire par bénéficiaire"
 
-#: lino_welfare/modlib/cbss/__init__.py:34 lino_welfare/modlib/pcsw/models.py:399
+#: lino_welfare/modlib/cbss/__init__.py:34
+#: lino_welfare/modlib/pcsw/models.py:401
 msgid "CBSS"
 msgstr "BCSS"
 
 #: lino_welfare/modlib/cbss/choicelists.py:20
 #: lino_welfare/modlib/cbss/mixins.py:85
 msgid "Sent"
 msgstr "Exécuté"
@@ -847,103 +869,104 @@
 msgid "First name"
 msgstr "Prénom"
 
 #: lino_welfare/modlib/cbss/mixins.py:684 lino_welfare/modlib/cbss/ui.py:185
 msgid "Last name"
 msgstr "Nom de famille"
 
-#: lino_welfare/modlib/cbss/models.py:40 lino_welfare/modlib/cbss/models.py:64
+#: lino_welfare/modlib/cbss/models.py:35 lino_welfare/modlib/cbss/models.py:59
 msgid "Sector"
 msgstr "Secteur"
 
-#: lino_welfare/modlib/cbss/models.py:41
+#: lino_welfare/modlib/cbss/models.py:36
 msgid "Sectors"
 msgstr "Secteurs"
 
-#: lino_welfare/modlib/cbss/models.py:45 lino_welfare/modlib/cbss/models.py:68
+#: lino_welfare/modlib/cbss/models.py:40 lino_welfare/modlib/cbss/models.py:63
 msgid "Code"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:46
+#: lino_welfare/modlib/cbss/models.py:41
 msgid "Subcode"
 msgstr "Sous-Code"
 
-#: lino_welfare/modlib/cbss/models.py:47
+#: lino_welfare/modlib/cbss/models.py:42
 msgid "Abbreviation"
 msgstr "Abbréviation"
 
-#: lino_welfare/modlib/cbss/models.py:61
+#: lino_welfare/modlib/cbss/models.py:56
 msgid "Purpose"
 msgstr "Code fonction"
 
-#: lino_welfare/modlib/cbss/models.py:62
+#: lino_welfare/modlib/cbss/models.py:57
 msgid "Purposes"
 msgstr "Codes fonction"
 
-#: lino_welfare/modlib/cbss/models.py:91
+#: lino_welfare/modlib/cbss/models.py:86
 msgid "IdentifyPerson Request"
 msgstr "Requête IdentifyPerson"
 
-#: lino_welfare/modlib/cbss/models.py:92
+#: lino_welfare/modlib/cbss/models.py:87
 msgid "IdentifyPerson Requests"
 msgstr "Requêtes IdentifyPerson"
 
-#: lino_welfare/modlib/cbss/models.py:96
+#: lino_welfare/modlib/cbss/models.py:91
 msgid "Middle name"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:101
+#: lino_welfare/modlib/cbss/models.py:96
 msgid "Tolerance"
 msgstr "Tolérance"
 
-#: lino_welfare/modlib/cbss/models.py:250
+#: lino_welfare/modlib/cbss/models.py:245
 msgid "ManageAccess Request"
 msgstr "Requête ManageAccess"
 
-#: lino_welfare/modlib/cbss/models.py:251
+#: lino_welfare/modlib/cbss/models.py:246
 msgid "ManageAccess Requests"
 msgstr "Requêtes ManageAccess"
 
-#: lino_welfare/modlib/cbss/models.py:287
+#: lino_welfare/modlib/cbss/models.py:282
 msgid "Period until"
 msgstr "Période au"
 
-#: lino_welfare/modlib/cbss/models.py:411
+#: lino_welfare/modlib/cbss/models.py:406
 msgid "Tx25 Request"
 msgstr "Requête Tx25"
 
-#: lino_welfare/modlib/cbss/models.py:412
+#: lino_welfare/modlib/cbss/models.py:407
 msgid "Tx25 Requests"
 msgstr "Requêtes Tx25"
 
-#: lino_welfare/modlib/cbss/models.py:420 lino_welfare/modlib/pcsw/models.py:513
+#: lino_welfare/modlib/cbss/models.py:415
+#: lino_welfare/modlib/pcsw/models.py:515
 msgid "History"
 msgstr "Historique"
 
-#: lino_welfare/modlib/cbss/models.py:563
+#: lino_welfare/modlib/cbss/models.py:558
 msgid "Requesting organisation"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:576
+#: lino_welfare/modlib/cbss/models.py:571
 msgid "SSDN User Id"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:582
+#: lino_welfare/modlib/cbss/models.py:577
 msgid "SSDN email address"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:589
+#: lino_welfare/modlib/cbss/models.py:584
 msgid "HTTP username"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:596
+#: lino_welfare/modlib/cbss/models.py:591
 msgid "HTTP password"
 msgstr ""
 
-#: lino_welfare/modlib/cbss/models.py:631
+#: lino_welfare/modlib/cbss/models.py:626
 msgid "CBSS summary"
 msgstr "Sommaire BCSS"
 
 #: lino_welfare/modlib/cbss/tx25.py:42
 msgid "until "
 msgstr "jusque "
 
@@ -1082,15 +1105,16 @@
 
 #: lino_welfare/modlib/cbss/tx25.py:709 lino_welfare/modlib/cbss/tx25.py:751
 msgid "SSIN "
 msgstr "NISS "
 
 #: lino_welfare/modlib/cbss/tx25.py:729
 #: lino_welfare/modlib/immersion/models.py:87
-#: lino_welfare/modlib/isip/models.py:149 lino_welfare/modlib/jobs/models.py:127
+#: lino_welfare/modlib/isip/models.py:149
+#: lino_welfare/modlib/jobs/models.py:127
 msgid "Organization"
 msgstr "Organisation"
 
 #: lino_welfare/modlib/cbss/tx25.py:810 lino_welfare/modlib/isip/models.py:56
 msgid "Reference"
 msgstr "Référence"
 
@@ -1332,16 +1356,17 @@
 msgid "Driving Licenses"
 msgstr "Permis de conduire"
 
 #: lino_welfare/modlib/cbss/tx25.py:1217
 msgid "Identity Cards"
 msgstr "Cartes d'identité"
 
-#: lino_welfare/modlib/cbss/tx25.py:1233 lino_welfare/modlib/pcsw/models.py:116
-#: lino_welfare/modlib/pcsw/models.py:905 lino_welfare/modlib/pcsw/models.py:961
+#: lino_welfare/modlib/cbss/tx25.py:1233 lino_welfare/modlib/pcsw/models.py:117
+#: lino_welfare/modlib/pcsw/models.py:907
+#: lino_welfare/modlib/pcsw/models.py:963
 #: lino_welfare/modlib/reception/models.py:108
 #: lino_welfare/modlib/reception/models.py:136
 msgid "Reason"
 msgstr "Raison"
 
 #: lino_welfare/modlib/cbss/tx25.py:1246
 msgid "Legal cohabitations"
@@ -1416,15 +1441,16 @@
 msgid "Birth location"
 msgstr "Lieu de naissance"
 
 #: lino_welfare/modlib/cbss/ui.py:205
 msgid "Civil state"
 msgstr "Etat civil"
 
-#: lino_welfare/modlib/cbss/ui.py:209 lino_welfare/modlib/xcourses/models.py:612
+#: lino_welfare/modlib/cbss/ui.py:209
+#: lino_welfare/modlib/xcourses/models.py:612
 msgid "Address"
 msgstr "Adresse"
 
 #: lino_welfare/modlib/cbss/ui.py:219 lino_welfare/modlib/cbss/ui.py:239
 msgid "Requested action"
 msgstr "Action demandée"
 
@@ -1474,21 +1500,21 @@
 #: lino_welfare/modlib/contacts/models.py:313
 msgid "Contact"
 msgstr "Contact"
 
 #: lino_welfare/modlib/contacts/models.py:149
 #: lino_welfare/modlib/contacts/models.py:237
 #: lino_welfare/modlib/contacts/models.py:328
-#: lino_welfare/modlib/pcsw/models.py:533
+#: lino_welfare/modlib/pcsw/models.py:535
 msgid "Miscellaneous"
 msgstr "Divers"
 
 #: lino_welfare/modlib/contacts/models.py:158
 #: lino_welfare/modlib/households/models.py:81
-#: lino_welfare/modlib/pcsw/models.py:449
+#: lino_welfare/modlib/pcsw/models.py:451
 msgid "Person"
 msgstr "Personne"
 
 #: lino_welfare/modlib/contacts/models.py:159
 msgid "Persons"
 msgstr "Personnes"
 
@@ -1510,51 +1536,37 @@
 msgstr "aussi données obsolètes"
 
 #: lino_welfare/modlib/contacts/models.py:276
 #, fuzzy
 msgid "VAT id"
 msgstr " chez "
 
-#: lino_welfare/modlib/cv/models.py:39
+#: lino_welfare/modlib/cv/models.py:23
+#, fuzzy
+msgid "Skills"
+msgstr "Autres atouts"
+
+#: lino_welfare/modlib/cv/models.py:24
+#, fuzzy
+msgid "Soft skills"
+msgstr "Autres atouts"
+
+#: lino_welfare/modlib/cv/models.py:25
+#, fuzzy
+msgid "Obstacles"
+msgstr "Autres freins"
+
+#: lino_welfare/modlib/cv/models.py:40
 msgid "Property"
 msgstr "Propriété"
 
-#: lino_welfare/modlib/cv/models.py:40
+#: lino_welfare/modlib/cv/models.py:41
 msgid "Properties"
 msgstr "Propriétés"
 
-#: lino_welfare/modlib/cv/models.py:101
-#, fuzzy, python-format
-msgid "(SiteConfig %s is empty)"
-msgstr "(les paramètres de site %s sont vides)"
-
-#: lino_welfare/modlib/cv/models.py:125
-msgid "Skills Property Group"
-msgstr "Groupe de propriétés 'Skills'"
-
-#: lino_welfare/modlib/cv/models.py:127
-msgid "The property group to be used as master for the SkillsByPerson table."
-msgstr ""
-
-#: lino_welfare/modlib/cv/models.py:136
-msgid "Soft Skills Property Group"
-msgstr "Groupe de propriétés 'Soft Skills'"
-
-#: lino_welfare/modlib/cv/models.py:138
-msgid "The property group to be used as master for the SoftSkillsByPerson table."
-msgstr ""
-
-#: lino_welfare/modlib/cv/models.py:147
-msgid "Obstacles Property Group"
-msgstr "Groupe de propriétés 'Freins'"
-
-#: lino_welfare/modlib/cv/models.py:149
-msgid "The property group to be used as master for the ObstaclesByPerson table."
-msgstr ""
-
 #: lino_welfare/modlib/debts/__init__.py:25
 msgid "Debts mediation"
 msgstr "Médiation de dettes"
 
 #: lino_welfare/modlib/debts/choicelists.py:23
 #, fuzzy
 msgid "Financial statement"
@@ -1685,15 +1697,16 @@
 msgid "Required for Households"
 msgstr "obligatoire pour ménages"
 
 #: lino_welfare/modlib/debts/models.py:78
 msgid "Required for Persons"
 msgstr "obligatoire pour personnes"
 
-#: lino_welfare/modlib/debts/models.py:79 lino_welfare/modlib/debts/models.py:449
+#: lino_welfare/modlib/debts/models.py:79
+#: lino_welfare/modlib/debts/models.py:449
 msgid "Periods"
 msgstr "Périodes"
 
 #: lino_welfare/modlib/debts/models.py:80
 msgid "Default amount"
 msgstr "Montant par défaut"
 
@@ -1841,16 +1854,16 @@
 #: lino_welfare/modlib/debts/models.py:462
 #: lino_welfare/modlib/debts/models.py:576 lino_welfare/modlib/debts/ui.py:473
 msgid "Debt collection agency"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:463
 msgid ""
-"Leave empty for simple debts, otherwise select         here the responsible "
-"bailiff or collection agency"
+"Leave empty for simple debts, otherwise select         here the "
+"responsible bailiff or collection agency"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:529
 msgid "Periods must be > 0"
 msgstr ""
 
 #: lino_welfare/modlib/debts/models.py:533
@@ -1970,15 +1983,16 @@
 msgstr "Répartition au marc-le-franc"
 
 #: lino_welfare/modlib/debts/ui.py:641
 msgid ""
 "Répartition au marc-le-franc.\n"
 "A table with one row per entry in Liabilities which has \"distribute\" "
 "checked,\n"
-"proportionally distributing the `Distributable amount` among the debtors.\n"
+"proportionally distributing the `Distributable amount` among the debtors."
+"\n"
 msgstr ""
 
 #: lino_welfare/modlib/debts/ui.py:679
 msgid "%"
 msgstr ""
 
 #: lino_welfare/modlib/debts/ui.py:683
@@ -2155,15 +2169,16 @@
 msgstr "Répartition au marc-le-franc"
 
 #: lino_welfare/modlib/finan/models.py:59
 #, fuzzy
 msgid "Internal reference"
 msgstr "référence circulaire ?"
 
-#: lino_welfare/modlib/finan/models.py:61 lino_welfare/modlib/finan/models.py:66
+#: lino_welfare/modlib/finan/models.py:61
+#: lino_welfare/modlib/finan/models.py:66
 #, fuzzy
 msgid "External reference"
 msgstr "référence circulaire ?"
 
 #: lino_welfare/modlib/households/models.py:133
 #, python-format
 msgid "%(count)d adult"
@@ -2207,25 +2222,26 @@
 msgstr "Objectif"
 
 #: lino_welfare/modlib/immersion/models.py:70
 msgid "Immersion training goals"
 msgstr "Objectifs"
 
 #: lino_welfare/modlib/immersion/models.py:97
-#: lino_welfare/modlib/isip/mixins.py:325
+#: lino_welfare/modlib/isip/mixins.py:326
 msgid "reference person"
 msgstr "persone de référence"
 
 #: lino_welfare/modlib/immersion/models.py:99
-#: lino_welfare/modlib/isip/mixins.py:327
+#: lino_welfare/modlib/isip/mixins.py:328
 msgid "responsibilities"
 msgstr "responsabilités"
 
 #: lino_welfare/modlib/immersion/models.py:117
-#: lino_welfare/modlib/isip/mixins.py:317 lino_welfare/modlib/isip/mixins.py:415
+#: lino_welfare/modlib/isip/mixins.py:318
+#: lino_welfare/modlib/isip/mixins.py:416
 #: lino_welfare/modlib/isip/models.py:214
 msgid "Responsible (IS)"
 msgstr "Titulaire (SI)"
 
 #: lino_welfare/modlib/immersion/ui.py:99
 msgid "Only immersion trainings of type"
 msgstr "Seulement stages d'immersion de ce type"
@@ -2263,15 +2279,15 @@
 msgid "Available"
 msgstr "Disponible"
 
 #: lino_welfare/modlib/integ/models.py:78
 msgid "Integration Clients"
 msgstr "Bénéficiares (SI)"
 
-#: lino_welfare/modlib/integ/models.py:95 lino_welfare/modlib/pcsw/models.py:81
+#: lino_welfare/modlib/integ/models.py:95 lino_welfare/modlib/pcsw/models.py:82
 msgid "Integration phase"
 msgstr "Phase d'insertion"
 
 #: lino_welfare/modlib/integ/models.py:97
 msgid "Language knowledge"
 msgstr "Connaissance de langue"
 
@@ -2367,15 +2383,16 @@
 msgstr ""
 
 #: lino_welfare/modlib/integ/models.py:599
 msgid "Activity Report"
 msgstr "Rapport d'activité"
 
 #: lino_welfare/modlib/integ/models.py:606
-#: lino_welfare/modlib/isip/__init__.py:14 lino_welfare/modlib/isip/models.py:183
+#: lino_welfare/modlib/isip/__init__.py:14
+#: lino_welfare/modlib/isip/models.py:183
 #: lino_welfare/modlib/isip/models.py:258
 msgid "ISIP"
 msgstr "PIIS"
 
 #: lino_welfare/modlib/integ/models.py:630
 msgid "Indicateurs généraux"
 msgstr ""
@@ -2459,80 +2476,80 @@
 msgid "Trainings"
 msgstr "Formations"
 
 #: lino_welfare/modlib/isip/mixins.py:51
 msgid "Full name"
 msgstr ""
 
-#: lino_welfare/modlib/isip/mixins.py:82
+#: lino_welfare/modlib/isip/mixins.py:83
 msgid "applies from"
 msgstr "Début de contrat"
 
-#: lino_welfare/modlib/isip/mixins.py:83
+#: lino_welfare/modlib/isip/mixins.py:84
 msgid "applies until"
 msgstr "Fin prévue"
 
-#: lino_welfare/modlib/isip/mixins.py:85
+#: lino_welfare/modlib/isip/mixins.py:86
 msgid "date decided"
 msgstr "Décidé le"
 
-#: lino_welfare/modlib/isip/mixins.py:87
+#: lino_welfare/modlib/isip/mixins.py:88
 msgid "date issued"
 msgstr "Date de signature"
 
-#: lino_welfare/modlib/isip/mixins.py:91 lino_welfare/modlib/isip/mixins.py:417
+#: lino_welfare/modlib/isip/mixins.py:92 lino_welfare/modlib/isip/mixins.py:418
 msgid "Responsible (GSS)"
 msgstr "Titulaire (SSG)"
 
-#: lino_welfare/modlib/isip/mixins.py:105
+#: lino_welfare/modlib/isip/mixins.py:106
 #: lino_welfare/modlib/xcourses/models.py:369
 msgid "date ended"
 msgstr "Date de fin"
 
-#: lino_welfare/modlib/isip/mixins.py:194
+#: lino_welfare/modlib/isip/mixins.py:195
 msgid "Contract ends before it started."
 msgstr "La date de fin est antérieure à la date de début"
 
-#: lino_welfare/modlib/isip/mixins.py:210
+#: lino_welfare/modlib/isip/mixins.py:211
 msgid "You must specify a contract type."
 msgstr ""
 
-#: lino_welfare/modlib/isip/mixins.py:242
+#: lino_welfare/modlib/isip/mixins.py:243
 #, python-format
 msgid "Evaluation %d"
 msgstr "Évaluation %d"
 
-#: lino_welfare/modlib/isip/mixins.py:253
+#: lino_welfare/modlib/isip/mixins.py:254
 msgid "Contract ends in a month"
 msgstr "Projet termine dans un mois"
 
-#: lino_welfare/modlib/isip/mixins.py:373
+#: lino_welfare/modlib/isip/mixins.py:374
 #, python-format
 msgid "Date range %(p1)s lies outside of coached period %(p2)s."
 msgstr "Période %(p1)s hors période d'intervention %(p2)s."
 
-#: lino_welfare/modlib/isip/mixins.py:379
+#: lino_welfare/modlib/isip/mixins.py:380
 #, fuzzy
 msgid "Date range overlaps with {ctype} #{id}."
 msgstr "Projet chevauche avec %(ctype)s #%(id)s"
 
-#: lino_welfare/modlib/isip/mixins.py:392
+#: lino_welfare/modlib/isip/mixins.py:393
 #, python-format
 msgid "%(ctype)s #%(id)s : %(msg)s"
 msgstr ""
 
-#: lino_welfare/modlib/isip/mixins.py:400
+#: lino_welfare/modlib/isip/mixins.py:401
 msgid "Check for overlapping contracts"
 msgstr ""
 
-#: lino_welfare/modlib/isip/mixins.py:420
+#: lino_welfare/modlib/isip/mixins.py:421
 msgid "Successfully ended"
 msgstr "Terminé avec succès"
 
-#: lino_welfare/modlib/isip/mixins.py:430
+#: lino_welfare/modlib/isip/mixins.py:431
 msgid "Only contracts with this company as partner."
 msgstr ""
 
 #: lino_welfare/modlib/isip/models.py:53
 msgid "ISIP Type"
 msgstr "Type de PIIS"
 
@@ -2561,16 +2578,18 @@
 msgid "Reason of termination"
 msgstr "Motif d'arrêt"
 
 #: lino_welfare/modlib/isip/models.py:111
 msgid "Contract termination reasons"
 msgstr "Motifs d’arrêt de contrat"
 
-#: lino_welfare/modlib/isip/models.py:113 lino_welfare/modlib/jobs/models.py:404
-#: lino_welfare/modlib/pcsw/models.py:825 lino_welfare/modlib/pcsw/models.py:1005
+#: lino_welfare/modlib/isip/models.py:113
+#: lino_welfare/modlib/jobs/models.py:404
+#: lino_welfare/modlib/pcsw/models.py:827
+#: lino_welfare/modlib/pcsw/models.py:1007
 msgid "Designation"
 msgstr "Désignation"
 
 #: lino_welfare/modlib/isip/models.py:118
 #, fuzzy
 msgid "Require date ended"
 msgstr "Date de fin"
@@ -2587,15 +2606,16 @@
 msgid "duties company"
 msgstr "Obligations de l'entreprise"
 
 #: lino_welfare/modlib/isip/models.py:184
 msgid "ISIPs"
 msgstr "PIISs"
 
-#: lino_welfare/modlib/isip/models.py:189 lino_welfare/modlib/jobs/models.py:263
+#: lino_welfare/modlib/isip/models.py:189
+#: lino_welfare/modlib/jobs/models.py:263
 msgid "Contract Type"
 msgstr "Type de contrat"
 
 #: lino_welfare/modlib/isip/models.py:194
 msgid "stages"
 msgstr "stages"
 
@@ -2617,19 +2637,19 @@
 
 #: lino_welfare/modlib/isip/models.py:209
 msgid "duties person"
 msgstr "Obligations du bénéficiaire"
 
 #: lino_welfare/modlib/isip/models.py:238
 msgid ""
-"Cannot print {} because there is no active aid confirmation and Duties (PCSW) "
-"is empty."
+"Cannot print {} because there is no active aid confirmation and Duties "
+"(PCSW) is empty."
 msgstr ""
 
-#: lino_welfare/modlib/isip/models.py:352
+#: lino_welfare/modlib/isip/models.py:354
 msgid "Proceedings"
 msgstr "Démarches"
 
 #: lino_welfare/modlib/jobs/__init__.py:18
 msgid "Job supplying"
 msgstr "Mise à l'emploi"
 
@@ -2713,15 +2733,16 @@
 msgid "Job Offer"
 msgstr "Offre d'emploi"
 
 #: lino_welfare/modlib/jobs/models.py:217
 msgid "Job Offers"
 msgstr "Offres d'emploi"
 
-#: lino_welfare/modlib/jobs/models.py:222 lino_welfare/modlib/jobs/models.py:258
+#: lino_welfare/modlib/jobs/models.py:222
+#: lino_welfare/modlib/jobs/models.py:258
 #: lino_welfare/modlib/xcourses/models.py:78
 #: lino_welfare/modlib/xcourses/models.py:108
 #: lino_welfare/modlib/xcourses/models.py:179
 msgid "Name"
 msgstr ""
 
 #: lino_welfare/modlib/jobs/models.py:227
@@ -2738,19 +2759,20 @@
 msgstr "Date de début"
 
 #: lino_welfare/modlib/jobs/models.py:254 lino_welfare/modlib/jobs/ui.py:434
 msgid "Job"
 msgstr "Poste de travail"
 
 #: lino_welfare/modlib/jobs/models.py:255 lino_welfare/modlib/jobs/ui.py:83
-#: lino_welfare/modlib/jobs/ui.py:102
+#: lino_welfare/modlib/jobs/ui.py:101
 msgid "Jobs"
 msgstr "Postes de travail"
 
-#: lino_welfare/modlib/jobs/models.py:259 lino_welfare/modlib/jobs/models.py:399
+#: lino_welfare/modlib/jobs/models.py:259
+#: lino_welfare/modlib/jobs/models.py:399
 msgid "Job Type"
 msgstr "Type de poste"
 
 #: lino_welfare/modlib/jobs/models.py:265
 msgid "capacity"
 msgstr "Capacité"
 
@@ -3007,15 +3029,15 @@
 msgstr ""
 
 #: lino_welfare/modlib/newcomers/models.py:124
 msgid "Competence"
 msgstr "Compétence"
 
 #: lino_welfare/modlib/newcomers/models.py:125
-#: lino_welfare/modlib/pcsw/models.py:550
+#: lino_welfare/modlib/pcsw/models.py:552
 msgid "Competences"
 msgstr "Compétences"
 
 #: lino_welfare/modlib/newcomers/models.py:143
 #, fuzzy
 msgid "User"
 msgstr "Refuser"
@@ -3129,15 +3151,15 @@
 
 #: lino_welfare/modlib/pcsw/actions.py:140
 #, python-format
 msgid "This will end %(count)d coachings of %(client)s."
 msgstr ""
 
 #: lino_welfare/modlib/pcsw/choicelists.py:15
-#: lino_welfare/modlib/pcsw/models.py:901
+#: lino_welfare/modlib/pcsw/models.py:903
 #, fuzzy
 msgid "Dispense"
 msgstr "Réponse"
 
 #: lino_welfare/modlib/pcsw/choicelists.py:27
 msgid "Penalty"
 msgstr ""
@@ -3162,298 +3184,298 @@
 msgid "Client did not return"
 msgstr "Client n'est plus revenu"
 
 #: lino_welfare/modlib/pcsw/models.py:73
 msgid "Clients"
 msgstr "Bénéficiaires"
 
-#: lino_welfare/modlib/pcsw/models.py:88
+#: lino_welfare/modlib/pcsw/models.py:89
 msgid "Lives in Belgium since"
 msgstr "en Belgique depuis"
 
-#: lino_welfare/modlib/pcsw/models.py:90
+#: lino_welfare/modlib/pcsw/models.py:91
 msgid "Residence until"
 msgstr "Inscription jusque"
 
-#: lino_welfare/modlib/pcsw/models.py:92
+#: lino_welfare/modlib/pcsw/models.py:93
 msgid "Unemployed since"
 msgstr "Inoccupé depuis"
 
-#: lino_welfare/modlib/pcsw/models.py:93
+#: lino_welfare/modlib/pcsw/models.py:94
 msgid "Since when the client has not been employed in any regular job."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:96
+#: lino_welfare/modlib/pcsw/models.py:97
 msgid "Seeking work since"
 msgstr "Cherche du travail depuis"
 
-#: lino_welfare/modlib/pcsw/models.py:97
+#: lino_welfare/modlib/pcsw/models.py:98
 msgid "Since when the client is seeking for a job."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:99
+#: lino_welfare/modlib/pcsw/models.py:100
 msgid "Needs residence permit"
 msgstr "besoin permis de séjour"
 
-#: lino_welfare/modlib/pcsw/models.py:101
+#: lino_welfare/modlib/pcsw/models.py:102
 msgid "Needs work permit"
 msgstr "besoin permis de travail"
 
-#: lino_welfare/modlib/pcsw/models.py:103
+#: lino_welfare/modlib/pcsw/models.py:104
 msgid "suspended until"
 msgstr "Suspendu jusque"
 
-#: lino_welfare/modlib/pcsw/models.py:107
+#: lino_welfare/modlib/pcsw/models.py:108
 msgid "Declared name"
 msgstr "Nom déclaré"
 
-#: lino_welfare/modlib/pcsw/models.py:109
+#: lino_welfare/modlib/pcsw/models.py:110
 msgid "is seeking work"
 msgstr "cherche du travail"
 
-#: lino_welfare/modlib/pcsw/models.py:113
+#: lino_welfare/modlib/pcsw/models.py:114
 msgid "Unavailable until"
 msgstr "Indisponible jusque"
 
-#: lino_welfare/modlib/pcsw/models.py:118
+#: lino_welfare/modlib/pcsw/models.py:119
 msgid "Other obstacles"
 msgstr "Autres freins"
 
-#: lino_welfare/modlib/pcsw/models.py:119
+#: lino_welfare/modlib/pcsw/models.py:120
 msgid "Other skills"
 msgstr "Autres atouts"
 
-#: lino_welfare/modlib/pcsw/models.py:124
+#: lino_welfare/modlib/pcsw/models.py:125
 msgid "Contact person at local job office"
 msgstr "Personne de contacte ALE ?"
 
-#: lino_welfare/modlib/pcsw/models.py:216
+#: lino_welfare/modlib/pcsw/models.py:217
 msgid "Circular reference"
 msgstr "référence circulaire ?"
 
-#: lino_welfare/modlib/pcsw/models.py:243
+#: lino_welfare/modlib/pcsw/models.py:244
 msgid "eID card expires in 2 months"
 msgstr "carte eID expire dans 2 mois"
 
-#: lino_welfare/modlib/pcsw/models.py:247
+#: lino_welfare/modlib/pcsw/models.py:248
 msgid "becomes available again in 1 month"
 msgstr "redevient disponible dans 1 mois"
 
-#: lino_welfare/modlib/pcsw/models.py:250
+#: lino_welfare/modlib/pcsw/models.py:251
 msgid "work permit suspension ends in 1 month"
 msgstr "fin de suspension du permis de travail dans 1 mois"
 
-#: lino_welfare/modlib/pcsw/models.py:330
+#: lino_welfare/modlib/pcsw/models.py:332
 msgid "Contract starts"
 msgstr "Contrat débute"
 
-#: lino_welfare/modlib/pcsw/models.py:336
+#: lino_welfare/modlib/pcsw/models.py:338
 msgid "Contract ends"
 msgstr "Contrat se termine"
 
-#: lino_welfare/modlib/pcsw/models.py:344
+#: lino_welfare/modlib/pcsw/models.py:346
 #, fuzzy
 msgid "Working at "
 msgstr "Travaille"
 
-#: lino_welfare/modlib/pcsw/models.py:351
+#: lino_welfare/modlib/pcsw/models.py:353
 msgid "Active contract"
 msgstr "Contrat actif"
 
-#: lino_welfare/modlib/pcsw/models.py:471
+#: lino_welfare/modlib/pcsw/models.py:473
 msgid "Human Links"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:476
+#: lino_welfare/modlib/pcsw/models.py:478
 msgid "Coaches"
 msgstr "Intervenants"
 
-#: lino_welfare/modlib/pcsw/models.py:499
+#: lino_welfare/modlib/pcsw/models.py:501
 msgid "Job search"
 msgstr "Recherche d'emploi"
 
-#: lino_welfare/modlib/pcsw/models.py:525
+#: lino_welfare/modlib/pcsw/models.py:527
 msgid "Calendar"
 msgstr "Calendrier"
 
-#: lino_welfare/modlib/pcsw/models.py:540
+#: lino_welfare/modlib/pcsw/models.py:542
 msgid "Career"
 msgstr "Parcours"
 
-#: lino_welfare/modlib/pcsw/models.py:545
+#: lino_welfare/modlib/pcsw/models.py:547
 msgid "Languages"
 msgstr "Langues"
 
-#: lino_welfare/modlib/pcsw/models.py:556
+#: lino_welfare/modlib/pcsw/models.py:558
 msgid "Contracts"
 msgstr "Contrats"
 
-#: lino_welfare/modlib/pcsw/models.py:589
+#: lino_welfare/modlib/pcsw/models.py:591
 msgid "Coached by"
 msgstr "Intervenant"
 
-#: lino_welfare/modlib/pcsw/models.py:593
+#: lino_welfare/modlib/pcsw/models.py:595
 msgid "and by"
 msgstr "et par"
 
-#: lino_welfare/modlib/pcsw/models.py:597
+#: lino_welfare/modlib/pcsw/models.py:599
 msgid "Nationality"
 msgstr "Nationalité"
 
-#: lino_welfare/modlib/pcsw/models.py:600
+#: lino_welfare/modlib/pcsw/models.py:602
 msgid "Extended filter criteria, e.g.:"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:602
+#: lino_welfare/modlib/pcsw/models.py:604
 msgid "Active: All those who have some active coaching."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:604
+#: lino_welfare/modlib/pcsw/models.py:606
 msgid "Only primary clients"
 msgstr "Dossiers titulaires seulement"
 
-#: lino_welfare/modlib/pcsw/models.py:743
+#: lino_welfare/modlib/pcsw/models.py:745
 msgid "and"
 msgstr "et"
 
-#: lino_welfare/modlib/pcsw/models.py:748
+#: lino_welfare/modlib/pcsw/models.py:750
 #, python-format
 msgid " on %(date)s"
 msgstr " le %(date)s"
 
-#: lino_welfare/modlib/pcsw/models.py:752
+#: lino_welfare/modlib/pcsw/models.py:754
 #, python-format
 msgid "Coached on %s"
 msgstr "Accompagné le %s"
 
-#: lino_welfare/modlib/pcsw/models.py:801
+#: lino_welfare/modlib/pcsw/models.py:803
 msgid "Check for valid identification"
 msgstr "Vérifier les données identifiantes"
 
-#: lino_welfare/modlib/pcsw/models.py:810
+#: lino_welfare/modlib/pcsw/models.py:812
 msgid "Neither valid eId data nor alternative identifying document."
 msgstr "Sans données eID ou document identifiant alternatif."
 
-#: lino_welfare/modlib/pcsw/models.py:826
+#: lino_welfare/modlib/pcsw/models.py:828
 msgid "Reference name"
 msgstr "Nom de référence"
 
-#: lino_welfare/modlib/pcsw/models.py:827
+#: lino_welfare/modlib/pcsw/models.py:829
 msgid "Considered active"
 msgstr "Considéré actif"
 
-#: lino_welfare/modlib/pcsw/models.py:832
+#: lino_welfare/modlib/pcsw/models.py:834
 msgid "Integration Phase"
 msgstr "Phase d'intégration"
 
-#: lino_welfare/modlib/pcsw/models.py:833
+#: lino_welfare/modlib/pcsw/models.py:835
 msgid "Integration Phases"
 msgstr "Phases d'intégration"
 
-#: lino_welfare/modlib/pcsw/models.py:840
+#: lino_welfare/modlib/pcsw/models.py:842
 msgid "Liste des phases d'intégration possibles."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:855
+#: lino_welfare/modlib/pcsw/models.py:857
 msgid "activity"
 msgstr "Activité"
 
-#: lino_welfare/modlib/pcsw/models.py:856
+#: lino_welfare/modlib/pcsw/models.py:858
 msgid "activities"
 msgstr "Activités"
 
-#: lino_welfare/modlib/pcsw/models.py:858
+#: lino_welfare/modlib/pcsw/models.py:860
 msgid "Appears in Listing 104"
 msgstr "Apparaît dans la liste 104"
 
-#: lino_welfare/modlib/pcsw/models.py:865
+#: lino_welfare/modlib/pcsw/models.py:867
 msgid "Liste des \"activités\" ou \"codes profession\"."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:880
+#: lino_welfare/modlib/pcsw/models.py:882
 msgid "Dispense reason"
 msgstr "Motif de dispense"
 
-#: lino_welfare/modlib/pcsw/models.py:881
+#: lino_welfare/modlib/pcsw/models.py:883
 msgid "Dispense reasons"
 msgstr "Motifs de dispense"
 
-#: lino_welfare/modlib/pcsw/models.py:890
+#: lino_welfare/modlib/pcsw/models.py:892
 msgid "A list of reasons for being dispensed"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:902
+#: lino_welfare/modlib/pcsw/models.py:904
 msgid "Dispenses"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:909
+#: lino_welfare/modlib/pcsw/models.py:911
 #, fuzzy
 msgid "Dispensed from"
 msgstr "Devoirs personne"
 
-#: lino_welfare/modlib/pcsw/models.py:917
+#: lino_welfare/modlib/pcsw/models.py:919
 msgid "Liste de dispenses"
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:935
+#: lino_welfare/modlib/pcsw/models.py:937
 msgid "Unemployment exclusion type"
 msgstr "Raison d'exclusion du chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:936
+#: lino_welfare/modlib/pcsw/models.py:938
 msgid "Unemployment exclusion types"
 msgstr "Types d'exclusion du chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:945
+#: lino_welfare/modlib/pcsw/models.py:947
 msgid ""
 "Liste des raisons possibles d'arrêter temporairement\n"
 "    le paiement d'une aide financière prévue."
 msgstr ""
 
-#: lino_welfare/modlib/pcsw/models.py:956
+#: lino_welfare/modlib/pcsw/models.py:958
 msgid "Exclusion from unemployment"
 msgstr "Exclusion du chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:957
+#: lino_welfare/modlib/pcsw/models.py:959
 msgid "Exclusions from unemployment"
 msgstr "Exclusions du chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:964
+#: lino_welfare/modlib/pcsw/models.py:966
 msgid "Excluded from"
 msgstr "Du"
 
-#: lino_welfare/modlib/pcsw/models.py:980
+#: lino_welfare/modlib/pcsw/models.py:982
 #, fuzzy
 msgid "Liste des exclusions."
 msgstr "exclusions"
 
-#: lino_welfare/modlib/pcsw/models.py:986
+#: lino_welfare/modlib/pcsw/models.py:988
 msgid "Unemployment situation"
 msgstr "Situation chômage"
 
-#: lino_welfare/modlib/pcsw/models.py:998
+#: lino_welfare/modlib/pcsw/models.py:1000
 msgid "Conviction"
 msgstr "Antécédent judiciaire"
 
-#: lino_welfare/modlib/pcsw/models.py:999
+#: lino_welfare/modlib/pcsw/models.py:1001
 msgid "Convictions"
 msgstr "Antécédents judiciaires"
 
-#: lino_welfare/modlib/pcsw/models.py:1003
+#: lino_welfare/modlib/pcsw/models.py:1005
 msgid "Prejudicial"
 msgstr "Préjudiciable"
 
-#: lino_welfare/modlib/pcsw/models.py:1038
+#: lino_welfare/modlib/pcsw/models.py:1040
 msgid "aid type"
 msgstr "Type d'aide sociale"
 
-#: lino_welfare/modlib/pcsw/models.py:1039
+#: lino_welfare/modlib/pcsw/models.py:1041
 msgid "aid types"
 msgstr "Types d'aide sociale"
 
-#: lino_welfare/modlib/pcsw/models.py:1043
+#: lino_welfare/modlib/pcsw/models.py:1045
 msgid "Liste des types d'aide financière."
 msgstr ""
 
 #: lino_welfare/modlib/pcsw/fixtures/std.py:26
 #, fuzzy
 msgid "Formation"
 msgstr "période d'essai"
@@ -3550,36 +3572,36 @@
 msgstr ""
 
 #: lino_welfare/modlib/reception/models.py:228
 msgid "Do you still want to issue an excerpt?"
 msgstr ""
 
 #: lino_welfare/modlib/reception/models.py:286
-#: lino_welfare/modlib/reception/models.py:370
+#: lino_welfare/modlib/reception/models.py:371
 msgid "Create appointment with"
 msgstr "Créer rendez-vous avec"
 
 #: lino_welfare/modlib/reception/models.py:315
 msgid "Agent"
 msgstr "Agent"
 
 #: lino_welfare/modlib/reception/models.py:319
 msgid "Coaching type"
 msgstr "Service"
 
 #: lino_welfare/modlib/reception/models.py:343
 #: lino_welfare/modlib/reception/models.py:347
-#: lino_welfare/modlib/reception/models.py:389
+#: lino_welfare/modlib/reception/models.py:390
 msgid "Visit"
 msgstr "Visite"
 
-#: lino_welfare/modlib/reception/models.py:359
 #: lino_welfare/modlib/reception/models.py:360
-#: lino_welfare/modlib/reception/models.py:396
+#: lino_welfare/modlib/reception/models.py:361
 #: lino_welfare/modlib/reception/models.py:397
+#: lino_welfare/modlib/reception/models.py:398
 msgid "Find date"
 msgstr "Trouver rendez-vous"
 
 #: lino_welfare/modlib/sepa/models.py:21
 msgid "Giro"
 msgstr ""
 
@@ -3661,16 +3683,18 @@
 #: lino_welfare/modlib/welfare/help_texts.py:7
 msgid "The plugin."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:8
 msgid ""
 "Optionally specify the primary key (an integer) of the last granting for\n"
-"which you want to deactivate date range validation in confirmations.  This\n"
-"is useful for keeping legacy confirmations that have been issued before the\n"
+"which you want to deactivate date range validation in confirmations.  "
+"This\n"
+"is useful for keeping legacy confirmations that have been issued before "
+"the\n"
 "rule was activated."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:12
 #: lino_welfare/modlib/welfare/help_texts.py:15
 #: lino_welfare/modlib/welfare/help_texts.py:76
 #: lino_welfare/modlib/welfare/help_texts.py:84
@@ -3807,15 +3831,16 @@
 "requests."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:60
 msgid ""
 "Validates the generated XML against the XSD files.\n"
 "Used by test suite.\n"
-"It is not necessary to validate each real request before actually sending it."
+"It is not necessary to validate each real request before actually sending"
+" it."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:63
 msgid "SSDN specific part of a request."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:64
@@ -4108,506 +4133,517 @@
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:168
 msgid "A request to the RetrieveTIGroups service (aka Tx25)"
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:169
-msgid ""
-"An account is an item of an account chart used to collect\n"
-"ledger transactions or other accountable items."
-msgstr ""
+#, fuzzy
+msgid "Whether to print empty rows."
+msgstr "Imprimer lignes vides"
+
+#: lino_welfare/modlib/welfare/help_texts.py:170
+#, fuzzy
+msgid "Whether to ignore yearly incomes."
+msgstr "Inclure revenus annuels"
 
 #: lino_welfare/modlib/welfare/help_texts.py:171
 msgid ""
-"The multilingual designation of this account, as the users see\n"
-"it."
+"Yield the entry groups for this budget, i.e. one item for each\n"
+"account group for which this budget has some data."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:173
-msgid ""
-"The account group to which this account belongs.  This must\n"
-"point to an instance of Group."
+msgid "The database model used to represent a budget actor."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:175
-msgid "The sequence number of this account within its group."
+#: lino_welfare/modlib/welfare/help_texts.py:174
+msgid "A detail row of a Budget."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:176
+#: lino_welfare/modlib/welfare/help_texts.py:175
 msgid ""
-"An optional unique name which can be used to reference a given\n"
-"account."
+"Optionally specify a budget actor who contributes this entry.\n"
+"Leave empty when the entry refers to the entire household."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:178
+#: lino_welfare/modlib/welfare/help_texts.py:177
 msgid ""
-"The account type of this account.  This must\n"
-"point to an item of\n"
-"lino_welfare.modlib.debts.AccountTypes."
+"The amount of money. An empty amount is different from a zero\n"
+"amount in that the latter will be printed while the former\n"
+"not."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:181
-msgid "Django model used to represent a debts mediation budget."
+#: lino_welfare/modlib/welfare/help_texts.py:180
+msgid "The related Account."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:182
+#: lino_welfare/modlib/welfare/help_texts.py:181
 msgid ""
-"Yield the entry groups for this budget, i.e. one item for each\n"
-"account group for which this budget has some data."
+"An account is an item of an account chart used to collect\n"
+"ledger transactions or other accountable items."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:184
+#: lino_welfare/modlib/welfare/help_texts.py:183
 msgid ""
-"An actor of a budget is a partner who is part of the household\n"
-"for which the budget has been established."
+"The multilingual designation of this account, as the users see\n"
+"it."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:186
-msgid "A detail row of a Budget."
+#: lino_welfare/modlib/welfare/help_texts.py:185
+msgid ""
+"The account group to which this account belongs.  This must\n"
+"point to an instance of Group."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:187
+msgid "The sequence number of this account within its group."
+msgstr ""
+
+#: lino_welfare/modlib/welfare/help_texts.py:188
 msgid ""
-"The amount of money. An empty amount is different from a zero\n"
-"amount in that the latter will be printed while the former\n"
-"not."
+"An optional unique name which can be used to reference a given\n"
+"account."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/help_texts.py:190
-msgid "The related Account."
+msgid ""
+"The account type of this account.  This must\n"
+"point to an item of\n"
+"lino_welfare.modlib.debts.AccountTypes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:191
+#: lino_welfare/modlib/welfare/help_texts.py:193
 msgid "The Django model that represents a client summary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:192
+#: lino_welfare/modlib/welfare/help_texts.py:194
 msgid "Base class for all tables on ClientSummary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:193
+#: lino_welfare/modlib/welfare/help_texts.py:195
 msgid "Lists all ESF summaries for all clients."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:194
+#: lino_welfare/modlib/welfare/help_texts.py:196
 msgid "Lists the ESF summaries for a given client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:195
+#: lino_welfare/modlib/welfare/help_texts.py:197
 msgid "Base class for all statistical fields."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:196
+#: lino_welfare/modlib/welfare/help_texts.py:198
 msgid "Used as the verbose_name of field."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:197
+#: lino_welfare/modlib/welfare/help_texts.py:199
 #, fuzzy
 msgid "The internal field name."
 msgstr "Mise en situation interne"
 
-#: lino_welfare/modlib/welfare/help_texts.py:198
+#: lino_welfare/modlib/welfare/help_texts.py:200
 msgid "The field descriptor (an instance of a Django Field)"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:199
+#: lino_welfare/modlib/welfare/help_texts.py:201
 msgid "Count the number of presences."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:200
+#: lino_welfare/modlib/welfare/help_texts.py:202
 msgid "Count the real hours of presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:201
+#: lino_welfare/modlib/welfare/help_texts.py:203
 msgid "Count the event’s duration for each presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:202
+#: lino_welfare/modlib/welfare/help_texts.py:204
 msgid "Count a fixed time for each presence."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:203
+#: lino_welfare/modlib/welfare/help_texts.py:205
 msgid ""
-"Shows the members of the primary household of this person together with an\n"
+"Shows the members of the primary household of this person together with "
+"an\n"
 "amount which depends on whether that member is adult or not."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:205
+#: lino_welfare/modlib/welfare/help_texts.py:207
 msgid ""
 "The amount to refund for children (household members less than\n"
 "lino_xl.lib.households.Plugin.adult_age years old)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:207
+#: lino_welfare/modlib/welfare/help_texts.py:209
 msgid ""
 "The amount to refund for children (household members who are\n"
 "lino_xl.lib.households.Plugin.adult_age years or older)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:209
+#: lino_welfare/modlib/welfare/help_texts.py:211
 msgid "The full name of the household member."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:210
+#: lino_welfare/modlib/welfare/help_texts.py:212
 msgid ""
 "The amount to pay. This is either child_tariff or\n"
 "adult_tarif depending on the age of the household member."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:212
+#: lino_welfare/modlib/welfare/help_texts.py:214
 msgid "Model mixin for all integration contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:213
+#: lino_welfare/modlib/welfare/help_texts.py:215
 msgid "The person who created this contract."
 msgstr "La personne qui a créé ce contrat."
 
-#: lino_welfare/modlib/welfare/help_texts.py:214
+#: lino_welfare/modlib/welfare/help_texts.py:216
 msgid "The responsible person at the general social service."
 msgstr "La personne responsable au service social général."
 
-#: lino_welfare/modlib/welfare/help_texts.py:215
+#: lino_welfare/modlib/welfare/help_texts.py:217
 msgid "The client for whom this contract is done."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:216
+#: lino_welfare/modlib/welfare/help_texts.py:218
 msgid "The start date of the contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:217
+#: lino_welfare/modlib/welfare/help_texts.py:219
 msgid "The planned end date of this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:218
+#: lino_welfare/modlib/welfare/help_texts.py:220
 msgid ""
 "The date when this contract was effectively ended.\n"
 "This field is set to the same value as applies_until."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:220
+#: lino_welfare/modlib/welfare/help_texts.py:222
 msgid ""
 "The reason of prematured ending.  Pointer to\n"
 "ContractEnding"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:222
+#: lino_welfare/modlib/welfare/help_texts.py:224
 msgid "When the contract was issued to the client and signed by them."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:223
+#: lino_welfare/modlib/welfare/help_texts.py:225
 msgid "When the contract was ratified by the responsible board."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:224
+#: lino_welfare/modlib/welfare/help_texts.py:226
 msgid ""
 "The language of this contract. Default value is the client’s\n"
 "language."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:226
+#: lino_welfare/modlib/welfare/help_texts.py:228
 msgid ""
 "The type of this contract. Pointer to a subclass of\n"
 "ContractTypeBase."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:228
+#: lino_welfare/modlib/welfare/help_texts.py:230
 msgid ""
 "The printed title of a contract specifies just the contract type\n"
 "(not the number and name of client)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:230
+#: lino_welfare/modlib/welfare/help_texts.py:232
 msgid ""
 "Overrides\n"
 "lino_xl.lib.excerpts.Certifiable.get_excerpt_templates()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:232
+#: lino_welfare/modlib/welfare/help_texts.py:234
 msgid ""
 "If the contract’s author is the client’s primary coach, then set\n"
 "user_asd to None, otherwise set user_asd to the primary coach.\n"
 "We no longer suppose that only integration agents write\n"
 "contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:236
+#: lino_welfare/modlib/welfare/help_texts.py:238
 msgid "Checks for the following error conditions:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:237
+#: lino_welfare/modlib/welfare/help_texts.py:239
 msgid ""
 "Returns the last aid confirmation that has been issued for this\n"
 "contract. May be used in .odt template."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:239
+#: lino_welfare/modlib/welfare/help_texts.py:241
 msgid ""
 "Automatic evaluation events have the client as mandatory\n"
 "participant, plus possibly some other coach."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:241
+#: lino_welfare/modlib/welfare/help_texts.py:243
 msgid ""
 "All contracts of a demo project (not only one) are being printed.\n"
 "Overrides\n"
 "lino.modlib.printing.Printable.get_printable_demo_objects()."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:244
+#: lino_welfare/modlib/welfare/help_texts.py:246
 msgid ""
 "Model mixin for integration contracts\n"
 "that have a single partner."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:246
+#: lino_welfare/modlib/welfare/help_texts.py:248
 msgid "Base for contract tables. Defines the following parameter fields:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:247
+#: lino_welfare/modlib/welfare/help_texts.py:249
 #, fuzzy
 msgid "See ContractEvents."
 msgstr "utilisable dans contrats"
 
-#: lino_welfare/modlib/welfare/help_texts.py:248
+#: lino_welfare/modlib/welfare/help_texts.py:250
 msgid ""
 "Show only contracts with the specified\n"
 "ContractEnding."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:250
+#: lino_welfare/modlib/welfare/help_texts.py:252
 msgid ""
 "Select “Yes” to show only contracts whose ending\n"
 "ContractEnding has\n"
 "is_success\n"
 "checked."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:254
+#: lino_welfare/modlib/welfare/help_texts.py:256
 msgid "The Django model representing an ISIP."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:255
+#: lino_welfare/modlib/welfare/help_texts.py:257
 msgid ""
 "The type of this contract.\n"
 "Pointer to ContractType."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:257
+#: lino_welfare/modlib/welfare/help_texts.py:259
 msgid ""
 "The type of study that is going to be followed during this\n"
 "contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:259
+#: lino_welfare/modlib/welfare/help_texts.py:261
 msgid "The table of all ISIP contract types."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:260
+#: lino_welfare/modlib/welfare/help_texts.py:262
 msgid "The type of a Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:261
+#: lino_welfare/modlib/welfare/help_texts.py:263
 msgid ""
 "Whether contracts of this type need their study_type\n"
 "field filled in."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:263
+#: lino_welfare/modlib/welfare/help_texts.py:265
 msgid "Django model to represent an examination policy."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:264
+#: lino_welfare/modlib/welfare/help_texts.py:266
 msgid "A possible reason for premature termination of a contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:265
+#: lino_welfare/modlib/welfare/help_texts.py:267
 msgid ""
 "Represents a third-party external partner who participates in this\n"
 "contract. For every partner there is a rich text field describing\n"
 "their duties."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:268
+#: lino_welfare/modlib/welfare/help_texts.py:270
 msgid ""
 "A list of observable events for filtering contracts\n"
 "(ContractBaseTable.observed_event)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:270
+#: lino_welfare/modlib/welfare/help_texts.py:272
 msgid ""
 "Whether the client has at least one ISIP contact during the\n"
 "observed date range."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:272
+#: lino_welfare/modlib/welfare/help_texts.py:274
 msgid ""
 "To see this table you need either IntegrationAgent or\n"
 "SocialCoordinator."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:274
+#: lino_welfare/modlib/welfare/help_texts.py:276
 msgid "Base class for all ContractType models."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:275
+#: lino_welfare/modlib/welfare/help_texts.py:277
 msgid ""
 "The full description of this contract type as used in printed\n"
 "documents."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:277
+#: lino_welfare/modlib/welfare/help_texts.py:279
 msgid ""
 "The default examination policy to be used for contracts of\n"
 "this type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:279
+#: lino_welfare/modlib/welfare/help_texts.py:281
 msgid ""
 "The overlap group to use when checking whether two contracts are\n"
 "overlapping or not. If this field is empty, Lino does not check at all\n"
 "for overlapping contracts."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:282
+#: lino_welfare/modlib/welfare/help_texts.py:284
 msgid ""
 "The main template to use instead of the default template\n"
 "defined on the excerpt type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:284
+#: lino_welfare/modlib/welfare/help_texts.py:286
 msgid ""
 "The list of all known overlap groups to be selected for the\n"
 "overlap_group\n"
 "of a contract type."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:287
+#: lino_welfare/modlib/welfare/help_texts.py:289
 msgid ""
 "Volatile object used to test for overlapping contracts.  It is\n"
 "responsible for issuing the following error messages:"
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:289
+#: lino_welfare/modlib/welfare/help_texts.py:291
 msgid "A given client cannot have two active contracts at the same time."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:290
+#: lino_welfare/modlib/welfare/help_texts.py:292
 msgid ""
 "Organisation bénéficiant de l’agrément « Initiative d’économie sociale »\n"
 "octroyé par la Wallonie."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:292
+#: lino_welfare/modlib/welfare/help_texts.py:294
 #, fuzzy
 msgid "Shows all Art60 job supplyments."
 msgstr "Mise à l'emploi art60§7"
 
-#: lino_welfare/modlib/welfare/help_texts.py:293
+#: lino_welfare/modlib/welfare/help_texts.py:295
 #, fuzzy
 msgid "Shows the Art60 job supplyments for this client."
 msgstr "Type de mise à l'emploi art.61"
 
-#: lino_welfare/modlib/welfare/help_texts.py:294
+#: lino_welfare/modlib/welfare/help_texts.py:296
 msgid ""
 "Model mixin for jobs.Contract\n"
 "and art61.Contract. And also\n"
 "for art60.Contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:297
+#: lino_welfare/modlib/welfare/help_texts.py:299
 msgid "The duration of this job supplyment (number of working days)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:298
+#: lino_welfare/modlib/welfare/help_texts.py:300
 msgid "Django model used to represent a beneficiary."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:299
+#: lino_welfare/modlib/welfare/help_texts.py:301
 msgid "Whether Lino should make ESF summaries for this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:300
+#: lino_welfare/modlib/welfare/help_texts.py:302
 msgid "A panel with general information about this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:301
+#: lino_welfare/modlib/welfare/help_texts.py:303
 msgid ""
 "A virtual field displaying a group of shortcut links for managing CVs\n"
 "(Curriculum Vitaes)."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:303
+#: lino_welfare/modlib/welfare/help_texts.py:305
 msgid ""
 "A virtual field displaying a group of buttons for managing the\n"
 "“identifying document”, i.e. an uploaded document which has been\n"
 "used as alternative to the eID card."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:306
+#: lino_welfare/modlib/welfare/help_texts.py:308
 msgid ""
 "Pointer to PersonGroup.\n"
 "The intergration phase of this client."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:308
+#: lino_welfare/modlib/welfare/help_texts.py:310
 msgid ""
 "The civil state of this client. Allowed choices are defined in\n"
 "CivilState."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:310
+#: lino_welfare/modlib/welfare/help_texts.py:312
 #, fuzzy
 msgid "Pointer to ClientStates."
 msgstr "Bénéficiares (SI)"
 
-#: lino_welfare/modlib/welfare/help_texts.py:311
+#: lino_welfare/modlib/welfare/help_texts.py:313
 msgid ""
 "The date when this client got unemployed and stopped to have a\n"
 "regular work."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:313
+#: lino_welfare/modlib/welfare/help_texts.py:315
 msgid ""
 "The date when this client registered as unemployed and started\n"
 "to look for a new job."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:315
+#: lino_welfare/modlib/welfare/help_texts.py:317
 msgid ""
 "Return the last note of type “First meeting” for this client.\n"
 "Usage example see debts and\n"
 "notes."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:318
+#: lino_welfare/modlib/welfare/help_texts.py:320
 msgid "The list that opens by Contacts ‣ Clients."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:319
+#: lino_welfare/modlib/welfare/help_texts.py:321
 msgid ""
 "If not empty, show only Clients whose client_state equals\n"
 "the specified value."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:321
+#: lino_welfare/modlib/welfare/help_texts.py:323
 msgid ""
 "Displays the response of an RetrieveTIGroupsRequest\n"
 "as a table."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:323
+#: lino_welfare/modlib/welfare/help_texts.py:325
 msgid "The Django database model."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:324
+#: lino_welfare/modlib/welfare/help_texts.py:326
 msgid "Yield a list of all subsidizations activated for this contract."
 msgstr ""
 
-#: lino_welfare/modlib/welfare/help_texts.py:325
+#: lino_welfare/modlib/welfare/help_texts.py:327
 #, fuzzy
 msgid "Shows the Art61 job supplyments for this client."
 msgstr "Type de mise à l'emploi art.61"
 
 #: lino_welfare/modlib/welfare/models.py:34
 msgid "Local job office"
 msgstr "Agence locale pour l'emploi"
@@ -4626,15 +4662,16 @@
 
 #: lino_welfare/modlib/welfare/models.py:71
 msgid "usable in contracts"
 msgstr "utilisable dans contrats"
 
 #: lino_welfare/modlib/welfare/models.py:73
 msgid ""
-"Whether Links of this type can be used as contact person of a job contract."
+"Whether Links of this type can be used as contact person of a job "
+"contract."
 msgstr ""
 
 #: lino_welfare/modlib/welfare/user_types.py:173
 msgid "Anonymous"
 msgstr "Anonyme"
 
 #: lino_welfare/modlib/welfare/user_types.py:175
@@ -5061,7 +5098,41 @@
 #~ msgstr "Activa"
 
 #~ msgid "SINE"
 #~ msgstr "Depuis"
 
 #~ msgid "responsible (IS)"
 #~ msgstr "Titulaire (ISP)"
+
+#~ msgid "(SiteConfig %s is empty)"
+#~ msgstr "(les paramètres de site %s sont vides)"
+
+#~ msgid "Skills Property Group"
+#~ msgstr "Groupe de propriétés 'Skills'"
+
+#~ msgid "The property group to be used as master for the SkillsByPerson table."
+#~ msgstr ""
+
+#~ msgid "Soft Skills Property Group"
+#~ msgstr "Groupe de propriétés 'Soft Skills'"
+
+#~ msgid ""
+#~ "The property group to be used as"
+#~ " master for the SoftSkillsByPerson table."
+#~ msgstr ""
+
+#~ msgid "Obstacles Property Group"
+#~ msgstr "Groupe de propriétés 'Freins'"
+
+#~ msgid ""
+#~ "The property group to be used as"
+#~ " master for the ObstaclesByPerson table."
+#~ msgstr ""
+
+#~ msgid "Django model used to represent a debts mediation budget."
+#~ msgstr ""
+
+#~ msgid ""
+#~ "An actor of a budget is a partner who is part of the household\n"
+#~ "for which the budget has been established."
+#~ msgstr ""
+
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/cpas2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/garble.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/garble.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/gd2lino.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/initdb_tim.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/management/commands/watch_tim.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/settings.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     # languages = 'en fr de nl'
     # hidden_languages = 'nl'
 
     migration_class = 'lino_welfare.migrate.Migrator'
     project_model = 'pcsw.Client'
     userdocs_prefix = 'welfare.'
-    auto_configure_logger_names = 'atelier schedule django lino lino_xl lino_welfare'
+    auto_configure_logger_names = 'atelier django lino lino_xl lino_welfare'
     # verbose_client_info_message = True
 
     # default_ui = "lino_react.react" # does not yet work because "Tried to get
     # static handle for debts.PrintEntriesByBudget"
 
     # default_build_method = "appyodt"
     default_build_method = "appypdf"
@@ -42,15 +42,15 @@
         yield ('clients', 'demo_coach', 'hubert')
         yield ('addresses', 'partner_model', 'contacts.Partner')
         yield ('excerpts', 'responsible_user', 'melanie')
         # if 'ledger' in self.plugins:
         yield ('ledger', 'ref_length', 16)
         yield ('ledger', 'project_model', 'pcsw.Client')
         yield ('cal', 'mytasks_start_date', -30)
-        yield ('help', 'interproject_specs', 'lino_welfare')
+        # yield ('help', 'interproject_specs', 'lino_welfare')
 
     def setup_quicklinks(self, user, tb):
         # tb.add_action(self.modules.pcsw.Clients.detail_action)
         super(Site, self).setup_quicklinks(user, tb)
         tb.add_action("pcsw.Clients.find_by_beid")
         tb.add_action(self.modules.integ.Clients)
         tb.add_action(self.modules.isip.MyContracts)
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/user_types.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/user_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from lino.modlib.users.roles import AuthorshipTaker
 from lino.modlib.search.roles import SiteSearcher
 from lino.modlib.office.roles import OfficeOperator, OfficeStaff, OfficeUser
 from lino_xl.lib.notes.roles import NotesUser, NotesStaff
 from lino_xl.lib.excerpts.roles import ExcerptsUser, ExcerptsStaff
 from lino_xl.lib.contacts.roles import ContactsStaff, ContactsUser, SimpleContactsUser
 from lino_xl.lib.ledger.roles import LedgerStaff, LedgerUser
-from lino_xl.lib.cal.roles import GuestOperator
+from lino_xl.lib.cal.roles import GuestOperator, CalendarReader
 from lino_xl.lib.courses.roles import CoursesUser, CoursesTeacher
 from lino_xl.lib.cv.roles import CareerUser, CareerStaff
 from lino_xl.lib.beid.roles import BeIdUser
 from lino_welfare.modlib.cbss.roles import CBSSUser, SecurityAdvisor
 from lino_welfare.modlib.pcsw.roles import SocialUser
 from lino_welfare.modlib.pcsw.roles import SocialStaff
 from lino_welfare.modlib.pcsw.roles import SocialCoordinator
@@ -41,15 +41,15 @@
 # class CoursesUser(CoursesUser, xCoursesUser):
 #     pass
 
 
 # 210
 class ReceptionClerk(SiteUser, AuthorshipTaker,
                      OfficeOperator, NotesUser,
-                     GuestOperator,
+                     GuestOperator, CalendarReader,
                      ContactsStaff, AidsStaff, CBSSUser, BeIdUser,
                      SepaUser, ExcerptsUser, CoursesUser,
                      SocialCoordinator, CoachingsStaff):
     pass
 
 
 class ReceptionClerkFlexible(SiteUser, AuthorshipTaker,
```

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/welfare/workflows.py` & `lino-welfare-23.6.0/lino_welfare/modlib/welfare/workflows.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/xcourses/__init__.py` & `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/candidates.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt` & `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/config/courses/Course/participants.odt`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/xcourses/fixtures/demo.py` & `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/modlib/xcourses/models.py` & `lino-welfare-23.6.0/lino_welfare/modlib/xcourses/models.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/print_tx25.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/print_tx25.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/demo.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/settings/mysql.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/settings/mysql.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_aids.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_aids.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_broken_gfks.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_cbss.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_cbss.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_clients.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import logging
 logger = logging.getLogger(__name__)
 
 from django.conf import settings
 from lino.utils.djangotest import RemoteAuthTestCase
 
 from lino.utils import i2d
-from lino_xl.lib.cal.choicelists import WORKDAYS
 from lino_xl.lib.clients.choicelists import ClientStates
 from lino.modlib.users.choicelists import UserTypes
 from lino.modlib.system.choicelists import Genders
 from lino.utils.instantiator import create_row as create
 from lino.api import rt
 
 
@@ -81,13 +80,13 @@
 robin a class\xe9 MUSTERMANN Max (100) comme <b>Refus\xe9</b>."""
         # print(expected)
         self.assertEqual(expected, result['message'])
         self.assertEqual(Note.objects.count(), 1)
         self.assertEqual(Message.objects.count(), 1)
         msg = Message.objects.all()[0]
         expected = """\
-robin a classé [client 100] (M. Max MUSTERMANN) comme <b>Refusé</b>.
+robin a classé [client 100] comme <b>Refusé</b>.
 Raison de refus: CPAS n'est pas compétent
 Wohnt noch in Lüttich. Wollte nach Eupen ziehen. Noch nicht zuständigg"""
         self.assertEqual(expected, msg.body)
 
         # print("20180503 test_clients.test01() done")
```

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_debts.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_debts.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/gerd/tests/test_watchtim.py` & `lino-welfare-23.6.0/lino_welfare/projects/gerd/tests/test_watchtim.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/demo.py` & `lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg` & `lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/123456789012.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg` & `lino-welfare-23.6.0/lino_welfare/projects/mathieu/settings/media/beid/591413288107.jpg`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/mathieu/tests/test_chatelet.py` & `lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/test_chatelet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,11 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2015-2022 Rumma & Ko Ltd
+# Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
-
-"""Miscellaneous tests on an empty database.
-
-You can run just these tests by issuing::
-
-  $ go mathieu
-  $ pm test tests.test_chatelet
-
-"""
+# $ pm test tests.test_chatelet
 
 from django.conf import settings
 from django.core.exceptions import ValidationError
 
 from lino.api import rt
 from lino.core import constants
 from lino.modlib.users.choicelists import UserTypes
@@ -110,27 +102,27 @@
         result = self.check_json_result(
             response,
             "detail_handler_name data_record rows "
             "close_window success message navinfo")
         self.assertEqual(result['success'], True)
         self.assertEqual(
             result['message'],
-            'B\xe9n\xe9ficiaire "LAST First (101)" a \xe9t\xe9 cr\xe9\xe9')
+            'Bénéficiaire "LAST First (101)" a été créé.')
 
     def test_suggest_cal_guests(self):
         """Tests a bugfix in :meth:`suggest_cal_guests
         <lino_xl.lib.courses.Course.suggest_cal_guests>`.
 
         """
         User = settings.SITE.user_model
         Guest = rt.models.cal.Guest
         Event = rt.models.cal.Event
         EventType = rt.models.cal.EventType
         GuestRole = rt.models.cal.GuestRole
-        Recurrencies = rt.models.cal.Recurrencies
+        Recurrencies = rt.models.system.Recurrencies
         Room = rt.models.cal.Room
         Enrolment = rt.models.courses.Enrolment
         Course = rt.models.courses.Course
         Line = rt.models.courses.Line
         EnrolmentStates = rt.models.courses.EnrolmentStates
         Pupil = rt.models.pcsw.Client
```

### Comparing `lino-welfare-23.1.0/lino_welfare/projects/mathieu/tests/test_notify.py` & `lino-welfare-23.6.0/lino_welfare/projects/mathieu/tests/test_notify.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/scripts/load_plp.py` & `lino-welfare-23.6.0/lino_welfare/scripts/load_plp.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/lino_welfare/setup_info.py` & `lino-welfare-23.6.0/lino_welfare/setup_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             'pytidylib',
             'django-iban', 'metafone',
             'cairocffi']
 requires.append('suds-py3')
 
 SETUP_INFO = dict(
     name='lino-welfare',
-    version='23.1.0',
+    version='23.6.0',
     install_requires=requires,
     test_suite='tests',
     tests_require=['pytest'],
     include_package_data=True,
     zip_safe=False,
     description="A Lino plugin library for Belgian PCSWs",
     long_description="""\
```

### Comparing `lino-welfare-23.1.0/lino_welfare.egg-info/PKG-INFO` & `lino-welfare-23.6.0/lino_welfare.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino-welfare
-Version: 23.1.0
+Version: 23.6.0
 Summary: A Lino plugin library for Belgian PCSWs
 Home-page: https://gitlab.com/lino-framework/welfare
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -57,9 +55,7 @@
 - For introductions, commercial information and hosting solutions
   see https://www.saffre-rumma.net
 
 - This is a sustainably free open-source project. Your contributions are
   welcome.  See https://community.lino-framework.org for details.
 
 
-
-
```

### Comparing `lino-welfare-23.1.0/lino_welfare.egg-info/SOURCES.txt` & `lino-welfare-23.6.0/lino_welfare.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -66,24 +66,18 @@
 lino_welfare/modlib/cbss/choicelists.py
 lino_welfare/modlib/cbss/mixins.py
 lino_welfare/modlib/cbss/models.py
 lino_welfare/modlib/cbss/roles.py
 lino_welfare/modlib/cbss/tx25.py
 lino_welfare/modlib/cbss/ui.py
 lino_welfare/modlib/cbss/utils.py
-lino_welfare/modlib/cbss/WSDL/2013HealthCareInsurance.wsdl
 lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v1.wsdl
 lino_welfare/modlib/cbss/WSDL/RetrieveTIGroups-v2.wsdl
 lino_welfare/modlib/cbss/WSDL/TestConnectionService.wsdl
 lino_welfare/modlib/cbss/WSDL/WebServiceConnector.wsdl
-lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataTypesV2.xsd
-lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.wsdl
-lino_welfare/modlib/cbss/WSDL/UnemploymentData/UnemploymentDataV2.xsd
-lino_welfare/modlib/cbss/XSD/HealthCareInsuranceTypesV1.xsd
-lino_welfare/modlib/cbss/XSD/HealthCareInsuranceV1.xsd
 lino_welfare/modlib/cbss/XSD/README.txt
 lino_welfare/modlib/cbss/XSD/TestConnectionServiceV1.xsd
 lino_welfare/modlib/cbss/XSD/20190612/RetrieveTIGroupsV5.xsd
 lino_welfare/modlib/cbss/XSD/20190612/rn25_Release201411.xsd
 lino_welfare/modlib/cbss/XSD/SSDN/Common/CommonDataTypes.xsd
 lino_welfare/modlib/cbss/XSD/SSDN/Common/ExtensionPlaceHolder.xsd
 lino_welfare/modlib/cbss/XSD/SSDN/Common/NamespaceRoot.xsd
@@ -333,15 +327,14 @@
 lino_welfare/projects/gerd/settings/__init__.py
 lino_welfare/projects/gerd/settings/demo.py
 lino_welfare/projects/gerd/settings/doctests.py
 lino_welfare/projects/gerd/settings/memory.py
 lino_welfare/projects/gerd/settings/mysql.py
 lino_welfare/projects/gerd/settings/media/beid/123456789012.jpg
 lino_welfare/projects/gerd/settings/media/beid/591413288107.jpg
-lino_welfare/projects/gerd/settings/media/beid/592382784616.jpg
 lino_welfare/projects/gerd/settings/media/webdav/userdocs/appyodt/jobs.JobsOverview.odt
 lino_welfare/projects/gerd/tests/__init__.py
 lino_welfare/projects/gerd/tests/test_aids.py
 lino_welfare/projects/gerd/tests/test_broken_gfks.py
 lino_welfare/projects/gerd/tests/test_cbss.py
 lino_welfare/projects/gerd/tests/test_clients.py
 lino_welfare/projects/gerd/tests/test_debts.py
```

### Comparing `lino-welfare-23.1.0/tasks.py` & `lino-welfare-23.6.0/tasks.py`

 * *Files identical despite different names*

### Comparing `lino-welfare-23.1.0/tests/__init__.py` & `lino-welfare-23.6.0/tests/__init__.py`

 * *Files identical despite different names*

