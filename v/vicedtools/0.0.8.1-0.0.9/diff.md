# Comparing `tmp/vicedtools-0.0.8.1.tar.gz` & `tmp/vicedtools-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vicedtools-0.0.8.1.tar", last modified: Fri Apr 14 16:38:57 2023, max compression
+gzip compressed data, was "vicedtools-0.0.9.tar", last modified: Tue Jun 20 10:28:26 2023, max compression
```

## Comparing `vicedtools-0.0.8.1.tar` & `vicedtools-0.0.9.tar`

### file list

```diff
@@ -1,51 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.996809 vicedtools-0.0.8.1/
--rw-rw-rw-   0        0        0    11558 2021-05-29 17:10:03.000000 vicedtools-0.0.8.1/LICENSE
--rw-rw-rw-   0        0        0     5212 2023-04-14 16:38:56.996809 vicedtools-0.0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     4636 2023-04-14 07:45:30.000000 vicedtools-0.0.8.1/README.md
--rw-rw-rw-   0        0        0      108 2021-05-29 17:13:52.000000 vicedtools-0.0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0      863 2023-04-14 16:38:56.999809 vicedtools-0.0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     3857 2023-04-14 06:14:58.000000 vicedtools-0.0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.774253 vicedtools-0.0.8.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.801418 vicedtools-0.0.8.1/src/vicedtools/
--rw-rw-rw-   0        0        0     1498 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.900111 vicedtools-0.0.8.1/src/vicedtools/acer/
--rw-rw-rw-   0        0        0     1341 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/acer/__init__.py
--rw-rw-rw-   0        0        0     4191 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/ewritesittings.py
--rw-rw-rw-   0        0        0     1188 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/extraoarsauthenticators.py
--rw-rw-rw-   0        0        0     7223 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oars.py
--rw-rw-rw-   0        0        0     2269 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oarsauthenticators.py
--rw-rw-rw-   0        0        0     4902 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oarscandidates.py
--rw-rw-rw-   0        0        0    16115 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oarssession.py
--rw-rw-rw-   0        0        0     5368 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/oarstests.py
--rw-rw-rw-   0        0        0     1878 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/patitems.py
--rw-rw-rw-   0        0        0    15529 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/patresults.py
--rw-rw-rw-   0        0        0     6964 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/acer/patsittings.py
--rw-rw-rw-   0        0        0    21888 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/acer/plots.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.926357 vicedtools-0.0.8.1/src/vicedtools/compass/
--rw-rw-rw-   0        0        0      982 2023-04-13 17:44:21.000000 vicedtools-0.0.8.1/src/vicedtools/compass/__init__.py
--rw-rw-rw-   0        0        0     4384 2023-04-13 17:44:21.000000 vicedtools-0.0.8.1/src/vicedtools/compass/compassauthenticators.py
--rw-rw-rw-   0        0        0    19553 2023-04-13 17:44:21.000000 vicedtools-0.0.8.1/src/vicedtools/compass/compasssession.py
--rw-rw-rw-   0        0        0     1113 2023-04-13 17:44:21.000000 vicedtools-0.0.8.1/src/vicedtools/compass/extraauthenticators.py
--rw-rw-rw-   0        0        0    18167 2023-04-14 16:23:35.000000 vicedtools-0.0.8.1/src/vicedtools/compass/reports.py
--rw-rw-rw-   0        0        0     3645 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/educationperfect.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.947019 vicedtools-0.0.8.1/src/vicedtools/gcp/
--rw-rw-rw-   0        0        0     1338 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/gcp/__init__.py
--rw-rw-rw-   0        0        0     2725 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/gcp/api.py
--rw-rw-rw-   0        0        0     2042 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/gcp/format.py
--rw-rw-rw-   0        0        0     6566 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/gcp/schema.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.972019 vicedtools-0.0.8.1/src/vicedtools/naplan/
--rw-rw-rw-   0        0        0      815 2023-04-13 17:39:12.000000 vicedtools-0.0.8.1/src/vicedtools/naplan/__init__.py
--rw-rw-rw-   0        0        0     5815 2023-04-13 17:39:11.000000 vicedtools-0.0.8.1/src/vicedtools/naplan/dataservicesession.py
--rw-rw-rw-   0        0        0     6193 2023-04-14 07:39:34.000000 vicedtools-0.0.8.1/src/vicedtools/naplan/sssrdata.py
--rw-rw-rw-   0        0        0     2004 2023-04-13 17:39:10.000000 vicedtools-0.0.8.1/src/vicedtools/sportstrak.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.994086 vicedtools-0.0.8.1/src/vicedtools/vce/
--rw-rw-rw-   0        0        0      798 2023-04-13 17:39:14.000000 vicedtools-0.0.8.1/src/vicedtools/vce/__init__.py
--rw-rw-rw-   0        0        0     3020 2023-04-13 17:39:13.000000 vicedtools-0.0.8.1/src/vicedtools/vce/schoolscores.py
--rw-rw-rw-   0        0        0    34328 2023-04-13 17:39:13.000000 vicedtools-0.0.8.1/src/vicedtools/vce/vasssession.py
-drwxrwxrwx   0        0        0        0 2023-04-14 16:38:56.849317 vicedtools-0.0.8.1/src/vicedtools.egg-info/
--rw-rw-rw-   0        0        0     5212 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1326 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3162 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-14 16:38:56.000000 vicedtools-0.0.8.1/src/vicedtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:26.442174 vicedtools-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2021-05-29 17:10:03.000000 vicedtools-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5210 2023-06-20 10:28:26.442174 vicedtools-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4636 2023-04-14 07:45:30.000000 vicedtools-0.0.9/README.md
+-rw-rw-rw-   0        0        0      108 2021-05-29 17:13:52.000000 vicedtools-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      861 2023-06-20 10:28:26.447174 vicedtools-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3857 2023-04-14 06:14:58.000000 vicedtools-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:25.318058 vicedtools-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:25.362553 vicedtools-0.0.9/src/vicedtools/
+-rw-rw-rw-   0        0        0     1498 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:25.417363 vicedtools-0.0.9/src/vicedtools/acer/
+-rw-rw-rw-   0        0        0     1341 2023-04-13 17:39:11.000000 vicedtools-0.0.9/src/vicedtools/acer/__init__.py
+-rw-rw-rw-   0        0        0     4191 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/ewritesittings.py
+-rw-rw-rw-   0        0        0     1188 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/extraoarsauthenticators.py
+-rw-rw-rw-   0        0        0     7223 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/oars.py
+-rw-rw-rw-   0        0        0     2269 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/oarsauthenticators.py
+-rw-rw-rw-   0        0        0     4902 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/oarscandidates.py
+-rw-rw-rw-   0        0        0    16115 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/oarssession.py
+-rw-rw-rw-   0        0        0     5368 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/oarstests.py
+-rw-rw-rw-   0        0        0     1878 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/patitems.py
+-rw-rw-rw-   0        0        0    15529 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/patresults.py
+-rw-rw-rw-   0        0        0     6964 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/acer/patsittings.py
+-rw-rw-rw-   0        0        0    21888 2023-06-19 23:18:13.000000 vicedtools-0.0.9/src/vicedtools/acer/plots.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:25.426145 vicedtools-0.0.9/src/vicedtools/compass/
+-rw-rw-rw-   0        0        0      982 2023-04-13 17:44:21.000000 vicedtools-0.0.9/src/vicedtools/compass/__init__.py
+-rw-rw-rw-   0        0        0     4384 2023-04-13 17:44:21.000000 vicedtools-0.0.9/src/vicedtools/compass/compassauthenticators.py
+-rw-rw-rw-   0        0        0    22937 2023-06-19 23:18:14.000000 vicedtools-0.0.9/src/vicedtools/compass/compasssession.py
+-rw-rw-rw-   0        0        0     1113 2023-04-13 17:44:21.000000 vicedtools-0.0.9/src/vicedtools/compass/extraauthenticators.py
+-rw-rw-rw-   0        0        0    18321 2023-06-19 23:18:14.000000 vicedtools-0.0.9/src/vicedtools/compass/reports.py
+-rw-rw-rw-   0        0        0     8750 2023-06-20 10:19:54.000000 vicedtools-0.0.9/src/vicedtools/config.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:25.431659 vicedtools-0.0.9/src/vicedtools/dal/
+-rw-rw-rw-   0        0        0      651 2023-05-02 06:27:52.000000 vicedtools-0.0.9/src/vicedtools/dal/__init__.py
+-rw-rw-rw-   0        0        0     2072 2023-06-19 23:18:14.000000 vicedtools-0.0.9/src/vicedtools/dal/utilities.py
+-rw-rw-rw-   0        0        0     3645 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/educationperfect.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:25.437768 vicedtools-0.0.9/src/vicedtools/gcp/
+-rw-rw-rw-   0        0        0     1395 2023-06-20 01:18:54.000000 vicedtools-0.0.9/src/vicedtools/gcp/__init__.py
+-rw-rw-rw-   0        0        0     2725 2023-04-13 17:39:11.000000 vicedtools-0.0.9/src/vicedtools/gcp/api.py
+-rw-rw-rw-   0        0        0     2042 2023-04-13 17:39:11.000000 vicedtools-0.0.9/src/vicedtools/gcp/format.py
+-rw-rw-rw-   0        0        0     7194 2023-06-20 01:18:02.000000 vicedtools-0.0.9/src/vicedtools/gcp/schema.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:25.443530 vicedtools-0.0.9/src/vicedtools/naplan/
+-rw-rw-rw-   0        0        0      815 2023-04-13 17:39:12.000000 vicedtools-0.0.9/src/vicedtools/naplan/__init__.py
+-rw-rw-rw-   0        0        0     5815 2023-04-13 17:39:11.000000 vicedtools-0.0.9/src/vicedtools/naplan/dataservicesession.py
+-rw-rw-rw-   0        0        0     6193 2023-04-14 07:39:34.000000 vicedtools-0.0.9/src/vicedtools/naplan/sssrdata.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:26.433176 vicedtools-0.0.9/src/vicedtools/scripts/
+-rw-rw-rw-   0        0        0      594 2023-06-20 10:27:58.000000 vicedtools-0.0.9/src/vicedtools/scripts/__init__.py
+-rw-rw-rw-   0        0        0     1537 2023-06-20 10:21:55.000000 vicedtools-0.0.9/src/vicedtools/scripts/compassreportstobq.py
+-rw-rw-rw-   0        0        0     2781 2023-06-20 10:22:08.000000 vicedtools-0.0.9/src/vicedtools/scripts/compassstudentdetailstobq.py
+-rw-rw-rw-   0        0        0     2282 2023-06-20 10:22:07.000000 vicedtools-0.0.9/src/vicedtools/scripts/compassstudentenrolmenttobq.py
+-rw-rw-rw-   0        0        0     2997 2023-06-20 10:22:04.000000 vicedtools-0.0.9/src/vicedtools/scripts/createcompassreportssummaries.py
+-rw-rw-rw-   0        0        0     1564 2023-06-20 10:22:05.000000 vicedtools-0.0.9/src/vicedtools/scripts/createcompasssubjectsmetadatacsv.py
+-rw-rw-rw-   0        0        0     4093 2023-06-20 10:22:06.000000 vicedtools-0.0.9/src/vicedtools/scripts/createnaplansummary.py
+-rw-rw-rw-   0        0        0     8893 2023-06-20 10:22:03.000000 vicedtools-0.0.9/src/vicedtools/scripts/createoarsstudentimports.py
+-rw-rw-rw-   0        0        0     4041 2023-06-20 10:22:54.000000 vicedtools-0.0.9/src/vicedtools/scripts/createpatparentlettertable.py
+-rw-rw-rw-   0        0        0     1397 2023-06-20 10:22:53.000000 vicedtools-0.0.9/src/vicedtools/scripts/createsportstrakxlsx.py
+-rw-rw-rw-   0        0        0     1698 2023-06-20 10:22:52.000000 vicedtools-0.0.9/src/vicedtools/scripts/ewritescorestobq.py
+-rw-rw-rw-   0        0        0     4181 2023-06-20 10:22:51.000000 vicedtools-0.0.9/src/vicedtools/scripts/ewritesittingstoscores.py
+-rw-rw-rw-   0        0        0     1379 2023-06-20 10:22:50.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassacademicgroups.py
+-rw-rw-rw-   0        0        0     1801 2023-06-20 10:22:49.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassattendancehalfday.py
+-rw-rw-rw-   0        0        0     2633 2023-06-20 10:22:45.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassclasses.py
+-rw-rw-rw-   0        0        0     3178 2023-06-20 10:22:42.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassenrolments.py
+-rw-rw-rw-   0        0        0     2385 2023-06-20 10:22:41.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompasslearningtask.py
+-rw-rw-rw-   0        0        0     2475 2023-06-20 10:22:40.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompasslearningtasks.py
+-rw-rw-rw-   0        0        0     1877 2023-06-20 10:22:39.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassprogressreport.py
+-rw-rw-rw-   0        0        0     1414 2023-06-20 10:22:37.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassprogressreportcycles.py
+-rw-rw-rw-   0        0        0     2645 2023-06-20 10:22:36.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassprogressreports.py
+-rw-rw-rw-   0        0        0     1686 2023-06-20 10:22:35.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassreport.py
+-rw-rw-rw-   0        0        0     1369 2023-06-20 10:22:34.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassreportcycles.py
+-rw-rw-rw-   0        0        0     2262 2023-06-20 10:22:32.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassreports.py
+-rw-rw-rw-   0        0        0     2186 2023-06-20 10:22:33.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompasssds.py
+-rw-rw-rw-   0        0        0     1308 2023-06-20 10:22:31.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassstudenthouseholdinformation.py
+-rw-rw-rw-   0        0        0     1250 2023-06-20 10:22:30.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompassstudents.py
+-rw-rw-rw-   0        0        0     2387 2023-06-20 10:22:30.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportcompasssubjectmetadata.py
+-rw-rw-rw-   0        0        0     1530 2023-06-20 10:22:29.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportnaplanoutcomes.py
+-rw-rw-rw-   0        0        0     1512 2023-06-20 10:22:27.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportnaplansssr.py
+-rw-rw-rw-   0        0        0     1483 2023-06-20 10:22:28.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportoarsmetadata.py
+-rw-rw-rw-   0        0        0     2230 2023-06-20 10:22:24.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportoarssittings.py
+-rw-rw-rw-   0        0        0     1163 2023-06-20 10:22:26.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportoarsstaff.py
+-rw-rw-rw-   0        0        0     1255 2023-06-20 10:22:23.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportoarsstudents.py
+-rw-rw-rw-   0        0        0     1579 2023-06-20 10:22:21.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportvassexternalscores.py
+-rw-rw-rw-   0        0        0     1463 2023-06-20 10:22:22.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportvassgatscores.py
+-rw-rw-rw-   0        0        0     1928 2023-06-20 10:22:21.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportvassmoderatedscores.py
+-rw-rw-rw-   0        0        0     1584 2023-06-20 10:22:20.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportvasspredictedscores.py
+-rw-rw-rw-   0        0        0     1584 2023-06-20 10:22:17.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportvassschoolprogram.py
+-rw-rw-rw-   0        0        0     1811 2023-06-20 10:22:18.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportvassschoolscores.py
+-rw-rw-rw-   0        0        0     1583 2023-06-20 10:22:16.000000 vicedtools-0.0.9/src/vicedtools/scripts/exportvassstudentdetails.py
+-rw-rw-rw-   0        0        0     1747 2023-06-20 10:22:57.000000 vicedtools-0.0.9/src/vicedtools/scripts/naplanoutcomestobq.py
+-rw-rw-rw-   0        0        0     2160 2023-06-20 10:22:14.000000 vicedtools-0.0.9/src/vicedtools/scripts/patmostrecentobq.py
+-rw-rw-rw-   0        0        0     1737 2023-06-20 10:22:02.000000 vicedtools-0.0.9/src/vicedtools/scripts/patscorestobq.py
+-rw-rw-rw-   0        0        0     1361 2023-06-20 10:22:11.000000 vicedtools-0.0.9/src/vicedtools/scripts/patscorestomostrecent.py
+-rw-rw-rw-   0        0        0     2510 2023-06-20 10:22:00.000000 vicedtools-0.0.9/src/vicedtools/scripts/patsittingstoscores.py
+-rw-rw-rw-   0        0        0     2004 2023-04-13 17:39:10.000000 vicedtools-0.0.9/src/vicedtools/sportstrak.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:26.440176 vicedtools-0.0.9/src/vicedtools/vce/
+-rw-rw-rw-   0        0        0      798 2023-04-13 17:39:14.000000 vicedtools-0.0.9/src/vicedtools/vce/__init__.py
+-rw-rw-rw-   0        0        0     3020 2023-04-13 17:39:13.000000 vicedtools-0.0.9/src/vicedtools/vce/schoolscores.py
+-rw-rw-rw-   0        0        0    34328 2023-04-13 17:39:13.000000 vicedtools-0.0.9/src/vicedtools/vce/vasssession.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:28:25.390819 vicedtools-0.0.9/src/vicedtools.egg-info/
+-rw-rw-rw-   0        0        0     5210 2023-06-20 10:28:25.000000 vicedtools-0.0.9/src/vicedtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3684 2023-06-20 10:28:25.000000 vicedtools-0.0.9/src/vicedtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:28:25.000000 vicedtools-0.0.9/src/vicedtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3162 2023-06-20 10:28:25.000000 vicedtools-0.0.9/src/vicedtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      119 2023-06-20 10:28:25.000000 vicedtools-0.0.9/src/vicedtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-20 10:28:25.000000 vicedtools-0.0.9/src/vicedtools.egg-info/top_level.txt
```

### Comparing `vicedtools-0.0.8.1/LICENSE` & `vicedtools-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/PKG-INFO` & `vicedtools-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicedtools
-Version: 0.0.8.1
+Version: 0.0.9
 Summary: A collection of tools for school data in Victorian schools.
 Home-page: https://github.com/gregbreese/vicedtools
 Author: Greg Breese
 Project-URL: Bug Tracker, https://github.com/gregbreese/vicedtools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vicedtools-0.0.8.1/README.md` & `vicedtools-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/setup.cfg` & `vicedtools-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6963 6564 746f 6f6c 730d 0a76   = vicedtools..v
-00000020: 6572 7369 6f6e 203d 2030 2e30 2e38 2e31  ersion = 0.0.8.1
-00000030: 0d0a 6175 7468 6f72 203d 2047 7265 6720  ..author = Greg 
-00000040: 4272 6565 7365 0d0a 6465 7363 7269 7074  Breese..descript
-00000050: 696f 6e20 3d20 4120 636f 6c6c 6563 7469  ion = A collecti
-00000060: 6f6e 206f 6620 746f 6f6c 7320 666f 7220  on of tools for 
-00000070: 7363 686f 6f6c 2064 6174 6120 696e 2056  school data in V
-00000080: 6963 746f 7269 616e 2073 6368 6f6f 6c73  ictorian schools
-00000090: 2e0d 0a6c 6f6e 675f 6465 7363 7269 7074  ...long_descript
-000000a0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
-000000b0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
-000000c0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
-000000d0: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
-000000e0: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
-000000f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f67  s://github.com/g
-00000100: 7265 6762 7265 6573 652f 7669 6365 6474  regbreese/vicedt
-00000110: 6f6f 6c73 0d0a 7072 6f6a 6563 745f 7572  ools..project_ur
-00000120: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
-00000130: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
-00000140: 7468 7562 2e63 6f6d 2f67 7265 6762 7265  thub.com/gregbre
-00000150: 6573 652f 7669 6365 6474 6f6f 6c73 2f69  ese/vicedtools/i
-00000160: 7373 7565 730d 0a63 6c61 7373 6966 6965  ssues..classifie
-00000170: 7273 203d 200d 0a09 5072 6f67 7261 6d6d  rs = ...Programm
-00000180: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000190: 5079 7468 6f6e 203a 3a20 330d 0a09 4c69  Python :: 3...Li
-000001a0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001b0: 726f 7665 6420 3a3a 2041 7061 6368 6520  roved :: Apache 
-000001c0: 536f 6674 7761 7265 204c 6963 656e 7365  Software License
-000001d0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-000001e0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000001f0: 6e64 656e 740d 0a09 4465 7665 6c6f 706d  ndent...Developm
-00000200: 656e 7420 5374 6174 7573 203a 3a20 3320  ent Status :: 3 
-00000210: 2d20 416c 7068 610d 0a0d 0a5b 6f70 7469  - Alpha....[opti
-00000220: 6f6e 735d 0d0a 7061 636b 6167 655f 6469  ons]..package_di
-00000230: 7220 3d20 0d0a 093d 2073 7263 0d0a 7061  r = ...= src..pa
-00000240: 636b 6167 6573 203d 2066 696e 643a 0d0a  ckages = find:..
-00000250: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
-00000260: 3d20 3e3d 332e 380d 0a69 6e73 7461 6c6c  = >=3.8..install
-00000270: 5f72 6571 7569 7265 7320 3d20 0d0a 0962  _requires = ...b
-00000280: 726f 7773 6572 5f63 6f6f 6b69 6533 0d0a  rowser_cookie3..
-00000290: 0962 7334 0d0a 0964 656d 6a73 6f6e 330d  .bs4...demjson3.
-000002a0: 0a09 676f 6f67 6c65 2d63 6c6f 7564 2d62  ..google-cloud-b
-000002b0: 6967 7175 6572 790d 0a09 676f 6f67 6c65  igquery...google
-000002c0: 2d63 6c6f 7564 2d73 746f 7261 6765 0d0a  -cloud-storage..
-000002d0: 096d 6174 706c 6f74 6c69 620d 0a09 6e75  .matplotlib...nu
-000002e0: 6d70 790d 0a09 7061 6e64 6173 0d0a 0973  mpy...pandas...s
-000002f0: 6561 626f 726e 0d0a 0973 656c 656e 6975  eaborn...seleniu
-00000300: 6d0d 0a09 746f 6d6c 690d 0a0d 0a5b 6f70  m...tomli....[op
-00000310: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-00000320: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-00000330: 630d 0a0d 0a5b 6567 675f 696e 666f 5d0d  c....[egg_info].
-00000340: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000350: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000020: 6572 7369 6f6e 203d 2030 2e30 2e39 0d0a  ersion = 0.0.9..
+00000030: 6175 7468 6f72 203d 2047 7265 6720 4272  author = Greg Br
+00000040: 6565 7365 0d0a 6465 7363 7269 7074 696f  eese..descriptio
+00000050: 6e20 3d20 4120 636f 6c6c 6563 7469 6f6e  n = A collection
+00000060: 206f 6620 746f 6f6c 7320 666f 7220 7363   of tools for sc
+00000070: 686f 6f6c 2064 6174 6120 696e 2056 6963  hool data in Vic
+00000080: 746f 7269 616e 2073 6368 6f6f 6c73 2e0d  torian schools..
+00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000a0: 6e20 3d20 6669 6c65 3a20 5245 4144 4d45  n = file: README
+000000b0: 2e6d 640d 0a6c 6f6e 675f 6465 7363 7269  .md..long_descri
+000000c0: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
+000000d0: 7065 203d 2074 6578 742f 6d61 726b 646f  pe = text/markdo
+000000e0: 776e 0d0a 7572 6c20 3d20 6874 7470 733a  wn..url = https:
+000000f0: 2f2f 6769 7468 7562 2e63 6f6d 2f67 7265  //github.com/gre
+00000100: 6762 7265 6573 652f 7669 6365 6474 6f6f  gbreese/vicedtoo
+00000110: 6c73 0d0a 7072 6f6a 6563 745f 7572 6c73  ls..project_urls
+00000120: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
+00000130: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
+00000140: 7562 2e63 6f6d 2f67 7265 6762 7265 6573  ub.com/gregbrees
+00000150: 652f 7669 6365 6474 6f6f 6c73 2f69 7373  e/vicedtools/iss
+00000160: 7565 730d 0a63 6c61 7373 6966 6965 7273  ues..classifiers
+00000170: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+00000180: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000190: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
+000001a0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000001b0: 7665 6420 3a3a 2041 7061 6368 6520 536f  ved :: Apache So
+000001c0: 6674 7761 7265 204c 6963 656e 7365 0d0a  ftware License..
+000001d0: 094f 7065 7261 7469 6e67 2053 7973 7465  .Operating Syste
+000001e0: 6d20 3a3a 204f 5320 496e 6465 7065 6e64  m :: OS Independ
+000001f0: 656e 740d 0a09 4465 7665 6c6f 706d 656e  ent...Developmen
+00000200: 7420 5374 6174 7573 203a 3a20 3320 2d20  t Status :: 3 - 
+00000210: 416c 7068 610d 0a0d 0a5b 6f70 7469 6f6e  Alpha....[option
+00000220: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000230: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000240: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000250: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000260: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
+00000270: 6571 7569 7265 7320 3d20 0d0a 0962 726f  equires = ...bro
+00000280: 7773 6572 5f63 6f6f 6b69 6533 0d0a 0962  wser_cookie3...b
+00000290: 7334 0d0a 0964 656d 6a73 6f6e 330d 0a09  s4...demjson3...
+000002a0: 676f 6f67 6c65 2d63 6c6f 7564 2d62 6967  google-cloud-big
+000002b0: 7175 6572 790d 0a09 676f 6f67 6c65 2d63  query...google-c
+000002c0: 6c6f 7564 2d73 746f 7261 6765 0d0a 096d  loud-storage...m
+000002d0: 6174 706c 6f74 6c69 620d 0a09 6e75 6d70  atplotlib...nump
+000002e0: 790d 0a09 7061 6e64 6173 0d0a 0973 6561  y...pandas...sea
+000002f0: 626f 726e 0d0a 0973 656c 656e 6975 6d0d  born...selenium.
+00000300: 0a09 746f 6d6c 690d 0a0d 0a5b 6f70 7469  ..tomli....[opti
+00000310: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+00000320: 645d 0d0a 7768 6572 6520 3d20 7372 630d  d]..where = src.
+00000330: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+00000340: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+00000350: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

### Comparing `vicedtools-0.0.8.1/setup.py` & `vicedtools-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/__init__.py` & `vicedtools-0.0.9/src/vicedtools/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/__init__.py` & `vicedtools-0.0.9/src/vicedtools/acer/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/ewritesittings.py` & `vicedtools-0.0.9/src/vicedtools/acer/ewritesittings.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/extraoarsauthenticators.py` & `vicedtools-0.0.9/src/vicedtools/acer/extraoarsauthenticators.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/oars.py` & `vicedtools-0.0.9/src/vicedtools/acer/oars.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/oarsauthenticators.py` & `vicedtools-0.0.9/src/vicedtools/acer/oarsauthenticators.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/oarscandidates.py` & `vicedtools-0.0.9/src/vicedtools/acer/oarscandidates.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/oarssession.py` & `vicedtools-0.0.9/src/vicedtools/acer/oarssession.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/oarstests.py` & `vicedtools-0.0.9/src/vicedtools/acer/oarstests.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/patitems.py` & `vicedtools-0.0.9/src/vicedtools/acer/patitems.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/patresults.py` & `vicedtools-0.0.9/src/vicedtools/acer/patresults.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/patsittings.py` & `vicedtools-0.0.9/src/vicedtools/acer/patsittings.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/acer/plots.py` & `vicedtools-0.0.9/src/vicedtools/acer/plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
             'Student v Question': A qualitative description of the relative
                 scale score of the students compared to the item. 
             'Response': 'A', 'B', 'C', 'D', 'E', or '✓'.
             'Percentage of responses': as float
     '''
     q_difficulty = pat_results.question_scales[question]
     if from_date and to_date:
-        rows = (pat_results.results["Completed"] >
-                from_date) & (pat_results.results["Completed"] < to_date)
+        rows = (pat_results.results["Completed"]
+                > from_date) & (pat_results.results["Completed"] < to_date)
         summary_df = pat_results.results.loc[rows, ["Scale", question]].copy()
     elif from_date:
         rows = (pat_results.results["Completed"] > from_date)
         summary_df = pat_results.results.loc[rows, ["Scale", question]].copy()
     elif to_date:
         rows = (pat_results.results["Completed"] < to_date)
         summary_df = pat_results.results.loc[rows, ["Scale", question]].copy()
```

### Comparing `vicedtools-0.0.8.1/src/vicedtools/compass/__init__.py` & `vicedtools-0.0.9/src/vicedtools/compass/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/compass/compassauthenticators.py` & `vicedtools-0.0.9/src/vicedtools/compass/compassauthenticators.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/compass/compasssession.py` & `vicedtools-0.0.9/src/vicedtools/compass/compasssession.py`

 * *Files 7% similar despite different names*

```diff
@@ -288,14 +288,55 @@
             url = f"https://{self.school_code}.compass.education/Services/FileDownload/CsvRequestHandler?type=37"
         else:
             url = f"https://{self.school_code}.compass.education/Services/FileDownload/CsvRequestHandler?type=38"
         r = self.get(url)
         with open(file_name, "wb") as f:
             f.write(r.content)
 
+    def export_student_custom_flags(self,
+                                    file_name: str = "student custom flags.csv"
+                                   ) -> None:
+        '''Exports student flags that have been added to Compass.
+
+        Note: Doesn't include flags imported through CASES.
+
+        Args:
+            file_name: The file path to save the csv export, including filename.
+        '''
+        url = f"https://{self.school_code}.compass.education/Services/FileDownload/CsvRequestHandler?type=17"
+        r = self.get(url)
+        with open(file_name, "wb") as f:
+            f.write(r.content)
+
+    def export_student_demographic_details(
+            self, file_name: str = "student custom flags.csv") -> None:
+        '''Exports student demographic details.
+
+        Args:
+            file_name: The file path to save the csv export, including filename.
+        '''
+        url = f"https://{self.school_code}.compass.education/Services/FileDownload/CsvRequestHandler?type=54"
+        r = self.get(url)
+        with open(file_name, "wb") as f:
+            f.write(r.content)
+
+    def export_parent_mailmerge(
+            self, file_name: str = "parent mailmerge.csv") -> None:
+        '''Exports each parent contact for use in mail merges.
+
+        The basic export includes student address, parent names and parent contact details.
+
+        Args:
+            file_name: The file path to save the csv export, including filename.
+        '''
+        url = f"https://{self.school_code}.compass.education/Services/FileDownload/CsvRequestHandler?type=24"
+        r = self.get(url)
+        with open(file_name, "wb") as f:
+            f.write(r.content)
+
     def export_student_household_information(
             self, file_name: str = "student household information.csv") -> None:
         '''Exports student household information from Compass.
 
         The basic export includes student address, parent names and parent contact details.
 
         Args:
@@ -437,13 +478,28 @@
             for enrolment in new_enrolments:
                 enrolment.update({"activity_id": activity_id})
 
         del self.headers['Content-Type']
 
         return new_enrolments
 
+    def export_attendance_cases_halfday(self,
+                                        start_date: str,
+                                        finish_date: str,
+                                        save_dir: str,
+                                        included_exited: bool = True):
+        """Exports attendance data in the CASES half-day csv format.
+        
+        Args:
+            start_date: The start date for the export as yyyy-mm-dd
+            finish_date: The finish date for the export as yyyy-mm-dd
+            save_dir: The folder to save the export into.
+        """
+        payload = f'{{"type":"5","parameters":"{{\\"reportName\\":\\"cases21HalfDayCsv\\",\\"filename\\":\\"CASES21_HalfDay.csv\\",\\"startDateIn\\":\\"{start_date}T13:00:00.000Z\\",\\"finishDateIn\\":\\"{finish_date}T13:00:00.000Z\\",\\"includeExitedStudents\\":{str(included_exited).lower()},\\"minimumAbsentDays\\":\\"\\",\\"includeOverSixteens\\":true,\\"includePLCStudents\\":true,\\"yearLevelId\\":\\"\\",\\"campuses\\":\\"\\",\\"semester\\":\\"1\\",\\"collection\\":\\"Semester 1\\",\\"modifiedSinceDateIn\\":null,\\"userIds\\":\\"19311\\",\\"yearLevels\\":\\"7|8|9|10\\",\\"startDatePickerAttendanceByDayReport\\":\\"2023-05-19T14:00:00.000Z\\",\\"exportDatePickerFullSchoolAuditRollReport\\":\\"2023-05-19T14:00:00.000Z\\",\\"teachingDaysNumber\\":\\"8\\",\\"includeComments\\":true,\\"yearLevelsPreSchool\\":\\"\\",\\"yearLevelsPrimary\\":\\"\\",\\"yearLevelsMiddle\\":\\"\\",\\"yearLevelsSenior\\":\\"\\",\\"groupBy\\":null,\\"ethnicities\\":\\"\\",\\"yearLevelIds\\":\\"\\",\"formGroups\\":\\"\\"}}"}}'
+        self.long_running_file_request(payload, save_dir)
+
 
 def get_report_cycle_id(cycles, year, name):
     for c in cycles:
         if c['year'] == year and c['name'] == name:
             return c['id']
     return None
```

### Comparing `vicedtools-0.0.8.1/src/vicedtools/compass/extraauthenticators.py` & `vicedtools-0.0.9/src/vicedtools/compass/extraauthenticators.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/compass/reports.py` & `vicedtools-0.0.9/src/vicedtools/compass/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,34 +407,37 @@
         self.data = pd.merge(self.data[reports_columns],
                              classes_df[classes_columns],
                              how="left",
                              on=["ClassCode", "Year"])
         if replace_values:
             self.data.replace(replace_values, inplace=True)
         self.data.drop(columns="Year", inplace=True)
+        # Force learning area names to all caps
+        self.data['LearningArea'] = self.data['LearningArea'].str.upper()
 
     def updateFromClassDetails(self) -> None:
         """Infills TeacherCode data with data available from other reports."""
 
         self.data.drop(columns="TeacherCode", inplace=True, errors="ignore")
         self.data = pd.merge(self.data,
                              self.class_details,
                              how="left",
                              on=["Time", "ClassCode"])
 
     def summary(self) -> pd.DataFrame:
         """Aggregates Academic and Work Habits results to produce a summary."""
-        columns = ['Time', 'ClassCode', 'StudentCode',
-       'ResultScore', 'Type', 'LearningArea', 'SubjectCode',
-       'SubjectName', 'TeacherCode']
+        columns = [
+            'Time', 'ClassCode', 'StudentCode', 'ResultScore', 'Type',
+            'LearningArea', 'SubjectCode', 'SubjectName', 'TeacherCode'
+        ]
         grpd = self.data[columns].groupby([
             'Time', 'ClassCode', 'StudentCode', 'Type', 'SubjectCode',
             'SubjectName', 'LearningArea', 'TeacherCode'
         ],
-                                 as_index=False).mean()
+                                          as_index=False).mean()
         pvtd = grpd.pivot_table(index=[
             'Time', 'ClassCode', 'StudentCode', 'SubjectCode', 'SubjectName',
             'LearningArea', 'TeacherCode'
         ],
                                 columns=["Type"],
                                 values="ResultScore").reset_index()
         pvtd.sort_values("Time", ascending=False, inplace=True)
```

### Comparing `vicedtools-0.0.8.1/src/vicedtools/educationperfect.py` & `vicedtools-0.0.9/src/vicedtools/educationperfect.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/gcp/__init__.py` & `vicedtools-0.0.9/src/vicedtools/gcp/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 from vicedtools.gcp.api import upload_csv_to_bigquery
 from vicedtools.gcp.format import create_student_details_gc_csv
 from vicedtools.gcp.schema import (
     STUDENT_DETAILS_SCHEMA, STUDENT_DETAILS_CLUSTERING_FIELDS,
     STUDENT_ENROLMENTS_SCHEMA, STUDENT_ENROLMENTS_CLUSTERING_FIELDS,
     REPORTS_SCHEMA, REPORTS_CLUSTERING_FIELDS, REPORTS_SUMMARY_SCHEMA,
     REPORTS_SUMMARY_CLUSTERING_FIELDS, NAPLAN_OUTCOMES_SCHEMA,
-    NAPLAN_OUTCOMES_CLUSTERING_FIELDS, GAT_SCHEMA, GAT_CLUSTERING_FIELDS,
-    PAT_SCORES_SCHEMA, PAT_SCORES_CLUSTERING_FIELDS, PAT_MOST_RECENT_SCHEMA,
-    PAT_MOST_RECENT_CLUSTERING_FIELDS, EWRITE_SCORES_SCHEMA,
-    EWRITE_SCORES_CLUSTERING_FIELDS, EWRITE_CRITERIA_SCHEMA,
-    EWRITE_CRITERIA_CLUSTERING_FIELDS)
+    NAPLAN_OUTCOMES_CLUSTERING_FIELDS, 
+    NAPLAN_OUTCOMES_MOST_RECENT_CLUSTERING_FIELDS, GAT_SCHEMA, 
+    GAT_CLUSTERING_FIELDS, PAT_SCORES_SCHEMA, PAT_SCORES_CLUSTERING_FIELDS, 
+    PAT_MOST_RECENT_SCHEMA, PAT_MOST_RECENT_CLUSTERING_FIELDS, 
+    EWRITE_SCORES_SCHEMA, EWRITE_SCORES_CLUSTERING_FIELDS, 
+    EWRITE_CRITERIA_SCHEMA, EWRITE_CRITERIA_CLUSTERING_FIELDS)
```

### Comparing `vicedtools-0.0.8.1/src/vicedtools/gcp/api.py` & `vicedtools-0.0.9/src/vicedtools/gcp/api.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/gcp/format.py` & `vicedtools-0.0.9/src/vicedtools/gcp/format.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/gcp/schema.py` & `vicedtools-0.0.9/src/vicedtools/gcp/schema.py`

 * *Files 19% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     bigquery.SchemaField("DateOfBirth", "DATE")
 ]
 STUDENT_DETAILS_CLUSTERING_FIELDS = [
     "Status", "StudentCode", "YearLevel", "Gender"
 ]
 
 STUDENT_ENROLMENTS_SCHEMA = [
-    bigquery.SchemaField("ClassCode", "STRING"),
+    bigquery.SchemaField("EnrolmentClassCode", "STRING"),
     bigquery.SchemaField("StudentCode", "STRING")
 ]
 
-STUDENT_ENROLMENTS_CLUSTERING_FIELDS = ["ClassCode", "StudentCode"]
+STUDENT_ENROLMENTS_CLUSTERING_FIELDS = ["EnrolmentClassCode", "StudentCode"]
 
 REPORTS_SCHEMA = [
     bigquery.SchemaField("Time", "DATE"),
     bigquery.SchemaField("ClassCode", "STRING"),
     bigquery.SchemaField("StudentCode", "STRING"),
     bigquery.SchemaField("ResultName", "STRING"),
     bigquery.SchemaField("ResultGrade", "STRING"),
@@ -65,33 +65,48 @@
 REPORTS_SUMMARY_CLUSTERING_FIELDS = [
     "StudentCode", "Time", "LearningArea", "TeacherCode"
 ]
 
 NAPLAN_OUTCOMES_SCHEMA = [
     bigquery.SchemaField("APS_Year", "STRING"),
     bigquery.SchemaField("Reporting_Test", "STRING"),
+    bigquery.SchemaField("Cases_ID", "STRING"),
     bigquery.SchemaField("First_Name", "STRING"),
     bigquery.SchemaField("Second_Name", "STRING"),
     bigquery.SchemaField("Surname", "STRING"),
     bigquery.SchemaField("READING_nb", "FLOAT"),
+    bigquery.SchemaField("READING_band", "INTEGER"),
+    bigquery.SchemaField("READING_toptwo", "BOOLEAN"),
+    bigquery.SchemaField("READING_bottomtwo", "BOOLEAN"),
     bigquery.SchemaField("WRITING_nb", "FLOAT"),
+    bigquery.SchemaField("WRITING_band", "INTEGER"),
+    bigquery.SchemaField("WRITING_toptwo", "BOOLEAN"),
+    bigquery.SchemaField("WRITING_bottomtwo", "BOOLEAN"),
     bigquery.SchemaField("SPELLING_nb", "FLOAT"),
+    bigquery.SchemaField("SPELLING_band", "INTEGER"),
+    bigquery.SchemaField("SPELLING_toptwo", "BOOLEAN"),
+    bigquery.SchemaField("SPELLING_bottomtwo", "BOOLEAN"),
     bigquery.SchemaField("NUMERACY_nb", "FLOAT"),
+    bigquery.SchemaField("NUMERACY_band", "INTEGER"),
+    bigquery.SchemaField("NUMERACY_toptwo", "BOOLEAN"),
+    bigquery.SchemaField("NUMERACY_bottomtwo", "BOOLEAN"),
     bigquery.SchemaField("GRAMMAR___PUNCTUATION_nb", "FLOAT"),
-    bigquery.SchemaField("Class", "STRING"),
-    bigquery.SchemaField("Date_of_Birth", "STRING"),
-    bigquery.SchemaField("Gender", "STRING"),
-    bigquery.SchemaField("LBOTE", "BOOLEAN"),
-    bigquery.SchemaField("ATSI", "BOOLEAN"),
-    bigquery.SchemaField("Home_School_Name", "STRING"),
-    bigquery.SchemaField("Reporting_School_Name", "STRING"),
-    bigquery.SchemaField("Cases_ID", "STRING"),
+    bigquery.SchemaField("GRAMMAR___PUNCTUATION_band", "INTEGER"),
+    bigquery.SchemaField("GRAMMAR___PUNCTUATION_toptwo", "BOOLEAN"),
+    bigquery.SchemaField("GRAMMAR___PUNCTUATION_bottomtwo", "BOOLEAN"),
 ]
+
 NAPLAN_OUTCOMES_CLUSTERING_FIELDS = [
-    "APS_Year", "Reporting_Test", "Cases_ID", "Gender"
+    "APS_Year",
+    "Reporting_Test",
+    "Cases_ID",
+]
+
+NAPLAN_OUTCOMES_MOST_RECENT_CLUSTERING_FIELDS = [
+    "Cases_ID",
 ]
 
 GAT_SCHEMA = [
     bigquery.SchemaField("Year", "STRING"),
     bigquery.SchemaField("candNum", "STRING"),
     bigquery.SchemaField("Student_Name", "STRING"),
     bigquery.SchemaField("incomplete", "BOOLEAN"),
```

### Comparing `vicedtools-0.0.8.1/src/vicedtools/naplan/__init__.py` & `vicedtools-0.0.9/src/vicedtools/naplan/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/naplan/dataservicesession.py` & `vicedtools-0.0.9/src/vicedtools/naplan/dataservicesession.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/naplan/sssrdata.py` & `vicedtools-0.0.9/src/vicedtools/naplan/sssrdata.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/sportstrak.py` & `vicedtools-0.0.9/src/vicedtools/sportstrak.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/vce/__init__.py` & `vicedtools-0.0.9/src/vicedtools/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/vce/schoolscores.py` & `vicedtools-0.0.9/src/vicedtools/vce/schoolscores.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools/vce/vasssession.py` & `vicedtools-0.0.9/src/vicedtools/vce/vasssession.py`

 * *Files identical despite different names*

### Comparing `vicedtools-0.0.8.1/src/vicedtools.egg-info/PKG-INFO` & `vicedtools-0.0.9/src/vicedtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vicedtools
-Version: 0.0.8.1
+Version: 0.0.9
 Summary: A collection of tools for school data in Victorian schools.
 Home-page: https://github.com/gregbreese/vicedtools
 Author: Greg Breese
 Project-URL: Bug Tracker, https://github.com/gregbreese/vicedtools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `vicedtools-0.0.8.1/src/vicedtools.egg-info/entry_points.txt` & `vicedtools-0.0.9/src/vicedtools.egg-info/entry_points.txt`

 * *Files identical despite different names*

