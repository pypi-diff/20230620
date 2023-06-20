# Comparing `tmp/seeq-spy-188.2.tar.gz` & `tmp/seeq-spy-188.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeq-spy-188.2.tar", last modified: Tue Jun  6 19:49:37 2023, max compression
+gzip compressed data, was "seeq-spy-188.3.tar", last modified: Tue Jun 20 20:16:07 2023, max compression
```

## Comparing `seeq-spy-188.2.tar` & `seeq-spy-188.3.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.775716 seeq-spy-188.2/
--rw-rw-rw-   0        0        0    33551 2023-02-10 21:28:23.000000 seeq-spy-188.2/LICENSE
--rw-rw-rw-   0        0        0      207 2023-02-10 21:28:23.000000 seeq-spy-188.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4606 2023-06-06 19:49:37.775716 seeq-spy-188.2/PKG-INFO
--rw-rw-rw-   0        0        0     4091 2023-04-18 17:55:42.000000 seeq-spy-188.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.449722 seeq-spy-188.2/seeq/
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.477723 seeq-spy-188.2/seeq/base/
--rw-rw-rw-   0        0        0       36 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/__init__.py
--rw-rw-rw-   0        0        0      875 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/proputil.py
--rw-rw-rw-   0        0        0    32534 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/seeq_names.py
--rw-rw-rw-   0        0        0      157 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/system.py
--rw-rw-rw-   0        0        0     4788 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/base/util.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.481722 seeq-spy-188.2/seeq/scripts/
--rw-rw-rw-   0        0        0    12250 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/scripts/create_monitoring_alerts.py
--rw-rw-rw-   0        0        0    49636 2023-06-06 19:49:28.000000 seeq-spy-188.2/seeq/scripts/create_monitoring_workbook.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.530479 seeq-spy-188.2/seeq/spy/
--rw-rw-rw-   0        0        0     1953 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/__init__.py
--rw-rw-rw-   0        0        0    32016 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_common.py
--rw-rw-rw-   0        0        0     4687 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_config.py
--rw-rw-rw-   0        0        0     4424 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_datalab.py
--rw-rw-rw-   0        0        0     9914 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_errors.py
--rw-rw-rw-   0        0        0    49041 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_login.py
--rw-rw-rw-   0        0        0    92226 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_metadata.py
--rw-rw-rw-   0        0        0     5822 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_metadata_push_results.py
--rw-rw-rw-   0        0        0     2954 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_plot.py
--rw-rw-rw-   0        0        0    55640 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_pull.py
--rw-rw-rw-   0        0        0    68835 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_push.py
--rw-rw-rw-   0        0        0     5155 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_redaction.py
--rw-rw-rw-   0        0        0    44741 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_search.py
--rw-rw-rw-   0        0        0    20309 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_session.py
--rw-rw-rw-   0        0        0    16507 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_status.py
--rw-rw-rw-   0        0        0    20657 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_swap.py
--rw-rw-rw-   0        0        0     3471 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_upgrade.py
--rw-rw-rw-   0        0        0    10707 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/_url.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.540480 seeq-spy-188.2/seeq/spy/acl/
--rw-rw-rw-   0        0        0      104 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/acl/__init__.py
--rw-rw-rw-   0        0        0    12172 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/acl/_pull.py
--rw-rw-rw-   0        0        0    11351 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/acl/_push.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.558480 seeq-spy-188.2/seeq/spy/addons/
--rw-rw-rw-   0        0        0      188 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/__init__.py
--rw-rw-rw-   0        0        0    26376 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/_install.py
--rw-rw-rw-   0        0        0     2408 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/_permissions.py
--rw-rw-rw-   0        0        0    12137 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/_search.py
--rw-rw-rw-   0        0        0     5334 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/addons/_uninstall.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.572480 seeq-spy-188.2/seeq/spy/assets/
--rw-rw-rw-   0        0        0      336 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/__init__.py
--rw-rw-rw-   0        0        0     3638 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/_brochure.py
--rw-rw-rw-   0        0        0    12419 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/_build.py
--rw-rw-rw-   0        0        0     3133 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/_context.py
--rw-rw-rw-   0        0        0    48189 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/_model.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.594478 seeq-spy-188.2/seeq/spy/assets/_trees/
--rw-rw-rw-   0        0        0       69 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/__init__.py
--rw-rw-rw-   0        0        0     1375 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_constants.py
--rw-rw-rw-   0        0        0     7325 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_csv.py
--rw-rw-rw-   0        0        0    22068 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_match.py
--rw-rw-rw-   0        0        0     2629 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_pandas.py
--rw-rw-rw-   0        0        0     6458 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_path.py
--rw-rw-rw-   0        0        0    23208 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_properties.py
--rw-rw-rw-   0        0        0    13381 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_pull.py
--rw-rw-rw-   0        0        0    58791 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_tree.py
--rw-rw-rw-   0        0        0     5897 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_utils.py
--rw-rw-rw-   0        0        0    25525 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/assets/_trees/_validate.py
--rw-rw-rw-   0        0        0     2538 2023-06-06 19:49:29.000000 seeq-spy-188.2/seeq/spy/assets/brochure.html
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.598480 seeq-spy-188.2/seeq/spy/docs/
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.637479 seeq-spy-188.2/seeq/spy/docs/Documentation/
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.639477 seeq-spy-188.2/seeq/spy/docs/Documentation/Administration/
--rw-rw-rw-   0        0        0     6577 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.651479 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/
--rw-rw-rw-   0        0        0    17428 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
--rw-rw-rw-   0        0        0    33412 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
--rw-rw-rw-   0        0        0    16700 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
--rw-rw-rw-   0        0        0     8406 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
--rw-rw-rw-   0        0        0    38889 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
--rw-rw-rw-   0        0        0      870 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
--rw-rw-rw-   0        0        0   186560 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
--rw-rw-rw-   0        0        0   239024 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
--rw-rw-rw-   0        0        0   229026 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
--rw-rw-rw-   0        0        0    24627 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.665478 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/
--rw-rw-rw-   0        0        0   135771 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
--rw-rw-rw-   0        0        0   152116 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
--rw-rw-rw-   0        0        0   207271 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
--rw-rw-rw-   0        0        0      325 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/Readme.txt
--rw-rw-rw-   0        0        0   141516 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
--rw-rw-rw-   0        0        0   439966 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
--rw-rw-rw-   0        0        0   189377 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
--rw-rw-rw-   0        0        0    15177 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Command Reference.ipynb
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.679478 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/
--rw-rw-rw-   0        0        0    94677 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Example Export.zip
--rw-rw-rw-   0        0        0   111771 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
--rw-rw-rw-   0        0        0   113084 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
--rw-rw-rw-   0        0        0  1083835 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
--rw-rw-rw-   0        0        0      429 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
--rw-rw-rw-   0        0        0   674467 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Tutorial.ipynb
--rw-rw-rw-   0        0        0    11595 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Version Considerations.ipynb
--rw-rw-rw-   0        0        0  1557151 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/Workbook Templates.ipynb
--rw-rw-rw-   0        0        0    54071 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.acl.ipynb
--rw-rw-rw-   0        0        0    11195 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.jobs.ipynb
--rw-rw-rw-   0        0        0    13015 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.login.ipynb
--rw-rw-rw-   0        0        0   128103 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.pull.ipynb
--rw-rw-rw-   0        0        0    99541 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.push.ipynb
--rw-rw-rw-   0        0        0    57289 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.search.ipynb
--rw-rw-rw-   0        0        0    95777 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.swap.ipynb
--rw-rw-rw-   0        0        0    10829 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.widgets.ipynb
--rw-rw-rw-   0        0        0    69828 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/Documentation/spy.workbooks.ipynb
--rw-rw-rw-   0        0        0       60 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/__init__.py
--rw-rw-rw-   0        0        0     1704 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/docs/_copy.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.688481 seeq-spy-188.2/seeq/spy/jobs/
--rw-rw-rw-   0        0        0      491 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/__init__.py
--rw-rw-rw-   0        0        0     9869 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/_execute.py
--rw-rw-rw-   0        0        0     6111 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/_pull.py
--rw-rw-rw-   0        0        0     9398 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/_push.py
--rw-rw-rw-   0        0        0    25737 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/jobs/_schedule.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.692479 seeq-spy-188.2/seeq/spy/notifications/
--rw-rw-rw-   0        0        0      153 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/notifications/__init__.py
--rw-rw-rw-   0        0        0    11927 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/notifications/_emails.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.694723 seeq-spy-188.2/seeq/spy/utils/
--rw-rw-rw-   0        0        0     1569 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.701716 seeq-spy-188.2/seeq/spy/widgets/
--rw-rw-rw-   0        0        0      200 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/widgets/__init__.py
--rw-rw-rw-   0        0        0     4158 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/widgets/_ipy_utils.py
--rw-rw-rw-   0        0        0    30480 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/widgets/_widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.759717 seeq-spy-188.2/seeq/spy/workbooks/
--rw-rw-rw-   0        0        0     3012 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/__init__.py
--rw-rw-rw-   0        0        0    43729 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_annotation.py
--rw-rw-rw-   0        0        0    34087 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_content.py
--rw-rw-rw-   0        0        0    40974 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_data.py
--rw-rw-rw-   0        0        0     6639 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_folder.py
--rw-rw-rw-   0        0        0    14611 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_item.py
--rw-rw-rw-   0        0        0     5448 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_item_map.py
--rw-rw-rw-   0        0        0     3033 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_load.py
--rw-rw-rw-   0        0        0     3456 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_mustache.py
--rw-rw-rw-   0        0        0    14175 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_pull.py
--rw-rw-rw-   0        0        0    23088 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_push.py
--rw-rw-rw-   0        0        0     6316 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_render.py
--rw-rw-rw-   0        0        0    27127 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_report_content_utilities.py
--rw-rw-rw-   0        0        0     4729 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_save.py
--rw-rw-rw-   0        0        0    15545 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_search.py
--rw-rw-rw-   0        0        0    37445 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_template.py
--rw-rw-rw-   0        0        0    11995 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_user.py
--rw-rw-rw-   0        0        0    52462 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_workbook.py
--rw-rw-rw-   0        0        0    48819 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_worksheet.py
--rw-rw-rw-   0        0        0    51518 2023-06-06 19:49:31.000000 seeq-spy-188.2/seeq/spy/workbooks/_workstep.py
--rw-rw-rw-   0        0        0   427362 2023-06-06 19:49:30.000000 seeq-spy-188.2/seeq/spy/workbooks/app.css
-drwxrwxrwx   0        0        0        0 2023-06-06 19:49:37.773716 seeq-spy-188.2/seeq_spy.egg-info/
--rw-rw-rw-   0        0        0     4606 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4785 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-26 16:53:37.000000 seeq-spy-188.2/seeq_spy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      311 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-06 19:49:37.000000 seeq-spy-188.2/seeq_spy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-06 19:49:37.776716 seeq-spy-188.2/setup.cfg
--rw-rw-rw-   0        0        0     1677 2023-06-06 19:45:32.000000 seeq-spy-188.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.508319 seeq-spy-188.3/
+-rw-rw-rw-   0        0        0    33551 2023-02-10 21:28:23.000000 seeq-spy-188.3/LICENSE
+-rw-rw-rw-   0        0        0      207 2023-02-10 21:28:23.000000 seeq-spy-188.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4606 2023-06-20 20:16:07.507318 seeq-spy-188.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4091 2023-04-18 17:55:42.000000 seeq-spy-188.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.329321 seeq-spy-188.3/seeq/
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.346319 seeq-spy-188.3/seeq/base/
+-rw-rw-rw-   0        0        0       36 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/__init__.py
+-rw-rw-rw-   0        0        0      875 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/proputil.py
+-rw-rw-rw-   0        0        0    32535 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/seeq_names.py
+-rw-rw-rw-   0        0        0      157 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/system.py
+-rw-rw-rw-   0        0        0     4788 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/base/util.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.348318 seeq-spy-188.3/seeq/scripts/
+-rw-rw-rw-   0        0        0    12250 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/scripts/create_monitoring_alerts.py
+-rw-rw-rw-   0        0        0    49636 2023-06-20 20:16:02.000000 seeq-spy-188.3/seeq/scripts/create_monitoring_workbook.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.370318 seeq-spy-188.3/seeq/spy/
+-rw-rw-rw-   0        0        0     1953 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/__init__.py
+-rw-rw-rw-   0        0        0    32016 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_common.py
+-rw-rw-rw-   0        0        0     4687 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_config.py
+-rw-rw-rw-   0        0        0     4424 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_datalab.py
+-rw-rw-rw-   0        0        0     9914 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_errors.py
+-rw-rw-rw-   0        0        0    49041 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_login.py
+-rw-rw-rw-   0        0        0    94326 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_metadata.py
+-rw-rw-rw-   0        0        0     5822 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_metadata_push_results.py
+-rw-rw-rw-   0        0        0     2954 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_plot.py
+-rw-rw-rw-   0        0        0    55640 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_pull.py
+-rw-rw-rw-   0        0        0    68835 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_push.py
+-rw-rw-rw-   0        0        0     5155 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_redaction.py
+-rw-rw-rw-   0        0        0    44741 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_search.py
+-rw-rw-rw-   0        0        0    20309 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_session.py
+-rw-rw-rw-   0        0        0    16507 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_status.py
+-rw-rw-rw-   0        0        0    20657 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_swap.py
+-rw-rw-rw-   0        0        0     3471 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_upgrade.py
+-rw-rw-rw-   0        0        0    10707 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/_url.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.374318 seeq-spy-188.3/seeq/spy/acl/
+-rw-rw-rw-   0        0        0      104 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/acl/__init__.py
+-rw-rw-rw-   0        0        0    12172 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/acl/_pull.py
+-rw-rw-rw-   0        0        0    11351 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/acl/_push.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.380318 seeq-spy-188.3/seeq/spy/addons/
+-rw-rw-rw-   0        0        0      188 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/__init__.py
+-rw-rw-rw-   0        0        0    26376 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/_install.py
+-rw-rw-rw-   0        0        0     2408 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/_permissions.py
+-rw-rw-rw-   0        0        0    12137 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/_search.py
+-rw-rw-rw-   0        0        0     5334 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/addons/_uninstall.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.388318 seeq-spy-188.3/seeq/spy/assets/
+-rw-rw-rw-   0        0        0      336 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/__init__.py
+-rw-rw-rw-   0        0        0     3638 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_brochure.py
+-rw-rw-rw-   0        0        0    12419 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_build.py
+-rw-rw-rw-   0        0        0     3133 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_context.py
+-rw-rw-rw-   0        0        0    48189 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_model.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.401318 seeq-spy-188.3/seeq/spy/assets/_trees/
+-rw-rw-rw-   0        0        0       69 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/__init__.py
+-rw-rw-rw-   0        0        0     1375 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_constants.py
+-rw-rw-rw-   0        0        0     7325 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_csv.py
+-rw-rw-rw-   0        0        0    22068 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_match.py
+-rw-rw-rw-   0        0        0     2629 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_pandas.py
+-rw-rw-rw-   0        0        0     6458 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_path.py
+-rw-rw-rw-   0        0        0    23208 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_properties.py
+-rw-rw-rw-   0        0        0    13381 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_pull.py
+-rw-rw-rw-   0        0        0    58791 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_tree.py
+-rw-rw-rw-   0        0        0     5897 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_utils.py
+-rw-rw-rw-   0        0        0    25525 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/_trees/_validate.py
+-rw-rw-rw-   0        0        0     2538 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/assets/brochure.html
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.404318 seeq-spy-188.3/seeq/spy/docs/
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.429319 seeq-spy-188.3/seeq/spy/docs/Documentation/
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.430318 seeq-spy-188.3/seeq/spy/docs/Documentation/Administration/
+-rw-rw-rw-   0        0        0     6577 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Administration/User Migration.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.438318 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/
+-rw-rw-rw-   0        0        0    17428 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb
+-rw-rw-rw-   0        0        0    33412 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb
+-rw-rw-rw-   0        0        0    16700 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb
+-rw-rw-rw-   0        0        0     8406 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb
+-rw-rw-rw-   0        0        0    38889 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb
+-rw-rw-rw-   0        0        0      870 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg
+-rw-rw-rw-   0        0        0   186560 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb
+-rw-rw-rw-   0        0        0   239024 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb
+-rw-rw-rw-   0        0        0   229026 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb
+-rw-rw-rw-   0        0        0    24627 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.448319 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/
+-rw-rw-rw-   0        0        0   135771 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg
+-rw-rw-rw-   0        0        0   152116 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg
+-rw-rw-rw-   0        0        0   207271 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg
+-rw-rw-rw-   0        0        0      325 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/Readme.txt
+-rw-rw-rw-   0        0        0   141516 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png
+-rw-rw-rw-   0        0        0   439966 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png
+-rw-rw-rw-   0        0        0   189377 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png
+-rw-rw-rw-   0        0        0    15177 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Command Reference.ipynb
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.457319 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/
+-rw-rw-rw-   0        0        0    94677 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Example Export.zip
+-rw-rw-rw-   0        0        0   111771 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip
+-rw-rw-rw-   0        0        0   113084 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip
+-rw-rw-rw-   0        0        0  1083835 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv
+-rw-rw-rw-   0        0        0      429 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/spy_tree_example.csv
+-rw-rw-rw-   0        0        0   674467 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Tutorial.ipynb
+-rw-rw-rw-   0        0        0    11595 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Version Considerations.ipynb
+-rw-rw-rw-   0        0        0  1557151 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/Workbook Templates.ipynb
+-rw-rw-rw-   0        0        0    54071 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.acl.ipynb
+-rw-rw-rw-   0        0        0    11195 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.jobs.ipynb
+-rw-rw-rw-   0        0        0    13015 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.login.ipynb
+-rw-rw-rw-   0        0        0   128103 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.pull.ipynb
+-rw-rw-rw-   0        0        0    99541 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.push.ipynb
+-rw-rw-rw-   0        0        0    57289 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.search.ipynb
+-rw-rw-rw-   0        0        0    95777 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.swap.ipynb
+-rw-rw-rw-   0        0        0    10829 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.widgets.ipynb
+-rw-rw-rw-   0        0        0    69828 2023-06-20 20:16:03.000000 seeq-spy-188.3/seeq/spy/docs/Documentation/spy.workbooks.ipynb
+-rw-rw-rw-   0        0        0       60 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/__init__.py
+-rw-rw-rw-   0        0        0     1704 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/docs/_copy.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.463318 seeq-spy-188.3/seeq/spy/jobs/
+-rw-rw-rw-   0        0        0      491 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/__init__.py
+-rw-rw-rw-   0        0        0     9869 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/_execute.py
+-rw-rw-rw-   0        0        0     6111 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/_pull.py
+-rw-rw-rw-   0        0        0     9398 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/_push.py
+-rw-rw-rw-   0        0        0    25737 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/jobs/_schedule.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.466318 seeq-spy-188.3/seeq/spy/notifications/
+-rw-rw-rw-   0        0        0      153 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/notifications/__init__.py
+-rw-rw-rw-   0        0        0    11927 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/notifications/_emails.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.467318 seeq-spy-188.3/seeq/spy/utils/
+-rw-rw-rw-   0        0        0     1569 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.470317 seeq-spy-188.3/seeq/spy/widgets/
+-rw-rw-rw-   0        0        0      200 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/widgets/__init__.py
+-rw-rw-rw-   0        0        0     4158 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/widgets/_ipy_utils.py
+-rw-rw-rw-   0        0        0    30480 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/widgets/_widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.497318 seeq-spy-188.3/seeq/spy/workbooks/
+-rw-rw-rw-   0        0        0     3012 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/__init__.py
+-rw-rw-rw-   0        0        0    43729 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_annotation.py
+-rw-rw-rw-   0        0        0    34087 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_content.py
+-rw-rw-rw-   0        0        0    40974 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_data.py
+-rw-rw-rw-   0        0        0     6639 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_folder.py
+-rw-rw-rw-   0        0        0    14611 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_item.py
+-rw-rw-rw-   0        0        0     5448 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_item_map.py
+-rw-rw-rw-   0        0        0     3033 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_load.py
+-rw-rw-rw-   0        0        0     3456 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_mustache.py
+-rw-rw-rw-   0        0        0    14175 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_pull.py
+-rw-rw-rw-   0        0        0    23088 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_push.py
+-rw-rw-rw-   0        0        0     6316 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_render.py
+-rw-rw-rw-   0        0        0    27127 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_report_content_utilities.py
+-rw-rw-rw-   0        0        0     4729 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_save.py
+-rw-rw-rw-   0        0        0    15545 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_search.py
+-rw-rw-rw-   0        0        0    37445 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_template.py
+-rw-rw-rw-   0        0        0    11995 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_user.py
+-rw-rw-rw-   0        0        0    52462 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_workbook.py
+-rw-rw-rw-   0        0        0    48819 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_worksheet.py
+-rw-rw-rw-   0        0        0    51518 2023-06-20 20:16:05.000000 seeq-spy-188.3/seeq/spy/workbooks/_workstep.py
+-rw-rw-rw-   0        0        0   427362 2023-06-20 20:16:04.000000 seeq-spy-188.3/seeq/spy/workbooks/app.css
+drwxrwxrwx   0        0        0        0 2023-06-20 20:16:07.506319 seeq-spy-188.3/seeq_spy.egg-info/
+-rw-rw-rw-   0        0        0     4606 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4785 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-26 16:53:37.000000 seeq-spy-188.3/seeq_spy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      311 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-20 20:16:07.000000 seeq-spy-188.3/seeq_spy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 20:16:07.508319 seeq-spy-188.3/setup.cfg
+-rw-rw-rw-   0        0        0     1677 2023-06-20 19:50:26.000000 seeq-spy-188.3/setup.py
```

### Comparing `seeq-spy-188.2/LICENSE` & `seeq-spy-188.3/LICENSE`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/PKG-INFO` & `seeq-spy-188.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 188.2
+Version: 188.3
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-188.2/README.md` & `seeq-spy-188.3/README.md`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/base/proputil.py` & `seeq-spy-188.3/seeq/base/proputil.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/base/seeq_names.py` & `seeq-spy-188.3/seeq/base/seeq_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
         cyg_net = 'CygNet'
         example_data = 'Time Series CSV Files'
         add_on_calc_python = 'Add-on Calculation Python'
         add_on_calc_excel = 'Add-on Calculation Excel VBA'
         file_folders = 'FileFolders'
         g_e_proficy = 'GE Proficy'
         i_b_a_h_d = 'IbaHD'
+        ignition = 'Ignition Gateway'
         influx_d_b = 'InfluxDB'
         influx_d_b2 = 'InfluxDB 2'
         i_p21 = 'AspenTech IP21'
         met_net = 'MetNet'
         n_o_a_a_weather = 'NOAA Weather Service'
         omnia = 'Equinor Omnia Plant'
         o_p_c_h_d_a = 'OPC-HDA'
@@ -226,15 +227,14 @@
         system = 'System'
         import_ = 'Import'
         monitors = 'Monitors'
         projects = 'Projects'
         content = 'Content'
         report_templates = 'ReportTemplates'
         condition_monitors = 'ConditionMonitors'
-        item_finders = 'ItemFinders'
         plugins = 'Plugins'
         displays = 'Displays'
         display_templates = 'DisplayTemplates'
         notification_configurations = 'NotificationConfigurations'
         label = 'Label'
         context = 'Context'
         table_definitions = 'TableDefinitions'
```

### Comparing `seeq-spy-188.2/seeq/base/util.py` & `seeq-spy-188.3/seeq/base/util.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/scripts/create_monitoring_alerts.py` & `seeq-spy-188.3/seeq/scripts/create_monitoring_alerts.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/scripts/create_monitoring_workbook.py` & `seeq-spy-188.3/seeq/scripts/create_monitoring_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/__init__.py` & `seeq-spy-188.3/seeq/spy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
 """
 
 __all__ = ['acl', 'addons', 'assets', 'docs', 'workbooks', 'widgets', 'login', 'logout', 'plot', 'pull', 'push',
            'search', 'swap', 'PATH_ROOT', 'DEFAULT_WORKBOOK_PATH', 'GLOBALS_ONLY', 'GLOBALS_AND_ALL_WORKBOOKS',
            'INHERIT_FROM_WORKBOOK', 'Session', 'Status', 'options', 'session', 'client', 'user', 'server_version',
            'jobs', 'notifications', 'upgrade', 'utils', 'errors']
 
-__version__ = '%d.%d' % (int('188'), int('2'))
+__version__ = '%d.%d' % (int('188'), int('3'))
```

### Comparing `seeq-spy-188.2/seeq/spy/_common.py` & `seeq-spy-188.3/seeq/spy/_common.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_config.py` & `seeq-spy-188.3/seeq/spy/_config.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_datalab.py` & `seeq-spy-188.3/seeq/spy/_datalab.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_errors.py` & `seeq-spy-188.3/seeq/spy/_errors.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_login.py` & `seeq-spy-188.3/seeq/spy/_login.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_metadata.py` & `seeq-spy-188.3/seeq/spy/_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
 import json
 import os
 import re
 from dataclasses import dataclass
-from typing import Callable, Dict, Optional, List, Tuple, Set
+from typing import Callable, Dict, Optional, List, Tuple, Set, Union
 
 import numpy as np
 import pandas as pd
+
 from seeq.base.seeq_names import SeeqNames
 from seeq.sdk import *
 from seeq.spy import _common, _login
 from seeq.spy._common import EMPTY_GUID
 from seeq.spy._errors import *
 from seeq.spy._metadata_push_results import PushResults
 from seeq.spy._push import WorkbookContext
@@ -489,17 +490,17 @@
                     threshold_metric_input.measured_item, push_context.workbook_context.workbook_id,
                     push_context.push_results)
             if threshold_metric_input.bounding_condition:
                 threshold_metric_input.bounding_condition = _item_id_from_parameter_value(
                     threshold_metric_input.bounding_condition, push_context.workbook_context.workbook_id,
                     push_context.push_results)
 
-            threshold_metric_input.thresholds = _convert_thresholds_dict_to_input(
+            threshold_metric_input.thresholds = _convert_thresholds_to_input(
                 threshold_metric_input.thresholds, push_context.workbook_context.workbook_id,
-                push_context.push_results)
+                push_context.push_results, row_dict)
 
             if _common.present(row_dict, 'Statistic'):
                 threshold_metric_input.aggregation_function = _common.statistic_to_aggregation_function(
                     row_dict['Statistic'])
                 push_context.push_results.at[
                     index, 'Aggregation Function'] = threshold_metric_input.aggregation_function
 
@@ -1513,38 +1514,14 @@
         else:
             item_push_output = create_item_endpoint(body=item_input)
         _set_push_result_string__from_post_loop(item_input.dataframe_index, item_push_output, status, push_results)
 
     item_inputs.clear()
 
 
-def _convert_thresholds_dict_to_input(thresholds_dict, workbook_id, push_results: PushResults):
-    """
-    Convert a dictionary with keys threshold levels and values of either scalars or metadata to a list of strings
-    with level=value/ID of the threshold.
-
-    :param thresholds_dict: A dictionary with keys of threshold levels and values of either number of metadata
-    dataframes
-    :return:  A list of strings 'level=value' or 'level=ID'
-    """
-    thresholds_list = list()
-    if thresholds_dict is not None:
-        if not isinstance(thresholds_dict, dict):
-            raise SPyTypeError(f'"Thresholds" value for Metric should be dict, but instead is type '
-                               f'{type(thresholds_dict).__name__} with value:\n{thresholds_dict}')
-
-        for k, v in thresholds_dict.items():
-            if isinstance(v, pd.DataFrame) or isinstance(v, dict):
-                thresholds_list.append(
-                    f'{k}={_item_id_from_parameter_value(v, workbook_id, push_results)}')
-            else:
-                thresholds_list.append(f'{k}={v}')
-    return thresholds_list
-
-
 def _add_no_dupe(lst, obj, attr='data_id', overwrite=False):
     for i in range(0, len(lst)):
         o = lst[i]
         if hasattr(o, attr):
             if getattr(o, attr) == getattr(obj, attr):
                 if overwrite:
                     lst[i] = obj
@@ -1832,14 +1809,87 @@
 
     if metric.thresholds:
         _add_thresholds('Thresholds', metric.thresholds)
 
     return formula_parameters
 
 
+def _get_threshold_level(threshold_entry: dict) -> str:
+    """
+    :param threshold_entry: A dictionary of a single Threshold, like Appserver outputs, which includes the
+    Priority (Name + Level + optional Color) and a Value (either a Scalar or ID).
+    :return: The Level as a string. Includes the numeric Level value plus the optional Color.
+    """
+    return '{}{}'.format(threshold_entry['Priority']['Level'],
+                         # A custom color can be specified for the threshold by appending it to the priority
+                         # number as a hex code. Example: '1#00ff00=10'
+                         threshold_entry['Priority']['Color'] if 'Color' in threshold_entry['Priority'] else '')
+
+
+def _get_threshold_value(threshold_entry: dict, item_map: Optional[dict] = None, current_item=None) -> Optional[str]:
+    """
+    :param threshold_entry: A dictionary of a single Threshold, like Appserver outputs, which includes the
+    Priority (Name + Level + optional Color) and a Value (either a Scalar or ID).
+    :param item_map: The optional map of old:new items being mapped to translate the specified ID.
+    :param current_item: The current item being pushed, just used for outputting errors.
+    :return: The value (scalar value or ID) of a single threshold entry.
+    """
+    _threshold_value = _common.get(threshold_entry, 'Value')
+    if _threshold_value is not None:
+        if isinstance(_threshold_value, dict):
+            return str_from_scalar_value_dict(_threshold_value)
+        else:
+            return _threshold_value
+    elif _common.present(threshold_entry, 'Item ID'):
+        if item_map is None:
+            return threshold_entry['Item ID']
+        if threshold_entry['Item ID'] not in item_map:
+            raise SPyDependencyNotFound(
+                f'{current_item} Threshold Metric threshold {threshold_entry["Item ID"]}) not found')
+
+
+def _convert_thresholds_to_input(thresholds_obj: Union[dict[str, any], list[Union[str, dict]]],
+                                 workbook_id: str, push_results: PushResults, current_item) -> list[str]:
+    """
+    Convert a dictionary with keys threshold levels and values of either scalars or metadata to a list of strings
+    with level=value/ID of the threshold.
+
+    :param thresholds_obj: Either a dictionary with keys of threshold levels and values of either number of metadata
+    dataframes or a list of threshold dictionaries like what Appserver returns.
+    :param workbook_id: The ID of the workbook being pushed. Used for looking up mapped item IDs.
+    :param push_results: The total push results. Used for looking up mapped item IDs.
+    :param current_item: The current item being pushed, just used for outputting errors.
+    :return: A list of strings 'level[#optional_color]=value' or 'level[#optional_color]=ID'
+    """
+    thresholds_list = list()
+    if thresholds_obj is None:
+        return thresholds_list
+
+    if isinstance(thresholds_obj, dict):
+        thresholds_dict = thresholds_obj
+    elif isinstance(thresholds_obj, list):
+        thresholds_dict = dict()
+        for threshold_entry in thresholds_obj:
+            level = _get_threshold_level(threshold_entry)
+            value = _get_threshold_value(threshold_entry, None, current_item)
+            if level and value:
+                thresholds_dict[level] = value
+    else:
+        raise SPyTypeError(f'{current_item} Threshold Metric "Thresholds" value should be dict or list, '
+                           f'but instead is type {type(thresholds_obj).__name__} with value:\n{thresholds_obj}')
+
+    for k, v in thresholds_dict.items():
+        threshold = f'{k}={_item_id_from_parameter_value(v, workbook_id, push_results)}' \
+            if isinstance(v, pd.DataFrame) or isinstance(v, dict) \
+            else f'{k}={v}'
+        thresholds_list.append(threshold)
+
+    return thresholds_list
+
+
 def threshold_metric_input_from_formula_parameters(parameters, *, item_object=None,
                                                    item_map=None) -> ThresholdMetricInputV1:
     new_item = ThresholdMetricInputV1()
 
     def _add_scalar_value(_attr, _key):
         if _common.present(parameters, _key):
             setattr(new_item, _attr, str_from_scalar_value_dict(parameters[_key]))
@@ -1852,46 +1902,32 @@
 
             if parameters[_key] not in item_map:
                 raise SPyDependencyNotFound(
                     f'{item_object} Threshold Metric parameter {_key} ({parameters[_key]}) not found')
 
             setattr(new_item, _attr, item_map[parameters[_key].upper()])
 
-    def _add_thresholds(_list, _key):
-        if not _common.present(parameters, _key):
-            return
-
-        for threshold_dict in parameters[_key]:
-            threshold_value = _common.get(threshold_dict, 'Value')
-            if threshold_value is not None:
-                if isinstance(threshold_value, dict):
-                    _list.append('%s=%s' % (threshold_dict['Priority']['Level'],
-                                            str_from_scalar_value_dict(threshold_value)))
-                else:
-                    _list.append('%s=%s' % (threshold_dict['Priority']['Level'], threshold_value))
-            elif _common.present(threshold_dict, 'Item ID'):
-                if item_map is None:
-                    _list.append('%s=%s' % (threshold_dict['Priority']['Level'], threshold_dict['Item ID']))
-                    return
-
-                if threshold_dict['Item ID'] not in item_map:
-                    raise SPyDependencyNotFound(
-                        f'{item_object} Threshold Metric threshold {threshold_dict["Item ID"]}) not found')
-
-                _list.append('%s=%s' % (threshold_dict['Priority']['Level'],
-                                        item_map[threshold_dict['Item ID']]))
+    def _get_thresholds() -> list[str]:
+        _thresholds_list = list()
+        if not _common.present(parameters, 'Thresholds'):
+            return _thresholds_list
+        for threshold_dict in parameters['Thresholds']:
+            level = _get_threshold_level(threshold_dict)
+            value = _get_threshold_value(threshold_dict, item_map, item_object)
+            if level and value:
+                _thresholds_list.append(f'{level}={value}')
+        return _thresholds_list
 
     new_item.aggregation_function = _common.get(parameters, 'Aggregation Function')
     _add_mapped_item('bounding_condition', 'Bounding Condition')
     _add_scalar_value('bounding_condition_maximum_duration', 'Bounding Condition Maximum Duration')
     _add_scalar_value('duration', 'Duration')
     _add_mapped_item('measured_item', 'Measured Item')
     _add_scalar_value('period', 'Period')
-    new_item.thresholds = list()
-    _add_thresholds(new_item.thresholds, 'Thresholds')
+    new_item.thresholds = _get_thresholds()
 
     return new_item
 
 
 RESERVED_SPY_STATUS_COLUMN_NAMES = [
     'Push Result', 'Push Count', 'Push Time',
     'Pull Result', 'Pull Count', 'Pull Time',
@@ -1943,11 +1979,12 @@
     SeeqNames.Properties.last_viewed_at
 ]
 
 ORIGINAL_INDEX_COLUMN = '__Original Index__'
 
 ADDITIONAL_RESERVED_PROPERTIES = [SeeqNames.Properties.scoped_to, SeeqNames.Properties.metadata_properties,
                                   SeeqNames.Properties.storage_location, SeeqNames.Properties.stored_in_seeq,
+                                  SeeqNames.Properties.aggregation_function,
                                   'Cached By Service', 'Data Version Check']
 
 IGNORED_PROPERTIES = (RESERVED_SPY_COLUMN_NAMES + RESERVED_ITEM_PROPERTIES + ADDITIONAL_RESERVED_PROPERTIES +
                       [ORIGINAL_INDEX_COLUMN])
```

### Comparing `seeq-spy-188.2/seeq/spy/_metadata_push_results.py` & `seeq-spy-188.3/seeq/spy/_metadata_push_results.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_plot.py` & `seeq-spy-188.3/seeq/spy/_plot.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_pull.py` & `seeq-spy-188.3/seeq/spy/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_push.py` & `seeq-spy-188.3/seeq/spy/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_redaction.py` & `seeq-spy-188.3/seeq/spy/_redaction.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_search.py` & `seeq-spy-188.3/seeq/spy/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_session.py` & `seeq-spy-188.3/seeq/spy/_session.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_status.py` & `seeq-spy-188.3/seeq/spy/_status.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_swap.py` & `seeq-spy-188.3/seeq/spy/_swap.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_upgrade.py` & `seeq-spy-188.3/seeq/spy/_upgrade.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/_url.py` & `seeq-spy-188.3/seeq/spy/_url.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/acl/_pull.py` & `seeq-spy-188.3/seeq/spy/acl/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/acl/_push.py` & `seeq-spy-188.3/seeq/spy/acl/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/addons/_install.py` & `seeq-spy-188.3/seeq/spy/addons/_install.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/addons/_permissions.py` & `seeq-spy-188.3/seeq/spy/addons/_permissions.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/addons/_search.py` & `seeq-spy-188.3/seeq/spy/addons/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/addons/_uninstall.py` & `seeq-spy-188.3/seeq/spy/addons/_uninstall.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_brochure.py` & `seeq-spy-188.3/seeq/spy/assets/_brochure.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_build.py` & `seeq-spy-188.3/seeq/spy/assets/_build.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_context.py` & `seeq-spy-188.3/seeq/spy/assets/_context.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_model.py` & `seeq-spy-188.3/seeq/spy/assets/_model.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_constants.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_constants.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_csv.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_csv.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_match.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_match.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_pandas.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_pandas.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_path.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_path.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_properties.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_properties.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_pull.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_tree.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_tree.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_utils.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/_trees/_validate.py` & `seeq-spy-188.3/seeq/spy/assets/_trees/_validate.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/assets/brochure.html` & `seeq-spy-188.3/seeq/spy/assets/brochure.html`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Administration/User Migration.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Administration/User Migration.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Add-on Installer.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notification Scheduler.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Notifier.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Email Unsubscriber.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Parameterized Jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Advanced Scheduling/Seeq Data Lab.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 1 - Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 2 - Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 3 - Report and Dashboard Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Asset Trees 4 - Accelerator Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot2.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/AnalysisTemplateScreenshot3.jpg`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/ReportAndDashboardTemplates1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot1.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Attached Images/TopicTemplateScreenshot2.png`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Command Reference.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Command Reference.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Example Export.zip` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Example Export.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Report and Dashboard Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/Workbook Templates.zip`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Support Files/csv_import_example.csv`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Tutorial.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Version Considerations.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Version Considerations.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/Workbook Templates.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/Workbook Templates.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.acl.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.acl.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.jobs.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.jobs.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.login.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.login.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.pull.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.pull.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.push.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.push.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.search.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.search.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.swap.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.swap.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.widgets.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.widgets.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/Documentation/spy.workbooks.ipynb` & `seeq-spy-188.3/seeq/spy/docs/Documentation/spy.workbooks.ipynb`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/docs/_copy.py` & `seeq-spy-188.3/seeq/spy/docs/_copy.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/jobs/_execute.py` & `seeq-spy-188.3/seeq/spy/jobs/_execute.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/jobs/_pull.py` & `seeq-spy-188.3/seeq/spy/jobs/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/jobs/_push.py` & `seeq-spy-188.3/seeq/spy/jobs/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/jobs/_schedule.py` & `seeq-spy-188.3/seeq/spy/jobs/_schedule.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/notifications/_emails.py` & `seeq-spy-188.3/seeq/spy/notifications/_emails.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/utils/__init__.py` & `seeq-spy-188.3/seeq/spy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/widgets/_ipy_utils.py` & `seeq-spy-188.3/seeq/spy/widgets/_ipy_utils.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/widgets/_widgets.py` & `seeq-spy-188.3/seeq/spy/widgets/_widgets.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/__init__.py` & `seeq-spy-188.3/seeq/spy/workbooks/__init__.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_annotation.py` & `seeq-spy-188.3/seeq/spy/workbooks/_annotation.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_content.py` & `seeq-spy-188.3/seeq/spy/workbooks/_content.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_data.py` & `seeq-spy-188.3/seeq/spy/workbooks/_data.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_folder.py` & `seeq-spy-188.3/seeq/spy/workbooks/_folder.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_item.py` & `seeq-spy-188.3/seeq/spy/workbooks/_item.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_item_map.py` & `seeq-spy-188.3/seeq/spy/workbooks/_item_map.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_load.py` & `seeq-spy-188.3/seeq/spy/workbooks/_load.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_mustache.py` & `seeq-spy-188.3/seeq/spy/workbooks/_mustache.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_pull.py` & `seeq-spy-188.3/seeq/spy/workbooks/_pull.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_push.py` & `seeq-spy-188.3/seeq/spy/workbooks/_push.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_render.py` & `seeq-spy-188.3/seeq/spy/workbooks/_render.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_report_content_utilities.py` & `seeq-spy-188.3/seeq/spy/workbooks/_report_content_utilities.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_save.py` & `seeq-spy-188.3/seeq/spy/workbooks/_save.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_search.py` & `seeq-spy-188.3/seeq/spy/workbooks/_search.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_template.py` & `seeq-spy-188.3/seeq/spy/workbooks/_template.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_user.py` & `seeq-spy-188.3/seeq/spy/workbooks/_user.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_workbook.py` & `seeq-spy-188.3/seeq/spy/workbooks/_workbook.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_worksheet.py` & `seeq-spy-188.3/seeq/spy/workbooks/_worksheet.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/_workstep.py` & `seeq-spy-188.3/seeq/spy/workbooks/_workstep.py`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq/spy/workbooks/app.css` & `seeq-spy-188.3/seeq/spy/workbooks/app.css`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/seeq_spy.egg-info/PKG-INFO` & `seeq-spy-188.3/seeq_spy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seeq-spy
-Version: 188.2
+Version: 188.3
 Summary: Easy-to-use Python interface for Seeq
 Home-page: https://www.seeq.com
 Author: Seeq Corporation
 Author-email: support@seeq.com
 Project-URL: Documentation, https://python-docs.seeq.com/
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `seeq-spy-188.2/seeq_spy.egg-info/SOURCES.txt` & `seeq-spy-188.3/seeq_spy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seeq-spy-188.2/setup.py` & `seeq-spy-188.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seeq-spy",
-    version="188.2",
+    version="188.3",
     author="Seeq Corporation",
     author_email="support@seeq.com",
     description="Easy-to-use Python interface for Seeq",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.seeq.com",
     project_urls={
```

