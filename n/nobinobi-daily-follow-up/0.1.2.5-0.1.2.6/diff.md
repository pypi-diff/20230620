# Comparing `tmp/nobinobi-daily-follow-up-0.1.2.5.tar.gz` & `tmp/nobinobi-daily-follow-up-0.1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobinobi-daily-follow-up-0.1.2.5.tar", last modified: Thu Jun 15 13:22:02 2023, max compression
+gzip compressed data, was "nobinobi-daily-follow-up-0.1.2.6.tar", last modified: Tue Jun 20 14:25:47 2023, max compression
```

## Comparing `nobinobi-daily-follow-up-0.1.2.5.tar` & `nobinobi-daily-follow-up-0.1.2.6.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.153694 nobinobi-daily-follow-up-0.1.2.5/
--rw-rw-rw-   0        0        0      166 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/AUTHORS.rst
--rw-rw-rw-   0        0        0     3491 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     4589 2023-06-15 13:21:22.000000 nobinobi-daily-follow-up-0.1.2.5/HISTORY.rst
--rw-rw-rw-   0        0        0    31999 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/LICENSE
--rw-rw-rw-   0        0        0      508 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     8347 2023-06-15 13:22:02.154726 nobinobi-daily-follow-up-0.1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     3016 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.848267 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/
--rw-rw-rw-   0        0        0      901 2023-06-15 13:21:22.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/__init__.py
--rw-rw-rw-   0        0        0     6644 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/admin.py
--rw-rw-rw-   0        0        0     2132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/apps.py
--rw-rw-rw-   0        0        0    24928 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/forms.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.758274 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.757757 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/en/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.855425 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0    36220 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.758274 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.890345 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0        0        0    17584 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0    43173 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     3840 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/menus.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.912077 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/
--rw-rw-rw-   0        0        0    21335 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0001_initial.py
--rw-rw-rw-   0        0        0    29811 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py
--rw-rw-rw-   0        0        0     1251 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py
--rw-rw-rw-   0        0        0      902 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py
--rw-rw-rw-   0        0        0     2218 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py
--rw-rw-rw-   0        0        0    18214 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py
--rw-rw-rw-   0        0        0     3355 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py
--rw-rw-rw-   0        0        0     1288 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0006_medication_child.py
--rw-rw-rw-   0        0        0     1313 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py
--rw-rw-rw-   0        0        0     1966 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py
--rw-rw-rw-   0        0        0     1357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py
--rw-rw-rw-   0        0        0     1577 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py
--rw-rw-rw-   0        0        0     1368 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py
--rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/__init__.py
--rw-rw-rw-   0        0        0    18845 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/models.py
--rw-rw-rw-   0        0        0     6365 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/serializers.py
--rw-rw-rw-   0        0        0    13848 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/signals.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.759807 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.914127 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/
--rw-rw-rw-   0        0        0     2723 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css
--rw-rw-rw-   0        0        0     1132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map
--rw-rw-rw-   0        0        0     2984 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.915141 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/
--rw-rw-rw-   0        0        0        0 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/.gitignore
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.028237 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/
--rw-rw-rw-   0        0        0    26606 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/anger.png
--rw-rw-rw-   0        0        0    26912 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/burn.png
--rw-rw-rw-   0        0        0    25533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/caca.png
--rw-rw-rw-   0        0        0    23167 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/confused.png
--rw-rw-rw-   0        0        0    24827 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/cool.png
--rw-rw-rw-   0        0        0    24276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/cry.png
--rw-rw-rw-   0        0        0    30248 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/fire.png
--rw-rw-rw-   0        0        0    30457 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/grimace.png
--rw-rw-rw-   0        0        0    27131 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/love.png
--rw-rw-rw-   0        0        0    23405 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/miao.png
--rw-rw-rw-   0        0        0    38098 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/nothing.png
--rw-rw-rw-   0        0        0   191276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/nothing.psd
--rw-rw-rw-   0        0        0    31987 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/prettiness.png
--rw-rw-rw-   0        0        0    26621 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/question.png
--rw-rw-rw-   0        0        0    23059 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/shout.png
--rw-rw-rw-   0        0        0    26669 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/slobber.png
--rw-rw-rw-   0        0        0    27523 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/smile.png
--rw-rw-rw-   0        0        0    22780 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/spook.png
--rw-rw-rw-   0        0        0    26432 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/startle.png
--rw-rw-rw-   0        0        0    31314 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/surprise.png
--rw-rw-rw-   0        0        0    24973 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/sweat.png
--rw-rw-rw-   0        0        0    24280 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/thirst.png
--rw-rw-rw-   0        0        0    27373 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/vomit.png
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.029258 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/
--rw-rw-rw-   0        0        0      805 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.031287 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/notifications/
--rw-rw-rw-   0        0        0     2602 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/notifications/notify.js
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.031287 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/vendor/
--rw-rw-rw-   0        0        0    38511 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.760827 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.032458 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_child/
--rw-rw-rw-   0        0        0     4633 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_child/base.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.033480 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.039768 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/
--rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html
--rw-rw-rw-   0        0        0      650 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html
--rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html
--rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html
--rw-rw-rw-   0        0        0     1598 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.041391 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/
--rw-rw-rw-   0        0        0      301 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/time-picker.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.049141 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/
--rw-rw-rw-   0        0        0     1542 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html
--rw-rw-rw-   0        0        0     1418 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html
--rw-rw-rw-   0        0        0     1718 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html
--rw-rw-rw-   0        0        0    45469 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html
--rw-rw-rw-   0        0        0     1407 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.054309 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/
--rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html
--rw-rw-rw-   0        0        0     1565 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html
--rw-rw-rw-   0        0        0     1567 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.057494 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/
--rw-rw-rw-   0        0        0      655 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html
--rw-rw-rw-   0        0        0     1416 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html
--rw-rw-rw-   0        0        0     1416 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.084154 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/
--rw-rw-rw-   0        0        0      782 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html
--rw-rw-rw-   0        0        0     1551 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html
--rw-rw-rw-   0        0        0      968 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html
--rw-rw-rw-   0        0        0     6663 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html
--rw-rw-rw-   0        0        0     1551 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.764146 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.089389 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/
--rw-rw-rw-   0        0        0       49 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/checkbox.html
--rw-rw-rw-   0        0        0      400 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio-input.html
--rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html
--rw-rw-rw-   0        0        0      490 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_option.html
--rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.094494 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/
--rw-rw-rw-   0        0        0      726 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html
--rw-rw-rw-   0        0        0     1540 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html
--rw-rw-rw-   0        0        0     1664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html
--rw-rw-rw-   0        0        0     1542 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.100710 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/
--rw-rw-rw-   0        0        0     2228 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html
--rw-rw-rw-   0        0        0     1647 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html
--rw-rw-rw-   0        0        0     2209 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html
--rw-rw-rw-   0        0        0     1689 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.103909 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/
--rw-rw-rw-   0        0        0      691 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html
--rw-rw-rw-   0        0        0     1536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html
--rw-rw-rw-   0        0        0     1549 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.105949 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/
--rw-rw-rw-   0        0        0     2235 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html
--rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.111191 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/
--rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html
--rw-rw-rw-   0        0        0     1565 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html
--rw-rw-rw-   0        0        0     1259 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html
--rw-rw-rw-   0        0        0     1567 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.113858 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/
--rw-rw-rw-   0        0        0      626 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html
--rw-rw-rw-   0        0        0     1533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html
--rw-rw-rw-   0        0        0     1533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.135144 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/
--rw-rw-rw-   0        0        0    32358 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html
--rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html
--rw-rw-rw-   0        0        0     1538 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html
--rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html
--rw-rw-rw-   0        0        0    21134 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html
--rw-rw-rw-   0        0        0    10664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html
--rw-rw-rw-   0        0        0     1158 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html
--rw-rw-rw-   0        0        0    52404 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.137186 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/
--rw-rw-rw-   0        0        0     1539 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.141269 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/
--rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html
--rw-rw-rw-   0        0        0     1797 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.143829 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/
--rw-rw-rw-   0        0        0     1498 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/__init__.py
--rw-rw-rw-   0        0        0     3742 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py
--rw-rw-rw-   0        0        0      978 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.145871 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/
--rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.151466 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/
--rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/__init__.py
--rw-rw-rw-   0        0        0      867 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/admin.py
--rw-rw-rw-   0        0        0      889 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:02.152474 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/migrations/
--rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py
--rw-rw-rw-   0        0        0      855 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/models.py
--rw-rw-rw-   0        0        0    25536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/urls.py
--rw-rw-rw-   0        0        0     3866 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/utils.py
--rw-rw-rw-   0        0        0   127708 2023-06-15 13:11:13.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/views.py
--rw-rw-rw-   0        0        0     1964 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/widgets.py
-drwxrwxrwx   0        0        0        0 2023-06-15 13:22:01.854410 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/
--rw-rw-rw-   0        0        0     8347 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10027 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      169 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-06-15 13:22:01.000000 nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      195 2023-06-14 13:30:37.000000 nobinobi-daily-follow-up-0.1.2.5/requirements.txt
--rw-rw-rw-   0        0        0      125 2023-06-15 10:29:37.000000 nobinobi-daily-follow-up-0.1.2.5/requirements_dev.txt
--rw-rw-rw-   0        0        0      192 2023-06-14 13:33:20.000000 nobinobi-daily-follow-up-0.1.2.5/requirements_test.txt
--rw-rw-rw-   0        0        0      301 2023-06-15 13:22:02.155748 nobinobi-daily-follow-up-0.1.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.667243 nobinobi-daily-follow-up-0.1.2.6/
+-rw-rw-rw-   0        0        0      166 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3491 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     4717 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.6/HISTORY.rst
+-rw-rw-rw-   0        0        0    31999 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/LICENSE
+-rw-rw-rw-   0        0        0      508 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     8475 2023-06-20 14:25:47.667243 nobinobi-daily-follow-up-0.1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3016 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.329452 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/
+-rw-rw-rw-   0        0        0      901 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/__init__.py
+-rw-rw-rw-   0        0        0     6644 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/admin.py
+-rw-rw-rw-   0        0        0     2132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/apps.py
+-rw-rw-rw-   0        0        0    24928 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/forms.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.231352 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.230352 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/en/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.338000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    36220 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.231352 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.368895 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0    17584 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0    43173 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     3840 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/menus.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.421690 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/
+-rw-rw-rw-   0        0        0    21335 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0    29811 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py
+-rw-rw-rw-   0        0        0     1251 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py
+-rw-rw-rw-   0        0        0      902 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py
+-rw-rw-rw-   0        0        0     2218 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py
+-rw-rw-rw-   0        0        0    18214 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py
+-rw-rw-rw-   0        0        0     3355 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py
+-rw-rw-rw-   0        0        0     1288 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0006_medication_child.py
+-rw-rw-rw-   0        0        0     1313 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py
+-rw-rw-rw-   0        0        0     1966 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py
+-rw-rw-rw-   0        0        0     1357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py
+-rw-rw-rw-   0        0        0     1577 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py
+-rw-rw-rw-   0        0        0     1368 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/__init__.py
+-rw-rw-rw-   0        0        0    18845 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/models.py
+-rw-rw-rw-   0        0        0     6365 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/serializers.py
+-rw-rw-rw-   0        0        0    13848 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.233569 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.426243 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/
+-rw-rw-rw-   0        0        0     2723 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css
+-rw-rw-rw-   0        0        0     1132 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map
+-rw-rw-rw-   0        0        0     2984 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.427239 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/
+-rw-rw-rw-   0        0        0        0 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/.gitignore
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.516753 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/
+-rw-rw-rw-   0        0        0    26606 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/anger.png
+-rw-rw-rw-   0        0        0    26912 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/burn.png
+-rw-rw-rw-   0        0        0    25533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/caca.png
+-rw-rw-rw-   0        0        0    23167 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/confused.png
+-rw-rw-rw-   0        0        0    24827 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/cool.png
+-rw-rw-rw-   0        0        0    24276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/cry.png
+-rw-rw-rw-   0        0        0    30248 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/fire.png
+-rw-rw-rw-   0        0        0    30457 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/grimace.png
+-rw-rw-rw-   0        0        0    27131 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/love.png
+-rw-rw-rw-   0        0        0    23405 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/miao.png
+-rw-rw-rw-   0        0        0    38098 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/nothing.png
+-rw-rw-rw-   0        0        0   191276 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/nothing.psd
+-rw-rw-rw-   0        0        0    31987 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/prettiness.png
+-rw-rw-rw-   0        0        0    26621 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/question.png
+-rw-rw-rw-   0        0        0    23059 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/shout.png
+-rw-rw-rw-   0        0        0    26669 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/slobber.png
+-rw-rw-rw-   0        0        0    27523 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/smile.png
+-rw-rw-rw-   0        0        0    22780 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/spook.png
+-rw-rw-rw-   0        0        0    26432 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/startle.png
+-rw-rw-rw-   0        0        0    31314 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/surprise.png
+-rw-rw-rw-   0        0        0    24973 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/sweat.png
+-rw-rw-rw-   0        0        0    24280 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/thirst.png
+-rw-rw-rw-   0        0        0    27373 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/vomit.png
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.518767 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/
+-rw-rw-rw-   0        0        0      805 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.519761 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/notifications/
+-rw-rw-rw-   0        0        0     2602 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/notifications/notify.js
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.520762 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/vendor/
+-rw-rw-rw-   0        0        0    38511 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.235598 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.522763 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_child/
+-rw-rw-rw-   0        0        0     4633 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_child/base.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.525273 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.532585 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html
+-rw-rw-rw-   0        0        0      650 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html
+-rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html
+-rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html
+-rw-rw-rw-   0        0        0     1598 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.533848 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/
+-rw-rw-rw-   0        0        0      301 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/bootstrap_datepicker_plus/time-picker.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.555490 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/
+-rw-rw-rw-   0        0        0     1542 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html
+-rw-rw-rw-   0        0        0     1418 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html
+-rw-rw-rw-   0        0        0     1718 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html
+-rw-rw-rw-   0        0        0    45469 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html
+-rw-rw-rw-   0        0        0     1407 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.561147 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/
+-rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1565 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html
+-rw-rw-rw-   0        0        0     1567 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.564147 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/
+-rw-rw-rw-   0        0        0      655 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html
+-rw-rw-rw-   0        0        0     1416 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html
+-rw-rw-rw-   0        0        0     1416 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.571190 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/
+-rw-rw-rw-   0        0        0      782 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html
+-rw-rw-rw-   0        0        0     1551 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html
+-rw-rw-rw-   0        0        0      968 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html
+-rw-rw-rw-   0        0        0     6663 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html
+-rw-rw-rw-   0        0        0     1551 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.238612 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.575188 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/
+-rw-rw-rw-   0        0        0       49 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/checkbox.html
+-rw-rw-rw-   0        0        0      400 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio-input.html
+-rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html
+-rw-rw-rw-   0        0        0      490 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_option.html
+-rw-rw-rw-   0        0        0      717 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.580300 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/
+-rw-rw-rw-   0        0        0      726 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1540 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html
+-rw-rw-rw-   0        0        0     1664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html
+-rw-rw-rw-   0        0        0     1542 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.585300 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/
+-rw-rw-rw-   0        0        0     2228 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html
+-rw-rw-rw-   0        0        0     1647 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html
+-rw-rw-rw-   0        0        0     2209 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html
+-rw-rw-rw-   0        0        0     1689 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.587821 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/
+-rw-rw-rw-   0        0        0      691 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html
+-rw-rw-rw-   0        0        0     1536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html
+-rw-rw-rw-   0        0        0     1549 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.591342 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/
+-rw-rw-rw-   0        0        0     2235 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html
+-rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.595851 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/
+-rw-rw-rw-   0        0        0      660 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html
+-rw-rw-rw-   0        0        0     1565 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html
+-rw-rw-rw-   0        0        0     1259 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html
+-rw-rw-rw-   0        0        0     1567 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.598864 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/
+-rw-rw-rw-   0        0        0      626 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html
+-rw-rw-rw-   0        0        0     1533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html
+-rw-rw-rw-   0        0        0     1533 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.634545 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/
+-rw-rw-rw-   0        0        0    32358 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html
+-rw-rw-rw-   0        0        0     1538 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html
+-rw-rw-rw-   0        0        0     1535 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html
+-rw-rw-rw-   0        0        0    21134 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html
+-rw-rw-rw-   0        0        0    10664 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html
+-rw-rw-rw-   0        0        0     1158 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html
+-rw-rw-rw-   0        0        0    52404 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.635545 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/
+-rw-rw-rw-   0        0        0     1539 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.638581 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/
+-rw-rw-rw-   0        0        0     1196 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html
+-rw-rw-rw-   0        0        0     1797 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.643099 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/
+-rw-rw-rw-   0        0        0     1498 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     3742 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py
+-rw-rw-rw-   0        0        0      978 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.644098 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.663720 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/__init__.py
+-rw-rw-rw-   0        0        0      867 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/admin.py
+-rw-rw-rw-   0        0        0      889 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.665229 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/migrations/
+-rw-rw-rw-   0        0        0      794 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py
+-rw-rw-rw-   0        0        0      855 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/models.py
+-rw-rw-rw-   0        0        0    25536 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/urls.py
+-rw-rw-rw-   0        0        0     3866 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/utils.py
+-rw-rw-rw-   0        0        0   130484 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/views.py
+-rw-rw-rw-   0        0        0     1964 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/widgets.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:25:47.336485 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/
+-rw-rw-rw-   0        0        0     8475 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10027 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      169 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-20 14:25:46.000000 nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      195 2023-06-14 13:30:37.000000 nobinobi-daily-follow-up-0.1.2.6/requirements.txt
+-rw-rw-rw-   0        0        0      125 2023-06-15 10:29:37.000000 nobinobi-daily-follow-up-0.1.2.6/requirements_dev.txt
+-rw-rw-rw-   0        0        0      205 2023-06-20 14:24:55.000000 nobinobi-daily-follow-up-0.1.2.6/requirements_test.txt
+-rw-rw-rw-   0        0        0      301 2023-06-20 14:25:47.668244 nobinobi-daily-follow-up-0.1.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2357 2023-06-09 07:18:16.000000 nobinobi-daily-follow-up-0.1.2.6/setup.py
```

### Comparing `nobinobi-daily-follow-up-0.1.2.5/CONTRIBUTING.rst` & `nobinobi-daily-follow-up-0.1.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/HISTORY.rst` & `nobinobi-daily-follow-up-0.1.2.6/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. :changelog:
 
 History
 -------
 
+0.1.2.6 (2023-06-20)
++++++++++++++++++++++++++
+
+* 33ddd86 - fix error in create presence day table
+* Update requirements
+
 0.1.2.5 (2023-06-15)
 +++++++++++++++++++++++++
 
 * 4e6cee2 - FIX: when create in presence day in table naps, lotion,medication, etc
 * 5e04f16 - Fix new version of crispy forms
 * Update requirements
```

### Comparing `nobinobi-daily-follow-up-0.1.2.5/LICENSE` & `nobinobi-daily-follow-up-0.1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/PKG-INFO` & `nobinobi-daily-follow-up-0.1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobinobi-daily-follow-up
-Version: 0.1.2.5
+Version: 0.1.2.6
 Summary: Application Daily follow-up for nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-daily-follow-up
 Author: Florian Alu
 Author-email: alu@prolibre.com
 Keywords: nobinobi-daily-follow-up
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.1
@@ -135,14 +135,20 @@
 
 
 
 
 History
 -------
 
+0.1.2.6 (2023-06-20)
++++++++++++++++++++++++++
+
+* 33ddd86 - fix error in create presence day table
+* Update requirements
+
 0.1.2.5 (2023-06-15)
 +++++++++++++++++++++++++
 
 * 4e6cee2 - FIX: when create in presence day in table naps, lotion,medication, etc
 * 5e04f16 - Fix new version of crispy forms
 * Update requirements
```

### Comparing `nobinobi-daily-follow-up-0.1.2.5/README.rst` & `nobinobi-daily-follow-up-0.1.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/__init__.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,9 @@
 #      but WITHOUT ANY WARRANTY; without even the implied warranty of
 #      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #      GNU Affero General Public License for more details.
 #
 #      You should have received a copy of the GNU Affero General Public License
 #      along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '0.1.2.5'
+__version__ = '0.1.2.6'
 default_app_config = 'nobinobi_daily_follow_up.apps.NobinobiDailyFollowUpConfig'
```

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/admin.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/apps.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/forms.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/forms.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/menus.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/menus.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0001_initial.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0001_initial_squashed_0011_auto_20200401_1117.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0002_auto_20190513_1535.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0002_auto_20230201_1346.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0003_troubleshooting.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0004_auto_20190815_1141.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0005_auto_20190923_1517.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0006_medication_child.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0006_medication_child.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0007_givemedication_date.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0008_auto_20191021_1443.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0009_fix_early_troubleshoting_relation.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0010_add_intermediary_departure_arrival_time.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/0011_auto_20200401_1117.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/migrations/__init__.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/models.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/serializers.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/serializers.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/signals.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/signals.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.css.map`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/css/nobinobi_daily_follow_up.scss`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/anger.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/anger.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/burn.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/burn.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/caca.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/caca.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/confused.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/confused.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/cool.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/cool.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/cry.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/cry.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/fire.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/fire.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/grimace.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/grimace.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/love.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/love.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/miao.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/miao.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/nothing.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/nothing.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/nothing.psd` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/nothing.psd`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/prettiness.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/prettiness.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/question.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/question.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/shout.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/shout.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/slobber.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/slobber.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/smile.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/smile.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/spook.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/spook.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/startle.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/startle.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/surprise.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/surprise.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/sweat.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/sweat.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/thirst.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/thirst.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/img/smiley/vomit.png` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/img/smiley/vomit.png`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/nobinobi_daily_follow_up.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/notifications/notify.js` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/notifications/notify.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/static/js/vendor/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_child/base.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_child/base.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/activity_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/activity/group_activity_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/dailyfollowup_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/group_daily_follow_up_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowup/summary_week_choice.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/dailyfollowuptomedication/dailyfollowuptomedication_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/diaperchange/diaperchange_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_detail.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/earlytroubleshooting/earlytroubleshooting_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline-img-radio.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/forms/widgets/inline_img_checkbox_select.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_delay.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/givemedication/givemedication_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/checkboxselectmultiple_inline_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/layout/radioselect_inline_image.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/lotiondailyfollowup/lotiondailyfollowup_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/meals/mealdailyfollowup_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_multiday.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/medication/medication_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/nap/nap_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/admin_presence_week_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_create.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_kindergarten_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence/presence_week_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_choice.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/presence_detail_list.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/reception/reception_update.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_choice_classroom.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templates/nobinobi_daily_follow_up/stroll/stroll_pdf.html`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/__init__.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/notifications_custom_tags.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/templatetags/replacement_classroom_tags.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/__init__.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/__init__.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/admin.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/admin.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/apps.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/apps.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/migrations/__init__.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/test_utils/test_app/models.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/test_utils/test_app/models.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/urls.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/urls.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/utils.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/utils.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up/widgets.py` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up/widgets.py`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/PKG-INFO` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobinobi-daily-follow-up
-Version: 0.1.2.5
+Version: 0.1.2.6
 Summary: Application Daily follow-up for nobinobi
 Home-page: https://github.com/prolibre-ch/nobinobi-daily-follow-up
 Author: Florian Alu
 Author-email: alu@prolibre.com
 Keywords: nobinobi-daily-follow-up
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django :: 3.1
@@ -135,14 +135,20 @@
 
 
 
 
 History
 -------
 
+0.1.2.6 (2023-06-20)
++++++++++++++++++++++++++
+
+* 33ddd86 - fix error in create presence day table
+* Update requirements
+
 0.1.2.5 (2023-06-15)
 +++++++++++++++++++++++++
 
 * 4e6cee2 - FIX: when create in presence day in table naps, lotion,medication, etc
 * 5e04f16 - Fix new version of crispy forms
 * Update requirements
```

### Comparing `nobinobi-daily-follow-up-0.1.2.5/nobinobi_daily_follow_up.egg-info/SOURCES.txt` & `nobinobi-daily-follow-up-0.1.2.6/nobinobi_daily_follow_up.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobinobi-daily-follow-up-0.1.2.5/setup.py` & `nobinobi-daily-follow-up-0.1.2.6/setup.py`

 * *Files identical despite different names*

