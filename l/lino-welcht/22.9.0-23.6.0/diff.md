# Comparing `tmp/lino-welcht-22.9.0.tar.gz` & `tmp/lino-welcht-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino-welcht-22.9.0.tar", last modified: Thu Sep 22 08:45:43 2022, max compression
+gzip compressed data, was "lino-welcht-23.6.0.tar", last modified: Tue Jun 20 12:12:37 2023, max compression
```

## Comparing `lino-welcht-22.9.0.tar` & `lino-welcht-23.6.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-07 12:55:58.000000 lino-welcht-22.9.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      110 2019-02-28 04:54:23.000000 lino-welcht-22.9.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1692 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      734 2021-08-19 05:39:07.000000 lino-welcht-22.9.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      880 2021-04-28 10:35:43.000000 lino-welcht-22.9.0/lino_welcht/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1696 2021-02-14 21:14:30.000000 lino-welcht-22.9.0/lino_welcht/help_texts.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1372 2022-03-11 06:24:09.000000 lino-welcht-22.9.0/lino_welcht/layouts.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/lib/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      258 2021-04-07 10:22:54.000000 lino-welcht-22.9.0/lino_welcht/lib/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/lib/courses/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      513 2021-04-07 10:22:54.000000 lino-welcht-22.9.0/lino_welcht/lib/courses/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.943876 lino-welcht-22.9.0/lino_welcht/lib/courses/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.943876 lino-welcht-22.9.0/lino_welcht/lib/courses/config/courses/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/lib/courses/config/courses/Enrolment/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1013 2015-09-19 03:53:35.000000 lino-welcht-22.9.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1465 2015-09-19 03:53:35.000000 lino-welcht-22.9.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1362 2021-04-07 10:22:54.000000 lino-welcht-22.9.0/lino_welcht/lib/courses/desktop.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/lib/courses/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:35.000000 lino-welcht-22.9.0/lino_welcht/lib/courses/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4722 2021-04-14 18:14:38.000000 lino-welcht-22.9.0/lino_welcht/lib/courses/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      907 2021-04-07 10:22:55.000000 lino-welcht-22.9.0/lino_welcht/lib/courses/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3380 2021-04-07 10:22:54.000000 lino-welcht-22.9.0/lino_welcht/lib/courses/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/lib/cv/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1134 2021-04-07 10:22:54.000000 lino-welcht-22.9.0/lino_welcht/lib/cv/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/lib/cv/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2015-09-19 03:53:36.000000 lino-welcht-22.9.0/lino_welcht/lib/cv/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      655 2021-04-15 06:04:50.000000 lino-welcht-22.9.0/lino_welcht/lib/cv/fixtures/demo.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      931 2021-04-07 10:22:55.000000 lino-welcht-22.9.0/lino_welcht/lib/cv/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7564 2021-04-14 14:08:01.000000 lino-welcht-22.9.0/lino_welcht/lib/cv/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/lib/isip/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      290 2021-04-07 10:22:54.000000 lino-welcht-22.9.0/lino_welcht/lib/isip/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1924 2021-04-15 16:44:04.000000 lino-welcht-22.9.0/lino_welcht/lib/isip/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/lib/pcsw/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      418 2021-04-07 10:22:54.000000 lino-welcht-22.9.0/lino_welcht/lib/pcsw/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      457 2021-04-07 10:22:54.000000 lino-welcht-22.9.0/lino_welcht/lib/pcsw/choicelists.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/lib/pcsw/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/lib/pcsw/config/pcsw/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      613 2015-09-19 03:53:35.000000 lino-welcht-22.9.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/lib/pcsw/fixtures/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2016-06-08 13:29:44.000000 lino-welcht-22.9.0/lino_welcht/lib/pcsw/fixtures/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       60 2017-04-22 06:37:57.000000 lino-welcht-22.9.0/lino_welcht/lib/pcsw/fixtures/demo2.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       58 2016-06-08 13:30:04.000000 lino-welcht-22.9.0/lino_welcht/lib/pcsw/fixtures/std.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7175 2022-09-05 23:22:02.000000 lino-welcht-22.9.0/lino_welcht/lib/pcsw/models.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/locale/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/locale/de/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39041 2018-12-10 08:06:01.000000 lino-welcht-22.9.0/lino_welcht/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    74719 2021-02-11 19:06:41.000000 lino-welcht-22.9.0/lino_welcht/locale/de/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/locale/fr/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     4021 2019-03-29 10:29:37.000000 lino-welcht-22.9.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)     9514 2021-02-11 19:06:42.000000 lino-welcht-22.9.0/lino_welcht/locale/fr/LC_MESSAGES/django.po
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht/locale/nl/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/lino_welcht/locale/nl/LC_MESSAGES/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      409 2015-09-19 03:53:53.000000 lino-welcht-22.9.0/lino_welcht/locale/nl/LC_MESSAGES/django.mo
--rw-rw-rw-   0 luc       (1000) www-data    (33)    93297 2021-02-11 17:36:49.000000 lino-welcht-22.9.0/lino_welcht/locale/nl/LC_MESSAGES/django.po
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7024 2021-04-07 10:22:53.000000 lino-welcht-22.9.0/lino_welcht/migrate.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     7445 2022-07-19 23:42:02.000000 lino-welcht-22.9.0/lino_welcht/settings.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)     5073 2022-09-22 07:31:27.000000 lino-welcht-22.9.0/lino_welcht/setup_info.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      247 2018-12-08 06:32:49.000000 lino-welcht-22.9.0/lino_welcht/workflows.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.947876 lino-welcht-22.9.0/lino_welcht.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1692 2022-09-22 08:45:43.000000 lino-welcht-22.9.0/lino_welcht.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1708 2022-09-22 08:45:43.000000 lino-welcht-22.9.0/lino_welcht.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2022-09-22 08:45:43.000000 lino-welcht-22.9.0/lino_welcht.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-02-27 20:03:15.000000 lino-welcht-22.9.0/lino_welcht.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)       72 2022-09-22 08:45:43.000000 lino-welcht-22.9.0/lino_welcht.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       12 2022-09-22 08:45:43.000000 lino-welcht-22.9.0/lino_welcht.egg-info/top_level.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1052 2021-05-05 05:16:56.000000 lino-welcht-22.9.0/requirements.python3.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      347 2021-05-05 05:16:56.000000 lino-welcht-22.9.0/requirements.stable.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)      931 2021-05-05 05:16:56.000000 lino-welcht-22.9.0/requirements.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      163 2019-02-27 13:45:16.000000 lino-welcht-22.9.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      377 2021-03-22 12:47:21.000000 lino-welcht-22.9.0/tasks.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2022-09-22 08:45:43.951876 lino-welcht-22.9.0/tests/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      552 2021-04-07 10:22:53.000000 lino-welcht-22.9.0/tests/__init__.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      171 2019-03-07 07:55:55.000000 lino-welcht-22.9.0/tests/test_docs.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.868260 lino-welcht-23.6.0/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/COPYING
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      110 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/MANIFEST.in
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1655 2023-06-20 12:12:37.868260 lino-welcht-23.6.0/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      734 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/README.rst
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      880 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      224 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/help_texts.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1549 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/layouts.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      258 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/courses/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      546 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/lib/courses/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1013 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1465 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4722 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      907 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1357 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/courses/ui.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/cv/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1134 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      655 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/demo.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      931 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7570 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/cv/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht/lib/isip/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      290 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/isip/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1924 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/isip/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      418 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      457 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/choicelists.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/pcsw/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      613 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/lib/pcsw/fixtures/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/fixtures/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       60 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/fixtures/demo2.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       58 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/fixtures/std.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7176 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/lib/pcsw/models.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/locale/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/locale/de/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39041 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    74719 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/django.po
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/locale/fr/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4021 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     9514 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/django.po
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.856260 lino-welcht-23.6.0/lino_welcht/locale/nl/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.864260 lino-welcht-23.6.0/lino_welcht/locale/nl/LC_MESSAGES/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      409 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/nl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    93297 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/locale/nl/LC_MESSAGES/django.po
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7024 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/migrate.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     7594 2023-03-31 11:55:46.000000 lino-welcht-23.6.0/lino_welcht/settings.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4938 2023-06-20 12:12:03.000000 lino-welcht-23.6.0/lino_welcht/setup_info.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      247 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht/workflows.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.860260 lino-welcht-23.6.0/lino_welcht.egg-info/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1655 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1703 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/SOURCES.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/dependency_links.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/lino_welcht.egg-info/not-zip-safe
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       72 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/requires.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       12 2023-06-20 12:12:37.000000 lino-welcht-23.6.0/lino_welcht.egg-info/top_level.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1052 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/requirements.python3.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      347 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/requirements.stable.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      931 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/requirements.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-06-20 12:12:37.868260 lino-welcht-23.6.0/setup.cfg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      163 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/setup.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      377 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/tasks.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-06-20 12:12:37.868260 lino-welcht-23.6.0/tests/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      552 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/tests/__init__.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      171 2023-02-28 05:23:18.000000 lino-welcht-23.6.0/tests/test_docs.py
```

### Comparing `lino-welcht-22.9.0/COPYING` & `lino-welcht-23.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/PKG-INFO` & `lino-welcht-23.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino-welcht
-Version: 22.9.0
+Version: 23.6.0
 Summary: A Lino Django application for the PCSW of Châtelet
 Home-page: https://gitlab.com/lino-framework/welcht
 Author: Rumma & Ko Ltd
 Author-email: hamza@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -40,9 +38,7 @@
   `Lino Welfare <https://welfare.lino-framework.org>`__.
 
 - The `French project homepage <https://fr.welfare.lino-framework.org>`__
   contains release notes and end-user docs.
 
 - Online demo site at https://welfare-demo.lino-framework.org
 
-
-
```

### Comparing `lino-welcht-22.9.0/README.rst` & `lino-welcht-23.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/__init__.py` & `lino-welcht-23.6.0/lino_welcht/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/courses/__init__.py` & `lino-welcht-23.6.0/lino_welcht/lib/courses/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 from django.utils.translation import gettext_lazy as _
 
 
 class Plugin(Plugin):
     extends_models = ['Course', 'Line', 'Enrolment']
     verbose_name = _("Workshops")
     pupil_model = 'pcsw.Client'
+    teacher_model = 'users.User'
     short_name = _("IO")  # "internal orientation"
```

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html` & `lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html` & `lino-welcht-23.6.0/lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/courses/desktop.py` & `lino-welcht-23.6.0/lino_welcht/lib/courses/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2014-2020 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 from lino.api import _
-from lino_xl.lib.courses.desktop import *
+from lino_xl.lib.courses.ui import *
 
 Enrolments.detail_layout = """
 request_date user
 course pupil
 remark workflow_buttons printed
 motivation problems
 """
```

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/courses/fixtures/demo.py` & `lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/courses/fixtures/std.py` & `lino-welcht-23.6.0/lino_welcht/lib/courses/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/courses/models.py` & `lino-welcht-23.6.0/lino_welcht/lib/courses/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 Does some adaptions.
 """
 
 from lino.api import dd, _
 
 from lino_xl.lib.courses.models import *
+from lino_xl.lib.courses.roles import CoursesTeacher
 
 ActivityLayouts.clear()
 add = ActivityLayouts.add_item
 # add('S', _("Integration workshops"), 'integ')  # no longer used
 add('B', _("Integration workshops"), 'default')  # , 'courses.BasicCourses')
 add('J', _("Job search workshops"), 'job', 'courses.JobCourses')
 # add('B', _("Social integration"), 'default')
@@ -59,14 +60,20 @@
 
 class Course(Course):
     class Meta:
         verbose_name = _("Workshop")
         verbose_name_plural = _('Workshops')
         abstract = dd.is_abstract_model(__name__, 'Course')
 
+    @dd.chooser()
+    def teacher_choices(cls):
+        assert dd.plugins.courses.teacher_model is rt.models.users.User
+        teacher_types = [t for t in rt.models.users.UserTypes.get_list_items()
+                  if t.has_required_roles([CoursesTeacher])]
+        return rt.models.users.User.objects.filter(user_type__in=teacher_types)
 
 # GUEST_ENROLMENT_STATES = set([
 #     EnrolmentStates.confirmed,
 #     EnrolmentStates.started])
 
 
 class Enrolment(Enrolment):
@@ -92,7 +99,10 @@
 
 class Line(Line):
     class Meta:
         app_label = 'courses'
         verbose_name = _("Workshop series")
         verbose_name_plural = _('Workshop lines')
         abstract = dd.is_abstract_model(__name__, 'Line')
+
+
+from .ui import *
```

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/cv/__init__.py` & `lino-welcht-23.6.0/lino_welcht/lib/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/cv/fixtures/demo.py` & `lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/cv/fixtures/std.py` & `lino-welcht-23.6.0/lino_welcht/lib/cv/fixtures/std.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/cv/models.py` & `lino-welcht-23.6.0/lino_welcht/lib/cv/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,17 +240,17 @@
 
 
 class ObstaclesByPerson(PropsByPerson, Obstacles):
     required_roles = dd.login_required(IntegUser)
     column_names = 'type user detected_date remark  *'
 
 
-dd.inject_field('system.SiteConfig', 'propgroup_skills', dd.DummyField())
-dd.inject_field('system.SiteConfig', 'propgroup_softskills', dd.DummyField())
-dd.inject_field('system.SiteConfig', 'propgroup_obstacles', dd.DummyField())
+# dd.inject_field('system.SiteConfig', 'propgroup_skills', dd.DummyField())
+# dd.inject_field('system.SiteConfig', 'propgroup_softskills', dd.DummyField())
+# dd.inject_field('system.SiteConfig', 'propgroup_obstacles', dd.DummyField())
 
 # print(StudiesByPerson.column_names)
 # print(TrainingsByPerson.column_names)
 # print(ExperiencesByPerson.column_names)
 
 StudiesByPerson.column_names = "type content start_date end_date duration_text school country state education_level remarks *"
 TrainingsByPerson.column_names = "type sector function start_date end_date duration_text school country state certificates remarks *"
```

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/isip/models.py` & `lino-welcht-23.6.0/lino_welcht/lib/isip/models.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html` & `lino-welcht-23.6.0/lino_welcht/lib/pcsw/config/pcsw/Coaching/coaching.body.html`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/lib/pcsw/models.py` & `lino-welcht-23.6.0/lino_welcht/lib/pcsw/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
     is_obsolete has_esf created modified
     remarks
     checkdata.MessagesByOwner:30 contacts.RolesByPerson:20
     """, label=_("Miscellaneous"), required_roles=dd.login_required(SocialStaff))
 
     contracts = dd.Panel("""
     jobs.CandidaturesByPerson
-    jobs.ContractsByClient
+    art60.ContractsByClient
     art61.ContractsByClient
     """, label=dd.plugins.jobs.verbose_name)
 
     # sis_tab = dd.Panel("""
     # #isip.ContractsByClient
     # sis_motif sis_attentes
     # sis_moteurs sis_objectifs
```

### Comparing `lino-welcht-22.9.0/lino_welcht/locale/de/LC_MESSAGES/django.mo` & `lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/locale/de/LC_MESSAGES/django.po` & `lino-welcht-23.6.0/lino_welcht/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo` & `lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/locale/fr/LC_MESSAGES/django.po` & `lino-welcht-23.6.0/lino_welcht/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/locale/nl/LC_MESSAGES/django.po` & `lino-welcht-23.6.0/lino_welcht/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/migrate.py` & `lino-welcht-23.6.0/lino_welcht/migrate.py`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/lino_welcht/settings.py` & `lino-welcht-23.6.0/lino_welcht/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     version = SETUP_INFO['version']
     url = SETUP_INFO['url']
 
     project_model = 'pcsw.Client'
     # catch_layout_exceptions = False # 20130804
 
     userdocs_prefix = 'welfare.'
-    auto_configure_logger_names = 'atelier schedule django lino lino_xl lino_cosi lino_welfare'
+    auto_configure_logger_names = 'atelier django lino lino_xl lino_cosi lino_welfare'
     # use_java = False  # temporarily
     # verbose_client_info_message = True
     # default_build_method = "appyodt"
     default_build_method = "appypdf"
     uppercase_last_name = True
     user_types_module = 'lino_welfare.modlib.welfare.user_types'
     # workflows_module = 'lino_xl.lib.reception.workflows'
@@ -78,14 +78,15 @@
         # yield 'lino_welfare.modlib.pcsw'
         # yield 'lino_welfare.modlib.ledger'
 
         yield 'lino_welcht.lib.cv'
         yield 'lino_welfare.modlib.integ'
         yield 'lino_welcht.lib.isip'
         yield 'lino_welfare.modlib.jobs'
+        yield 'lino_welfare.modlib.art60'
         yield 'lino_welfare.modlib.art61'
         yield 'lino_welfare.modlib.immersion'
         yield 'lino_welfare.modlib.active_job_search'
         yield 'lino_welcht.lib.courses'
         yield 'lino_welfare.modlib.newcomers'
         yield 'lino_welfare.modlib.cbss'  # must come after pcsw
         yield 'lino_welfare.modlib.households'  # must come after pcsw
@@ -131,16 +132,17 @@
         for i in super(Site, self).get_plugin_configs():
             yield i
         yield ('clients', 'client_model', 'pcsw.Client')
         yield ('addresses', 'partner_model', 'contacts.Partner')
         yield ('excerpts', 'responsible_user', 'melanie')
         yield ('integ', 'only_primary', True)
         yield ('coachings', 'multiple_primary_coachings', True)
-        yield ('help', 'interproject_specs', 'lino_welfare')
+        # yield ('help', 'interproject_specs', 'lino_welfare')
         yield ('help', 'make_help_pages', True)
+        yield ('jobs', 'with_employer_model', True)
 
     # def get_default_language(self):
     #     return 'fr'
 
     def get_dashboard_items(self, user):
         """Defines the items to show in :xfile:`admin_main.html`.
         See :meth:`lino.core.site.Site.get_dashboard_items`.
@@ -188,9 +190,10 @@
     def setup_quicklinks(self, user, tb):
         # tb.add_action(self.modules.pcsw.Clients.detail_action)
 
         super(Site, self).setup_quicklinks(user, tb)
         tb.add_action("pcsw.Clients.find_by_beid")
         tb.add_action(self.modules.integ.Clients)
         tb.add_action(self.modules.isip.MyContracts)
-        tb.add_action(self.modules.jobs.MyContracts)
+        # tb.add_action(self.modules.art60.MyContracts)
+        # tb.add_action(self.modules.art60.MyContractsGSS)
         tb.add_action(self.modules.cal.EntriesByDay)
```

### Comparing `lino-welcht-22.9.0/lino_welcht/setup_info.py` & `lino-welcht-23.6.0/lino_welcht/setup_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 # -*- coding: UTF-8 -*-
-# Copyright 2002-2019 Rumma & Ko Ltd
+# Copyright 2002-2022 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
-# This module is part of the Lino Welfare test suite.
-# To test only this module:
-#
-#   $ python setup.py test -s tests.PackagesTests
 
 import sys
 PY2 = sys.version_info[0] == 2
 
 
 requires = ['lino-welfare',
             'pytidylib',
@@ -23,21 +19,21 @@
     requires.append('suds-py3')
     # requires.append('suds-jurko')
 
 
 
 SETUP_INFO = dict(
     name='lino-welcht',
-    version='22.9.0',
+    version='23.6.0',
     install_requires=requires,
     test_suite='tests',
     tests_require=['pytest'],
     include_package_data=True,
     zip_safe=False,
-    description=u"A Lino Django application for the PCSW of Châtelet",
+    description="A Lino Django application for the PCSW of Châtelet",
     long_description=u"""\
 **Lino Welfare Châtelet** is a
 `Lino Welfare <https://welfare.lino-framework.org>`__
 application developed and maintained for the PCSW of Châtelet in Belgium.
 
 - The central project homepage is http://welcht.lino-framework.org
```

### Comparing `lino-welcht-22.9.0/lino_welcht.egg-info/PKG-INFO` & `lino-welcht-23.6.0/lino_welcht.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: lino-welcht
-Version: 22.9.0
+Version: 23.6.0
 Summary: A Lino Django application for the PCSW of Châtelet
 Home-page: https://gitlab.com/lino-framework/welcht
 Author: Rumma & Ko Ltd
 Author-email: hamza@lino-framework.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
@@ -40,9 +38,7 @@
   `Lino Welfare <https://welfare.lino-framework.org>`__.
 
 - The `French project homepage <https://fr.welfare.lino-framework.org>`__
   contains release notes and end-user docs.
 
 - Online demo site at https://welfare-demo.lino-framework.org
 
-
-
```

### Comparing `lino-welcht-22.9.0/lino_welcht.egg-info/SOURCES.txt` & `lino-welcht-23.6.0/lino_welcht.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 lino_welcht.egg-info/SOURCES.txt
 lino_welcht.egg-info/dependency_links.txt
 lino_welcht.egg-info/not-zip-safe
 lino_welcht.egg-info/requires.txt
 lino_welcht.egg-info/top_level.txt
 lino_welcht/lib/__init__.py
 lino_welcht/lib/courses/__init__.py
-lino_welcht/lib/courses/desktop.py
 lino_welcht/lib/courses/models.py
+lino_welcht/lib/courses/ui.py
 lino_welcht/lib/courses/config/courses/Enrolment/enrolment.body.html
 lino_welcht/lib/courses/config/courses/Enrolment/intervention.body.html
 lino_welcht/lib/courses/fixtures/__init__.py
 lino_welcht/lib/courses/fixtures/demo.py
 lino_welcht/lib/courses/fixtures/std.py
 lino_welcht/lib/cv/__init__.py
 lino_welcht/lib/cv/models.py
```

### Comparing `lino-welcht-22.9.0/requirements.python3.txt` & `lino-welcht-23.6.0/requirements.python3.txt`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/requirements.txt` & `lino-welcht-23.6.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `lino-welcht-22.9.0/tests/__init__.py` & `lino-welcht-23.6.0/tests/__init__.py`

 * *Files identical despite different names*

