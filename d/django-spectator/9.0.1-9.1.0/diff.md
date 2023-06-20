# Comparing `tmp/django-spectator-9.0.1.tar.gz` & `tmp/django-spectator-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-spectator-9.0.1.tar", last modified: Wed Aug  7 17:25:26 2019, max compression
+gzip compressed data, was "dist/django-spectator-9.1.0.tar", last modified: Sat Oct 19 17:03:05 2019, max compression
```

## Comparing `django-spectator-9.0.1.tar` & `django-spectator-9.1.0.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/
--rw-r--r--   0 phil       (501) staff       (20)     1356 2019-05-05 18:41:22.000000 django-spectator-9.0.1/.travis.yml
--rw-r--r--   0 phil       (501) staff       (20)     1079 2017-02-28 18:49:02.000000 django-spectator-9.0.1/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      267 2017-08-22 14:54:13.000000 django-spectator-9.0.1/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)    23442 2019-08-07 17:25:26.000000 django-spectator-9.0.1/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)    17904 2019-07-31 15:52:27.000000 django-spectator-9.0.1/README.rst
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/django_spectator.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)    23442 2019-08-07 17:25:25.000000 django-spectator-9.0.1/django_spectator.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     8212 2019-08-07 17:25:26.000000 django-spectator-9.0.1/django_spectator.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2019-08-07 17:25:25.000000 django-spectator-9.0.1/django_spectator.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       65 2019-08-07 17:25:25.000000 django-spectator-9.0.1/django_spectator.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)       10 2019-08-07 17:25:25.000000 django-spectator-9.0.1/django_spectator.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)       38 2019-08-07 17:25:26.000000 django-spectator-9.0.1/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     3063 2019-07-31 15:52:27.000000 django-spectator-9.0.1/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/
--rw-r--r--   0 phil       (501) staff       (20)      200 2019-08-07 17:22:44.000000 django-spectator-9.0.1/spectator/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/
--rw-r--r--   0 phil       (501) staff       (20)       67 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/core/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      618 2018-01-02 09:12:05.000000 django-spectator-9.0.1/spectator/core/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      884 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)     1716 2017-04-17 16:10:03.000000 django-spectator-9.0.1/spectator/core/apps.py
--rw-r--r--   0 phil       (501) staff       (20)      518 2019-07-31 16:19:20.000000 django-spectator-9.0.1/spectator/core/factories.py
--rw-r--r--   0 phil       (501) staff       (20)     8615 2018-10-24 14:10:15.000000 django-spectator-9.0.1/spectator/core/fields.py
--rw-r--r--   0 phil       (501) staff       (20)     1329 2019-08-07 17:22:02.000000 django-spectator-9.0.1/spectator/core/imagegenerators.py
--rw-r--r--   0 phil       (501) staff       (20)     3778 2018-03-26 14:02:42.000000 django-spectator-9.0.1/spectator/core/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/migrations/
--rw-r--r--   0 phil       (501) staff       (20)     1352 2017-04-17 17:14:55.000000 django-spectator-9.0.1/spectator/core/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      438 2017-11-01 09:03:01.000000 django-spectator-9.0.1/spectator/core/migrations/0002_creator_slug.py
--rw-r--r--   0 phil       (501) staff       (20)      461 2018-01-03 11:42:52.000000 django-spectator-9.0.1/spectator/core/migrations/0003_set_creator_slug.py
--rw-r--r--   0 phil       (501) staff       (20)     1262 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/core/migrations/0004_auto_20180102_0959.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/core/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     5646 2018-04-17 13:06:48.000000 django-spectator-9.0.1/spectator/core/models.py
--rw-r--r--   0 phil       (501) staff       (20)    11256 2017-04-17 12:58:47.000000 django-spectator-9.0.1/spectator/core/paginator.py
--rw-r--r--   0 phil       (501) staff       (20)      273 2017-10-31 17:17:51.000000 django-spectator-9.0.1/spectator/core/sitemaps.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/static/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/static/css/
--rwxr-xr-x   0 phil       (501) staff       (20)   155758 2019-02-13 08:01:40.000000 django-spectator-9.0.1/spectator/core/static/css/bootstrap.min.css
--rwxr-xr-x   0 phil       (501) staff       (20)   625953 2019-02-13 08:01:40.000000 django-spectator-9.0.1/spectator/core/static/css/bootstrap.min.css.map
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/admin/
--rw-r--r--   0 phil       (501) staff       (20)      424 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/admin/detail_thumbnail.html
--rw-r--r--   0 phil       (501) staff       (20)      278 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/admin/list_thumbnail.html
--rw-r--r--   0 phil       (501) staff       (20)     3807 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/base.html
--rw-r--r--   0 phil       (501) staff       (20)     1597 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/creator_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1614 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/creator_list.html
--rw-r--r--   0 phil       (501) staff       (20)      903 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/
--rw-r--r--   0 phil       (501) staff       (20)      452 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/card_change_object_link.html
--rw-r--r--   0 phil       (501) staff       (20)      977 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/card_chart.html
--rw-r--r--   0 phil       (501) staff       (20)      376 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/card_nav.html
--rw-r--r--   0 phil       (501) staff       (20)     1922 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/chart.html
--rw-r--r--   0 phil       (501) staff       (20)      799 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/pager.html
--rw-r--r--   0 phil       (501) staff       (20)     2013 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/pagination.html
--rw-r--r--   0 phil       (501) staff       (20)      661 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/roles.html
--rw-r--r--   0 phil       (501) staff       (20)      692 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/roles_list.html
--rw-r--r--   0 phil       (501) staff       (20)      755 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/thumbnail_detail.html
--rw-r--r--   0 phil       (501) staff       (20)      745 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/thumbnail_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/core/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     5566 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/core/templatetags/spectator_core.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/core/urls/
--rw-r--r--   0 phil       (501) staff       (20)      723 2017-12-14 14:41:37.000000 django-spectator-9.0.1/spectator/core/urls/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      266 2018-03-09 16:41:16.000000 django-spectator-9.0.1/spectator/core/urls/core.py
--rw-r--r--   0 phil       (501) staff       (20)      535 2017-12-14 14:41:03.000000 django-spectator-9.0.1/spectator/core/urls/creators.py
--rw-r--r--   0 phil       (501) staff       (20)     2587 2018-03-10 16:11:32.000000 django-spectator-9.0.1/spectator/core/utils.py
--rw-r--r--   0 phil       (501) staff       (20)     4860 2018-03-10 15:16:25.000000 django-spectator-9.0.1/spectator/core/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/
--rw-r--r--   0 phil       (501) staff       (20)       71 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/events/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     6005 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      272 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)      241 2017-04-17 16:09:32.000000 django-spectator-9.0.1/spectator/events/apps.py
--rw-r--r--   0 phil       (501) staff       (20)     2510 2019-07-31 16:27:46.000000 django-spectator-9.0.1/spectator/events/factories.py
--rw-r--r--   0 phil       (501) staff       (20)     1085 2018-03-10 16:25:45.000000 django-spectator-9.0.1/spectator/events/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/migrations/
--rw-r--r--   0 phil       (501) staff       (20)    21252 2017-04-17 17:14:55.000000 django-spectator-9.0.1/spectator/events/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      503 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/events/migrations/0002_event_slug.py
--rw-r--r--   0 phil       (501) staff       (20)     1145 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/events/migrations/0003_auto_20171101_1645.py
--rw-r--r--   0 phil       (501) staff       (20)      514 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/events/migrations/0004_venue_slug.py
--rw-r--r--   0 phil       (501) staff       (20)      836 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/events/migrations/0005_auto_20180102_0959.py
--rw-r--r--   0 phil       (501) staff       (20)     1307 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/events/migrations/0006_event_slug_20180102_1127.py
--rw-r--r--   0 phil       (501) staff       (20)     2497 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/events/migrations/0007_work_slug_20180102_1137.py
--rw-r--r--   0 phil       (501) staff       (20)     1316 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/events/migrations/0008_venue_slug_20180102_1147.py
--rw-r--r--   0 phil       (501) staff       (20)      477 2018-01-18 09:03:36.000000 django-spectator-9.0.1/spectator/events/migrations/0009_event_note.py
--rw-r--r--   0 phil       (501) staff       (20)      477 2018-01-18 09:06:01.000000 django-spectator-9.0.1/spectator/events/migrations/0010_auto_20180118_0906.py
--rw-r--r--   0 phil       (501) staff       (20)     1489 2018-01-25 14:27:27.000000 django-spectator-9.0.1/spectator/events/migrations/0011_auto_20180125_1348.py
--rw-r--r--   0 phil       (501) staff       (20)     2549 2018-01-25 17:39:32.000000 django-spectator-9.0.1/spectator/events/migrations/0012_add_classical_and_dance_through_models.py
--rw-r--r--   0 phil       (501) staff       (20)     1183 2018-01-25 17:50:38.000000 django-spectator-9.0.1/spectator/events/migrations/0013_copy_classical_and_dance_data.py
--rw-r--r--   0 phil       (501) staff       (20)      622 2018-01-25 17:57:28.000000 django-spectator-9.0.1/spectator/events/migrations/0014_remove_old_classical_dance.py
--rw-r--r--   0 phil       (501) staff       (20)     1208 2018-01-25 17:58:31.000000 django-spectator-9.0.1/spectator/events/migrations/0015_rename_classical_dance_on_event.py
--rw-r--r--   0 phil       (501) staff       (20)     3385 2018-01-26 09:07:59.000000 django-spectator-9.0.1/spectator/events/migrations/0016_add_movies_plays_m2ms_on_event.py
--rw-r--r--   0 phil       (501) staff       (20)      993 2018-01-26 09:14:08.000000 django-spectator-9.0.1/spectator/events/migrations/0017_copy_movies_and_plays_data.py
--rw-r--r--   0 phil       (501) staff       (20)      581 2018-01-26 09:17:01.000000 django-spectator-9.0.1/spectator/events/migrations/0018_remove_old_movie_play_fields.py
--rw-r--r--   0 phil       (501) staff       (20)      840 2018-01-27 16:53:48.000000 django-spectator-9.0.1/spectator/events/migrations/0019_auto_20180127_1653.py
--rw-r--r--   0 phil       (501) staff       (20)      483 2018-01-29 17:32:11.000000 django-spectator-9.0.1/spectator/events/migrations/0020_venue_note.py
--rw-r--r--   0 phil       (501) staff       (20)      488 2018-01-29 17:35:01.000000 django-spectator-9.0.1/spectator/events/migrations/0021_auto_20180129_1735.py
--rw-r--r--   0 phil       (501) staff       (20)      507 2018-01-29 17:52:13.000000 django-spectator-9.0.1/spectator/events/migrations/0022_auto_20180129_1752.py
--rw-r--r--   0 phil       (501) staff       (20)      528 2018-01-31 14:35:49.000000 django-spectator-9.0.1/spectator/events/migrations/0023_venue_cinema_treasures_id.py
--rw-r--r--   0 phil       (501) staff       (20)      878 2018-01-31 16:03:45.000000 django-spectator-9.0.1/spectator/events/migrations/0024_event_venue_name.py
--rw-r--r--   0 phil       (501) staff       (20)      523 2018-01-31 17:55:03.000000 django-spectator-9.0.1/spectator/events/migrations/0025_auto_20180131_1755.py
--rw-r--r--   0 phil       (501) staff       (20)     4182 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0026_auto_20180208_1126.py
--rw-r--r--   0 phil       (501) staff       (20)     1394 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0027_classicalworks_to_works.py
--rw-r--r--   0 phil       (501) staff       (20)     1381 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0028_dancepieces_to_works.py
--rw-r--r--   0 phil       (501) staff       (20)     1336 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0029_plays_to_works.py
--rw-r--r--   0 phil       (501) staff       (20)     1392 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0030_movies_to_works.py
--rw-r--r--   0 phil       (501) staff       (20)      879 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0031_auto_20180208_1412.py
--rw-r--r--   0 phil       (501) staff       (20)     1200 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0032_recreate_work_slugs.py
--rw-r--r--   0 phil       (501) staff       (20)     3705 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0033_auto_20180208_1613.py
--rw-r--r--   0 phil       (501) staff       (20)      669 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/migrations/0034_auto_20180208_1618.py
--rw-r--r--   0 phil       (501) staff       (20)      701 2018-02-14 13:27:02.000000 django-spectator-9.0.1/spectator/events/migrations/0035_change_event_kinds.py
--rw-r--r--   0 phil       (501) staff       (20)      702 2018-04-17 12:18:20.000000 django-spectator-9.0.1/spectator/events/migrations/0036_auto_20180417_1218.py
--rw-r--r--   0 phil       (501) staff       (20)      550 2018-04-17 12:19:55.000000 django-spectator-9.0.1/spectator/events/migrations/0037_exhibition_to_museum.py
--rw-r--r--   0 phil       (501) staff       (20)      674 2018-04-17 12:24:05.000000 django-spectator-9.0.1/spectator/events/migrations/0038_auto_20180417_1224.py
--rw-r--r--   0 phil       (501) staff       (20)     2357 2018-04-17 13:54:08.000000 django-spectator-9.0.1/spectator/events/migrations/0039_populate_exhibitions.py
--rw-r--r--   0 phil       (501) staff       (20)      537 2018-04-17 17:21:44.000000 django-spectator-9.0.1/spectator/events/migrations/0040_auto_20180417_1721.py
--rw-r--r--   0 phil       (501) staff       (20)      486 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/migrations/0041_event_ticket.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/events/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    25950 2019-07-31 16:30:37.000000 django-spectator-9.0.1/spectator/events/models.py
--rw-r--r--   0 phil       (501) staff       (20)      524 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/events/signals.py
--rw-r--r--   0 phil       (501) staff       (20)      848 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/sitemaps.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/static/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/static/css/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/static/css/admin/
--rw-r--r--   0 phil       (501) staff       (20)      105 2017-04-17 12:58:47.000000 django-spectator-9.0.1/spectator/events/static/css/admin/location_picker.css
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/static/js/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/static/js/admin/
--rw-r--r--   0 phil       (501) staff       (20)     5864 2017-05-31 18:15:43.000000 django-spectator-9.0.1/spectator/events/static/js/admin/location_picker.js
--rw-r--r--   0 phil       (501) staff       (20)     1111 2017-04-17 12:58:47.000000 django-spectator-9.0.1/spectator/events/static/js/venue_map.js
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/
--rw-r--r--   0 phil       (501) staff       (20)      982 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/base.html
--rw-r--r--   0 phil       (501) staff       (20)     1287 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/event_archive_year.html
--rw-r--r--   0 phil       (501) staff       (20)     1797 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/event_detail.html
--rw-r--r--   0 phil       (501) staff       (20)      993 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/event_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/
--rw-r--r--   0 phil       (501) staff       (20)     1083 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/card_annual_event_counts.html
--rw-r--r--   0 phil       (501) staff       (20)      450 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/card_events.html
--rw-r--r--   0 phil       (501) staff       (20)      571 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/card_nav.html
--rw-r--r--   0 phil       (501) staff       (20)      955 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/card_years.html
--rw-r--r--   0 phil       (501) staff       (20)     1201 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/event_list_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)      614 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/events.html
--rw-r--r--   0 phil       (501) staff       (20)      590 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/events_paginated.html
--rw-r--r--   0 phil       (501) staff       (20)      626 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/selections.html
--rw-r--r--   0 phil       (501) staff       (20)      890 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/visits.html
--rw-r--r--   0 phil       (501) staff       (20)      492 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/work.html
--rw-r--r--   0 phil       (501) staff       (20)      551 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/works.html
--rw-r--r--   0 phil       (501) staff       (20)      751 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/works_paginated.html
--rw-r--r--   0 phil       (501) staff       (20)     2357 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/venue_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1366 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/venue_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1552 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/work_detail.html
--rw-r--r--   0 phil       (501) staff       (20)      879 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/events/templates/spectator_events/work_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/events/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/events/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7889 2018-04-17 16:34:22.000000 django-spectator-9.0.1/spectator/events/templatetags/spectator_events.py
--rw-r--r--   0 phil       (501) staff       (20)     1434 2018-02-08 17:32:04.000000 django-spectator-9.0.1/spectator/events/urls.py
--rw-r--r--   0 phil       (501) staff       (20)     8036 2018-04-16 16:24:28.000000 django-spectator-9.0.1/spectator/events/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/reading/
--rw-r--r--   0 phil       (501) staff       (20)       73 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/reading/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     3305 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      276 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)      183 2017-04-17 16:10:08.000000 django-spectator-9.0.1/spectator/reading/apps.py
--rw-r--r--   0 phil       (501) staff       (20)     1041 2019-07-31 16:27:12.000000 django-spectator-9.0.1/spectator/reading/factories.py
--rw-r--r--   0 phil       (501) staff       (20)     1805 2018-10-24 14:10:15.000000 django-spectator-9.0.1/spectator/reading/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/reading/migrations/
--rw-r--r--   0 phil       (501) staff       (20)     6022 2017-04-17 17:14:55.000000 django-spectator-9.0.1/spectator/reading/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      516 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/reading/migrations/0002_publicationseries_slug.py
--rw-r--r--   0 phil       (501) staff       (20)      525 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/reading/migrations/0003_publication_slug.py
--rw-r--r--   0 phil       (501) staff       (20)     1833 2018-01-02 12:40:19.000000 django-spectator-9.0.1/spectator/reading/migrations/0004_slugs_20180102_1153.py
--rw-r--r--   0 phil       (501) staff       (20)      639 2018-01-25 13:48:48.000000 django-spectator-9.0.1/spectator/reading/migrations/0005_auto_20180125_1348.py
--rw-r--r--   0 phil       (501) staff       (20)      500 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/migrations/0006_publication_cover.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.0.1/spectator/reading/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     8160 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/models.py
--rw-r--r--   0 phil       (501) staff       (20)      524 2017-10-31 17:17:08.000000 django-spectator-9.0.1/spectator/reading/sitemaps.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/reading/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/
--rw-r--r--   0 phil       (501) staff       (20)      899 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/base.html
--rw-r--r--   0 phil       (501) staff       (20)      979 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/
--rw-r--r--   0 phil       (501) staff       (20)     2528 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/card_annual_reading_counts.html
--rw-r--r--   0 phil       (501) staff       (20)      659 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/card_nav.html
--rw-r--r--   0 phil       (501) staff       (20)      512 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/card_publications.html
--rw-r--r--   0 phil       (501) staff       (20)      968 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/card_years.html
--rw-r--r--   0 phil       (501) staff       (20)     1773 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/publication.html
--rw-r--r--   0 phil       (501) staff       (20)      674 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/publications.html
--rw-r--r--   0 phil       (501) staff       (20)      806 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/publications_paginated.html
--rw-r--r--   0 phil       (501) staff       (20)      246 2017-04-17 12:58:47.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/reading.html
--rw-r--r--   0 phil       (501) staff       (20)     2291 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/publication_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1177 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/publication_list.html
--rw-r--r--   0 phil       (501) staff       (20)      816 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/publicationseries_detail.html
--rw-r--r--   0 phil       (501) staff       (20)      555 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/publicationseries_list.html
--rw-r--r--   0 phil       (501) staff       (20)     2437 2019-07-31 15:52:27.000000 django-spectator-9.0.1/spectator/reading/templates/spectator_reading/reading_archive_year.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-08-07 17:25:26.000000 django-spectator-9.0.1/spectator/reading/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:47.000000 django-spectator-9.0.1/spectator/reading/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     9427 2018-10-24 14:10:15.000000 django-spectator-9.0.1/spectator/reading/templatetags/spectator_reading.py
--rw-r--r--   0 phil       (501) staff       (20)     1283 2018-10-24 14:10:15.000000 django-spectator-9.0.1/spectator/reading/urls.py
--rw-r--r--   0 phil       (501) staff       (20)     2238 2018-10-24 14:10:15.000000 django-spectator-9.0.1/spectator/reading/utils.py
--rw-r--r--   0 phil       (501) staff       (20)     6119 2018-10-24 14:10:15.000000 django-spectator-9.0.1/spectator/reading/views.py
--rw-r--r--   0 phil       (501) staff       (20)     1780 2019-05-05 15:44:55.000000 django-spectator-9.0.1/tox.ini
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:05.000000 django-spectator-9.1.0/
+-rw-r--r--   0 phil       (501) staff       (20)     1356 2019-05-05 18:41:22.000000 django-spectator-9.1.0/.travis.yml
+-rw-r--r--   0 phil       (501) staff       (20)     1079 2017-02-28 18:49:02.000000 django-spectator-9.1.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      267 2017-08-22 14:54:13.000000 django-spectator-9.1.0/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)    23442 2019-10-19 17:03:05.000000 django-spectator-9.1.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)    17904 2019-07-31 15:52:27.000000 django-spectator-9.1.0/README.rst
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/django_spectator.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)    23442 2019-10-19 17:03:04.000000 django-spectator-9.1.0/django_spectator.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     8212 2019-10-19 17:03:04.000000 django-spectator-9.1.0/django_spectator.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2019-10-19 17:03:04.000000 django-spectator-9.1.0/django_spectator.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       65 2019-10-19 17:03:04.000000 django-spectator-9.1.0/django_spectator.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)       10 2019-10-19 17:03:04.000000 django-spectator-9.1.0/django_spectator.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)       38 2019-10-19 17:03:05.000000 django-spectator-9.1.0/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     3063 2019-10-19 16:59:22.000000 django-spectator-9.1.0/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/
+-rw-r--r--   0 phil       (501) staff       (20)      200 2019-10-19 17:02:26.000000 django-spectator-9.1.0/spectator/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/
+-rw-r--r--   0 phil       (501) staff       (20)       67 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/core/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      618 2018-01-02 09:12:05.000000 django-spectator-9.1.0/spectator/core/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      884 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)     1716 2017-04-17 16:10:03.000000 django-spectator-9.1.0/spectator/core/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)      518 2019-07-31 16:19:20.000000 django-spectator-9.1.0/spectator/core/factories.py
+-rw-r--r--   0 phil       (501) staff       (20)     9335 2019-10-19 16:29:25.000000 django-spectator-9.1.0/spectator/core/fields.py
+-rw-r--r--   0 phil       (501) staff       (20)     1329 2019-08-07 17:22:02.000000 django-spectator-9.1.0/spectator/core/imagegenerators.py
+-rw-r--r--   0 phil       (501) staff       (20)     3778 2018-03-26 14:02:42.000000 django-spectator-9.1.0/spectator/core/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)     1352 2017-04-17 17:14:55.000000 django-spectator-9.1.0/spectator/core/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      438 2017-11-01 09:03:01.000000 django-spectator-9.1.0/spectator/core/migrations/0002_creator_slug.py
+-rw-r--r--   0 phil       (501) staff       (20)      461 2018-01-03 11:42:52.000000 django-spectator-9.1.0/spectator/core/migrations/0003_set_creator_slug.py
+-rw-r--r--   0 phil       (501) staff       (20)     1262 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/core/migrations/0004_auto_20180102_0959.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/core/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     5646 2018-04-17 13:06:48.000000 django-spectator-9.1.0/spectator/core/models.py
+-rw-r--r--   0 phil       (501) staff       (20)    11256 2017-04-17 12:58:47.000000 django-spectator-9.1.0/spectator/core/paginator.py
+-rw-r--r--   0 phil       (501) staff       (20)      273 2017-10-31 17:17:51.000000 django-spectator-9.1.0/spectator/core/sitemaps.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/static/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/static/css/
+-rwxr-xr-x   0 phil       (501) staff       (20)   155758 2019-02-13 08:01:40.000000 django-spectator-9.1.0/spectator/core/static/css/bootstrap.min.css
+-rwxr-xr-x   0 phil       (501) staff       (20)   625953 2019-02-13 08:01:40.000000 django-spectator-9.1.0/spectator/core/static/css/bootstrap.min.css.map
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/admin/
+-rw-r--r--   0 phil       (501) staff       (20)      424 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/admin/detail_thumbnail.html
+-rw-r--r--   0 phil       (501) staff       (20)      278 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/admin/list_thumbnail.html
+-rw-r--r--   0 phil       (501) staff       (20)     3807 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     1597 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/creator_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1614 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/creator_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      903 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/
+-rw-r--r--   0 phil       (501) staff       (20)      452 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/card_change_object_link.html
+-rw-r--r--   0 phil       (501) staff       (20)      977 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/card_chart.html
+-rw-r--r--   0 phil       (501) staff       (20)      376 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/card_nav.html
+-rw-r--r--   0 phil       (501) staff       (20)     1922 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/chart.html
+-rw-r--r--   0 phil       (501) staff       (20)      799 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/pager.html
+-rw-r--r--   0 phil       (501) staff       (20)     2013 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/pagination.html
+-rw-r--r--   0 phil       (501) staff       (20)      661 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/roles.html
+-rw-r--r--   0 phil       (501) staff       (20)      692 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/roles_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      755 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/thumbnail_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)      760 2019-10-19 16:09:33.000000 django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/thumbnail_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/core/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     5566 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/core/templatetags/spectator_core.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/core/urls/
+-rw-r--r--   0 phil       (501) staff       (20)      723 2017-12-14 14:41:37.000000 django-spectator-9.1.0/spectator/core/urls/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      266 2018-03-09 16:41:16.000000 django-spectator-9.1.0/spectator/core/urls/core.py
+-rw-r--r--   0 phil       (501) staff       (20)      535 2017-12-14 14:41:03.000000 django-spectator-9.1.0/spectator/core/urls/creators.py
+-rw-r--r--   0 phil       (501) staff       (20)     2587 2018-03-10 16:11:32.000000 django-spectator-9.1.0/spectator/core/utils.py
+-rw-r--r--   0 phil       (501) staff       (20)     4860 2018-03-10 15:16:25.000000 django-spectator-9.1.0/spectator/core/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/
+-rw-r--r--   0 phil       (501) staff       (20)       71 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/events/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     6005 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      272 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)      241 2017-04-17 16:09:32.000000 django-spectator-9.1.0/spectator/events/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)     2510 2019-07-31 16:27:46.000000 django-spectator-9.1.0/spectator/events/factories.py
+-rw-r--r--   0 phil       (501) staff       (20)     1085 2018-03-10 16:25:45.000000 django-spectator-9.1.0/spectator/events/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)    21252 2017-04-17 17:14:55.000000 django-spectator-9.1.0/spectator/events/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      503 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/events/migrations/0002_event_slug.py
+-rw-r--r--   0 phil       (501) staff       (20)     1145 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/events/migrations/0003_auto_20171101_1645.py
+-rw-r--r--   0 phil       (501) staff       (20)      514 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/events/migrations/0004_venue_slug.py
+-rw-r--r--   0 phil       (501) staff       (20)      836 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/events/migrations/0005_auto_20180102_0959.py
+-rw-r--r--   0 phil       (501) staff       (20)     1307 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/events/migrations/0006_event_slug_20180102_1127.py
+-rw-r--r--   0 phil       (501) staff       (20)     2497 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/events/migrations/0007_work_slug_20180102_1137.py
+-rw-r--r--   0 phil       (501) staff       (20)     1316 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/events/migrations/0008_venue_slug_20180102_1147.py
+-rw-r--r--   0 phil       (501) staff       (20)      477 2018-01-18 09:03:36.000000 django-spectator-9.1.0/spectator/events/migrations/0009_event_note.py
+-rw-r--r--   0 phil       (501) staff       (20)      477 2018-01-18 09:06:01.000000 django-spectator-9.1.0/spectator/events/migrations/0010_auto_20180118_0906.py
+-rw-r--r--   0 phil       (501) staff       (20)     1489 2018-01-25 14:27:27.000000 django-spectator-9.1.0/spectator/events/migrations/0011_auto_20180125_1348.py
+-rw-r--r--   0 phil       (501) staff       (20)     2549 2018-01-25 17:39:32.000000 django-spectator-9.1.0/spectator/events/migrations/0012_add_classical_and_dance_through_models.py
+-rw-r--r--   0 phil       (501) staff       (20)     1183 2018-01-25 17:50:38.000000 django-spectator-9.1.0/spectator/events/migrations/0013_copy_classical_and_dance_data.py
+-rw-r--r--   0 phil       (501) staff       (20)      622 2018-01-25 17:57:28.000000 django-spectator-9.1.0/spectator/events/migrations/0014_remove_old_classical_dance.py
+-rw-r--r--   0 phil       (501) staff       (20)     1208 2018-01-25 17:58:31.000000 django-spectator-9.1.0/spectator/events/migrations/0015_rename_classical_dance_on_event.py
+-rw-r--r--   0 phil       (501) staff       (20)     3385 2018-01-26 09:07:59.000000 django-spectator-9.1.0/spectator/events/migrations/0016_add_movies_plays_m2ms_on_event.py
+-rw-r--r--   0 phil       (501) staff       (20)      993 2018-01-26 09:14:08.000000 django-spectator-9.1.0/spectator/events/migrations/0017_copy_movies_and_plays_data.py
+-rw-r--r--   0 phil       (501) staff       (20)      581 2018-01-26 09:17:01.000000 django-spectator-9.1.0/spectator/events/migrations/0018_remove_old_movie_play_fields.py
+-rw-r--r--   0 phil       (501) staff       (20)      840 2018-01-27 16:53:48.000000 django-spectator-9.1.0/spectator/events/migrations/0019_auto_20180127_1653.py
+-rw-r--r--   0 phil       (501) staff       (20)      483 2018-01-29 17:32:11.000000 django-spectator-9.1.0/spectator/events/migrations/0020_venue_note.py
+-rw-r--r--   0 phil       (501) staff       (20)      488 2018-01-29 17:35:01.000000 django-spectator-9.1.0/spectator/events/migrations/0021_auto_20180129_1735.py
+-rw-r--r--   0 phil       (501) staff       (20)      507 2018-01-29 17:52:13.000000 django-spectator-9.1.0/spectator/events/migrations/0022_auto_20180129_1752.py
+-rw-r--r--   0 phil       (501) staff       (20)      528 2018-01-31 14:35:49.000000 django-spectator-9.1.0/spectator/events/migrations/0023_venue_cinema_treasures_id.py
+-rw-r--r--   0 phil       (501) staff       (20)      878 2018-01-31 16:03:45.000000 django-spectator-9.1.0/spectator/events/migrations/0024_event_venue_name.py
+-rw-r--r--   0 phil       (501) staff       (20)      523 2018-01-31 17:55:03.000000 django-spectator-9.1.0/spectator/events/migrations/0025_auto_20180131_1755.py
+-rw-r--r--   0 phil       (501) staff       (20)     4182 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0026_auto_20180208_1126.py
+-rw-r--r--   0 phil       (501) staff       (20)     1394 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0027_classicalworks_to_works.py
+-rw-r--r--   0 phil       (501) staff       (20)     1381 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0028_dancepieces_to_works.py
+-rw-r--r--   0 phil       (501) staff       (20)     1336 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0029_plays_to_works.py
+-rw-r--r--   0 phil       (501) staff       (20)     1392 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0030_movies_to_works.py
+-rw-r--r--   0 phil       (501) staff       (20)      879 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0031_auto_20180208_1412.py
+-rw-r--r--   0 phil       (501) staff       (20)     1200 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0032_recreate_work_slugs.py
+-rw-r--r--   0 phil       (501) staff       (20)     3705 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0033_auto_20180208_1613.py
+-rw-r--r--   0 phil       (501) staff       (20)      669 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/migrations/0034_auto_20180208_1618.py
+-rw-r--r--   0 phil       (501) staff       (20)      701 2018-02-14 13:27:02.000000 django-spectator-9.1.0/spectator/events/migrations/0035_change_event_kinds.py
+-rw-r--r--   0 phil       (501) staff       (20)      702 2018-04-17 12:18:20.000000 django-spectator-9.1.0/spectator/events/migrations/0036_auto_20180417_1218.py
+-rw-r--r--   0 phil       (501) staff       (20)      550 2018-04-17 12:19:55.000000 django-spectator-9.1.0/spectator/events/migrations/0037_exhibition_to_museum.py
+-rw-r--r--   0 phil       (501) staff       (20)      674 2018-04-17 12:24:05.000000 django-spectator-9.1.0/spectator/events/migrations/0038_auto_20180417_1224.py
+-rw-r--r--   0 phil       (501) staff       (20)     2357 2018-04-17 13:54:08.000000 django-spectator-9.1.0/spectator/events/migrations/0039_populate_exhibitions.py
+-rw-r--r--   0 phil       (501) staff       (20)      537 2018-04-17 17:21:44.000000 django-spectator-9.1.0/spectator/events/migrations/0040_auto_20180417_1721.py
+-rw-r--r--   0 phil       (501) staff       (20)      486 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/migrations/0041_event_ticket.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/events/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    25950 2019-07-31 16:30:37.000000 django-spectator-9.1.0/spectator/events/models.py
+-rw-r--r--   0 phil       (501) staff       (20)      524 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/events/signals.py
+-rw-r--r--   0 phil       (501) staff       (20)      848 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/sitemaps.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/static/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/static/css/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/static/css/admin/
+-rw-r--r--   0 phil       (501) staff       (20)      105 2017-04-17 12:58:47.000000 django-spectator-9.1.0/spectator/events/static/css/admin/location_picker.css
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/static/js/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/static/js/admin/
+-rw-r--r--   0 phil       (501) staff       (20)     5864 2017-05-31 18:15:43.000000 django-spectator-9.1.0/spectator/events/static/js/admin/location_picker.js
+-rw-r--r--   0 phil       (501) staff       (20)     1111 2017-04-17 12:58:47.000000 django-spectator-9.1.0/spectator/events/static/js/venue_map.js
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/
+-rw-r--r--   0 phil       (501) staff       (20)      982 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     1287 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/event_archive_year.html
+-rw-r--r--   0 phil       (501) staff       (20)     1797 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/event_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)      993 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/event_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/
+-rw-r--r--   0 phil       (501) staff       (20)     1083 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/card_annual_event_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)      450 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/card_events.html
+-rw-r--r--   0 phil       (501) staff       (20)      571 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/card_nav.html
+-rw-r--r--   0 phil       (501) staff       (20)      955 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/card_years.html
+-rw-r--r--   0 phil       (501) staff       (20)     1201 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/event_list_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)      614 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/events.html
+-rw-r--r--   0 phil       (501) staff       (20)      590 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/events_paginated.html
+-rw-r--r--   0 phil       (501) staff       (20)      626 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/selections.html
+-rw-r--r--   0 phil       (501) staff       (20)      890 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/visits.html
+-rw-r--r--   0 phil       (501) staff       (20)      492 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/work.html
+-rw-r--r--   0 phil       (501) staff       (20)      551 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/works.html
+-rw-r--r--   0 phil       (501) staff       (20)      751 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/works_paginated.html
+-rw-r--r--   0 phil       (501) staff       (20)     2357 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/venue_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1366 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/venue_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1552 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/work_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)      879 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/events/templates/spectator_events/work_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/events/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/events/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7889 2018-04-17 16:34:22.000000 django-spectator-9.1.0/spectator/events/templatetags/spectator_events.py
+-rw-r--r--   0 phil       (501) staff       (20)     1434 2018-02-08 17:32:04.000000 django-spectator-9.1.0/spectator/events/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)     8036 2018-04-16 16:24:28.000000 django-spectator-9.1.0/spectator/events/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/reading/
+-rw-r--r--   0 phil       (501) staff       (20)       73 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/reading/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     3305 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      276 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)      183 2017-04-17 16:10:08.000000 django-spectator-9.1.0/spectator/reading/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)     1041 2019-07-31 16:27:12.000000 django-spectator-9.1.0/spectator/reading/factories.py
+-rw-r--r--   0 phil       (501) staff       (20)     1805 2018-10-24 14:10:15.000000 django-spectator-9.1.0/spectator/reading/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/reading/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)     6022 2017-04-17 17:14:55.000000 django-spectator-9.1.0/spectator/reading/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      516 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/reading/migrations/0002_publicationseries_slug.py
+-rw-r--r--   0 phil       (501) staff       (20)      525 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/reading/migrations/0003_publication_slug.py
+-rw-r--r--   0 phil       (501) staff       (20)     1833 2018-01-02 12:40:19.000000 django-spectator-9.1.0/spectator/reading/migrations/0004_slugs_20180102_1153.py
+-rw-r--r--   0 phil       (501) staff       (20)      639 2018-01-25 13:48:48.000000 django-spectator-9.1.0/spectator/reading/migrations/0005_auto_20180125_1348.py
+-rw-r--r--   0 phil       (501) staff       (20)      500 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/migrations/0006_publication_cover.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:46.000000 django-spectator-9.1.0/spectator/reading/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     8311 2019-10-19 15:50:32.000000 django-spectator-9.1.0/spectator/reading/models.py
+-rw-r--r--   0 phil       (501) staff       (20)      524 2017-10-31 17:17:08.000000 django-spectator-9.1.0/spectator/reading/sitemaps.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:04.000000 django-spectator-9.1.0/spectator/reading/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:05.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/
+-rw-r--r--   0 phil       (501) staff       (20)      899 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/base.html
+-rw-r--r--   0 phil       (501) staff       (20)      979 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:05.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/
+-rw-r--r--   0 phil       (501) staff       (20)     2528 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/card_annual_reading_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)      659 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/card_nav.html
+-rw-r--r--   0 phil       (501) staff       (20)      512 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/card_publications.html
+-rw-r--r--   0 phil       (501) staff       (20)      968 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/card_years.html
+-rw-r--r--   0 phil       (501) staff       (20)     1773 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/publication.html
+-rw-r--r--   0 phil       (501) staff       (20)      674 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/publications.html
+-rw-r--r--   0 phil       (501) staff       (20)      806 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/publications_paginated.html
+-rw-r--r--   0 phil       (501) staff       (20)      246 2017-04-17 12:58:47.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/reading.html
+-rw-r--r--   0 phil       (501) staff       (20)     2291 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/publication_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1177 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/publication_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      816 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/publicationseries_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)      555 2019-07-31 15:52:27.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/publicationseries_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     2613 2019-10-19 15:56:41.000000 django-spectator-9.1.0/spectator/reading/templates/spectator_reading/reading_archive_year.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2019-10-19 17:03:05.000000 django-spectator-9.1.0/spectator/reading/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-04-17 12:58:47.000000 django-spectator-9.1.0/spectator/reading/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     9427 2018-10-24 14:10:15.000000 django-spectator-9.1.0/spectator/reading/templatetags/spectator_reading.py
+-rw-r--r--   0 phil       (501) staff       (20)     1283 2018-10-24 14:10:15.000000 django-spectator-9.1.0/spectator/reading/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)     2238 2018-10-24 14:10:15.000000 django-spectator-9.1.0/spectator/reading/utils.py
+-rw-r--r--   0 phil       (501) staff       (20)     6620 2019-10-19 15:57:57.000000 django-spectator-9.1.0/spectator/reading/views.py
+-rw-r--r--   0 phil       (501) staff       (20)     1780 2019-05-05 15:44:55.000000 django-spectator-9.1.0/tox.ini
```

### Comparing `django-spectator-9.0.1/.travis.yml` & `django-spectator-9.1.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/LICENSE` & `django-spectator-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/PKG-INFO` & `django-spectator-9.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-spectator
-Version: 9.0.1
+Version: 9.1.0
 Summary: A Django app to track book reading, movie viewing, gig going, play watching, etc.
 Home-page: https://github.com/philgyford/django-spectator
 Author: Phil Gyford
 Author-email: phil@gyford.com
 License: MIT
 Description: ==================
          Django Spectator
```

### Comparing `django-spectator-9.0.1/README.rst` & `django-spectator-9.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/django_spectator.egg-info/PKG-INFO` & `django-spectator-9.1.0/django_spectator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-spectator
-Version: 9.0.1
+Version: 9.1.0
 Summary: A Django app to track book reading, movie viewing, gig going, play watching, etc.
 Home-page: https://github.com/philgyford/django-spectator
 Author: Phil Gyford
 Author-email: phil@gyford.com
 License: MIT
 Description: ==================
          Django Spectator
```

### Comparing `django-spectator-9.0.1/django_spectator.egg-info/SOURCES.txt` & `django-spectator-9.1.0/django_spectator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/setup.py` & `django-spectator-9.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 setup(
     name="django-spectator",
     version=get_version(),
     packages=["spectator"],
     install_requires=[
         "django-imagekit>=4.0,<4.1",
         "hashids>=1.2.0,<1.3",
-        "pillow>=6.1.0,<6.2",
+        "pillow>=6.1.0,<6.3",
     ],
     dependency_links=[],
     tests_require=[
         "factory-boy>=2.11.1,<3.0",
         "freezegun>=0.3.11,<0.4",
         "coverage"
     ],
```

### Comparing `django-spectator-9.0.1/spectator/core/admin.py` & `django-spectator-9.1.0/spectator/core/admin.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/app_settings.py` & `django-spectator-9.1.0/spectator/core/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/apps.py` & `django-spectator-9.1.0/spectator/core/apps.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/factories.py` & `django-spectator-9.1.0/spectator/core/factories.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/fields.py` & `django-spectator-9.1.0/spectator/core/fields.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 from .utils import truncate_string
 
 logger = logging.getLogger(__name__)
 
 
 class UniqueFieldMixin(object):
     """
-    Taken from https://github.com/django-extensions/django-extensions/blob/b5404a4a5ed3a5893727b3be3d6a50bc21c534e3/django_extensions/db/fields/__init__.py
+    Taken from https://github.com/django-extensions/django-extensions/blob/b5404a4a5ed3a5893727b3be3d6a50bc21c534e3/django_extensions/db/fields/__init__.py  # noqa: E501
     """
 
     def check_is_bool(self, attrname):
         if not isinstance(getattr(self, attrname), bool):
             raise ValueError("'{}' argument must be True or False".format(attrname))
 
     @staticmethod
     def _get_fields(model_cls):
         return [
-            (f, f.model if f.model != model_cls else None) for f in model_cls._meta.get_fields()
+            (f, f.model if f.model != model_cls else None)
+            for f in model_cls._meta.get_fields()
             if not f.is_relation or f.one_to_one or (f.many_to_one and f.related_model)
         ]
 
     def get_queryset(self, model_cls, slug_field):
         for field, model in self._get_fields(model_cls):
             if model and field == slug_field:
                 return model._default_manager.all()
@@ -100,20 +101,20 @@
 
     def __init__(self, for_field, *args, **kwargs):
         """
         for_field - The name of the field to base this field's string on.
                     e.g. 'title' or 'name'.
         """
         self.for_field = for_field
-        kwargs.setdefault('db_index', True)
-        kwargs.setdefault('editable', False)
-        kwargs.setdefault('max_length', 255)
+        kwargs.setdefault("db_index", True)
+        kwargs.setdefault("editable", False)
+        kwargs.setdefault("max_length", 255)
 
         # For use in pre_save()
-        self.max_length = kwargs['max_length']
+        self.max_length = kwargs["max_length"]
 
         super(NaturalSortField, self).__init__(**kwargs)
 
     def deconstruct(self):
         name, path, args, kwargs = super().deconstruct()
         args.append(self.for_field)
         return name, path, args, kwargs
@@ -121,132 +122,169 @@
     def pre_save(self, model_instance, add):
         try:
             string = getattr(model_instance, self.for_field)
         except AttributeError as e:
             # During migrations a model being saved does not have access
             # to any of its methods. So we can't access, for example,
             # the @property Event.title_to_sort()
-            logger.error("Error in NaturalSortField.pre_save(): {}: The value of the '{}' field will not be changed.".format(e, self.attname))
+            logger.error(
+                "Error in NaturalSortField.pre_save(): {}: "
+                "The value of the '{}' field will not be changed.".format(
+                    e, self.attname
+                )
+            )
 
             string = getattr(model_instance, self.attname)
         else:
             string = string.strip()
 
-            if hasattr(model_instance, 'sort_as') and model_instance.sort_as == 'person':
+            if (
+                hasattr(model_instance, "sort_as")
+                and model_instance.sort_as == "person"
+            ):
                 string = self.naturalize_person(string)
                 # The case of the name is important, so we lowercase afterwards:
                 string = string.lower()
             else:
                 string = string.lower()
                 string = self.naturalize_thing(string)
 
         # Ensure the string isn't over long:
-        string = truncate_string(string, chars=self.max_length, truncate='…', at_word_boundary=True)
+        string = truncate_string(
+            string, chars=self.max_length, truncate="…", at_word_boundary=True
+        )
 
         return string
 
     def naturalize_thing(self, string):
         """
         Make a naturalized version of a general string, not a person's name.
         e.g., title of a book, a band's name, etc.
 
         string -- a lowercase string.
         """
 
         # Things we want to move to the back of the string:
         articles = [
-                        'a', 'an', 'the',
-                        'un', 'une', 'le', 'la', 'les', "l'", "l’",
-                        'ein', 'eine', 'der', 'die', 'das',
-                        'una', 'el', 'los', 'las',
-                    ]
+            "a",
+            "an",
+            "the",
+            "un",
+            "une",
+            "le",
+            "la",
+            "les",
+            "l'",
+            "l’",
+            "ein",
+            "eine",
+            "der",
+            "die",
+            "das",
+            "una",
+            "el",
+            "los",
+            "las",
+        ]
+
+        parentheses = ""  # (1)
 
         sort_string = string
-        parts = string.split(' ')
+        parts = string.split(" ")
+
+        if parts[-1].startswith("("):
+            # Remove so we can add it back at the end.
+            parentheses = parts.pop()
 
         if len(parts) > 1 and parts[0] in articles:
             if parts[0] != parts[1]:
                 # Don't do this if the name is 'The The' or 'La La Land'.
                 # Makes 'long blondes, the':
-                sort_string = '{}, {}'.format(' '.join(parts[1:]), parts[0])
+                sort_string = "{}, {}".format(" ".join(parts[1:]), parts[0])
+
+        if parentheses:
+            # Add it back on.
+            sort_string = "{} {}".format(sort_string, parentheses)
 
         sort_string = self._naturalize_numbers(sort_string)
 
         return sort_string
 
     def naturalize_person(self, string):
         """
         Attempt to make a version of the string that has the surname, if any,
         at the start.
 
-        'John, Brown' to 'Brown, John'
-        'Sir John Brown Jr' to 'Brown, Sir John Jr'
-        'Prince' to 'Prince'
+        'John, Brown' to 'brown, john'
+        'Sir John Brown Jr' to 'brown, sir john jr'
+        'Prince' to 'prince'
+        'Sam Taylor (1)' to 'taylor, sam (00000001)'
 
         string -- The string to change.
         """
-        suffixes = [
-                    'Jr', 'Jr.', 'Sr', 'Sr.',
-                    'I', 'II', 'III', 'IV', 'V',
-                    ]
+        suffixes = ["Jr", "Jr.", "Sr", "Sr.", "I", "II", "III", "IV", "V"]
         # Add lowercase versions:
         suffixes = suffixes + [s.lower() for s in suffixes]
 
         # If a name has a capitalised particle in we use that to sort.
         # So 'Le Carre, John' but 'Carre, John le'.
-        particles = [
-                    'Le', 'La',
-                    'Von', 'Van',
-                    'Du', 'De',
-                    ]
-
-        surname = '' # Smith
-        names = ''   # Fred James
-        suffix = ''  # Jr
+        particles = ["Le", "La", "Von", "Van", "Du", "De"]
+
+        suffix = ""  # Jr
+        parentheses = ""  # (1)
 
         sort_string = string
-        parts = string.split(' ')
+        parts = string.split(" ")
+
+        if parts[-1].startswith("("):
+            # Remove so we can add it back at the end.
+            parentheses = parts.pop()
 
         if parts[-1] in suffixes:
             # Remove suffixes entirely, as we'll add them back on the end.
             suffix = parts[-1]
-            parts = parts[0:-1] # Remove suffix from parts
-            sort_string = ' '.join(parts)
+            parts = parts[0:-1]  # Remove suffix from parts
+            sort_string = " ".join(parts)
 
         if len(parts) > 1:
 
             if parts[-2] in particles:
                 # From ['Alan', 'Barry', 'Le', 'Carré']
                 # to   ['Alan', 'Barry', 'Le Carré']:
-                parts = parts[0:-2] + [ ' '.join(parts[-2:]) ]
+                parts = parts[0:-2] + [" ".join(parts[-2:])]
 
             # From 'David Foster Wallace' to 'Wallace, David Foster':
-            sort_string = '{}, {}'.format(parts[-1], ' '.join(parts[:-1]))
+            sort_string = "{}, {}".format(parts[-1], " ".join(parts[:-1]))
 
         if suffix:
             # Add it back on.
-            sort_string = '{} {}'.format(sort_string, suffix)
+            sort_string = "{} {}".format(sort_string, suffix)
+
+        if parentheses:
+            # Add it back on.
+            sort_string = "{} {}".format(sort_string, parentheses)
 
         # In case this name has any numbers in it.
         sort_string = self._naturalize_numbers(sort_string)
 
         return sort_string
 
     def _naturalize_numbers(self, string):
         """
         Makes any integers into very zero-padded numbers.
         e.g. '1' becomes '00000001'.
         """
 
         def naturalize_int_match(match):
-            return '%08d' % (int(match.group(0)),)
+            return "%08d" % (int(match.group(0)),)
 
-        string = re.sub(r'\d+', naturalize_int_match, string)
+        string = re.sub(r"\d+", naturalize_int_match, string)
 
         return string
 
 
 class PersonNaturalSortField(NaturalSortField):
     pass
 
+
 class PersonDisplayNaturalSortField(NaturalSortField):
     pass
```

### Comparing `django-spectator-9.0.1/spectator/core/imagegenerators.py` & `django-spectator-9.1.0/spectator/core/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/managers.py` & `django-spectator-9.1.0/spectator/core/managers.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/migrations/0001_initial.py` & `django-spectator-9.1.0/spectator/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/migrations/0004_auto_20180102_0959.py` & `django-spectator-9.1.0/spectator/core/migrations/0004_auto_20180102_0959.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/models.py` & `django-spectator-9.1.0/spectator/core/models.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/paginator.py` & `django-spectator-9.1.0/spectator/core/paginator.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/static/css/bootstrap.min.css` & `django-spectator-9.1.0/spectator/core/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/static/css/bootstrap.min.css.map` & `django-spectator-9.1.0/spectator/core/static/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/base.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/base.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/creator_detail.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/creator_detail.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/creator_list.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/creator_list.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/home.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/home.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/card_chart.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/card_chart.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/chart.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/chart.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/pager.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/pager.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/pagination.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/roles.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/roles.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/roles_list.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/roles_list.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/thumbnail_detail.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/thumbnail_detail.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/templates/spectator_core/includes/thumbnail_list.html` & `django-spectator-9.1.0/spectator/core/templates/spectator_core/includes/thumbnail_list.html`

 * *Files 3% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 {% load imagekit %}
 
 {% generateimage 'spectator:list_thumbnail' source=field as img %}
 {% generateimage 'spectator:list_thumbnail2x' source=field as img2x %}
 
 {% with link_url=url|default:field.url %}
   <a href="{{ link_url }}">
-    <img src="{{ img.url }}" srcset="{{ img.url }} 1x, {{ img2x.url }} 2x" width="{{ img.width }}" height="{{ img.height }}" alt="{{ alt_text }}" class="align-top border mr-3">
+    <img src="{{ img.url }}" srcset="{{ img.url }} 1x, {{ img2x.url }} 2x" width="{{ img.width }}" height="{{ img.height }}" alt="{{ alt_text }}" class="align-top border mr-3" loading="lazy">
   </a>
 {% endwith %}
```

### Comparing `django-spectator-9.0.1/spectator/core/templatetags/spectator_core.py` & `django-spectator-9.1.0/spectator/core/templatetags/spectator_core.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/urls/__init__.py` & `django-spectator-9.1.0/spectator/core/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/urls/creators.py` & `django-spectator-9.1.0/spectator/core/urls/creators.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/utils.py` & `django-spectator-9.1.0/spectator/core/utils.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/core/views.py` & `django-spectator-9.1.0/spectator/core/views.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/admin.py` & `django-spectator-9.1.0/spectator/events/admin.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/factories.py` & `django-spectator-9.1.0/spectator/events/factories.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/managers.py` & `django-spectator-9.1.0/spectator/events/managers.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0001_initial.py` & `django-spectator-9.1.0/spectator/events/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0003_auto_20171101_1645.py` & `django-spectator-9.1.0/spectator/events/migrations/0003_auto_20171101_1645.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0004_venue_slug.py` & `django-spectator-9.1.0/spectator/events/migrations/0004_venue_slug.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0005_auto_20180102_0959.py` & `django-spectator-9.1.0/spectator/events/migrations/0005_auto_20180102_0959.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0006_event_slug_20180102_1127.py` & `django-spectator-9.1.0/spectator/events/migrations/0006_event_slug_20180102_1127.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0007_work_slug_20180102_1137.py` & `django-spectator-9.1.0/spectator/events/migrations/0007_work_slug_20180102_1137.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0008_venue_slug_20180102_1147.py` & `django-spectator-9.1.0/spectator/events/migrations/0008_venue_slug_20180102_1147.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0011_auto_20180125_1348.py` & `django-spectator-9.1.0/spectator/events/migrations/0011_auto_20180125_1348.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0012_add_classical_and_dance_through_models.py` & `django-spectator-9.1.0/spectator/events/migrations/0012_add_classical_and_dance_through_models.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0013_copy_classical_and_dance_data.py` & `django-spectator-9.1.0/spectator/events/migrations/0013_copy_classical_and_dance_data.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0014_remove_old_classical_dance.py` & `django-spectator-9.1.0/spectator/events/migrations/0014_remove_old_classical_dance.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0015_rename_classical_dance_on_event.py` & `django-spectator-9.1.0/spectator/events/migrations/0015_rename_classical_dance_on_event.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0016_add_movies_plays_m2ms_on_event.py` & `django-spectator-9.1.0/spectator/events/migrations/0016_add_movies_plays_m2ms_on_event.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0017_copy_movies_and_plays_data.py` & `django-spectator-9.1.0/spectator/events/migrations/0017_copy_movies_and_plays_data.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0018_remove_old_movie_play_fields.py` & `django-spectator-9.1.0/spectator/events/migrations/0018_remove_old_movie_play_fields.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0019_auto_20180127_1653.py` & `django-spectator-9.1.0/spectator/events/migrations/0019_auto_20180127_1653.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0023_venue_cinema_treasures_id.py` & `django-spectator-9.1.0/spectator/events/migrations/0023_venue_cinema_treasures_id.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0024_event_venue_name.py` & `django-spectator-9.1.0/spectator/events/migrations/0024_event_venue_name.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0025_auto_20180131_1755.py` & `django-spectator-9.1.0/spectator/events/migrations/0025_auto_20180131_1755.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0026_auto_20180208_1126.py` & `django-spectator-9.1.0/spectator/events/migrations/0026_auto_20180208_1126.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0027_classicalworks_to_works.py` & `django-spectator-9.1.0/spectator/events/migrations/0027_classicalworks_to_works.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0028_dancepieces_to_works.py` & `django-spectator-9.1.0/spectator/events/migrations/0028_dancepieces_to_works.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0029_plays_to_works.py` & `django-spectator-9.1.0/spectator/events/migrations/0029_plays_to_works.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0030_movies_to_works.py` & `django-spectator-9.1.0/spectator/events/migrations/0030_movies_to_works.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0031_auto_20180208_1412.py` & `django-spectator-9.1.0/spectator/events/migrations/0031_auto_20180208_1412.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0032_recreate_work_slugs.py` & `django-spectator-9.1.0/spectator/events/migrations/0032_recreate_work_slugs.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0033_auto_20180208_1613.py` & `django-spectator-9.1.0/spectator/events/migrations/0033_auto_20180208_1613.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0034_auto_20180208_1618.py` & `django-spectator-9.1.0/spectator/events/migrations/0034_auto_20180208_1618.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0035_change_event_kinds.py` & `django-spectator-9.1.0/spectator/events/migrations/0035_change_event_kinds.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0036_auto_20180417_1218.py` & `django-spectator-9.1.0/spectator/events/migrations/0036_auto_20180417_1218.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0037_exhibition_to_museum.py` & `django-spectator-9.1.0/spectator/events/migrations/0037_exhibition_to_museum.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0038_auto_20180417_1224.py` & `django-spectator-9.1.0/spectator/events/migrations/0038_auto_20180417_1224.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0039_populate_exhibitions.py` & `django-spectator-9.1.0/spectator/events/migrations/0039_populate_exhibitions.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/migrations/0040_auto_20180417_1721.py` & `django-spectator-9.1.0/spectator/events/migrations/0040_auto_20180417_1721.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/models.py` & `django-spectator-9.1.0/spectator/events/models.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/signals.py` & `django-spectator-9.1.0/spectator/events/signals.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/sitemaps.py` & `django-spectator-9.1.0/spectator/events/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/static/js/admin/location_picker.js` & `django-spectator-9.1.0/spectator/events/static/js/admin/location_picker.js`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/static/js/venue_map.js` & `django-spectator-9.1.0/spectator/events/static/js/venue_map.js`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/base.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/base.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/event_archive_year.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/event_archive_year.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/event_detail.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/event_detail.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/event_list.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/event_list.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/card_annual_event_counts.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/card_annual_event_counts.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/card_nav.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/card_nav.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/card_years.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/card_years.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/event_list_tabs.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/event_list_tabs.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/events.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/events.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/events_paginated.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/events_paginated.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/selections.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/selections.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/visits.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/visits.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/works.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/works.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/includes/works_paginated.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/includes/works_paginated.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/venue_detail.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/venue_detail.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/venue_list.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/venue_list.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/work_detail.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/work_detail.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templates/spectator_events/work_list.html` & `django-spectator-9.1.0/spectator/events/templates/spectator_events/work_list.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/templatetags/spectator_events.py` & `django-spectator-9.1.0/spectator/events/templatetags/spectator_events.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/urls.py` & `django-spectator-9.1.0/spectator/events/urls.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/events/views.py` & `django-spectator-9.1.0/spectator/events/views.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/admin.py` & `django-spectator-9.1.0/spectator/reading/admin.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/factories.py` & `django-spectator-9.1.0/spectator/reading/factories.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/managers.py` & `django-spectator-9.1.0/spectator/reading/managers.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/migrations/0001_initial.py` & `django-spectator-9.1.0/spectator/reading/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/migrations/0002_publicationseries_slug.py` & `django-spectator-9.1.0/spectator/reading/migrations/0002_publicationseries_slug.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/migrations/0003_publication_slug.py` & `django-spectator-9.1.0/spectator/reading/migrations/0003_publication_slug.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/migrations/0004_slugs_20180102_1153.py` & `django-spectator-9.1.0/spectator/reading/migrations/0004_slugs_20180102_1153.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/migrations/0005_auto_20180125_1348.py` & `django-spectator-9.1.0/spectator/reading/migrations/0005_auto_20180125_1348.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/models.py` & `django-spectator-9.1.0/spectator/reading/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -252,20 +252,24 @@
 
 
 class Reading(TimeStampedModelMixin, models.Model):
     """
     A period when a Publication was read.
     """
 
+    DATE_GRANULARITY_DAY = 3
+    DATE_GRANULARITY_MONTH = 4
+    DATE_GRANULARITY_YEAR = 6
+
     # Via https://www.flickr.com/services/api/misc.dates.html
     DATE_GRANULARITIES = (
         # (0, 'Y-m-d H:i:s'),
-        (3, "Y-m-d"),
-        (4, "Y-m"),
-        (6, "Y"),
+        (DATE_GRANULARITY_DAY, "Y-m-d"),
+        (DATE_GRANULARITY_MONTH, "Y-m"),
+        (DATE_GRANULARITY_YEAR, "Y"),
         # (8, 'Circa...'),
     )
 
     publication = models.ForeignKey(
         "spectator_reading.Publication",
         null=False,
         blank=False,
```

### Comparing `django-spectator-9.0.1/spectator/reading/sitemaps.py` & `django-spectator-9.1.0/spectator/reading/sitemaps.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/base.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/base.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/home.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/home.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/card_annual_reading_counts.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/card_annual_reading_counts.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/card_nav.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/card_nav.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/card_publications.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/card_publications.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/card_years.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/card_years.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/publication.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/publication.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/publications.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/publications.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/includes/publications_paginated.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/includes/publications_paginated.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/publication_detail.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/publication_detail.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/publication_list.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/publication_list.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/publicationseries_detail.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/publicationseries_detail.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/publicationseries_list.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/publicationseries_list.html`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/templates/spectator_reading/reading_archive_year.html` & `django-spectator-9.1.0/spectator/reading/templates/spectator_reading/reading_archive_year.html`

 * *Files 14% similar despite different names*

```diff
@@ -33,22 +33,29 @@
         </li>
       {% endif %}
     </ul>
   {% endif %}
 
   {% if reading_list|length > 0 %}
 
+    {% if show_months|default_if_none:"True" is False %}
+      <ul>
+    {% endif %}
+
     {% for reading in reading_list %}
-      {% ifchanged reading.end_date|date:"m" %}
-        {% if not forloop.first %}
-          </ul>
-        {% endif %}
-        <h2>{{ reading.end_date|date:"F"}}</h2>
-        <ul>
-      {% endifchanged %}
+
+      {% if show_months|default_if_none:"True" is True %}
+        {% ifchanged reading.end_date|date:"m" %}
+          {% if not forloop.first %}
+            </ul>
+          {% endif %}
+          <h2>{{ reading.end_date|date:"F"}}</h2>
+          <ul>
+        {% endifchanged %}
+      {% endif %}
       <li class="mb-2">
         {% include 'spectator_reading/includes/publication.html' with publication=reading.publication show_readings='none' show_thumbnail=True only %}
       </li>
     {% endfor %}
     </ul>
 
     {% include 'spectator_core/includes/pager.html' with url_name='spectator:reading:reading_year_archive' previous=previous_year next=next_year only %}
```

### Comparing `django-spectator-9.0.1/spectator/reading/templatetags/spectator_reading.py` & `django-spectator-9.1.0/spectator/reading/templatetags/spectator_reading.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/urls.py` & `django-spectator-9.1.0/spectator/reading/urls.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/utils.py` & `django-spectator-9.1.0/spectator/reading/utils.py`

 * *Files identical despite different names*

### Comparing `django-spectator-9.0.1/spectator/reading/views.py` & `django-spectator-9.1.0/spectator/reading/views.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,155 +1,185 @@
 from django.db.models import Min
 from django.http import Http404
 from django.utils.encoding import force_text
 from django.utils.translation import ugettext as _
 from django.views.generic import DetailView, ListView, YearArchiveView
 from django.views.generic.detail import SingleObjectMixin
 
-from spectator.core.models import Creator
 from spectator.core.views import PaginatedListView
 from .models import Publication, PublicationSeries, Reading
 
 
 class ReadingHomeView(ListView):
     model = Publication
-    template_name = 'spectator_reading/home.html'
-    queryset = Publication.unread_objects.select_related('series')\
-                            .prefetch_related('roles__creator').all()
-    ordering = ['time_created',]
+    template_name = "spectator_reading/home.html"
+    queryset = (
+        Publication.unread_objects.select_related("series")
+        .prefetch_related("roles__creator")
+        .all()
+    )
+    ordering = ["time_created"]
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['in_progress_publication_list'] = \
-                                            Publication.in_progress_objects\
-                                            .select_related('series')\
-                                            .prefetch_related('roles__creator')\
-                                            .all()
+        context["in_progress_publication_list"] = (
+            Publication.in_progress_objects.select_related("series")
+            .prefetch_related("roles__creator")
+            .all()
+        )
         return context
 
 
 class PublicationSeriesListView(ListView):
     model = PublicationSeries
 
 
 class PublicationSeriesDetailView(SingleObjectMixin, PaginatedListView):
-    template_name = 'spectator_reading/publicationseries_detail.html'
+    template_name = "spectator_reading/publicationseries_detail.html"
 
     def get(self, request, *args, **kwargs):
         self.object = self.get_object(queryset=PublicationSeries.objects.all())
         return super().get(request, *args, **kwargs)
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['publicationseries'] = self.object
-        context['publication_list'] = context['object_list']
+        context["publicationseries"] = self.object
+        context["publication_list"] = context["object_list"]
         return context
 
     def get_queryset(self):
-        return self.object.publication_set.select_related('series')\
-                            .prefetch_related('roles__creator').all()
+        return (
+            self.object.publication_set.select_related("series")
+            .prefetch_related("roles__creator")
+            .all()
+        )
 
 
 class PublicationListView(PaginatedListView):
     model = Publication
-    publication_kind = 'book'
+    publication_kind = "book"
 
     def get(self, request, *args, **kwargs):
         # Are we should 'book's (default) or 'periodical's?
-        if self.kwargs.get('kind', None) == 'periodical':
-            self.publication_kind = 'periodical'
+        if self.kwargs.get("kind", None) == "periodical":
+            self.publication_kind = "periodical"
         return super().get(request, *args, **kwargs)
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['publication_kind'] = self.publication_kind
-        context['book_count'] = Publication.objects.filter(kind='book').count()
-        context['periodical_count'] = Publication.objects.filter(
-                                                    kind='periodical').count()
+        context["publication_kind"] = self.publication_kind
+        context["book_count"] = Publication.objects.filter(kind="book").count()
+        context["periodical_count"] = Publication.objects.filter(
+            kind="periodical"
+        ).count()
         return context
 
     def get_queryset(self):
         qs = super().get_queryset()
-        qs = qs.filter(kind=self.publication_kind)\
-                .select_related('series')\
-                .prefetch_related('roles__creator')
+        qs = (
+            qs.filter(kind=self.publication_kind)
+            .select_related("series")
+            .prefetch_related("roles__creator")
+        )
         return qs
 
     def get_ordering(self):
-        if self.publication_kind == 'periodical':
-            return ('series__title_sort', 'title_sort',)
+        if self.publication_kind == "periodical":
+            return ("series__title_sort", "title_sort")
         else:
-            return ('title_sort',)
+            return ("title_sort",)
 
 
 class PublicationDetailView(DetailView):
     model = Publication
 
 
 class ReadingYearArchiveView(YearArchiveView):
     allow_empty = True
-    date_field = 'end_date'
+    date_field = "end_date"
     make_object_list = True
     model = Reading
-    ordering = 'end_date'
+    ordering = "end_date"
     # Could be set to 'periodical' or 'book' in get():
     publication_kind = None
     # Will be a QS of all publications finished this year:
     all_publications_queryset = None
 
     def get(self, request, *args, **kwargs):
         # Are we should 'book's (default) or 'periodical's?
-        kind = self.kwargs.get('kind', None)
-        if kind == 'periodicals':
-            self.publication_kind = 'periodical'
-        elif kind == 'books':
-            self.publication_kind = 'book'
+        kind = self.kwargs.get("kind", None)
+        if kind == "periodicals":
+            self.publication_kind = "periodical"
+        elif kind == "books":
+            self.publication_kind = "book"
         elif kind is not None:
             raise Http404("'{}' is not a valid publication kind".format(kind))
 
         return super().get(request, *args, **kwargs)
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
-        context['publication_kind'] = self.publication_kind
+        context["publication_kind"] = self.publication_kind
+
+        context["publication_count"] = self.all_publications_queryset.count()
+        context["book_count"] = self.all_publications_queryset.filter(
+            publication__kind="book"
+        ).count()
+        context["periodical_count"] = self.all_publications_queryset.filter(
+            publication__kind="periodical"
+        ).count()
+
+        # Should we divide the readings up by month in the template?
+        context["show_months"] = True
+
+        objects = context["object_list"]
+        if len(objects) > 1:
+            if (
+                objects.first().end_granularity == Reading.DATE_GRANULARITY_YEAR
+                and objects.last().end_granularity == Reading.DATE_GRANULARITY_YEAR
+            ):
+                # If the first and last publications only have year-based
+                # granularity, assume everything does, so we shouldn't
+                # show the months in the template.
+                context["show_months"] = False
 
-        context['publication_count'] = self.all_publications_queryset.count()
-        context['book_count'] = self.all_publications_queryset \
-                                .filter(publication__kind='book').count()
-        context['periodical_count'] = self.all_publications_queryset \
-                                .filter(publication__kind='periodical').count()
         return context
 
     def get_queryset(self):
         "Reduce the number of queries and speed things up."
         qs = super().get_queryset()
 
-        qs = qs.select_related('publication__series') \
-                .prefetch_related('publication__roles__creator')
+        qs = qs.select_related("publication__series").prefetch_related(
+            "publication__roles__creator"
+        )
 
         return qs
 
     def get_dated_items(self):
         items, qs, info = super().get_dated_items()
 
-        if 'year' in info and info['year']:
+        if "year" in info and info["year"]:
             # Get the earliest date we have a Reading for:
-            end_date_min = Reading.objects.aggregate(
-                                            Min('end_date'))['end_date__min']
+            end_date_min = Reading.objects.aggregate(Min("end_date"))["end_date__min"]
             # Make it a 'yyyy-01-01' date:
             min_year_date = end_date_min.replace(month=1, day=1)
-            if info['year'] < min_year_date:
+            if info["year"] < min_year_date:
                 # The year we're viewing is before our minimum date, so 404.
-                raise Http404(_("No %(verbose_name_plural)s available") % {
-                    'verbose_name_plural': force_text(qs.model._meta.verbose_name_plural)
-                })
-            elif info['year'] == min_year_date:
+                raise Http404(
+                    _("No %(verbose_name_plural)s available")
+                    % {
+                        "verbose_name_plural": force_text(
+                            qs.model._meta.verbose_name_plural
+                        )
+                    }
+                )
+            elif info["year"] == min_year_date:
                 # This is the earliest year we have readings for, so
                 # there is no previous year.
-                info['previous_year'] = None
+                info["previous_year"] = None
 
         # Save the QuerySet for ALL kinds for use in get_context_data():
         self.all_publications_queryset = qs
 
         # Now filter the results if necessary:
         if self.publication_kind is not None:
             qs = qs.filter(publication__kind=self.publication_kind)
```

### Comparing `django-spectator-9.0.1/tox.ini` & `django-spectator-9.1.0/tox.ini`

 * *Files identical despite different names*

