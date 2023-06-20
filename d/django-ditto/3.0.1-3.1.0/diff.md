# Comparing `tmp/django-ditto-3.0.1.tar.gz` & `tmp/django-ditto-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ditto-3.0.1.tar", last modified: Mon May 22 11:19:45 2023, max compression
+gzip compressed data, was "django-ditto-3.1.0.tar", last modified: Tue Jun 20 10:59:04 2023, max compression
```

## Comparing `django-ditto-3.0.1.tar` & `django-ditto-3.1.0.tar`

### file list

```diff
@@ -1,385 +1,385 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.697795 django-ditto-3.0.1/
--rw-r--r--   0 phil       (501) staff       (20)     1083 2021-10-22 16:10:52.000000 django-ditto-3.0.1/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      326 2022-03-25 12:40:03.000000 django-ditto-3.0.1/MANIFEST.in
--rw-r--r--   0 phil       (501) staff       (20)     4266 2023-05-22 11:19:45.697898 django-ditto-3.0.1/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     2454 2023-05-09 16:29:45.000000 django-ditto-3.0.1/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.628518 django-ditto-3.0.1/ditto/
--rw-r--r--   0 phil       (501) staff       (20)      196 2023-05-22 10:58:53.000000 django-ditto-3.0.1/ditto/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.630361 django-ditto-3.0.1/ditto/core/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:28.000000 django-ditto-3.0.1/ditto/core/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      263 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/core/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      708 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/core/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)     1809 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/core/apps.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.623845 django-ditto-3.0.1/ditto/core/management/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.630769 django-ditto-3.0.1/ditto/core/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)     2009 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/core/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)      272 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/core/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.631024 django-ditto-3.0.1/ditto/core/migrations/
--rw-r--r--   0 phil       (501) staff       (20)        0 2020-05-23 15:29:03.000000 django-ditto-3.0.1/ditto/core/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     5469 2022-11-09 15:48:27.000000 django-ditto-3.0.1/ditto/core/models.py
--rw-r--r--   0 phil       (501) staff       (20)    11616 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/core/paginator.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.624043 django-ditto-3.0.1/ditto/core/static/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.624239 django-ditto-3.0.1/ditto/core/static/ditto-core/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.632211 django-ditto-3.0.1/ditto/core/static/ditto-core/css/
--rw-rw-r--   0 phil       (501) staff       (20)   162264 2022-07-19 15:13:44.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/css/bootstrap.min.css
--rw-rw-r--   0 phil       (501) staff       (20)   654593 2022-07-19 15:13:44.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/css/bootstrap.min.css.map
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.633735 django-ditto-3.0.1/ditto/core/static/ditto-core/img/
--rw-r--r--   0 phil       (501) staff       (20)      142 2016-09-06 12:05:37.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/img/default_avatar.png
--rw-r--r--   0 phil       (501) staff       (20)     3520 2016-09-06 12:05:37.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/img/original_error.jpg
--rw-r--r--   0 phil       (501) staff       (20)     3309 2016-09-06 12:05:37.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/img/original_missing.jpg
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.634827 django-ditto-3.0.1/ditto/core/static/ditto-core/js/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.636433 django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/
--rw-rw-r--   0 phil       (501) staff       (20)    20871 2022-07-19 15:13:44.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/carousel.js
--rw-rw-r--   0 phil       (501) staff       (20)    38793 2022-07-19 15:13:44.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/carousel.js.map
--rw-rw-r--   0 phil       (501) staff       (20)    13394 2022-07-19 15:13:44.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/collapse.js
--rw-rw-r--   0 phil       (501) staff       (20)    24048 2022-07-19 15:13:44.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/collapse.js.map
--rw-rw-r--   0 phil       (501) staff       (20)     6631 2022-07-19 15:13:44.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/util.js
--rw-rw-r--   0 phil       (501) staff       (20)    12040 2022-07-19 15:13:44.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/util.js.map
--rw-r--r--   0 phil       (501) staff       (20)    72380 2020-05-24 12:52:06.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.js
--rw-r--r--   0 phil       (501) staff       (20)   110382 2020-05-24 12:52:06.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.map
--rw-r--r--   0 phil       (501) staff       (20)    21233 2020-11-19 17:03:58.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/popper.min.js
--rw-r--r--   0 phil       (501) staff       (20)   117179 2018-04-16 15:41:13.000000 django-ditto-3.0.1/ditto/core/static/ditto-core/js/popper.min.js.map
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.624422 django-ditto-3.0.1/ditto/core/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.637516 django-ditto-3.0.1/ditto/core/templates/ditto/
--rw-r--r--   0 phil       (501) staff       (20)     2230 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/archive_day.html
--rw-r--r--   0 phil       (501) staff       (20)     4738 2020-08-10 13:47:31.000000 django-ditto-3.0.1/ditto/core/templates/ditto/base.html
--rw-r--r--   0 phil       (501) staff       (20)     1029 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.638990 django-ditto-3.0.1/ditto/core/templates/ditto/includes/
--rw-r--r--   0 phil       (501) staff       (20)      643 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/includes/account_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1180 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/includes/item_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1760 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/includes/item_lists.html
--rw-r--r--   0 phil       (501) staff       (20)     1108 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/includes/pager.html
--rw-r--r--   0 phil       (501) staff       (20)     2478 2017-08-22 13:41:35.000000 django-ditto-3.0.1/ditto/core/templates/ditto/includes/pagination.html
--rw-r--r--   0 phil       (501) staff       (20)     2272 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/includes/variety_nav.html
--rw-r--r--   0 phil       (501) staff       (20)      681 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/tag_detail.html
--rw-r--r--   0 phil       (501) staff       (20)      399 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/core/templates/ditto/tag_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.639218 django-ditto-3.0.1/ditto/core/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.0.1/ditto/core/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     5149 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/core/templatetags/ditto_core.py
--rw-r--r--   0 phil       (501) staff       (20)      634 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/core/urls.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.639650 django-ditto-3.0.1/ditto/core/utils/
--rw-r--r--   0 phil       (501) staff       (20)     3510 2023-05-09 16:23:11.000000 django-ditto-3.0.1/ditto/core/utils/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     3509 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/core/utils/downloader.py
--rw-r--r--   0 phil       (501) staff       (20)    23806 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/core/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.642567 django-ditto-3.0.1/ditto/flickr/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:33.000000 django-ditto-3.0.1/ditto/flickr/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    12102 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      444 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)      345 2021-04-07 17:01:46.000000 django-ditto-3.0.1/ditto/flickr/apps.py
--rw-r--r--   0 phil       (501) staff       (20)      881 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/checks.py
--rw-r--r--   0 phil       (501) staff       (20)     4046 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/factories.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.643689 django-ditto-3.0.1/ditto/flickr/fetch/
--rw-r--r--   0 phil       (501) staff       (20)       38 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/fetch/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    20064 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/fetch/fetchers.py
--rw-r--r--   0 phil       (501) staff       (20)     4656 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/fetch/filesfetchers.py
--rw-r--r--   0 phil       (501) staff       (20)     4508 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/fetch/multifetchers.py
--rw-r--r--   0 phil       (501) staff       (20)    16307 2023-05-09 16:24:02.000000 django-ditto-3.0.1/ditto/flickr/fetch/savers.py
--rw-r--r--   0 phil       (501) staff       (20)     3065 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/imagegenerators.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.624956 django-ditto-3.0.1/ditto/flickr/management/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.644756 django-ditto-3.0.1/ditto/flickr/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)     2892 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2641 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/management/commands/fetch_flickr_account_user.py
--rw-r--r--   0 phil       (501) staff       (20)     1424 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/management/commands/fetch_flickr_originals.py
--rw-r--r--   0 phil       (501) staff       (20)     1440 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/management/commands/fetch_flickr_photos.py
--rw-r--r--   0 phil       (501) staff       (20)      855 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/management/commands/fetch_flickr_photosets.py
--rw-r--r--   0 phil       (501) staff       (20)     1923 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.651125 django-ditto-3.0.1/ditto/flickr/migrations/
--rw-r--r--   0 phil       (501) staff       (20)    23757 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      426 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0002_auto_20160406_1548.py
--rw-r--r--   0 phil       (501) staff       (20)     1069 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0003_auto_20160413_0906.py
--rw-r--r--   0 phil       (501) staff       (20)     4134 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0004_auto_20160414_1120.py
--rw-r--r--   0 phil       (501) staff       (20)     7502 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0005_auto_20160414_1427.py
--rw-r--r--   0 phil       (501) staff       (20)      556 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0006_auto_20160414_1459.py
--rw-r--r--   0 phil       (501) staff       (20)      703 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0007_auto_20160414_1637.py
--rw-r--r--   0 phil       (501) staff       (20)     4347 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0008_auto_20160429_1559.py
--rw-r--r--   0 phil       (501) staff       (20)      584 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0009_photoset_fetch_time.py
--rw-r--r--   0 phil       (501) staff       (20)      463 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0010_photo_photosets.py
--rw-r--r--   0 phil       (501) staff       (20)     1042 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0011_auto_20160502_1645.py
--rw-r--r--   0 phil       (501) staff       (20)     1205 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0012_auto_20160503_1457.py
--rw-r--r--   0 phil       (501) staff       (20)      539 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0013_photoset_photos_raw.py
--rw-r--r--   0 phil       (501) staff       (20)      569 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0014_photo_original_file.py
--rw-r--r--   0 phil       (501) staff       (20)      572 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0015_auto_20160514_1456.py
--rw-r--r--   0 phil       (501) staff       (20)      662 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0016_photo_video_original_file.py
--rw-r--r--   0 phil       (501) staff       (20)      856 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0017_auto_20160524_1350.py
--rw-r--r--   0 phil       (501) staff       (20)      681 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0018_auto_20160525_1011.py
--rw-r--r--   0 phil       (501) staff       (20)      585 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0019_auto_20160713_1127.py
--rw-r--r--   0 phil       (501) staff       (20)      981 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0020_auto_20161117_1622.py
--rw-r--r--   0 phil       (501) staff       (20)      941 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0021_photo_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)      979 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/flickr/migrations/0022_photo_taken_year.py
--rw-r--r--   0 phil       (501) staff       (20)      598 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0023_auto_20180104_1457.py
--rw-r--r--   0 phil       (501) staff       (20)     1708 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/migrations/0024_auto_20201119_1539.py
--rw-r--r--   0 phil       (501) staff       (20)     1908 2020-11-19 17:05:34.000000 django-ditto-3.0.1/ditto/flickr/migrations/0025_backfill_photo_sizes.py
--rw-r--r--   0 phil       (501) staff       (20)      983 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/migrations/0026_alter_taggedphoto_content_object_and_more.py
--rw-r--r--   0 phil       (501) staff       (20)      724 2022-03-24 08:27:58.000000 django-ditto-3.0.1/ditto/flickr/migrations/0027_alter_user_photos_url_alter_user_profile_url.py
--rw-r--r--   0 phil       (501) staff       (20)      418 2022-03-24 08:27:58.000000 django-ditto-3.0.1/ditto/flickr/migrations/0028_alter_user_iconfarm.py
--rw-r--r--   0 phil       (501) staff       (20)      533 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/migrations/0029_alter_user_options_alter_user_realname.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.0.1/ditto/flickr/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    32990 2022-11-09 15:46:41.000000 django-ditto-3.0.1/ditto/flickr/models.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.625214 django-ditto-3.0.1/ditto/flickr/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.653182 django-ditto-3.0.1/ditto/flickr/templates/flickr/
--rw-r--r--   0 phil       (501) staff       (20)      291 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/base.html
--rw-r--r--   0 phil       (501) staff       (20)     1686 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.654352 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/
--rw-r--r--   0 phil       (501) staff       (20)      858 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/annual_photo_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     1572 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/nav_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)     1102 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/photo.html
--rw-r--r--   0 phil       (501) staff       (20)     2551 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/photo_columns.html
--rw-r--r--   0 phil       (501) staff       (20)      457 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/photoset_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     1456 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/photoset_list.html
--rw-r--r--   0 phil       (501) staff       (20)      836 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/sorting.html
--rw-r--r--   0 phil       (501) staff       (20)     1896 2022-03-24 08:27:58.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/user.html
--rw-r--r--   0 phil       (501) staff       (20)    10421 2018-04-16 15:46:10.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/photo_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     2615 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/photoset_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1560 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/photoset_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1781 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/tag_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1326 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/tag_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1194 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/user_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1167 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/user_photoset_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1966 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/flickr/templates/flickr/user_tag_detail.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.654684 django-ditto-3.0.1/ditto/flickr/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.0.1/ditto/flickr/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     3944 2023-05-09 16:24:02.000000 django-ditto-3.0.1/ditto/flickr/templatetags/ditto_flickr.py
--rw-r--r--   0 phil       (501) staff       (20)     1175 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/urls.py
--rw-r--r--   0 phil       (501) staff       (20)     9356 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/flickr/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.657264 django-ditto-3.0.1/ditto/lastfm/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:37.000000 django-ditto-3.0.1/ditto/lastfm/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4349 2023-05-22 10:46:56.000000 django-ditto-3.0.1/ditto/lastfm/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      237 2021-04-07 17:01:57.000000 django-ditto-3.0.1/ditto/lastfm/apps.py
--rw-r--r--   0 phil       (501) staff       (20)     1585 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/lastfm/factories.py
--rw-r--r--   0 phil       (501) staff       (20)    11423 2023-05-09 14:47:12.000000 django-ditto-3.0.1/ditto/lastfm/fetch.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.625546 django-ditto-3.0.1/ditto/lastfm/management/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.657603 django-ditto-3.0.1/ditto/lastfm/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.0.1/ditto/lastfm/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     1835 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/lastfm/management/commands/fetch_lastfm_scrobbles.py
--rw-r--r--   0 phil       (501) staff       (20)     5973 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/lastfm/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.659258 django-ditto-3.0.1/ditto/lastfm/migrations/
--rw-r--r--   0 phil       (501) staff       (20)    11231 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/lastfm/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      616 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/lastfm/migrations/0002_auto_20161012_1012.py
--rw-r--r--   0 phil       (501) staff       (20)     1536 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/lastfm/migrations/0003_auto_20161026_1539.py
--rw-r--r--   0 phil       (501) staff       (20)     2292 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/lastfm/migrations/0004_auto_20161026_1540.py
--rw-r--r--   0 phil       (501) staff       (20)      987 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/lastfm/migrations/0005_auto_20161117_1622.py
--rw-r--r--   0 phil       (501) staff       (20)      947 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/lastfm/migrations/0006_scrobble_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)      669 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/lastfm/migrations/0007_set_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)      607 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/lastfm/migrations/0008_auto_20180104_1457.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.0.1/ditto/lastfm/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    11172 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/lastfm/models.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.625727 django-ditto-3.0.1/ditto/lastfm/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.662060 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/
--rw-r--r--   0 phil       (501) staff       (20)     1755 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/album_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1187 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/album_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1286 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/artist_albums.html
--rw-r--r--   0 phil       (501) staff       (20)     1171 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/artist_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1191 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/artist_list.html
--rw-r--r--   0 phil       (501) staff       (20)      292 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/base.html
--rw-r--r--   0 phil       (501) staff       (20)     2006 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.663610 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/
--rw-r--r--   0 phil       (501) staff       (20)     1569 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/album_sidebar.html
--rw-r--r--   0 phil       (501) staff       (20)      891 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/annual_scrobble_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     1718 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/artist_sidebar.html
--rw-r--r--   0 phil       (501) staff       (20)     3033 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/chart.html
--rw-r--r--   0 phil       (501) staff       (20)      729 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/day_filter.html
--rw-r--r--   0 phil       (501) staff       (20)      679 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/nav_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)     2964 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/page_navigation.html
--rw-r--r--   0 phil       (501) staff       (20)     1338 2017-02-09 11:48:12.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/scrobble.html
--rw-r--r--   0 phil       (501) staff       (20)     1741 2017-02-09 11:48:12.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/scrobble_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1593 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/track_sidebar.html
--rw-r--r--   0 phil       (501) staff       (20)     1047 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/scrobble_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1485 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/track_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1187 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/track_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1341 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_album_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1345 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_artist_list.html
--rw-r--r--   0 phil       (501) staff       (20)     2223 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1201 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_scrobble_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1341 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_track_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.663821 django-ditto-3.0.1/ditto/lastfm/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.0.1/ditto/lastfm/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    10731 2023-05-09 14:51:28.000000 django-ditto-3.0.1/ditto/lastfm/templatetags/ditto_lastfm.py
--rw-r--r--   0 phil       (501) staff       (20)     2172 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/lastfm/urls.py
--rw-r--r--   0 phil       (501) staff       (20)      746 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/lastfm/utils.py
--rw-r--r--   0 phil       (501) staff       (20)    10230 2022-02-14 11:48:22.000000 django-ditto-3.0.1/ditto/lastfm/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.665760 django-ditto-3.0.1/ditto/pinboard/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:41.000000 django-ditto-3.0.1/ditto/pinboard/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     3153 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      355 2021-04-07 17:02:04.000000 django-ditto-3.0.1/ditto/pinboard/apps.py
--rw-r--r--   0 phil       (501) staff       (20)      890 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/checks.py
--rw-r--r--   0 phil       (501) staff       (20)     1020 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/factories.py
--rw-r--r--   0 phil       (501) staff       (20)    10396 2023-05-09 14:52:22.000000 django-ditto-3.0.1/ditto/pinboard/fetch.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.665981 django-ditto-3.0.1/ditto/pinboard/management/
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-20 14:31:00.000000 django-ditto-3.0.1/ditto/pinboard/management/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.666180 django-ditto-3.0.1/ditto/pinboard/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-20 14:31:06.000000 django-ditto-3.0.1/ditto/pinboard/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2969 2022-08-08 11:31:11.000000 django-ditto-3.0.1/ditto/pinboard/management/commands/fetch_pinboard_bookmarks.py
--rw-r--r--   0 phil       (501) staff       (20)     1842 2023-05-09 14:30:15.000000 django-ditto-3.0.1/ditto/pinboard/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.671771 django-ditto-3.0.1/ditto/pinboard/migrations/
--rw-r--r--   0 phil       (501) staff       (20)     4338 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      568 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0002_auto_20150626_1521.py
--rw-r--r--   0 phil       (501) staff       (20)      377 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0003_auto_20150626_1558.py
--rw-r--r--   0 phil       (501) staff       (20)      469 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0004_auto_20150626_1603.py
--rw-r--r--   0 phil       (501) staff       (20)      608 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0005_auto_20150626_1702.py
--rw-r--r--   0 phil       (501) staff       (20)      897 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0006_auto_20150723_1322.py
--rw-r--r--   0 phil       (501) staff       (20)     2239 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0007_auto_20150724_1957.py
--rw-r--r--   0 phil       (501) staff       (20)      643 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0008_bookmark_tags.py
--rw-r--r--   0 phil       (501) staff       (20)      531 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0009_auto_20150729_1056.py
--rw-r--r--   0 phil       (501) staff       (20)      709 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0010_auto_20150730_1112.py
--rw-r--r--   0 phil       (501) staff       (20)     4132 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0011_auto_20151002_1525.py
--rw-r--r--   0 phil       (501) staff       (20)      492 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0012_account_is_active.py
--rw-r--r--   0 phil       (501) staff       (20)     3773 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0013_auto_20151026_1546.py
--rw-r--r--   0 phil       (501) staff       (20)      733 2022-08-08 11:31:11.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0014_auto_20151028_1556.py
--rw-r--r--   0 phil       (501) staff       (20)      574 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0015_auto_20151110_1308.py
--rw-r--r--   0 phil       (501) staff       (20)      862 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0016_auto_20151119_1702.py
--rw-r--r--   0 phil       (501) staff       (20)      540 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0017_auto_20160413_0906.py
--rw-r--r--   0 phil       (501) staff       (20)      711 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0018_auto_20160414_1637.py
--rw-r--r--   0 phil       (501) staff       (20)      903 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0019_auto_20160428_1525.py
--rw-r--r--   0 phil       (501) staff       (20)      579 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0020_auto_20160428_1526.py
--rw-r--r--   0 phil       (501) staff       (20)      637 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0021_auto_20160428_1533.py
--rw-r--r--   0 phil       (501) staff       (20)      827 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0022_auto_20160428_1542.py
--rw-r--r--   0 phil       (501) staff       (20)      989 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0023_auto_20161117_1622.py
--rw-r--r--   0 phil       (501) staff       (20)      954 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0024_bookmark_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)     1291 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0025_auto_20201223_1509.py
--rw-r--r--   0 phil       (501) staff       (20)     1041 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0026_alter_taggedbookmark_content_type_and_more.py
--rw-r--r--   0 phil       (501) staff       (20)      497 2022-11-28 14:50:18.000000 django-ditto-3.0.1/ditto/pinboard/migrations/0027_alter_bookmarktag_slug.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-16 18:14:06.000000 django-ditto-3.0.1/ditto/pinboard/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     8147 2023-05-09 14:30:15.000000 django-ditto-3.0.1/ditto/pinboard/models.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.626321 django-ditto-3.0.1/ditto/pinboard/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.673980 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/
--rw-r--r--   0 phil       (501) staff       (20)     1097 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/account_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1925 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/account_tag_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1707 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/account_toread.html
--rw-r--r--   0 phil       (501) staff       (20)      297 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/base.html
--rw-r--r--   0 phil       (501) staff       (20)     2388 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/bookmark_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1399 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.675191 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/
--rw-r--r--   0 phil       (501) staff       (20)     1086 2017-08-22 13:41:35.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/account.html
--rw-r--r--   0 phil       (501) staff       (20)      904 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/annual_bookmark_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     2205 2018-04-16 15:45:40.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/bookmark.html
--rw-r--r--   0 phil       (501) staff       (20)      963 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/bookmark_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1153 2017-02-09 11:48:12.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/nav_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)      757 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/popular_tags.html
--rw-r--r--   0 phil       (501) staff       (20)     2542 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/tag_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1339 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/tag_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1372 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/pinboard/templates/pinboard/toread_list.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.675464 django-ditto-3.0.1/ditto/pinboard/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-10-14 14:00:53.000000 django-ditto-3.0.1/ditto/pinboard/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     2032 2023-05-09 16:14:31.000000 django-ditto-3.0.1/ditto/pinboard/templatetags/ditto_pinboard.py
--rw-r--r--   0 phil       (501) staff       (20)     1014 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/pinboard/urls.py
--rw-r--r--   0 phil       (501) staff       (20)     5265 2023-05-09 14:30:55.000000 django-ditto-3.0.1/ditto/pinboard/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.675708 django-ditto-3.0.1/ditto/scripts/
--rw-r--r--   0 phil       (501) staff       (20)     1073 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/scripts/flickr_authorize.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.678959 django-ditto-3.0.1/ditto/twitter/
--rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:45.000000 django-ditto-3.0.1/ditto/twitter/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     8899 2022-02-14 11:48:22.000000 django-ditto-3.0.1/ditto/twitter/admin.py
--rw-r--r--   0 phil       (501) staff       (20)      351 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/app_settings.py
--rw-r--r--   0 phil       (501) staff       (20)      239 2021-04-07 17:02:14.000000 django-ditto-3.0.1/ditto/twitter/apps.py
--rw-r--r--   0 phil       (501) staff       (20)     3845 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/factories.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.679932 django-ditto-3.0.1/ditto/twitter/fetch/
--rw-r--r--   0 phil       (501) staff       (20)       38 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/fetch/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    18076 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/fetch/fetch.py
--rw-r--r--   0 phil       (501) staff       (20)     7722 2022-08-08 11:31:12.000000 django-ditto-3.0.1/ditto/twitter/fetch/fetchers.py
--rw-r--r--   0 phil       (501) staff       (20)    14698 2023-05-09 14:53:30.000000 django-ditto-3.0.1/ditto/twitter/fetch/savers.py
--rw-r--r--   0 phil       (501) staff       (20)     1346 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/twitter/imagegenerators.py
--rw-r--r--   0 phil       (501) staff       (20)    11221 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/ingest.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.680199 django-ditto-3.0.1/ditto/twitter/management/
--rw-r--r--   0 phil       (501) staff       (20)        0 2020-05-23 16:03:25.000000 django-ditto-3.0.1/ditto/twitter/management/__init__.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.682021 django-ditto-3.0.1/ditto/twitter/management/commands/
--rw-r--r--   0 phil       (501) staff       (20)     3061 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/twitter/management/commands/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     1562 2020-05-23 18:57:17.000000 django-ditto-3.0.1/ditto/twitter/management/commands/fetch_twitter_accounts.py
--rw-r--r--   0 phil       (501) staff       (20)      797 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/management/commands/fetch_twitter_favorites.py
--rw-r--r--   0 phil       (501) staff       (20)     1005 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/management/commands/fetch_twitter_files.py
--rw-r--r--   0 phil       (501) staff       (20)      787 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/management/commands/fetch_twitter_tweets.py
--rw-r--r--   0 phil       (501) staff       (20)     1408 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/management/commands/generate_twitter_tweet_html.py
--rw-r--r--   0 phil       (501) staff       (20)     3138 2022-02-14 11:48:22.000000 django-ditto-3.0.1/ditto/twitter/management/commands/import_twitter_tweets.py
--rw-r--r--   0 phil       (501) staff       (20)      528 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/management/commands/update_twitter_tweets.py
--rw-r--r--   0 phil       (501) staff       (20)      521 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/management/commands/update_twitter_users.py
--rw-r--r--   0 phil       (501) staff       (20)     2159 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/managers.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.693524 django-ditto-3.0.1/ditto/twitter/migrations/
--rw-r--r--   0 phil       (501) staff       (20)     1589 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0001_initial.py
--rw-r--r--   0 phil       (501) staff       (20)      913 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0002_auto_20150729_1704.py
--rw-r--r--   0 phil       (501) staff       (20)    12119 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0003_auto_20150730_1112.py
--rw-r--r--   0 phil       (501) staff       (20)     1640 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0004_auto_20150730_1116.py
--rw-r--r--   0 phil       (501) staff       (20)      780 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0005_auto_20150730_1350.py
--rw-r--r--   0 phil       (501) staff       (20)      480 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0006_auto_20150730_1450.py
--rw-r--r--   0 phil       (501) staff       (20)     1303 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0007_auto_20150807_1432.py
--rw-r--r--   0 phil       (501) staff       (20)      350 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0008_remove_user_twitter_id_str.py
--rw-r--r--   0 phil       (501) staff       (20)      556 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0009_account_last_fetch_id.py
--rw-r--r--   0 phil       (501) staff       (20)      344 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0010_remove_tweet_text.py
--rw-r--r--   0 phil       (501) staff       (20)      445 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0011_tweet_text.py
--rw-r--r--   0 phil       (501) staff       (20)      942 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0012_auto_20150814_1730.py
--rw-r--r--   0 phil       (501) staff       (20)      475 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0013_user_favorites.py
--rw-r--r--   0 phil       (501) staff       (20)     1175 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0014_auto_20150819_1342.py
--rw-r--r--   0 phil       (501) staff       (20)      893 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0015_auto_20150819_1349.py
--rw-r--r--   0 phil       (501) staff       (20)    10191 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0016_auto_20151002_1525.py
--rw-r--r--   0 phil       (501) staff       (20)      488 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0017_account_is_active.py
--rw-r--r--   0 phil       (501) staff       (20)      482 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0018_tweet_text_html.py
--rw-r--r--   0 phil       (501) staff       (20)     4357 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0019_auto_20151028_1556.py
--rw-r--r--   0 phil       (501) staff       (20)      482 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0020_auto_20151028_1611.py
--rw-r--r--   0 phil       (501) staff       (20)     5411 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0021_video.py
--rw-r--r--   0 phil       (501) staff       (20)      986 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0022_auto_20151104_0840.py
--rw-r--r--   0 phil       (501) staff       (20)     5483 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0023_media.py
--rw-r--r--   0 phil       (501) staff       (20)      846 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0024_auto_20151104_1157.py
--rw-r--r--   0 phil       (501) staff       (20)      682 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0025_auto_20151109_1651.py
--rw-r--r--   0 phil       (501) staff       (20)      542 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0026_auto_20151110_1131.py
--rw-r--r--   0 phil       (501) staff       (20)      353 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0027_remove_user_profile_image_url.py
--rw-r--r--   0 phil       (501) staff       (20)      407 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0028_auto_20151110_1139.py
--rw-r--r--   0 phil       (501) staff       (20)      891 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0029_auto_20151110_1308.py
--rw-r--r--   0 phil       (501) staff       (20)      538 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0030_auto_20151119_1649.py
--rw-r--r--   0 phil       (501) staff       (20)      782 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0031_auto_20160413_0906.py
--rw-r--r--   0 phil       (501) staff       (20)      704 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0032_auto_20160414_1637.py
--rw-r--r--   0 phil       (501) staff       (20)     3113 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0033_auto_20160421_1602.py
--rw-r--r--   0 phil       (501) staff       (20)      495 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0034_user_description_html.py
--rw-r--r--   0 phil       (501) staff       (20)      665 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0035_auto_20160505_1137.py
--rw-r--r--   0 phil       (501) staff       (20)     1383 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0036_auto_20160505_1156.py
--rw-r--r--   0 phil       (501) staff       (20)      604 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0037_user_avatar.py
--rw-r--r--   0 phil       (501) staff       (20)      548 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0038_tweet_retweeted_status_id.py
--rw-r--r--   0 phil       (501) staff       (20)      794 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0039_auto_20160603_1301.py
--rw-r--r--   0 phil       (501) staff       (20)      767 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0040_auto_20160603_1302.py
--rw-r--r--   0 phil       (501) staff       (20)      390 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0041_remove_media_tweet.py
--rw-r--r--   0 phil       (501) staff       (20)      482 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0042_auto_20160603_1422.py
--rw-r--r--   0 phil       (501) staff       (20)      395 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0043_remove_media_is_private.py
--rw-r--r--   0 phil       (501) staff       (20)      439 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0044_auto_20160613_1600.py
--rw-r--r--   0 phil       (501) staff       (20)      579 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0045_media_original_image_file.py
--rw-r--r--   0 phil       (501) staff       (20)      649 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0046_auto_20160615_1038.py
--rw-r--r--   0 phil       (501) staff       (20)      669 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0047_media_video_file.py
--rw-r--r--   0 phil       (501) staff       (20)      761 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/migrations/0048_auto_20160615_1045.py
--rw-r--r--   0 phil       (501) staff       (20)      989 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0049_auto_20160713_1127.py
--rw-r--r--   0 phil       (501) staff       (20)      663 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0050_auto_20160713_1400.py
--rw-r--r--   0 phil       (501) staff       (20)      613 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0051_auto_20160713_1444.py
--rw-r--r--   0 phil       (501) staff       (20)      982 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0052_auto_20161117_1622.py
--rw-r--r--   0 phil       (501) staff       (20)      940 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0053_tweet_post_year.py
--rw-r--r--   0 phil       (501) staff       (20)      476 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0054_auto_20171113_1001.py
--rw-r--r--   0 phil       (501) staff       (20)      584 2020-05-23 18:57:18.000000 django-ditto-3.0.1/ditto/twitter/migrations/0055_re_save_tweets_for_new_html.py
--rw-r--r--   0 phil       (501) staff       (20)      616 2022-08-08 11:24:44.000000 django-ditto-3.0.1/ditto/twitter/migrations/0056_add_count_index.py
--rw-r--r--   0 phil       (501) staff       (20)     1142 2022-02-14 11:48:22.000000 django-ditto-3.0.1/ditto/twitter/migrations/0057_alter_account_access_token_and_more.py
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-07-29 16:20:01.000000 django-ditto-3.0.1/ditto/twitter/migrations/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    28211 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/models.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.627024 django-ditto-3.0.1/ditto/twitter/templates/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.695251 django-ditto-3.0.1/ditto/twitter/templates/twitter/
--rw-r--r--   0 phil       (501) staff       (20)     1406 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/account_favorite_list.html
--rw-r--r--   0 phil       (501) staff       (20)      294 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/base.html
--rw-r--r--   0 phil       (501) staff       (20)     1421 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/favorite_list.html
--rw-r--r--   0 phil       (501) staff       (20)     1294 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/home.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.696513 django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/
--rw-r--r--   0 phil       (501) staff       (20)     1248 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/annual_tweet_counts.html
--rw-r--r--   0 phil       (501) staff       (20)     2799 2022-02-13 12:12:56.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/media.html
--rw-r--r--   0 phil       (501) staff       (20)     1175 2016-05-07 11:14:06.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/nav_tabs.html
--rw-r--r--   0 phil       (501) staff       (20)     4132 2022-02-14 11:48:22.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/tweet.html
--rw-r--r--   0 phil       (501) staff       (20)     1106 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/tweet_list.html
--rw-r--r--   0 phil       (501) staff       (20)     2437 2017-08-22 13:41:35.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/user.html
--rw-r--r--   0 phil       (501) staff       (20)     2680 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/tweet_detail.html
--rw-r--r--   0 phil       (501) staff       (20)     1255 2022-08-08 11:24:43.000000 django-ditto-3.0.1/ditto/twitter/templates/twitter/user_detail.html
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.696756 django-ditto-3.0.1/ditto/twitter/templatetags/
--rw-r--r--   0 phil       (501) staff       (20)        0 2015-10-16 16:15:35.000000 django-ditto-3.0.1/ditto/twitter/templatetags/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     4772 2023-05-09 16:13:55.000000 django-ditto-3.0.1/ditto/twitter/templatetags/ditto_twitter.py
--rw-r--r--   0 phil       (501) staff       (20)      673 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/urls.py
--rw-r--r--   0 phil       (501) staff       (20)     5790 2022-08-08 11:24:45.000000 django-ditto-3.0.1/ditto/twitter/utils.py
--rw-r--r--   0 phil       (501) staff       (20)     3912 2023-05-09 14:29:27.000000 django-ditto-3.0.1/ditto/twitter/views.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-05-22 11:19:45.697681 django-ditto-3.0.1/django_ditto.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)     4266 2023-05-22 11:19:45.000000 django-ditto-3.0.1/django_ditto.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)    14951 2023-05-22 11:19:45.000000 django-ditto-3.0.1/django_ditto.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-05-22 11:19:45.000000 django-ditto-3.0.1/django_ditto.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       47 2016-04-25 12:13:07.000000 django-ditto-3.0.1/django_ditto.egg-info/pbr.json
--rw-r--r--   0 phil       (501) staff       (20)      470 2023-05-22 11:19:45.000000 django-ditto-3.0.1/django_ditto.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        6 2023-05-22 11:19:45.000000 django-ditto-3.0.1/django_ditto.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)      208 2022-08-08 11:30:07.000000 django-ditto-3.0.1/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)      139 2023-05-22 11:19:45.698157 django-ditto-3.0.1/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     4145 2023-05-22 10:49:25.000000 django-ditto-3.0.1/setup.py
--rw-r--r--   0 phil       (501) staff       (20)     1390 2023-05-09 16:29:19.000000 django-ditto-3.0.1/tox.ini
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.900832 django-ditto-3.1.0/
+-rw-r--r--   0 phil       (501) staff       (20)     1083 2021-10-22 16:10:52.000000 django-ditto-3.1.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      326 2022-03-25 12:40:03.000000 django-ditto-3.1.0/MANIFEST.in
+-rw-r--r--   0 phil       (501) staff       (20)     3869 2023-06-20 10:59:04.900910 django-ditto-3.1.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     2454 2023-05-09 16:29:45.000000 django-ditto-3.1.0/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.825577 django-ditto-3.1.0/ditto/
+-rw-r--r--   0 phil       (501) staff       (20)      196 2023-06-20 10:52:34.000000 django-ditto-3.1.0/ditto/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.827695 django-ditto-3.1.0/ditto/core/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:28.000000 django-ditto-3.1.0/ditto/core/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      263 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/core/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      708 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/core/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)     1809 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/core/apps.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.820916 django-ditto-3.1.0/ditto/core/management/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.828175 django-ditto-3.1.0/ditto/core/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)     2009 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/core/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)      272 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/core/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.828394 django-ditto-3.1.0/ditto/core/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2020-05-23 15:29:03.000000 django-ditto-3.1.0/ditto/core/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     5469 2022-11-09 15:48:27.000000 django-ditto-3.1.0/ditto/core/models.py
+-rw-r--r--   0 phil       (501) staff       (20)    11616 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/core/paginator.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.821084 django-ditto-3.1.0/ditto/core/static/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.821248 django-ditto-3.1.0/ditto/core/static/ditto-core/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.829307 django-ditto-3.1.0/ditto/core/static/ditto-core/css/
+-rw-rw-r--   0 phil       (501) staff       (20)   162264 2022-07-19 15:13:44.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/css/bootstrap.min.css
+-rw-rw-r--   0 phil       (501) staff       (20)   654593 2022-07-19 15:13:44.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/css/bootstrap.min.css.map
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.830770 django-ditto-3.1.0/ditto/core/static/ditto-core/img/
+-rw-r--r--   0 phil       (501) staff       (20)      142 2016-09-06 12:05:37.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/img/default_avatar.png
+-rw-r--r--   0 phil       (501) staff       (20)     3520 2016-09-06 12:05:37.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/img/original_error.jpg
+-rw-r--r--   0 phil       (501) staff       (20)     3309 2016-09-06 12:05:37.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/img/original_missing.jpg
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.831846 django-ditto-3.1.0/ditto/core/static/ditto-core/js/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.833455 django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/
+-rw-rw-r--   0 phil       (501) staff       (20)    20871 2022-07-19 15:13:44.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/carousel.js
+-rw-rw-r--   0 phil       (501) staff       (20)    38793 2022-07-19 15:13:44.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/carousel.js.map
+-rw-rw-r--   0 phil       (501) staff       (20)    13394 2022-07-19 15:13:44.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/collapse.js
+-rw-rw-r--   0 phil       (501) staff       (20)    24048 2022-07-19 15:13:44.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/collapse.js.map
+-rw-rw-r--   0 phil       (501) staff       (20)     6631 2022-07-19 15:13:44.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/util.js
+-rw-rw-r--   0 phil       (501) staff       (20)    12040 2022-07-19 15:13:44.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/util.js.map
+-rw-r--r--   0 phil       (501) staff       (20)    72380 2020-05-24 12:52:06.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.js
+-rw-r--r--   0 phil       (501) staff       (20)   110382 2020-05-24 12:52:06.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.map
+-rw-r--r--   0 phil       (501) staff       (20)    21233 2020-11-19 17:03:58.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/popper.min.js
+-rw-r--r--   0 phil       (501) staff       (20)   117179 2018-04-16 15:41:13.000000 django-ditto-3.1.0/ditto/core/static/ditto-core/js/popper.min.js.map
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.821415 django-ditto-3.1.0/ditto/core/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.834525 django-ditto-3.1.0/ditto/core/templates/ditto/
+-rw-r--r--   0 phil       (501) staff       (20)     2230 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/archive_day.html
+-rw-r--r--   0 phil       (501) staff       (20)     4738 2020-08-10 13:47:31.000000 django-ditto-3.1.0/ditto/core/templates/ditto/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     1029 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.836397 django-ditto-3.1.0/ditto/core/templates/ditto/includes/
+-rw-r--r--   0 phil       (501) staff       (20)      643 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/includes/account_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1180 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/includes/item_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1760 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/includes/item_lists.html
+-rw-r--r--   0 phil       (501) staff       (20)     1108 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/includes/pager.html
+-rw-r--r--   0 phil       (501) staff       (20)     2478 2017-08-22 13:41:35.000000 django-ditto-3.1.0/ditto/core/templates/ditto/includes/pagination.html
+-rw-r--r--   0 phil       (501) staff       (20)     2272 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/includes/variety_nav.html
+-rw-r--r--   0 phil       (501) staff       (20)      681 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/tag_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)      399 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/core/templates/ditto/tag_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.836610 django-ditto-3.1.0/ditto/core/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.1.0/ditto/core/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     5149 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/core/templatetags/ditto_core.py
+-rw-r--r--   0 phil       (501) staff       (20)      634 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/core/urls.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.837142 django-ditto-3.1.0/ditto/core/utils/
+-rw-r--r--   0 phil       (501) staff       (20)     3510 2023-05-09 16:23:11.000000 django-ditto-3.1.0/ditto/core/utils/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     3509 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/core/utils/downloader.py
+-rw-r--r--   0 phil       (501) staff       (20)    23806 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/core/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.840665 django-ditto-3.1.0/ditto/flickr/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:33.000000 django-ditto-3.1.0/ditto/flickr/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    12102 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      444 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)      345 2021-04-07 17:01:46.000000 django-ditto-3.1.0/ditto/flickr/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)      881 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/checks.py
+-rw-r--r--   0 phil       (501) staff       (20)     4046 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/factories.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.841748 django-ditto-3.1.0/ditto/flickr/fetch/
+-rw-r--r--   0 phil       (501) staff       (20)       38 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/fetch/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    20064 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/fetch/fetchers.py
+-rw-r--r--   0 phil       (501) staff       (20)     4656 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/fetch/filesfetchers.py
+-rw-r--r--   0 phil       (501) staff       (20)     4508 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/fetch/multifetchers.py
+-rw-r--r--   0 phil       (501) staff       (20)    16307 2023-05-09 16:24:02.000000 django-ditto-3.1.0/ditto/flickr/fetch/savers.py
+-rw-r--r--   0 phil       (501) staff       (20)     3065 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/imagegenerators.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.821863 django-ditto-3.1.0/ditto/flickr/management/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.842854 django-ditto-3.1.0/ditto/flickr/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)     2892 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2641 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/management/commands/fetch_flickr_account_user.py
+-rw-r--r--   0 phil       (501) staff       (20)     1424 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/management/commands/fetch_flickr_originals.py
+-rw-r--r--   0 phil       (501) staff       (20)     1440 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/management/commands/fetch_flickr_photos.py
+-rw-r--r--   0 phil       (501) staff       (20)      855 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/management/commands/fetch_flickr_photosets.py
+-rw-r--r--   0 phil       (501) staff       (20)     1923 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.849884 django-ditto-3.1.0/ditto/flickr/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)    23757 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      426 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0002_auto_20160406_1548.py
+-rw-r--r--   0 phil       (501) staff       (20)     1069 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0003_auto_20160413_0906.py
+-rw-r--r--   0 phil       (501) staff       (20)     4134 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0004_auto_20160414_1120.py
+-rw-r--r--   0 phil       (501) staff       (20)     7502 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0005_auto_20160414_1427.py
+-rw-r--r--   0 phil       (501) staff       (20)      556 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0006_auto_20160414_1459.py
+-rw-r--r--   0 phil       (501) staff       (20)      703 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0007_auto_20160414_1637.py
+-rw-r--r--   0 phil       (501) staff       (20)     4347 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0008_auto_20160429_1559.py
+-rw-r--r--   0 phil       (501) staff       (20)      584 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0009_photoset_fetch_time.py
+-rw-r--r--   0 phil       (501) staff       (20)      463 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0010_photo_photosets.py
+-rw-r--r--   0 phil       (501) staff       (20)     1042 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0011_auto_20160502_1645.py
+-rw-r--r--   0 phil       (501) staff       (20)     1205 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0012_auto_20160503_1457.py
+-rw-r--r--   0 phil       (501) staff       (20)      539 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0013_photoset_photos_raw.py
+-rw-r--r--   0 phil       (501) staff       (20)      569 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0014_photo_original_file.py
+-rw-r--r--   0 phil       (501) staff       (20)      572 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0015_auto_20160514_1456.py
+-rw-r--r--   0 phil       (501) staff       (20)      662 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0016_photo_video_original_file.py
+-rw-r--r--   0 phil       (501) staff       (20)      856 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0017_auto_20160524_1350.py
+-rw-r--r--   0 phil       (501) staff       (20)      681 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0018_auto_20160525_1011.py
+-rw-r--r--   0 phil       (501) staff       (20)      585 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0019_auto_20160713_1127.py
+-rw-r--r--   0 phil       (501) staff       (20)      981 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0020_auto_20161117_1622.py
+-rw-r--r--   0 phil       (501) staff       (20)      941 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0021_photo_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      979 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/flickr/migrations/0022_photo_taken_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      598 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0023_auto_20180104_1457.py
+-rw-r--r--   0 phil       (501) staff       (20)     1708 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/migrations/0024_auto_20201119_1539.py
+-rw-r--r--   0 phil       (501) staff       (20)     1908 2020-11-19 17:05:34.000000 django-ditto-3.1.0/ditto/flickr/migrations/0025_backfill_photo_sizes.py
+-rw-r--r--   0 phil       (501) staff       (20)      983 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/migrations/0026_alter_taggedphoto_content_object_and_more.py
+-rw-r--r--   0 phil       (501) staff       (20)      724 2022-03-24 08:27:58.000000 django-ditto-3.1.0/ditto/flickr/migrations/0027_alter_user_photos_url_alter_user_profile_url.py
+-rw-r--r--   0 phil       (501) staff       (20)      418 2022-03-24 08:27:58.000000 django-ditto-3.1.0/ditto/flickr/migrations/0028_alter_user_iconfarm.py
+-rw-r--r--   0 phil       (501) staff       (20)      533 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/migrations/0029_alter_user_options_alter_user_realname.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.1.0/ditto/flickr/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    32990 2022-11-09 15:46:41.000000 django-ditto-3.1.0/ditto/flickr/models.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.822121 django-ditto-3.1.0/ditto/flickr/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.852397 django-ditto-3.1.0/ditto/flickr/templates/flickr/
+-rw-r--r--   0 phil       (501) staff       (20)      291 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     1686 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.853551 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/
+-rw-r--r--   0 phil       (501) staff       (20)      858 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/annual_photo_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     1572 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/nav_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)     1102 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/photo.html
+-rw-r--r--   0 phil       (501) staff       (20)     2551 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/photo_columns.html
+-rw-r--r--   0 phil       (501) staff       (20)      457 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/photoset_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     1456 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/photoset_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      836 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/sorting.html
+-rw-r--r--   0 phil       (501) staff       (20)     1896 2022-03-24 08:27:58.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/user.html
+-rw-r--r--   0 phil       (501) staff       (20)    10421 2018-04-16 15:46:10.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/photo_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     2615 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/photoset_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1560 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/photoset_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1781 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/tag_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1326 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/tag_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1194 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/user_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1167 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/user_photoset_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1966 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/flickr/templates/flickr/user_tag_detail.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.853909 django-ditto-3.1.0/ditto/flickr/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2016-04-21 14:19:24.000000 django-ditto-3.1.0/ditto/flickr/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     3944 2023-05-09 16:24:02.000000 django-ditto-3.1.0/ditto/flickr/templatetags/ditto_flickr.py
+-rw-r--r--   0 phil       (501) staff       (20)     1175 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)     9356 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/flickr/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.856292 django-ditto-3.1.0/ditto/lastfm/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:37.000000 django-ditto-3.1.0/ditto/lastfm/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4349 2023-05-22 10:46:56.000000 django-ditto-3.1.0/ditto/lastfm/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      237 2021-04-07 17:01:57.000000 django-ditto-3.1.0/ditto/lastfm/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)     1585 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/lastfm/factories.py
+-rw-r--r--   0 phil       (501) staff       (20)    11423 2023-05-09 14:47:12.000000 django-ditto-3.1.0/ditto/lastfm/fetch.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.822503 django-ditto-3.1.0/ditto/lastfm/management/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.856617 django-ditto-3.1.0/ditto/lastfm/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.1.0/ditto/lastfm/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     1835 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/lastfm/management/commands/fetch_lastfm_scrobbles.py
+-rw-r--r--   0 phil       (501) staff       (20)     5973 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/lastfm/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.858501 django-ditto-3.1.0/ditto/lastfm/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)    11231 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/lastfm/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      616 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/lastfm/migrations/0002_auto_20161012_1012.py
+-rw-r--r--   0 phil       (501) staff       (20)     1536 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/lastfm/migrations/0003_auto_20161026_1539.py
+-rw-r--r--   0 phil       (501) staff       (20)     2292 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/lastfm/migrations/0004_auto_20161026_1540.py
+-rw-r--r--   0 phil       (501) staff       (20)      987 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/lastfm/migrations/0005_auto_20161117_1622.py
+-rw-r--r--   0 phil       (501) staff       (20)      947 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/lastfm/migrations/0006_scrobble_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      669 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/lastfm/migrations/0007_set_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      607 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/lastfm/migrations/0008_auto_20180104_1457.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.1.0/ditto/lastfm/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    11172 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/lastfm/models.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.822669 django-ditto-3.1.0/ditto/lastfm/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.861869 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/
+-rw-r--r--   0 phil       (501) staff       (20)     1755 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/album_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1187 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/album_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1286 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/artist_albums.html
+-rw-r--r--   0 phil       (501) staff       (20)     1171 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/artist_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1191 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/artist_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      292 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     2006 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.863786 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/
+-rw-r--r--   0 phil       (501) staff       (20)     1569 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/album_sidebar.html
+-rw-r--r--   0 phil       (501) staff       (20)      891 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/annual_scrobble_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     1718 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/artist_sidebar.html
+-rw-r--r--   0 phil       (501) staff       (20)     3033 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/chart.html
+-rw-r--r--   0 phil       (501) staff       (20)      729 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/day_filter.html
+-rw-r--r--   0 phil       (501) staff       (20)      679 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/nav_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)     2964 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/page_navigation.html
+-rw-r--r--   0 phil       (501) staff       (20)     1338 2017-02-09 11:48:12.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/scrobble.html
+-rw-r--r--   0 phil       (501) staff       (20)     1741 2017-02-09 11:48:12.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/scrobble_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1593 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/track_sidebar.html
+-rw-r--r--   0 phil       (501) staff       (20)     1047 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/scrobble_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1485 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/track_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1187 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/track_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1341 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_album_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1345 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_artist_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     2223 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1201 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_scrobble_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1341 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_track_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.864040 django-ditto-3.1.0/ditto/lastfm/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2017-02-09 11:48:12.000000 django-ditto-3.1.0/ditto/lastfm/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    10731 2023-05-09 14:51:28.000000 django-ditto-3.1.0/ditto/lastfm/templatetags/ditto_lastfm.py
+-rw-r--r--   0 phil       (501) staff       (20)     2172 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/lastfm/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)      746 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/lastfm/utils.py
+-rw-r--r--   0 phil       (501) staff       (20)    10230 2022-02-14 11:48:22.000000 django-ditto-3.1.0/ditto/lastfm/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.866056 django-ditto-3.1.0/ditto/pinboard/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:41.000000 django-ditto-3.1.0/ditto/pinboard/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     3153 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      355 2021-04-07 17:02:04.000000 django-ditto-3.1.0/ditto/pinboard/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)      890 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/checks.py
+-rw-r--r--   0 phil       (501) staff       (20)     1020 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/factories.py
+-rw-r--r--   0 phil       (501) staff       (20)    10396 2023-05-09 14:52:22.000000 django-ditto-3.1.0/ditto/pinboard/fetch.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.867468 django-ditto-3.1.0/ditto/pinboard/management/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-20 14:31:00.000000 django-ditto-3.1.0/ditto/pinboard/management/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.867684 django-ditto-3.1.0/ditto/pinboard/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-20 14:31:06.000000 django-ditto-3.1.0/ditto/pinboard/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2969 2022-08-08 11:31:11.000000 django-ditto-3.1.0/ditto/pinboard/management/commands/fetch_pinboard_bookmarks.py
+-rw-r--r--   0 phil       (501) staff       (20)     1842 2023-05-09 14:30:15.000000 django-ditto-3.1.0/ditto/pinboard/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.873215 django-ditto-3.1.0/ditto/pinboard/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)     4338 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      568 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0002_auto_20150626_1521.py
+-rw-r--r--   0 phil       (501) staff       (20)      377 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0003_auto_20150626_1558.py
+-rw-r--r--   0 phil       (501) staff       (20)      469 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0004_auto_20150626_1603.py
+-rw-r--r--   0 phil       (501) staff       (20)      608 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0005_auto_20150626_1702.py
+-rw-r--r--   0 phil       (501) staff       (20)      897 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0006_auto_20150723_1322.py
+-rw-r--r--   0 phil       (501) staff       (20)     2239 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0007_auto_20150724_1957.py
+-rw-r--r--   0 phil       (501) staff       (20)      643 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0008_bookmark_tags.py
+-rw-r--r--   0 phil       (501) staff       (20)      531 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0009_auto_20150729_1056.py
+-rw-r--r--   0 phil       (501) staff       (20)      709 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0010_auto_20150730_1112.py
+-rw-r--r--   0 phil       (501) staff       (20)     4132 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0011_auto_20151002_1525.py
+-rw-r--r--   0 phil       (501) staff       (20)      492 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0012_account_is_active.py
+-rw-r--r--   0 phil       (501) staff       (20)     3773 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0013_auto_20151026_1546.py
+-rw-r--r--   0 phil       (501) staff       (20)      733 2022-08-08 11:31:11.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0014_auto_20151028_1556.py
+-rw-r--r--   0 phil       (501) staff       (20)      574 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0015_auto_20151110_1308.py
+-rw-r--r--   0 phil       (501) staff       (20)      862 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0016_auto_20151119_1702.py
+-rw-r--r--   0 phil       (501) staff       (20)      540 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0017_auto_20160413_0906.py
+-rw-r--r--   0 phil       (501) staff       (20)      711 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0018_auto_20160414_1637.py
+-rw-r--r--   0 phil       (501) staff       (20)      903 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0019_auto_20160428_1525.py
+-rw-r--r--   0 phil       (501) staff       (20)      579 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0020_auto_20160428_1526.py
+-rw-r--r--   0 phil       (501) staff       (20)      637 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0021_auto_20160428_1533.py
+-rw-r--r--   0 phil       (501) staff       (20)      827 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0022_auto_20160428_1542.py
+-rw-r--r--   0 phil       (501) staff       (20)      989 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0023_auto_20161117_1622.py
+-rw-r--r--   0 phil       (501) staff       (20)      954 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0024_bookmark_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)     1291 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0025_auto_20201223_1509.py
+-rw-r--r--   0 phil       (501) staff       (20)     1041 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0026_alter_taggedbookmark_content_type_and_more.py
+-rw-r--r--   0 phil       (501) staff       (20)      497 2022-11-28 14:50:18.000000 django-ditto-3.1.0/ditto/pinboard/migrations/0027_alter_bookmarktag_slug.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-06-16 18:14:06.000000 django-ditto-3.1.0/ditto/pinboard/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     8147 2023-05-09 14:30:15.000000 django-ditto-3.1.0/ditto/pinboard/models.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.823285 django-ditto-3.1.0/ditto/pinboard/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.875791 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/
+-rw-r--r--   0 phil       (501) staff       (20)     1097 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/account_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1925 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/account_tag_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1707 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/account_toread.html
+-rw-r--r--   0 phil       (501) staff       (20)      297 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     2388 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/bookmark_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1399 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.877068 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/
+-rw-r--r--   0 phil       (501) staff       (20)     1086 2017-08-22 13:41:35.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/account.html
+-rw-r--r--   0 phil       (501) staff       (20)      904 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/annual_bookmark_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     2205 2018-04-16 15:45:40.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/bookmark.html
+-rw-r--r--   0 phil       (501) staff       (20)      963 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/bookmark_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1153 2017-02-09 11:48:12.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/nav_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)      757 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/popular_tags.html
+-rw-r--r--   0 phil       (501) staff       (20)     2542 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/tag_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1339 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/tag_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1372 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/pinboard/templates/pinboard/toread_list.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.877303 django-ditto-3.1.0/ditto/pinboard/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-10-14 14:00:53.000000 django-ditto-3.1.0/ditto/pinboard/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     2032 2023-05-09 16:14:31.000000 django-ditto-3.1.0/ditto/pinboard/templatetags/ditto_pinboard.py
+-rw-r--r--   0 phil       (501) staff       (20)     1014 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/pinboard/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)     5265 2023-05-09 14:30:55.000000 django-ditto-3.1.0/ditto/pinboard/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.877528 django-ditto-3.1.0/ditto/scripts/
+-rw-r--r--   0 phil       (501) staff       (20)     1073 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/scripts/flickr_authorize.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.881160 django-ditto-3.1.0/ditto/twitter/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2022-03-24 14:12:45.000000 django-ditto-3.1.0/ditto/twitter/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     8899 2022-02-14 11:48:22.000000 django-ditto-3.1.0/ditto/twitter/admin.py
+-rw-r--r--   0 phil       (501) staff       (20)      351 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/app_settings.py
+-rw-r--r--   0 phil       (501) staff       (20)      239 2021-04-07 17:02:14.000000 django-ditto-3.1.0/ditto/twitter/apps.py
+-rw-r--r--   0 phil       (501) staff       (20)     3845 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/factories.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.882251 django-ditto-3.1.0/ditto/twitter/fetch/
+-rw-r--r--   0 phil       (501) staff       (20)       38 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/fetch/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    18076 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/fetch/fetch.py
+-rw-r--r--   0 phil       (501) staff       (20)     7722 2022-08-08 11:31:12.000000 django-ditto-3.1.0/ditto/twitter/fetch/fetchers.py
+-rw-r--r--   0 phil       (501) staff       (20)    14698 2023-05-09 14:53:30.000000 django-ditto-3.1.0/ditto/twitter/fetch/savers.py
+-rw-r--r--   0 phil       (501) staff       (20)     1346 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/twitter/imagegenerators.py
+-rw-r--r--   0 phil       (501) staff       (20)    11221 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/ingest.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.882502 django-ditto-3.1.0/ditto/twitter/management/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2020-05-23 16:03:25.000000 django-ditto-3.1.0/ditto/twitter/management/__init__.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.884228 django-ditto-3.1.0/ditto/twitter/management/commands/
+-rw-r--r--   0 phil       (501) staff       (20)     3061 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/twitter/management/commands/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     1562 2020-05-23 18:57:17.000000 django-ditto-3.1.0/ditto/twitter/management/commands/fetch_twitter_accounts.py
+-rw-r--r--   0 phil       (501) staff       (20)      797 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/management/commands/fetch_twitter_favorites.py
+-rw-r--r--   0 phil       (501) staff       (20)     1005 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/management/commands/fetch_twitter_files.py
+-rw-r--r--   0 phil       (501) staff       (20)      787 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/management/commands/fetch_twitter_tweets.py
+-rw-r--r--   0 phil       (501) staff       (20)     1408 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/management/commands/generate_twitter_tweet_html.py
+-rw-r--r--   0 phil       (501) staff       (20)     3138 2022-02-14 11:48:22.000000 django-ditto-3.1.0/ditto/twitter/management/commands/import_twitter_tweets.py
+-rw-r--r--   0 phil       (501) staff       (20)      528 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/management/commands/update_twitter_tweets.py
+-rw-r--r--   0 phil       (501) staff       (20)      521 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/management/commands/update_twitter_users.py
+-rw-r--r--   0 phil       (501) staff       (20)     2159 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/managers.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.897181 django-ditto-3.1.0/ditto/twitter/migrations/
+-rw-r--r--   0 phil       (501) staff       (20)     1589 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0001_initial.py
+-rw-r--r--   0 phil       (501) staff       (20)      913 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0002_auto_20150729_1704.py
+-rw-r--r--   0 phil       (501) staff       (20)    12119 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0003_auto_20150730_1112.py
+-rw-r--r--   0 phil       (501) staff       (20)     1640 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0004_auto_20150730_1116.py
+-rw-r--r--   0 phil       (501) staff       (20)      780 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0005_auto_20150730_1350.py
+-rw-r--r--   0 phil       (501) staff       (20)      480 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0006_auto_20150730_1450.py
+-rw-r--r--   0 phil       (501) staff       (20)     1303 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0007_auto_20150807_1432.py
+-rw-r--r--   0 phil       (501) staff       (20)      350 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0008_remove_user_twitter_id_str.py
+-rw-r--r--   0 phil       (501) staff       (20)      556 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0009_account_last_fetch_id.py
+-rw-r--r--   0 phil       (501) staff       (20)      344 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0010_remove_tweet_text.py
+-rw-r--r--   0 phil       (501) staff       (20)      445 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0011_tweet_text.py
+-rw-r--r--   0 phil       (501) staff       (20)      942 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0012_auto_20150814_1730.py
+-rw-r--r--   0 phil       (501) staff       (20)      475 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0013_user_favorites.py
+-rw-r--r--   0 phil       (501) staff       (20)     1175 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0014_auto_20150819_1342.py
+-rw-r--r--   0 phil       (501) staff       (20)      893 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0015_auto_20150819_1349.py
+-rw-r--r--   0 phil       (501) staff       (20)    10191 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0016_auto_20151002_1525.py
+-rw-r--r--   0 phil       (501) staff       (20)      488 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0017_account_is_active.py
+-rw-r--r--   0 phil       (501) staff       (20)      482 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0018_tweet_text_html.py
+-rw-r--r--   0 phil       (501) staff       (20)     4357 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0019_auto_20151028_1556.py
+-rw-r--r--   0 phil       (501) staff       (20)      482 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0020_auto_20151028_1611.py
+-rw-r--r--   0 phil       (501) staff       (20)     5411 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0021_video.py
+-rw-r--r--   0 phil       (501) staff       (20)      986 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0022_auto_20151104_0840.py
+-rw-r--r--   0 phil       (501) staff       (20)     5483 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0023_media.py
+-rw-r--r--   0 phil       (501) staff       (20)      846 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0024_auto_20151104_1157.py
+-rw-r--r--   0 phil       (501) staff       (20)      682 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0025_auto_20151109_1651.py
+-rw-r--r--   0 phil       (501) staff       (20)      542 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0026_auto_20151110_1131.py
+-rw-r--r--   0 phil       (501) staff       (20)      353 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0027_remove_user_profile_image_url.py
+-rw-r--r--   0 phil       (501) staff       (20)      407 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0028_auto_20151110_1139.py
+-rw-r--r--   0 phil       (501) staff       (20)      891 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0029_auto_20151110_1308.py
+-rw-r--r--   0 phil       (501) staff       (20)      538 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0030_auto_20151119_1649.py
+-rw-r--r--   0 phil       (501) staff       (20)      782 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0031_auto_20160413_0906.py
+-rw-r--r--   0 phil       (501) staff       (20)      704 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0032_auto_20160414_1637.py
+-rw-r--r--   0 phil       (501) staff       (20)     3113 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0033_auto_20160421_1602.py
+-rw-r--r--   0 phil       (501) staff       (20)      495 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0034_user_description_html.py
+-rw-r--r--   0 phil       (501) staff       (20)      665 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0035_auto_20160505_1137.py
+-rw-r--r--   0 phil       (501) staff       (20)     1383 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0036_auto_20160505_1156.py
+-rw-r--r--   0 phil       (501) staff       (20)      604 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0037_user_avatar.py
+-rw-r--r--   0 phil       (501) staff       (20)      548 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0038_tweet_retweeted_status_id.py
+-rw-r--r--   0 phil       (501) staff       (20)      794 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0039_auto_20160603_1301.py
+-rw-r--r--   0 phil       (501) staff       (20)      767 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0040_auto_20160603_1302.py
+-rw-r--r--   0 phil       (501) staff       (20)      390 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0041_remove_media_tweet.py
+-rw-r--r--   0 phil       (501) staff       (20)      482 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0042_auto_20160603_1422.py
+-rw-r--r--   0 phil       (501) staff       (20)      395 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0043_remove_media_is_private.py
+-rw-r--r--   0 phil       (501) staff       (20)      439 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0044_auto_20160613_1600.py
+-rw-r--r--   0 phil       (501) staff       (20)      579 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0045_media_original_image_file.py
+-rw-r--r--   0 phil       (501) staff       (20)      649 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0046_auto_20160615_1038.py
+-rw-r--r--   0 phil       (501) staff       (20)      669 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0047_media_video_file.py
+-rw-r--r--   0 phil       (501) staff       (20)      761 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/migrations/0048_auto_20160615_1045.py
+-rw-r--r--   0 phil       (501) staff       (20)      989 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0049_auto_20160713_1127.py
+-rw-r--r--   0 phil       (501) staff       (20)      663 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0050_auto_20160713_1400.py
+-rw-r--r--   0 phil       (501) staff       (20)      613 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0051_auto_20160713_1444.py
+-rw-r--r--   0 phil       (501) staff       (20)      982 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0052_auto_20161117_1622.py
+-rw-r--r--   0 phil       (501) staff       (20)      940 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0053_tweet_post_year.py
+-rw-r--r--   0 phil       (501) staff       (20)      476 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0054_auto_20171113_1001.py
+-rw-r--r--   0 phil       (501) staff       (20)      584 2020-05-23 18:57:18.000000 django-ditto-3.1.0/ditto/twitter/migrations/0055_re_save_tweets_for_new_html.py
+-rw-r--r--   0 phil       (501) staff       (20)      616 2022-08-08 11:24:44.000000 django-ditto-3.1.0/ditto/twitter/migrations/0056_add_count_index.py
+-rw-r--r--   0 phil       (501) staff       (20)     1142 2022-02-14 11:48:22.000000 django-ditto-3.1.0/ditto/twitter/migrations/0057_alter_account_access_token_and_more.py
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-07-29 16:20:01.000000 django-ditto-3.1.0/ditto/twitter/migrations/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    28211 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/models.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.824103 django-ditto-3.1.0/ditto/twitter/templates/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.898733 django-ditto-3.1.0/ditto/twitter/templates/twitter/
+-rw-r--r--   0 phil       (501) staff       (20)     1406 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/account_favorite_list.html
+-rw-r--r--   0 phil       (501) staff       (20)      294 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/base.html
+-rw-r--r--   0 phil       (501) staff       (20)     1421 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/favorite_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     1294 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/home.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.899766 django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/
+-rw-r--r--   0 phil       (501) staff       (20)     1248 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/annual_tweet_counts.html
+-rw-r--r--   0 phil       (501) staff       (20)     2799 2022-02-13 12:12:56.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/media.html
+-rw-r--r--   0 phil       (501) staff       (20)     1175 2016-05-07 11:14:06.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/nav_tabs.html
+-rw-r--r--   0 phil       (501) staff       (20)     4132 2022-02-14 11:48:22.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/tweet.html
+-rw-r--r--   0 phil       (501) staff       (20)     1106 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/tweet_list.html
+-rw-r--r--   0 phil       (501) staff       (20)     2437 2017-08-22 13:41:35.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/user.html
+-rw-r--r--   0 phil       (501) staff       (20)     2680 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/tweet_detail.html
+-rw-r--r--   0 phil       (501) staff       (20)     1255 2022-08-08 11:24:43.000000 django-ditto-3.1.0/ditto/twitter/templates/twitter/user_detail.html
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.899983 django-ditto-3.1.0/ditto/twitter/templatetags/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2015-10-16 16:15:35.000000 django-ditto-3.1.0/ditto/twitter/templatetags/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     4772 2023-05-09 16:13:55.000000 django-ditto-3.1.0/ditto/twitter/templatetags/ditto_twitter.py
+-rw-r--r--   0 phil       (501) staff       (20)      673 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/urls.py
+-rw-r--r--   0 phil       (501) staff       (20)     5790 2022-08-08 11:24:45.000000 django-ditto-3.1.0/ditto/twitter/utils.py
+-rw-r--r--   0 phil       (501) staff       (20)     3912 2023-05-09 14:29:27.000000 django-ditto-3.1.0/ditto/twitter/views.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-20 10:59:04.900736 django-ditto-3.1.0/django_ditto.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)     3869 2023-06-20 10:59:04.000000 django-ditto-3.1.0/django_ditto.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)    14951 2023-06-20 10:59:04.000000 django-ditto-3.1.0/django_ditto.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-20 10:59:04.000000 django-ditto-3.1.0/django_ditto.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       47 2016-04-25 12:13:07.000000 django-ditto-3.1.0/django_ditto.egg-info/pbr.json
+-rw-r--r--   0 phil       (501) staff       (20)      470 2023-06-20 10:59:04.000000 django-ditto-3.1.0/django_ditto.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        6 2023-06-20 10:59:04.000000 django-ditto-3.1.0/django_ditto.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)      208 2022-08-08 11:30:07.000000 django-ditto-3.1.0/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)      139 2023-06-20 10:59:04.901141 django-ditto-3.1.0/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     4145 2023-05-22 10:49:25.000000 django-ditto-3.1.0/setup.py
+-rw-r--r--   0 phil       (501) staff       (20)     1429 2023-06-20 10:33:47.000000 django-ditto-3.1.0/tox.ini
```

### Comparing `django-ditto-3.0.1/LICENSE` & `django-ditto-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/PKG-INFO` & `django-ditto-3.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,19 @@
 Metadata-Version: 2.1
 Name: django-ditto
-Version: 3.0.1
+Version: 3.1.0
 Summary: A Django app to copy stuff from your accounts on Flickr, Last.fm, Pinboard and Twitter.
 Home-page: https://github.com/philgyford/django-ditto
 Author: Phil Gyford
 Author-email: phil@gyford.com
 License: MIT
 Project-URL: Blog posts, https://www.gyford.com/phil/writing/tags/django-ditto/
 Project-URL: Bug Reports, https://github.com/philgyford/django-ditto/issues
 Project-URL: Documentation, https://django-ditto.readthedocs.io/
 Project-URL: Source, https://github.com/philgyford/django-ditto
-Description: Django Ditto
-        ============
-        
-        [![image](https://github.com/philgyford/django-ditto/actions/workflows/tests.yml/badge.svg)](https://github.com/philgyford/django-ditto/actions/workflows/tests.yml "Tests status")
-        [![codecov](https://codecov.io/gh/philgyford/django-ditto/branch/main/graph/badge.svg?token=T7TMMDS64A)](https://codecov.io/gh/philgyford/django-ditto)
-        [![image](https://readthedocs.org/projects/django-ditto/badge/?version=stable)](https://django-ditto.readthedocs.io/en/stable/?badge=stable "Documentation status")
-        [![Code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-        [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-        
-        
-        A collection of Django apps for copying things from third-party sites and services. Requires Python 3.9 to 3.11, and Django 3.2, 4.1, or 4.2.
-        
-        [Read the documentation.](http://django-ditto.readthedocs.io/en/latest/)
-        
-        [See screenshots of a site using the supplied templates.](https://github.com/philgyford/django-ditto/tree/main/screenshots)
-        
-        Install using [pip](https://pip.pypa.io/en/stable/):
-        
-            $ pip install django-ditto
-        
-        NOTE 1: It will install [Pillow](http://pillow.readthedocs.io/en/latest/), among other things, which has prerequisites of its own, such as libjpeg and zlib. Sorry.
-        
-        NOTE 2: As of 2023 I'm unsure how well the Twitter integration still works given the state of its API etc.
-        
-        Currently, Ditto can copy these things from these services:
-        
-        - [Flickr](https://flickr.com/)
-          - Photos
-          - Photosets
-          - Original image and video files
-          - Users
-        - [Last.fm](https://www.last.fm/)
-          - Scrobbles (Artist, Track and Album)
-        - [Pinboard](https://pinboard.in/)
-          - Bookmarks
-        - [Twitter](https://twitter.com/)
-          - Tweets
-          - Favorites/Likes
-          - Images and Animated GIFs (but not videos)
-          - Users
-        
-        The Ditto apps provide:
-        
-        - Models
-        - Admin
-        - Management commands to fetch the data/files
-        - Views and URLs
-        - Templates (that use [Bootstrap 4](https://getbootstrap.com))
-        - Template tags for common things (eg, most recent Tweets, or Flickr photos uploaded on a particular day)
-        
 Keywords: ditto twitter flickr pinboard last.fm
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
@@ -78,7 +26,62 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+Django Ditto
+============
+
+[![image](https://github.com/philgyford/django-ditto/actions/workflows/tests.yml/badge.svg)](https://github.com/philgyford/django-ditto/actions/workflows/tests.yml "Tests status")
+[![codecov](https://codecov.io/gh/philgyford/django-ditto/branch/main/graph/badge.svg?token=T7TMMDS64A)](https://codecov.io/gh/philgyford/django-ditto)
+[![image](https://readthedocs.org/projects/django-ditto/badge/?version=stable)](https://django-ditto.readthedocs.io/en/stable/?badge=stable "Documentation status")
+[![Code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+
+
+A collection of Django apps for copying things from third-party sites and services. Requires Python 3.9 to 3.11, and Django 3.2, 4.1, or 4.2.
+
+[Read the documentation.](http://django-ditto.readthedocs.io/en/latest/)
+
+[See screenshots of a site using the supplied templates.](https://github.com/philgyford/django-ditto/tree/main/screenshots)
+
+Install using [pip](https://pip.pypa.io/en/stable/):
+
+    $ pip install django-ditto
+
+NOTE 1: It will install [Pillow](http://pillow.readthedocs.io/en/latest/), among other things, which has prerequisites of its own, such as libjpeg and zlib. Sorry.
+
+NOTE 2: As of 2023 I'm unsure how well the Twitter integration still works given the state of its API etc.
+
+Currently, Ditto can copy these things from these services:
+
+- [Flickr](https://flickr.com/)
+  - Photos
+  - Photosets
+  - Original image and video files
+  - Users
+- [Last.fm](https://www.last.fm/)
+  - Scrobbles (Artist, Track and Album)
+- [Pinboard](https://pinboard.in/)
+  - Bookmarks
+- [Twitter](https://twitter.com/)
+  - Tweets
+  - Favorites/Likes
+  - Images and Animated GIFs (but not videos)
+  - Users
+
+The Ditto apps provide:
+
+- Models
+- Admin
+- Management commands to fetch the data/files
+- Views and URLs
+- Templates (that use [Bootstrap 4](https://getbootstrap.com))
+- Template tags for common things (eg, most recent Tweets, or Flickr photos uploaded on a particular day)
+
+
```

### Comparing `django-ditto-3.0.1/README.md` & `django-ditto-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/app_settings.py` & `django-ditto-3.1.0/ditto/core/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/apps.py` & `django-ditto-3.1.0/ditto/core/apps.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/management/commands/__init__.py` & `django-ditto-3.1.0/ditto/core/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/models.py` & `django-ditto-3.1.0/ditto/core/models.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/paginator.py` & `django-ditto-3.1.0/ditto/core/paginator.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/css/bootstrap.min.css` & `django-ditto-3.1.0/ditto/core/static/ditto-core/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/css/bootstrap.min.css.map` & `django-ditto-3.1.0/ditto/core/static/ditto-core/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/img/original_error.jpg` & `django-ditto-3.1.0/ditto/core/static/ditto-core/img/original_error.jpg`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/img/original_missing.jpg` & `django-ditto-3.1.0/ditto/core/static/ditto-core/img/original_missing.jpg`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/carousel.js` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/carousel.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/carousel.js.map` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/carousel.js.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/collapse.js` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/collapse.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/collapse.js.map` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/collapse.js.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/util.js` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/util.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/bootstrap/util.js.map` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/bootstrap/util.js.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.js` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.map` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/jquery-3.5.1.slim.min.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/popper.min.js` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/popper.min.js`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/static/ditto-core/js/popper.min.js.map` & `django-ditto-3.1.0/ditto/core/static/ditto-core/js/popper.min.js.map`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/archive_day.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/archive_day.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/base.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/base.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/home.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/includes/account_list.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/includes/account_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/includes/item_list.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/includes/item_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/includes/item_lists.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/includes/item_lists.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/includes/pager.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/includes/pager.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/includes/pagination.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/includes/variety_nav.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/includes/variety_nav.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templates/ditto/tag_detail.html` & `django-ditto-3.1.0/ditto/core/templates/ditto/tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/templatetags/ditto_core.py` & `django-ditto-3.1.0/ditto/core/templatetags/ditto_core.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/urls.py` & `django-ditto-3.1.0/ditto/core/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/utils/__init__.py` & `django-ditto-3.1.0/ditto/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/utils/downloader.py` & `django-ditto-3.1.0/ditto/core/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/core/views.py` & `django-ditto-3.1.0/ditto/core/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/admin.py` & `django-ditto-3.1.0/ditto/flickr/admin.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/checks.py` & `django-ditto-3.1.0/ditto/flickr/checks.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/factories.py` & `django-ditto-3.1.0/ditto/flickr/factories.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/fetch/fetchers.py` & `django-ditto-3.1.0/ditto/flickr/fetch/fetchers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/fetch/filesfetchers.py` & `django-ditto-3.1.0/ditto/flickr/fetch/filesfetchers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/fetch/multifetchers.py` & `django-ditto-3.1.0/ditto/flickr/fetch/multifetchers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/fetch/savers.py` & `django-ditto-3.1.0/ditto/flickr/fetch/savers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/imagegenerators.py` & `django-ditto-3.1.0/ditto/flickr/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/management/commands/__init__.py` & `django-ditto-3.1.0/ditto/flickr/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/management/commands/fetch_flickr_account_user.py` & `django-ditto-3.1.0/ditto/flickr/management/commands/fetch_flickr_account_user.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/management/commands/fetch_flickr_originals.py` & `django-ditto-3.1.0/ditto/flickr/management/commands/fetch_flickr_originals.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/management/commands/fetch_flickr_photos.py` & `django-ditto-3.1.0/ditto/flickr/management/commands/fetch_flickr_photos.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/management/commands/fetch_flickr_photosets.py` & `django-ditto-3.1.0/ditto/flickr/management/commands/fetch_flickr_photosets.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/managers.py` & `django-ditto-3.1.0/ditto/flickr/managers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0001_initial.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0003_auto_20160413_0906.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0003_auto_20160413_0906.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0004_auto_20160414_1120.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0004_auto_20160414_1120.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0005_auto_20160414_1427.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0005_auto_20160414_1427.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0006_auto_20160414_1459.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0006_auto_20160414_1459.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0007_auto_20160414_1637.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0007_auto_20160414_1637.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0008_auto_20160429_1559.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0008_auto_20160429_1559.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0009_photoset_fetch_time.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0009_photoset_fetch_time.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0011_auto_20160502_1645.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0011_auto_20160502_1645.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0012_auto_20160503_1457.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0012_auto_20160503_1457.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0013_photoset_photos_raw.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0013_photoset_photos_raw.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0014_photo_original_file.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0014_photo_original_file.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0015_auto_20160514_1456.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0015_auto_20160514_1456.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0016_photo_video_original_file.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0016_photo_video_original_file.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0017_auto_20160524_1350.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0017_auto_20160524_1350.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0018_auto_20160525_1011.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0018_auto_20160525_1011.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0019_auto_20160713_1127.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0019_auto_20160713_1127.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0020_auto_20161117_1622.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0020_auto_20161117_1622.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0021_photo_post_year.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0021_photo_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0022_photo_taken_year.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0022_photo_taken_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0023_auto_20180104_1457.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0023_auto_20180104_1457.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0024_auto_20201119_1539.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0024_auto_20201119_1539.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0025_backfill_photo_sizes.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0025_backfill_photo_sizes.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0026_alter_taggedphoto_content_object_and_more.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0026_alter_taggedphoto_content_object_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0027_alter_user_photos_url_alter_user_profile_url.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0027_alter_user_photos_url_alter_user_profile_url.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/migrations/0029_alter_user_options_alter_user_realname.py` & `django-ditto-3.1.0/ditto/flickr/migrations/0029_alter_user_options_alter_user_realname.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/models.py` & `django-ditto-3.1.0/ditto/flickr/models.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/home.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/annual_photo_counts.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/annual_photo_counts.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/nav_tabs.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/nav_tabs.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/photo.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/photo.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/photo_columns.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/photo_columns.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/photoset_list.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/photoset_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/sorting.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/sorting.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/includes/user.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/includes/user.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/photo_detail.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/photo_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/photoset_detail.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/photoset_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/photoset_list.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/photoset_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/tag_detail.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/tag_list.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/tag_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/user_detail.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/user_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/user_photoset_list.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/user_photoset_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templates/flickr/user_tag_detail.html` & `django-ditto-3.1.0/ditto/flickr/templates/flickr/user_tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/templatetags/ditto_flickr.py` & `django-ditto-3.1.0/ditto/flickr/templatetags/ditto_flickr.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/urls.py` & `django-ditto-3.1.0/ditto/flickr/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/flickr/views.py` & `django-ditto-3.1.0/ditto/flickr/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/admin.py` & `django-ditto-3.1.0/ditto/lastfm/admin.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/factories.py` & `django-ditto-3.1.0/ditto/lastfm/factories.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/fetch.py` & `django-ditto-3.1.0/ditto/lastfm/fetch.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/management/commands/fetch_lastfm_scrobbles.py` & `django-ditto-3.1.0/ditto/lastfm/management/commands/fetch_lastfm_scrobbles.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/managers.py` & `django-ditto-3.1.0/ditto/lastfm/managers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/migrations/0001_initial.py` & `django-ditto-3.1.0/ditto/lastfm/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/migrations/0002_auto_20161012_1012.py` & `django-ditto-3.1.0/ditto/lastfm/migrations/0002_auto_20161012_1012.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/migrations/0003_auto_20161026_1539.py` & `django-ditto-3.1.0/ditto/lastfm/migrations/0003_auto_20161026_1539.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/migrations/0004_auto_20161026_1540.py` & `django-ditto-3.1.0/ditto/lastfm/migrations/0004_auto_20161026_1540.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/migrations/0005_auto_20161117_1622.py` & `django-ditto-3.1.0/ditto/lastfm/migrations/0005_auto_20161117_1622.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/migrations/0006_scrobble_post_year.py` & `django-ditto-3.1.0/ditto/lastfm/migrations/0006_scrobble_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/migrations/0007_set_post_year.py` & `django-ditto-3.1.0/ditto/lastfm/migrations/0007_set_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/migrations/0008_auto_20180104_1457.py` & `django-ditto-3.1.0/ditto/lastfm/migrations/0008_auto_20180104_1457.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/models.py` & `django-ditto-3.1.0/ditto/lastfm/models.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/album_detail.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/album_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/album_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/album_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/artist_albums.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/artist_albums.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/artist_detail.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/artist_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/artist_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/artist_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/home.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/album_sidebar.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/album_sidebar.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/annual_scrobble_counts.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/annual_scrobble_counts.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/artist_sidebar.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/artist_sidebar.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/chart.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/chart.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/day_filter.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/day_filter.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/nav_tabs.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/nav_tabs.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/page_navigation.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/page_navigation.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/scrobble.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/scrobble.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/scrobble_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/scrobble_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/includes/track_sidebar.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/includes/track_sidebar.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/scrobble_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/scrobble_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/track_detail.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/track_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/track_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/track_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_album_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_album_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_artist_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_artist_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_detail.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_scrobble_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_scrobble_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templates/lastfm/user_track_list.html` & `django-ditto-3.1.0/ditto/lastfm/templates/lastfm/user_track_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/templatetags/ditto_lastfm.py` & `django-ditto-3.1.0/ditto/lastfm/templatetags/ditto_lastfm.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/urls.py` & `django-ditto-3.1.0/ditto/lastfm/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/utils.py` & `django-ditto-3.1.0/ditto/lastfm/utils.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/lastfm/views.py` & `django-ditto-3.1.0/ditto/lastfm/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/admin.py` & `django-ditto-3.1.0/ditto/pinboard/admin.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/checks.py` & `django-ditto-3.1.0/ditto/pinboard/checks.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/factories.py` & `django-ditto-3.1.0/ditto/pinboard/factories.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/fetch.py` & `django-ditto-3.1.0/ditto/pinboard/fetch.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/management/commands/fetch_pinboard_bookmarks.py` & `django-ditto-3.1.0/ditto/pinboard/management/commands/fetch_pinboard_bookmarks.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/managers.py` & `django-ditto-3.1.0/ditto/pinboard/managers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0001_initial.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0002_auto_20150626_1521.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0002_auto_20150626_1521.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0005_auto_20150626_1702.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0005_auto_20150626_1702.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0006_auto_20150723_1322.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0006_auto_20150723_1322.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0007_auto_20150724_1957.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0007_auto_20150724_1957.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0008_bookmark_tags.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0008_bookmark_tags.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0009_auto_20150729_1056.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0009_auto_20150729_1056.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0010_auto_20150730_1112.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0010_auto_20150730_1112.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0011_auto_20151002_1525.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0011_auto_20151002_1525.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0013_auto_20151026_1546.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0013_auto_20151026_1546.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0014_auto_20151028_1556.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0014_auto_20151028_1556.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0015_auto_20151110_1308.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0015_auto_20151110_1308.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0016_auto_20151119_1702.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0016_auto_20151119_1702.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0017_auto_20160413_0906.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0017_auto_20160413_0906.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0018_auto_20160414_1637.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0018_auto_20160414_1637.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0019_auto_20160428_1525.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0019_auto_20160428_1525.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0020_auto_20160428_1526.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0020_auto_20160428_1526.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0021_auto_20160428_1533.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0021_auto_20160428_1533.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0022_auto_20160428_1542.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0022_auto_20160428_1542.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0023_auto_20161117_1622.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0023_auto_20161117_1622.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0024_bookmark_post_year.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0024_bookmark_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0025_auto_20201223_1509.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0025_auto_20201223_1509.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/migrations/0026_alter_taggedbookmark_content_type_and_more.py` & `django-ditto-3.1.0/ditto/pinboard/migrations/0026_alter_taggedbookmark_content_type_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/models.py` & `django-ditto-3.1.0/ditto/pinboard/models.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/account_detail.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/account_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/account_tag_detail.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/account_tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/account_toread.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/account_toread.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/bookmark_detail.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/bookmark_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/home.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/account.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/account.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/annual_bookmark_counts.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/annual_bookmark_counts.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/bookmark.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/bookmark.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/bookmark_list.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/bookmark_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/nav_tabs.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/nav_tabs.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/includes/popular_tags.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/includes/popular_tags.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/tag_detail.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/tag_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/tag_list.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/tag_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templates/pinboard/toread_list.html` & `django-ditto-3.1.0/ditto/pinboard/templates/pinboard/toread_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/templatetags/ditto_pinboard.py` & `django-ditto-3.1.0/ditto/pinboard/templatetags/ditto_pinboard.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/urls.py` & `django-ditto-3.1.0/ditto/pinboard/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/pinboard/views.py` & `django-ditto-3.1.0/ditto/pinboard/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/scripts/flickr_authorize.py` & `django-ditto-3.1.0/ditto/scripts/flickr_authorize.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/admin.py` & `django-ditto-3.1.0/ditto/twitter/admin.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/factories.py` & `django-ditto-3.1.0/ditto/twitter/factories.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/fetch/fetch.py` & `django-ditto-3.1.0/ditto/twitter/fetch/fetch.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/fetch/fetchers.py` & `django-ditto-3.1.0/ditto/twitter/fetch/fetchers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/fetch/savers.py` & `django-ditto-3.1.0/ditto/twitter/fetch/savers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/imagegenerators.py` & `django-ditto-3.1.0/ditto/twitter/imagegenerators.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/ingest.py` & `django-ditto-3.1.0/ditto/twitter/ingest.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/__init__.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/fetch_twitter_accounts.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/fetch_twitter_accounts.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/fetch_twitter_favorites.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/fetch_twitter_favorites.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/fetch_twitter_files.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/fetch_twitter_files.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/fetch_twitter_tweets.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/fetch_twitter_tweets.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/generate_twitter_tweet_html.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/generate_twitter_tweet_html.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/import_twitter_tweets.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/import_twitter_tweets.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/update_twitter_tweets.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/update_twitter_tweets.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/management/commands/update_twitter_users.py` & `django-ditto-3.1.0/ditto/twitter/management/commands/update_twitter_users.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/managers.py` & `django-ditto-3.1.0/ditto/twitter/managers.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0001_initial.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0002_auto_20150729_1704.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0002_auto_20150729_1704.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0003_auto_20150730_1112.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0003_auto_20150730_1112.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0004_auto_20150730_1116.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0004_auto_20150730_1116.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0005_auto_20150730_1350.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0005_auto_20150730_1350.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0007_auto_20150807_1432.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0007_auto_20150807_1432.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0009_account_last_fetch_id.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0009_account_last_fetch_id.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0012_auto_20150814_1730.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0012_auto_20150814_1730.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0014_auto_20150819_1342.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0014_auto_20150819_1342.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0015_auto_20150819_1349.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0015_auto_20150819_1349.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0016_auto_20151002_1525.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0016_auto_20151002_1525.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0019_auto_20151028_1556.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0019_auto_20151028_1556.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0021_video.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0021_video.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0022_auto_20151104_0840.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0022_auto_20151104_0840.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0023_media.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0023_media.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0024_auto_20151104_1157.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0024_auto_20151104_1157.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0025_auto_20151109_1651.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0025_auto_20151109_1651.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0026_auto_20151110_1131.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0026_auto_20151110_1131.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0029_auto_20151110_1308.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0029_auto_20151110_1308.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0030_auto_20151119_1649.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0030_auto_20151119_1649.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0031_auto_20160413_0906.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0031_auto_20160413_0906.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0032_auto_20160414_1637.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0032_auto_20160414_1637.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0033_auto_20160421_1602.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0033_auto_20160421_1602.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0035_auto_20160505_1137.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0035_auto_20160505_1137.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0036_auto_20160505_1156.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0036_auto_20160505_1156.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0037_user_avatar.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0037_user_avatar.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0038_tweet_retweeted_status_id.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0038_tweet_retweeted_status_id.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0039_auto_20160603_1301.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0039_auto_20160603_1301.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0040_auto_20160603_1302.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0040_auto_20160603_1302.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0045_media_original_image_file.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0045_media_original_image_file.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0046_auto_20160615_1038.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0046_auto_20160615_1038.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0047_media_video_file.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0047_media_video_file.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0048_auto_20160615_1045.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0048_auto_20160615_1045.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0049_auto_20160713_1127.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0049_auto_20160713_1127.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0050_auto_20160713_1400.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0050_auto_20160713_1400.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0051_auto_20160713_1444.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0051_auto_20160713_1444.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0052_auto_20161117_1622.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0052_auto_20161117_1622.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0053_tweet_post_year.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0053_tweet_post_year.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0055_re_save_tweets_for_new_html.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0055_re_save_tweets_for_new_html.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0056_add_count_index.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0056_add_count_index.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/migrations/0057_alter_account_access_token_and_more.py` & `django-ditto-3.1.0/ditto/twitter/migrations/0057_alter_account_access_token_and_more.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/models.py` & `django-ditto-3.1.0/ditto/twitter/models.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/account_favorite_list.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/account_favorite_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/favorite_list.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/favorite_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/home.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/home.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/annual_tweet_counts.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/annual_tweet_counts.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/media.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/media.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/nav_tabs.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/nav_tabs.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/tweet.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/tweet.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/tweet_list.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/tweet_list.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/includes/user.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/includes/user.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/tweet_detail.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/tweet_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templates/twitter/user_detail.html` & `django-ditto-3.1.0/ditto/twitter/templates/twitter/user_detail.html`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/templatetags/ditto_twitter.py` & `django-ditto-3.1.0/ditto/twitter/templatetags/ditto_twitter.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/urls.py` & `django-ditto-3.1.0/ditto/twitter/urls.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/utils.py` & `django-ditto-3.1.0/ditto/twitter/utils.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/ditto/twitter/views.py` & `django-ditto-3.1.0/ditto/twitter/views.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/django_ditto.egg-info/PKG-INFO` & `django-ditto-3.1.0/django_ditto.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,19 @@
 Metadata-Version: 2.1
 Name: django-ditto
-Version: 3.0.1
+Version: 3.1.0
 Summary: A Django app to copy stuff from your accounts on Flickr, Last.fm, Pinboard and Twitter.
 Home-page: https://github.com/philgyford/django-ditto
 Author: Phil Gyford
 Author-email: phil@gyford.com
 License: MIT
 Project-URL: Blog posts, https://www.gyford.com/phil/writing/tags/django-ditto/
 Project-URL: Bug Reports, https://github.com/philgyford/django-ditto/issues
 Project-URL: Documentation, https://django-ditto.readthedocs.io/
 Project-URL: Source, https://github.com/philgyford/django-ditto
-Description: Django Ditto
-        ============
-        
-        [![image](https://github.com/philgyford/django-ditto/actions/workflows/tests.yml/badge.svg)](https://github.com/philgyford/django-ditto/actions/workflows/tests.yml "Tests status")
-        [![codecov](https://codecov.io/gh/philgyford/django-ditto/branch/main/graph/badge.svg?token=T7TMMDS64A)](https://codecov.io/gh/philgyford/django-ditto)
-        [![image](https://readthedocs.org/projects/django-ditto/badge/?version=stable)](https://django-ditto.readthedocs.io/en/stable/?badge=stable "Documentation status")
-        [![Code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
-        [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-        
-        
-        A collection of Django apps for copying things from third-party sites and services. Requires Python 3.9 to 3.11, and Django 3.2, 4.1, or 4.2.
-        
-        [Read the documentation.](http://django-ditto.readthedocs.io/en/latest/)
-        
-        [See screenshots of a site using the supplied templates.](https://github.com/philgyford/django-ditto/tree/main/screenshots)
-        
-        Install using [pip](https://pip.pypa.io/en/stable/):
-        
-            $ pip install django-ditto
-        
-        NOTE 1: It will install [Pillow](http://pillow.readthedocs.io/en/latest/), among other things, which has prerequisites of its own, such as libjpeg and zlib. Sorry.
-        
-        NOTE 2: As of 2023 I'm unsure how well the Twitter integration still works given the state of its API etc.
-        
-        Currently, Ditto can copy these things from these services:
-        
-        - [Flickr](https://flickr.com/)
-          - Photos
-          - Photosets
-          - Original image and video files
-          - Users
-        - [Last.fm](https://www.last.fm/)
-          - Scrobbles (Artist, Track and Album)
-        - [Pinboard](https://pinboard.in/)
-          - Bookmarks
-        - [Twitter](https://twitter.com/)
-          - Tweets
-          - Favorites/Likes
-          - Images and Animated GIFs (but not videos)
-          - Users
-        
-        The Ditto apps provide:
-        
-        - Models
-        - Admin
-        - Management commands to fetch the data/files
-        - Views and URLs
-        - Templates (that use [Bootstrap 4](https://getbootstrap.com))
-        - Template tags for common things (eg, most recent Tweets, or Flickr photos uploaded on a particular day)
-        
 Keywords: ditto twitter flickr pinboard last.fm
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
@@ -78,7 +26,62 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+Django Ditto
+============
+
+[![image](https://github.com/philgyford/django-ditto/actions/workflows/tests.yml/badge.svg)](https://github.com/philgyford/django-ditto/actions/workflows/tests.yml "Tests status")
+[![codecov](https://codecov.io/gh/philgyford/django-ditto/branch/main/graph/badge.svg?token=T7TMMDS64A)](https://codecov.io/gh/philgyford/django-ditto)
+[![image](https://readthedocs.org/projects/django-ditto/badge/?version=stable)](https://django-ditto.readthedocs.io/en/stable/?badge=stable "Documentation status")
+[![Code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square)](https://github.com/prettier/prettier)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+
+
+A collection of Django apps for copying things from third-party sites and services. Requires Python 3.9 to 3.11, and Django 3.2, 4.1, or 4.2.
+
+[Read the documentation.](http://django-ditto.readthedocs.io/en/latest/)
+
+[See screenshots of a site using the supplied templates.](https://github.com/philgyford/django-ditto/tree/main/screenshots)
+
+Install using [pip](https://pip.pypa.io/en/stable/):
+
+    $ pip install django-ditto
+
+NOTE 1: It will install [Pillow](http://pillow.readthedocs.io/en/latest/), among other things, which has prerequisites of its own, such as libjpeg and zlib. Sorry.
+
+NOTE 2: As of 2023 I'm unsure how well the Twitter integration still works given the state of its API etc.
+
+Currently, Ditto can copy these things from these services:
+
+- [Flickr](https://flickr.com/)
+  - Photos
+  - Photosets
+  - Original image and video files
+  - Users
+- [Last.fm](https://www.last.fm/)
+  - Scrobbles (Artist, Track and Album)
+- [Pinboard](https://pinboard.in/)
+  - Bookmarks
+- [Twitter](https://twitter.com/)
+  - Tweets
+  - Favorites/Likes
+  - Images and Animated GIFs (but not videos)
+  - Users
+
+The Ditto apps provide:
+
+- Models
+- Admin
+- Management commands to fetch the data/files
+- Views and URLs
+- Templates (that use [Bootstrap 4](https://getbootstrap.com))
+- Template tags for common things (eg, most recent Tweets, or Flickr photos uploaded on a particular day)
+
+
```

### Comparing `django-ditto-3.0.1/django_ditto.egg-info/SOURCES.txt` & `django-ditto-3.1.0/django_ditto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/setup.py` & `django-ditto-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-ditto-3.0.1/tox.ini` & `django-ditto-3.1.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tox]
 ; Minimum version of Tox
 minversion = 1.8
 
 envlist =
     py39-django{32,41,42,main}
     py310-django{32,41,42,main}
-    py311-django{32,41,42,main}
+    py311-django{41,42,main}
+    py312-django{42,main}
     flake8
 
 [gh-actions]
 ; Maps GitHub Actions python version numbers to tox env vars:
 python =
     3.9: py39
     3.10: py310
     3.11: py311
+    3.12: py312
 
 [gh-actions:env]
 ; Maps GitHub Actions DJANGO version env var to tox env vars:
 DJANGO =
     3.2: django32
     4.1: django41
     4.2: django42
```

