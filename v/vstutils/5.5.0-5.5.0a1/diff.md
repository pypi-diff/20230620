# Comparing `tmp/vstutils-5.5.0.tar.gz` & `tmp/vstutils-5.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.5.0.tar", last modified: Tue Jun 20 05:39:43 2023, max compression
+gzip compressed data, was "vstutils-5.5.0a1.tar", last modified: Sat Jun 17 04:45:38 2023, max compression
```

## Comparing `vstutils-5.5.0.tar` & `vstutils-5.5.0a1.tar`

### file list

```diff
@@ -1,253 +1,253 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.604236 vstutils-5.5.0/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:37:08.000000 vstutils-5.5.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-05-24 07:40:20.000000 vstutils-5.5.0/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-05-24 07:40:20.000000 vstutils-5.5.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4431 2023-06-20 05:39:43.604236 vstutils-5.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2393 2023-05-24 07:40:20.000000 vstutils-5.5.0/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 04:30:57.000000 vstutils-5.5.0/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:37:08.000000 vstutils-5.5.0/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:37:08.000000 vstutils-5.5.0/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-24 07:40:20.000000 vstutils-5.5.0/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-07 23:11:00.000000 vstutils-5.5.0/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-20 04:06:50.000000 vstutils-5.5.0/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-15 03:16:12.000000 vstutils-5.5.0/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      525 2023-06-20 04:06:50.000000 vstutils-5.5.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-20 05:39:43.608236 vstutils-5.5.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16554 2023-06-15 03:16:12.000000 vstutils-5.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.564236 vstutils-5.5.0/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-20 05:26:27.000000 vstutils-5.5.0/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.572235 vstutils-5.5.0/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:52.000000 vstutils-5.5.0/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    29374 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:42.000000 vstutils-5.5.0/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:42.000000 vstutils-5.5.0/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    13792 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:14:38.000000 vstutils-5.5.0/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.572235 vstutils-5.5.0/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.572235 vstutils-5.5.0/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    28263 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9995 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:14:38.000000 vstutils-5.5.0/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5660 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3219 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:03.000000 vstutils-5.5.0/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.556235 vstutils-5.5.0/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.576235 vstutils-5.5.0/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.576235 vstutils-5.5.0/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-20 05:39:43.612236 vstutils-5.5.0/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.576235 vstutils-5.5.0/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3467 2023-06-01 04:30:57.000000 vstutils-5.5.0/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.576235 vstutils-5.5.0/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.576235 vstutils-5.5.0/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-07 00:01:26.000000 vstutils-5.5.0/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.580236 vstutils-5.5.0/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:53.000000 vstutils-5.5.0/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25943 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:53.000000 vstutils-5.5.0/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:53.000000 vstutils-5.5.0/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:14:38.000000 vstutils-5.5.0/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    55685 2023-06-17 04:39:03.000000 vstutils-5.5.0/vstutils/settings.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:30:57.000000 vstutils-5.5.0/vstutils/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.556235 vstutils-5.5.0/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.592235 vstutils-5.5.0/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126295 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38336 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    71086 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536206 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    89997 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      476 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355788 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1798980 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/959.js
--rw-r--r--   0 root         (0) root         (0)     2191 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/959.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    77026 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303656 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-06-20 05:39:43.000000 vstutils-5.5.0/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3597 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   434535 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.592235 vstutils-5.5.0/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.592235 vstutils-5.5.0/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5182 2023-05-29 08:14:38.000000 vstutils-5.5.0/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.592235 vstutils-5.5.0/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.592235 vstutils-5.5.0/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 07:56:30.000000 vstutils-5.5.0/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.592235 vstutils-5.5.0/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.596236 vstutils-5.5.0/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.596236 vstutils-5.5.0/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.596236 vstutils-5.5.0/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.600236 vstutils-5.5.0/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.600236 vstutils-5.5.0/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.600236 vstutils-5.5.0/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.600236 vstutils-5.5.0/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.600236 vstutils-5.5.0/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.604236 vstutils-5.5.0/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.604236 vstutils-5.5.0/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.604236 vstutils-5.5.0/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.604236 vstutils-5.5.0/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    18153 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.604236 vstutils-5.5.0/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-05-24 07:40:20.000000 vstutils-5.5.0/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.5.0/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-15 03:16:12.000000 vstutils-5.5.0/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-06-06 00:37:44.000000 vstutils-5.5.0/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:37:08.000000 vstutils-5.5.0/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 05:39:43.564236 vstutils-5.5.0/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4431 2023-06-20 05:39:43.000000 vstutils-5.5.0/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7664 2023-06-20 05:39:43.000000 vstutils-5.5.0/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-06-20 05:39:43.000000 vstutils-5.5.0/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-20 05:39:43.000000 vstutils-5.5.0/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 05:38:33.000000 vstutils-5.5.0/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1812 2023-06-20 05:39:43.000000 vstutils-5.5.0/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-20 05:39:43.000000 vstutils-5.5.0/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.306711 vstutils-5.5.0a1/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-06-17 04:45:38.306711 vstutils-5.5.0a1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-06-01 04:30:57.000000 vstutils-5.5.0a1/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-06-07 23:11:00.000000 vstutils-5.5.0a1/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      511 2023-06-16 02:15:53.000000 vstutils-5.5.0a1/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-06-17 04:45:38.306711 vstutils-5.5.0a1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16554 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.254711 vstutils-5.5.0a1/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-16 04:50:59.000000 vstutils-5.5.0a1/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.262711 vstutils-5.5.0a1/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15484 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13047 2023-06-14 21:58:52.000000 vstutils-5.5.0a1/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    29374 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24041 2023-05-31 09:34:42.000000 vstutils-5.5.0a1/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    19097 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51748 2023-05-31 09:34:42.000000 vstutils-5.5.0a1/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    13792 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2023-05-29 08:14:38.000000 vstutils-5.5.0a1/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.262711 vstutils-5.5.0a1/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4641 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.262711 vstutils-5.5.0a1/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    28263 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9995 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     8435 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10788 2023-05-29 08:14:38.000000 vstutils-5.5.0a1/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5660 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3219 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-06-17 04:39:03.000000 vstutils-5.5.0a1/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.238711 vstutils-5.5.0a1/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-06-17 04:45:38.326711 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3467 2023-06-01 04:30:57.000000 vstutils-5.5.0a1/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.266711 vstutils-5.5.0a1/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10689 2023-06-07 00:01:26.000000 vstutils-5.5.0a1/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.270711 vstutils-5.5.0a1/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10729 2023-06-16 02:15:53.000000 vstutils-5.5.0a1/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25943 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    13510 2023-06-16 02:15:53.000000 vstutils-5.5.0a1/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3035 2023-06-16 02:15:53.000000 vstutils-5.5.0a1/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7976 2023-05-29 08:14:38.000000 vstutils-5.5.0a1/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    55685 2023-06-17 04:39:03.000000 vstutils-5.5.0a1/vstutils/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-01 04:30:57.000000 vstutils-5.5.0a1/vstutils/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.238711 vstutils-5.5.0a1/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.290711 vstutils-5.5.0a1/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126295 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38336 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    71086 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536206 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    89997 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      476 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355788 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1798980 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/959.js
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/959.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    77026 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303656 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-06-17 04:45:37.000000 vstutils-5.5.0a1/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   433009 2023-06-17 04:43:24.000000 vstutils-5.5.0a1/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.290711 vstutils-5.5.0a1/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.290711 vstutils-5.5.0a1/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5182 2023-05-29 08:14:38.000000 vstutils-5.5.0a1/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.290711 vstutils-5.5.0a1/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.294711 vstutils-5.5.0a1/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 07:56:30.000000 vstutils-5.5.0a1/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.294711 vstutils-5.5.0a1/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.294711 vstutils-5.5.0a1/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.294711 vstutils-5.5.0a1/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.298711 vstutils-5.5.0a1/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.298711 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.298711 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.302711 vstutils-5.5.0a1/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    18153 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.306711 vstutils-5.5.0a1/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-05-24 07:40:20.000000 vstutils-5.5.0a1/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2865 2023-06-07 00:47:44.000000 vstutils-5.5.0a1/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    47153 2023-06-15 03:16:12.000000 vstutils-5.5.0a1/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-06-06 00:37:44.000000 vstutils-5.5.0a1/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:37:08.000000 vstutils-5.5.0a1/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 04:45:38.254711 vstutils-5.5.0a1/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7664 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 04:43:25.000000 vstutils-5.5.0a1/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-06-17 04:45:38.000000 vstutils-5.5.0a1/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.5.0/LICENSE` & `vstutils-5.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/MANIFEST.in` & `vstutils-5.5.0a1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/NOTICE` & `vstutils-5.5.0a1/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/PKG-INFO` & `vstutils-5.5.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.5.0
+Version: 5.5.0a1
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.5.0/README.rst` & `vstutils-5.5.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/setup.cfg` & `vstutils-5.5.0a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/setup.py` & `vstutils-5.5.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/actions.py` & `vstutils-5.5.0a1/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/admin.py` & `vstutils-5.5.0a1/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/auth.py` & `vstutils-5.5.0a1/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/base.py` & `vstutils-5.5.0a1/vstutils/api/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/decorators.py` & `vstutils-5.5.0a1/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/decorators.pyi` & `vstutils-5.5.0a1/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/doc_generator.py` & `vstutils-5.5.0a1/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/endpoint.py` & `vstutils-5.5.0a1/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/fields.py` & `vstutils-5.5.0a1/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/filter_backends.py` & `vstutils-5.5.0a1/vstutils/api/filter_backends.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/filters.py` & `vstutils-5.5.0a1/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/health.py` & `vstutils-5.5.0a1/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/meta.py` & `vstutils-5.5.0a1/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/metrics.py` & `vstutils-5.5.0a1/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/migrations/0001_initial.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.5.0a1/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/models.py` & `vstutils-5.5.0a1/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/pagination.py` & `vstutils-5.5.0a1/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/parsers.py` & `vstutils-5.5.0a1/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/permissions.py` & `vstutils-5.5.0a1/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/renderers.py` & `vstutils-5.5.0a1/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/responses.py` & `vstutils-5.5.0a1/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/responses.pyi` & `vstutils-5.5.0a1/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/routers.py` & `vstutils-5.5.0a1/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/routers.pyi` & `vstutils-5.5.0a1/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/schema/generators.py` & `vstutils-5.5.0a1/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/schema/info.py` & `vstutils-5.5.0a1/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/schema/inspectors.py` & `vstutils-5.5.0a1/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/schema/schema.py` & `vstutils-5.5.0a1/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/serializers.py` & `vstutils-5.5.0a1/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/throttling.py` & `vstutils-5.5.0a1/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/validators.py` & `vstutils-5.5.0a1/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/api/views.py` & `vstutils-5.5.0a1/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/asgi.py` & `vstutils-5.5.0a1/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/asgi_worker.py` & `vstutils-5.5.0a1/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/auth.py` & `vstutils-5.5.0a1/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/auth.pyi` & `vstutils-5.5.0a1/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/celery_beat_scheduler.py` & `vstutils-5.5.0a1/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.5.0a1/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/environment.py` & `vstutils-5.5.0a1/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/exceptions.py` & `vstutils-5.5.0a1/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/gui/context.py` & `vstutils-5.5.0a1/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/gui/forms.py` & `vstutils-5.5.0a1/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/gui/pwa_manifest.py` & `vstutils-5.5.0a1/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/gui/views.py` & `vstutils-5.5.0a1/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/ldap_utils.py` & `vstutils-5.5.0a1/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/management/commands/_base.py` & `vstutils-5.5.0a1/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/management/commands/celery_inspect.py` & `vstutils-5.5.0a1/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/management/commands/dockerrun.py` & `vstutils-5.5.0a1/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/management/commands/newproject.py` & `vstutils-5.5.0a1/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/management/commands/run_task.py` & `vstutils-5.5.0a1/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/management/commands/runrpc.py` & `vstutils-5.5.0a1/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/management/commands/runserver.py` & `vstutils-5.5.0a1/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/management/commands/web.py` & `vstutils-5.5.0a1/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/middleware.py` & `vstutils-5.5.0a1/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/models/__init__.py` & `vstutils-5.5.0a1/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/models/base.py` & `vstutils-5.5.0a1/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/models/cent_notify.py` & `vstutils-5.5.0a1/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/models/custom_model.py` & `vstutils-5.5.0a1/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/models/custom_model.pyi` & `vstutils-5.5.0a1/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/models/decorators.py` & `vstutils-5.5.0a1/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/models/fields.py` & `vstutils-5.5.0a1/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/models/queryset.py` & `vstutils-5.5.0a1/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/settings.ini` & `vstutils-5.5.0a1/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/settings.py` & `vstutils-5.5.0a1/vstutils/settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/281.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/296.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/345.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/368.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/421.js` & `vstutils-5.5.0a1/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.5.0a1/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/618.js` & `vstutils-5.5.0a1/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/683.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/686.js` & `vstutils-5.5.0a1/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/742.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.5.0a1/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/755.js` & `vstutils-5.5.0a1/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/826.chunk.js` & `vstutils-5.5.0a1/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.5.0a1/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/844.js` & `vstutils-5.5.0a1/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/959.js` & `vstutils-5.5.0a1/vstutils/static/bundle/959.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2312,15 +2312,15 @@
                 G = o(90548),
                 Y = o(77656),
                 K = o(34952),
                 J = o(8366),
                 Q = o(76445),
                 Z = o(92649),
                 ee = o(56039),
-                te = o(79806),
+                te = o(29159),
                 oe = o(29526),
                 ne = o(37791),
                 re = o(50123),
                 ie = o(91577),
                 pe = o(4942);
             o(57658), o(33948);
             class ce {
```

### Comparing `vstutils-5.5.0/vstutils/static/bundle/959.js.LICENSE.txt` & `vstutils-5.5.0a1/vstutils/static/bundle/959.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/app_loader.js` & `vstutils-5.5.0a1/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/base.js` & `vstutils-5.5.0a1/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.5.0a1/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.5.0a1/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/output.json` & `vstutils-5.5.0a1/vstutils/static/bundle/output.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964192708333334%*

 * *Differences: {"'entrypoints'": "{'spa': {'assets': {0: {'size': 433009}}, 'assetsSize': 3679552}}"}*

```diff
@@ -26,15 +26,15 @@
             "filteredAuxiliaryAssets": 0,
             "name": "base"
         },
         "spa": {
             "assets": [
                 {
                     "name": "vstutils.js",
-                    "size": 434535
+                    "size": 433009
                 },
                 {
                     "name": "755.js",
                     "size": 89997
                 },
                 {
                     "name": "421.js",
@@ -57,15 +57,15 @@
                     "size": 1798980
                 },
                 {
                     "name": "spa.js",
                     "size": 3597
                 }
             ],
-            "assetsSize": 3681078,
+            "assetsSize": 3679552,
             "auxiliaryAssetsSize": 117924,
             "filteredAssets": 0,
             "filteredAuxiliaryAssets": 2,
             "name": "spa"
         }
     },
     "errors": []
```

### Comparing `vstutils-5.5.0/vstutils/static/bundle/spa.js` & `vstutils-5.5.0a1/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static/bundle/vstutils.js` & `vstutils-5.5.0a1/vstutils/static/bundle/vstutils.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1178,15 +1178,15 @@
                     }
                 },
                 computed: {
                     attrs() {
                         return (0, i.Zf)(this.field)
                     },
                     aria_label() {
-                        return this.field.title
+                        return this.field.options.title || this.field.options.name + "field"
                     }
                 }
             };
             t.Z = s
         },
         57800: function(e, t) {
             const n = {
@@ -1881,14 +1881,48 @@
                     t || (t = e), r.error(e), console.error(t)
                 }
                 defineErrorAndShow(e) {
                     return this.showError(this.errorToString(e))
                 }
             }
         },
+        29159: function(e, t, n) {
+            n.r(t), n.d(t, {
+                RouterConstructor: function() {
+                    return a
+                }
+            }), n(33948), n(57658);
+            var i = n(78345),
+                s = n(64765);
+            class a {
+                constructor(e) {
+                    this.views = e, this.routes = this.formAllRoutes()
+                }
+                getRoutes() {
+                    return this.routes
+                }
+                formAllRoutes() {
+                    let e = [];
+                    return e = e.concat(this.formRoutesBasedOnViews()), s.pp.emit("allRoutes.created", e), e
+                }
+                formRoutesBasedOnViews() {
+                    let e = [];
+                    for (let t of this.views.values()) t.hidden || (e.push(t.toRoute()), this.emitSignalAboutRouteCreation(e.last));
+                    return e
+                }
+                emitSignalAboutRouteCreation(e) {
+                    s.pp.emit("routes[" + e.name + "].created", e)
+                }
+                getRouter() {
+                    return new i.ZP({
+                        routes: this.getRoutes()
+                    })
+                }
+            }
+        },
         97320: function(e, t, n) {
             n.r(t), n(88449), n(2490), n(59849), n(15306);
             var i = n(70538),
                 s = n(59198);
             i.default.filter("capitalize", s.capitalize), i.default.filter("split", (function(e) {
                 return e ? e.replace(/_/g, " ") : ""
             })), i.default.filter("lower", (function(e) {
@@ -2164,72 +2198,78 @@
         },
         32465: function(e, t, n) {
             n.d(t, {
                 Nv: function() {
                     return N
                 },
                 le: function() {
-                    return z
+                    return W
                 },
                 zr: function() {
                     return A
                 },
                 cO: function() {
-                    return L
+                    return q
                 },
                 t$: function() {
                     return E
                 },
                 pi: function() {
                     return _
                 },
                 _y: function() {
                     return S
                 },
                 kC: function() {
                     return p
                 },
                 F3: function() {
-                    return ae
+                    return le
                 },
                 NC: function() {
-                    return K
+                    return J
                 },
                 vQ: function() {
-                    return D
+                    return j
                 },
                 vZ: function() {
                     return w
                 },
                 lS: function() {
-                    return j
+                    return L
                 },
                 Xv: function() {
-                    return H
+                    return G
                 },
                 _q: function() {
                     return P
                 },
+                dI: function() {
+                    return D
+                },
                 fq: function() {
-                    return Y
+                    return K
                 },
                 F2: function() {
-                    return le
+                    return pe
                 },
                 zs: function() {
-                    return Q
+                    return Y
                 },
                 ej: function() {
                     return b
                 },
                 JG: function() {
                     return M
                 },
                 PP: function() {
-                    return oe
+                    return ce
+                },
+                xH: function() {
+                    return de
                 },
                 NN: function() {
                     return Z
                 },
                 lf: function() {
                     return d
                 },
@@ -2239,90 +2279,99 @@
                 mR: function() {
                     return F
                 },
                 Qr: function() {
                     return g
                 },
                 MU: function() {
-                    return ee
+                    return ne
                 },
                 Kn: function() {
                     return I
                 },
+                mF: function() {
+                    return se
+                },
+                RQ: function() {
+                    return te
+                },
                 zO: function() {
                     return h
                 },
                 OS: function() {
-                    return G
+                    return z
                 },
                 O3: function() {
-                    return te
+                    return ie
                 },
                 Pe: function() {
-                    return de
+                    return he
                 },
                 XP: function() {
-                    return ue
+                    return fe
                 },
                 QA: function() {
                     return O
                 },
                 Ee: function() {
                     return R
                 },
                 Dv: function() {
                     return f
                 },
                 D$: function() {
                     return T
                 },
                 NB: function() {
-                    return W
+                    return Q
                 },
                 MP: function() {
                     return C
                 },
+                Qb: function() {
+                    return me
+                },
                 MW: function() {
-                    return J
+                    return X
                 },
                 NI: function() {
-                    return X
+                    return ee
                 },
                 tn: function() {
                     return V
                 },
                 ri: function() {
-                    return U
+                    return H
                 },
                 O1: function() {
                     return k
                 },
                 Z7: function() {
-                    return se
+                    return oe
                 },
                 Wu: function() {
                     return y
                 },
                 _v: function() {
-                    return q
+                    return $
                 },
                 TB: function() {
                     return v
                 },
                 yp: function() {
-                    return ie
+                    return re
                 },
                 $l: function() {
-                    return ne
+                    return ae
                 },
                 hb: function() {
                     return x
                 },
                 bF: function() {
-                    return re
+                    return ue
                 },
                 XK: function() {
                     return B
                 },
                 A2: function() {
                     return m
                 }
@@ -2650,161 +2699,201 @@
             }
             const N = {
                 LIST: "list",
                 READ_ONLY: "readonly",
                 EDIT: "edit"
             };
 
-            function D(e) {
+            function D(e, t) {
+                let n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : null;
+                for (const [n, i] of Object.entries(t)) e = e.replace("{".concat(n, "}"), i);
+                return n ? e.replace(/{.+}/, n.getPkValue()) : e
+            }
+
+            function j(e) {
                 if (void 0 === navigator.clipboard) {
                     const t = document.createElement("textarea");
                     t.value = e, t.style.position = "fixed", document.body.appendChild(t), t.focus(), t.select();
                     try {
                         document.execCommand("copy")
                     } catch (e) {
                         console.warning("Was not possible to copy text: ", e)
                     }
                     document.body.removeChild(t)
                 } else navigator.clipboard.writeText(e || "").catch(console.warn)
             }
 
-            function j(e) {
+            function L(e) {
                 let t;
                 t = "" === e.mediaType ? e.content : "data:".concat(e.mediaType || "text/plain", ";base64,").concat(e.content);
                 const n = document.createElement("a");
                 n.href = t, n.download = e.name, n.click()
             }
-            const L = {
+            const q = {
                 LIST: "LIST",
                 PAGE: "PAGE",
                 PAGE_NEW: "PAGE_NEW",
                 PAGE_EDIT: "PAGE_EDIT",
                 PAGE_REMOVE: "PAGE_REMOVE",
                 ACTION: "ACTION"
             };
 
-            function q(e) {
+            function $(e) {
                 return new Promise((t => setTimeout(t, e)))
             }
 
-            function $(e, t) {
+            function U(e, t) {
                 return Math.floor(Math.random() * (t - e) + e)
             }
 
-            function U(e, t) {
-                return q($(e, t))
+            function H(e, t) {
+                return $(U(e, t))
             }
 
-            function H(e) {
+            function G(e) {
                 return e.replace(/&/g, "&amp;").replace(/</g, "&lt;").replace(/>/g, "&gt;").replace(/"/g, "&quot;").replace(/'/g, "&#039;")
             }
 
-            function G(e) {
+            function z(e) {
                 return "" === e.mediaType ? e.content : "data:".concat(e.mediaType || "image/png", ";base64,").concat(e.content)
             }
-            const z = ["offset", "limit", "page", "__deep_parent"];
+            const W = ["offset", "limit", "page", "__deep_parent"];
 
-            function W(e) {
+            function Q(e) {
                 const t = new FormData;
                 for (let [n, i] of Object.entries(e)) t.append(n, i);
                 return t
             }
 
-            function Q(e) {
+            function Y(e) {
                 let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789",
                     n = "";
                 const i = t.length;
                 for (let s = 0; s < e; s++) n += t.charAt(Math.floor(Math.random() * i));
                 return n
             }
 
-            function Y() {
-                return Q(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 32, "ABCDEFGHIJKLMNOPQRSTUVWXYZ234567")
+            function K() {
+                return Y(arguments.length > 0 && void 0 !== arguments[0] ? arguments[0] : 32, "ABCDEFGHIJKLMNOPQRSTUVWXYZ234567")
             }
 
-            function K(e, t) {
+            function J(e, t) {
                 return e.filter((e => "choices" === e.format || "boolean" === e.type)).map((e => {
                     let n = "field-".concat(e.name);
                     const i = e._getValueFromData(t);
-                    return void 0 !== i && (n += "-".concat(re(i))), n
+                    return void 0 !== i && (n += "-".concat(ue(i))), n
                 }))
             }
 
-            function J(e) {
-                return e ? "string" == typeof e ? e : e.detail ? J(e.detail) : Array.isArray(e) ? e.join("<br>") : "object" == typeof e ? Object.entries(e).reduce(((e, t) => {
+            function X(e) {
+                return e ? "string" == typeof e ? e : e.detail ? X(e.detail) : Array.isArray(e) ? e.join("<br>") : "object" == typeof e ? Object.entries(e).reduce(((e, t) => {
                     let [n, i] = t;
                     return e + "<b>".concat(n, ":</b> ").concat(i, "<br>")
                 }), "") : "" : ""
             }
 
-            function X(e) {
+            function ee(e) {
                 return e.replace(/^\/|\/$/g, "").split("/")
             }
 
-            function ee(e, t) {
+            function te() {
+                for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
+                return t.reduce(((e, t) => e + "/" + String(t).replace(/^\/|\/$/g, "")), "") + "/"
+            }
+
+            function ne(e, t) {
                 if (e === t) return !0;
                 if (!e || !t) return !1;
                 if (e.length !== t.length) return !1;
                 for (let n = 0; n < e.length; n++)
                     if (!e[n].isEqual(t[n])) return !1;
                 return !0
             }
 
-            function te(e, t) {
+            function ie(e, t) {
                 const n = {};
                 for (const i in e) c(e, i) && (n[i] = t(e[i], i));
                 return n
             }
 
-            function ne(e) {
+            function se(e, t) {
+                for (const n of e)
+                    if (t(n)) return n
+            }
+
+            function ae(e) {
                 "Enter" === e.code && e.stopPropagation()
             }
 
-            function ie(e) {
-                e.addEventListener("keyup", ne)
+            function re(e) {
+                e.addEventListener("keyup", ae)
             }
 
-            function se(e) {
-                e.removeEventListener("keyup", ne)
+            function oe(e) {
+                e.removeEventListener("keyup", ae)
             }
 
-            function ae(e, t) {
+            function le(e, t) {
                 return e.reduce(((e, n, i) => {
                     const s = Math.floor(i / t);
                     return e[s] || (e[s] = []), e[s].push(n), e
                 }), [])
             }
 
-            function re(e) {
+            function ue(e) {
                 return "string" != typeof e && (e = String(e)), e.replace(/\s/g, "")
             }
-            const oe = null !== (i = globalThis.crypto) && void 0 !== i && i.getRandomValues ? e => crypto.getRandomValues(new Uint8Array(e)) : e => Array.from(new Array(e), (() => Math.round(255 * Math.random())));
 
-            function le() {
+            function de(e, t) {
+                if (!e || "object" != typeof e || !t) return;
+                const n = (0, l.M)(),
+                    i = se(t.fields.values(), (e => e.redirect));
+                if (!i) return;
+                const s = i.redirect;
+                let a = "";
+                s.depend_field && (a += e[s.depend_field].toLowerCase()), a && !s.concat_field_name || (a += s.operation_name), a += "_get";
+                const r = n.viewsTree.findInAllPaths((e => e.operationId === a && e));
+                if (r) {
+                    if (![null, void 0].includes(e[i.name])) return D(r.path, {
+                        ...n.router.currentRoute.params,
+                        [r.pkParamName]: e[i.name]
+                    })
+                } else console.warn("Can't find redirect view for operationId: ".concat(a), i, e)
+            }
+            const ce = null !== (i = globalThis.crypto) && void 0 !== i && i.getRandomValues ? e => crypto.getRandomValues(new Uint8Array(e)) : e => Array.from(new Array(e), (() => Math.round(255 * Math.random())));
+
+            function pe() {
                 const e = [];
                 for (const t of ["ABCDEFGHIJKLMNOPQRSTUVWXYZ", "abcdefghijklmnopqrstuvwxyz", "~!@-#$", "0123456789"])
-                    for (const n of oe($(3, 5))) e.push(t[n % t.length]);
+                    for (const n of ce(U(3, 5))) e.push(t[n % t.length]);
                 return e.sort((() => Math.random() - .5)).join("")
             }
 
-            function ue(e) {
+            function fe(e) {
                 const t = {};
                 for (const n of e) t[n] = function() {
                     return this.store[n]
                 };
                 return t
             }
 
-            function de(e) {
+            function he(e) {
                 const t = {};
                 for (const n of e) t[n] = function() {
                     return this.store[n](...arguments)
                 };
                 return t
             }
+
+            function me(e) {
+                let t = arguments.length > 1 && void 0 !== arguments[1] ? arguments[1] : void 0;
+                const n = (0, l.M)().router,
+                    i = e.appendFragment ? te(n.currentRoute.path, e.appendFragment) : e.href;
+                return n.push(D(i, n.currentRoute.params, t))
+            }
         },
         60113: function(e, t, n) {
             n.d(t, {
                 Z: function() {
                     return B
                 }
             }), n(15306), n(31672), n(2490), n(59461), n(33948), n(10072), n(23042), n(99137), n(71957), n(96306), n(103), n(74592), n(58276), n(35082), n(12813), n(18222), n(38563), n(50336), n(7512), n(57640), n(9924), n(21703), n(57658), n(88449), n(59849);
@@ -3296,24 +3385,24 @@
                             const s = i[n];
                             if (!s) continue;
                             const d = s[this.dictionary.paths.operation_id.name],
                                 c = Object.values(null !== (f = s.parameters) && void 0 !== f ? f : []).find(M),
                                 p = c ? this._getOperationModel(c) : null,
                                 m = Object.keys(s.responses).find(V),
                                 v = s.responses[m],
-                                g = "file" === (null === (h = v.schema) || void 0 === h ? void 0 : h.type),
+                                g = null === (h = v.schema) || void 0 === h ? void 0 : h.type,
                                 _ = this._getOperationModel(v),
                                 b = (0, a.mergeDeep)({
                                     method: n,
                                     requestModel: p,
                                     responseModel: _,
                                     isDeepNested: Boolean(P)
                                 }, y, s, this.getOperationOptions(d, e, n));
                             if (b["x-label"] && (b.title = b["x-label"]), b.type !== a.ViewTypes.LIST) {
-                                if (b.type === a.ViewTypes.PAGE) b.isFileResponse = g, C = new u.B4(b, null), C.filtersModelClass = this.getDetailFiltersModelClass(b.parameters), C.filtersModelClass && C.actions.set("filter", {
+                                if (b.type === a.ViewTypes.PAGE) b.isFileResponse = "file" === g, C = new u.B4(b, null), C.filtersModelClass = this.getDetailFiltersModelClass(b.parameters), C.filtersModelClass && C.actions.set("filter", {
                                     ...this.dictionary.paths.operations.page.filters
                                 }), t.set(C.path, C);
                                 else if (b.type === a.ViewTypes.PAGE_NEW) k = new u.Uc(b, null), t.set(k.path, k);
                                 else if (b.type === a.ViewTypes.PAGE_EDIT) S = new u.W(b, null), t.set(S.path, S);
                                 else if (b.type === a.ViewTypes.PAGE_REMOVE) F = !0;
                                 else if (b.type === a.ViewTypes.ACTION) {
                                     const i = !p || 0 === p.writableFields.length || p === l.NoModel,
@@ -3324,27 +3413,25 @@
                                             title: b["x-title"] || b.title,
                                             method: n,
                                             path: e,
                                             requestModel: p,
                                             responseModel: _,
                                             isMultiAction: s,
                                             isEmpty: i,
-                                            isFileResponse: g,
                                             hidden: b["x-hidden"],
                                             iconClasses: b["x-icons"] || b.iconClasses
                                         };
                                     if (i) o.confirmationRequired = r;
                                     else {
                                         b.action = o;
                                         const e = new u.kl(b, null),
                                             n = {
                                                 ...this.dictionary.paths.operations.action.execute,
                                                 title: b["x-action-name"] || b.title,
-                                                confirmationRequired: r,
-                                                isFileResponse: g
+                                                confirmationRequired: r
                                             };
                                         e.actions.set(n.name, n), o.appendFragment = (0, a.pathToArray)(e.path).last, o.view = e, t.set(e.path, e)
                                     }
                                     Z = o
                                 }
                             } else {
                                 b.filters = this._generateFilters(e, b.parameters, _);
@@ -3374,19 +3461,18 @@
                             const e = S.isPartial ? a.RequestTypes.PARTIAL_UPDATE : a.RequestTypes.UPDATE;
                             C.objects.models[e] = S.modelsList, S.objects = C.objects
                         }
                         if (E && I && !w.hidden && _.sublinks.set(w.params.name, {
                                 name: w.params.name,
                                 title: w.params.title,
                                 appendFragment: w.params.name
-                            }), A && S && C && (t.delete(S.path), t.set(C.path, S), S.path = C.path, S.isEditStyleOnly = !0, C = S), E && D && !C.hidden && _.sublinks.set(C.name, {
-                                name: C.name,
-                                title: C.title,
-                                href: C.path,
-                                isFileResponse: C.isFileResponse
+                            }), A && S && C && (t.delete(S.path), t.set(C.path, S), S.path = C.path, S.isEditStyleOnly = !0, C = S), E && D && !C.hidden && _.sublinks.set(C.params.name, {
+                                name: C.params.name,
+                                title: C.params.title,
+                                href: C.path
                             }), C && j && (_.pageView = C, C.listView = _, S && (S.listView = _)), S) {
                             const e = (0, a.mergeDeep)({}, this.dictionary.paths.operations.page_edit.save),
                                 t = (0, a.mergeDeep)({}, this.dictionary.paths.operations.page_edit.reload);
                             S.actions.set(e.name, e), S.actions.set(t.name, t)
                         }
                         if (S && !A && !S.hidden) {
                             const e = (0, a.mergeDeep)({
@@ -3577,19 +3663,20 @@
                         path: n,
                         method: t
                     })
                 }
             }
             class l {
                 constructor() {
+                    var e;
                     (0, s.Z)(this, "appConfig", null), (0, s.Z)(this, "openapi", null), (0, s.Z)(this, "defaultVersion", null), (0, s.Z)(this, "endpointURL", null), (0, s.Z)(this, "headers", void 0), (0, s.Z)(this, "bulkCollector", {
                         bulkParts: []
-                    }), (0, s.Z)(this, "baseURL", null), (0, s.Z)(this, "_etagsCachePrefix", null), (0, s.Z)(this, "_etagsCacheName", null), this.headers = {};
-                    const e = (0, i.getCookie)("csrftoken");
-                    e && (this.headers["X-CSRFToken"] = e)
+                    }), (0, s.Z)(this, "baseURL", null), (0, s.Z)(this, "_etagsCachePrefix", null), (0, s.Z)(this, "_etagsCacheName", null), this.headers = {
+                        "X-CSRFToken": null !== (e = (0, i.getCookie)("csrftoken")) && void 0 !== e ? e : ""
+                    }
                 }
                 initConfiguration(e) {
                     var t;
                     this.appConfig = e, this.openapi = e.schema, this.defaultVersion = this.openapi.info.version, this.endpointURL = String(e.endpointUrl);
                     const n = null === (t = this.openapi.basePath) || void 0 === t ? void 0 : t.replace(this.defaultVersion, "").replace(/\/$/, "");
                     return this.baseURL = "".concat(this.openapi.schemes[0], "://").concat(this.openapi.host).concat(n), r && (this._etagsCachePrefix = "etags-cache", this._etagsCacheName = "".concat(this._etagsCachePrefix, "-").concat(this.appConfig.fullUserVersion), this._removeOldEtagsCaches()), this
                 }
@@ -3604,33 +3691,31 @@
                         };
                         e.version && (t.version = e.version);
                         const n = (0, i.makeQueryString)(e.query, !0);
                         n && (t.query = n), e.headers && (t.headers = e.headers), e.data && (t.data = e.data);
                         const s = await this.bulkQuery(t);
                         return new o(s)
                     } {
-                        const t = {
-                            ...this.headers,
-                            ...e.headers
-                        };
-                        let n;
-                        void 0 !== e.data && (e.data instanceof FormData ? n = e.data : (n = JSON.stringify(e.data), t["Content-Type"] = "application/json"));
-                        const s = Array.isArray(e.path) ? e.path.join("/") : e.path.replace(/^\//, ""),
-                            a = "".concat(this.getFullUrl(s)).concat((0, i.makeQueryString)(e.query)),
-                            r = await fetch(a, {
+                        var t;
+                        const n = Array.isArray(e.path) ? e.path.join("/") : e.path.replace(/^\/|\/$/g, ""),
+                            s = {
+                                ...this.headers,
+                                ...e.headers
+                            };
+                        let a;
+                        void 0 !== e.data && (e.data instanceof FormData ? a = e.data : (a = JSON.stringify(e.data), s["Content-Type"] = "application/json"));
+                        const r = [this.baseURL, null !== (t = e.version) && void 0 !== t ? t : this.defaultVersion, n, (0, i.makeQueryString)(e.query)].join("/"),
+                            l = await fetch(r, {
                                 method: e.method,
-                                headers: t,
-                                body: n
+                                headers: s,
+                                body: a
                             });
-                        return e.rawResponse ? r : await o.fromFetchResponse(r, e.method, a)
+                        return await o.fromFetchResponse(l, e.method, r)
                     }
                 }
-                getFullUrl(e) {
-                    return e = e.replace(/^\/|\/$/g, ""), "".concat(this.baseURL, "/").concat(this.defaultVersion, "/").concat(e, "/")
-                }
                 _bulkItemToRequest(e) {
                     let {
                         version: t = this.defaultVersion,
                         method: n,
                         path: s,
                         query: a = "",
                         headers: r
@@ -3827,29 +3912,20 @@
                         action: t,
                         instance: n,
                         redirect: i = !0,
                         disablePopUp: s = !1
                     } = e;
                     const a = (0, l.formatPath)(t.path, this.app.router.currentRoute.params, n);
                     try {
-                        let e;
-                        if (t.isFileResponse) {
-                            const e = await this.app.api.makeRequest({
-                                method: t.method,
-                                path: a,
-                                rawResponse: !0
-                            });
-                            await (0, l.downloadResponse)(e)
-                        } else e = await this.app.api.makeRequest({
+                        const e = await this.app.api.makeRequest({
                             useBulk: !0,
                             method: t.method,
                             path: a
                         });
-                        var r;
-                        if (s || o.guiPopUp.success(u.a.t(o.pop_up_msg.instance.success.executeEmpty, [u.a.t(t.title), (null == n ? void 0 : n.getViewFieldString()) || u.a.t(this.currentView.title), (0, l.parseResponseMessage)(null === (r = e) || void 0 === r ? void 0 : r.data)])), t.onAfter && t.onAfter({
+                        if (s || o.guiPopUp.success(u.a.t(o.pop_up_msg.instance.success.executeEmpty, [u.a.t(t.title), (null == n ? void 0 : n.getViewFieldString()) || u.a.t(this.currentView.title), (0, l.parseResponseMessage)(e.data)])), t.onAfter && t.onAfter({
                                 app: this.app,
                                 action: t,
                                 instance: n,
                                 response: e
                             }), i && e && e.data) try {
                             const n = (0, l.getRedirectUrlFromResponse)(e.data, t.responseModel);
                             if (n) return void(0, l.openPage)(n)
@@ -3878,31 +3954,21 @@
                     } catch (e) {
                         if (this.app.error_handler.defineErrorAndShow(e), r) throw e;
                         return
                     }
                     const p = (0, l.emptyInnerData)();
                     for (const e of i._fields.values())(c || e.required || i.sandbox.changedFields.has(e.name)) && (p[e.name] = t[e.name]);
                     try {
-                        let e;
-                        if (n.isFileResponse) {
-                            const e = await this.app.api.makeRequest({
-                                method: s,
-                                path: null != a ? a : (0, l.formatPath)(n.path, this.app.router.currentRoute.params),
-                                data: t,
-                                rawResponse: !0
-                            });
-                            await (0, l.downloadResponse)(e)
-                        } else e = await this.app.api.makeRequest({
+                        const e = await this.app.api.makeRequest({
                             method: s,
                             path: null != a ? a : (0, l.formatPath)(n.path, this.app.router.currentRoute.params),
                             data: t,
                             useBulk: i.shouldUseBulk(s)
                         });
-                        var f;
-                        return d || o.guiPopUp.success(u.a.t(o.pop_up_msg.instance.success.execute, [u.a.t(this.currentView.title), (0, l.parseResponseMessage)(null === (f = e) || void 0 === f ? void 0 : f.data)])), n.onAfter && n.onAfter({
+                        return d || o.guiPopUp.success(u.a.t(o.pop_up_msg.instance.success.execute, [u.a.t(this.currentView.title), (0, l.parseResponseMessage)(e.data)])), n.onAfter && n.onAfter({
                             app: this.app,
                             action: n,
                             instance: i,
                             response: e
                         }), e
                     } catch (e) {
                         const t = i.parseModelError(e.data);
@@ -3944,15 +4010,15 @@
             }
             var f = n(35853),
                 h = n(94363),
                 m = n(50123),
                 v = n(77656),
                 g = n(8366),
                 _ = n(76445),
-                b = n(79806),
+                b = n(29159),
                 y = n(64765),
                 w = n(56039),
                 x = n(92649),
                 C = n(60113);
             class S {
                 constructor(e, t, n) {
                     (0, i.Z)(this, "config", void 0), (0, i.Z)(this, "vue", void 0), (0, i.Z)(this, "cache", void 0), (0, i.Z)(this, "schema", void 0), (0, i.Z)(this, "fieldsResolver", void 0), (0, i.Z)(this, "modelsResolver", void 0), (0, i.Z)(this, "translationsManager", void 0), (0, i.Z)(this, "qsResolver", void 0), (0, i.Z)(this, "error_handler", void 0), (0, i.Z)(this, "viewsTree", null), (0, i.Z)(this, "global_components", void 0), (0, i.Z)(this, "centrifugoClient", void 0), (0, i.Z)(this, "router", void 0), (0, i.Z)(this, "i18n", void 0), (0, i.Z)(this, "api", void 0), (0, i.Z)(this, "languages", void 0), (0, i.Z)(this, "rawUser", void 0), (0, i.Z)(this, "user", void 0), (0, i.Z)(this, "appRootComponent", void 0), (0, i.Z)(this, "additionalRootMixins", void 0), (0, i.Z)(this, "views", new Map), (0, i.Z)(this, "store", void 0), (0, i.Z)(this, "userSettingsStore", void 0), (0, i.Z)(this, "localSettingsStore", null), (0, i.Z)(this, "localSettingsModel", void 0), (0, i.Z)(this, "autoUpdateController", void 0), (0, i.Z)(this, "actions", void 0), (0, i.Z)(this, "rootVm", null), (0, i.Z)(this, "application", null), globalThis.__currentApp = this, this.config = e, this.vue = null != n ? n : globalThis.Vue, this.schema = e.schema, this.router = null, this.cache = t, this.i18n = u.a, this.api = c.apiConnector.initConfiguration(e), this.translationsManager = new p(c.apiConnector, t), this.centrifugoClient = function(e, t) {
@@ -14191,38 +14257,27 @@
                 _isModelInstance(e) {
                     return Boolean(e && "_getInnerData" in e && "function" == typeof e._getInnerData)
                 }
                 async execute(e) {
                     var t;
                     const n = e.data,
                         i = this._isModelInstance(n),
-                        s = null !== (t = e.useBulk) && void 0 !== t ? t : !i || n.shouldUseBulk(e.method),
-                        a = {
+                        s = {
+                            useBulk: null !== (t = e.useBulk) && void 0 !== t ? t : !i || n.shouldUseBulk(e.method),
                             method: e.method,
                             path: e.path,
                             query: e.query,
                             headers: e.headers,
                             version: e.version
                         };
                     if (void 0 !== n) {
                         const e = i ? n._getInnerData() : n;
-                        return s ? r.apiConnector.makeRequest({
-                            ...a,
-                            useBulk: s,
-                            data: e
-                        }) : r.apiConnector.makeRequest({
-                            ...a,
-                            useBulk: s,
-                            data: (0, l.objectToFormData)(e)
-                        })
+                        s.useBulk ? s.data = e : s.data = (0, l.objectToFormData)(e)
                     }
-                    return r.apiConnector.makeRequest({
-                        ...a,
-                        useBulk: s
-                    })
+                    return r.apiConnector.makeRequest(s)
                 }
                 clearCache() {
                     this.cache = void 0
                 }
             }
             class h extends Error {
                 constructor() {
@@ -14274,53 +14329,14 @@
                 }
             }
             const g = new Map([
                     ["QuerySet", f]
                 ]),
                 _ = (0, l.mapToObjectProxy)(g)
         },
-        79806: function(e, t, n) {
-            n.r(t), n.d(t, {
-                RouterConstructor: function() {
-                    return r
-                }
-            });
-            var i = n(4942),
-                s = (n(33948), n(57658), n(78345)),
-                a = n(64765);
-            class r {
-                constructor(e) {
-                    (0, i.Z)(this, "views", void 0), (0, i.Z)(this, "routes", void 0), this.views = e, this.routes = this.formAllRoutes()
-                }
-                getRoutes() {
-                    return this.routes
-                }
-                formAllRoutes() {
-                    const e = this.formRoutesBasedOnViews();
-                    return a.pp.emit("allRoutes.created", e), e
-                }
-                formRoutesBasedOnViews() {
-                    const e = [];
-                    for (const t of this.views.values()) {
-                        const n = t.toRoute();
-                        n && (e.push(n), this.emitSignalAboutRouteCreation(n))
-                    }
-                    return e
-                }
-                emitSignalAboutRouteCreation(e) {
-                    var t;
-                    a.pp.emit("routes[" + (null !== (t = e.name) && void 0 !== t ? t : e.path) + "].created", e)
-                }
-                getRouter() {
-                    return new s.ZP({
-                        routes: this.getRoutes()
-                    })
-                }
-            }
-        },
         56430: function(e, t, n) {
             n.d(t, {
                 G: function() {
                     return a
                 }
             });
             var i = n(70538),
@@ -14856,15 +14872,15 @@
                                         action: s,
                                         instance: t.instance.value,
                                         method: e.method,
                                         path: e.getRequestPath(n.router.currentRoute),
                                         throwError: !0
                                     });
                                 var i;
-                                t.instance.value.sandbox.markUnchanged(), t.fieldsErrors.value = {}, s.redirectPath ? (0, r.openPage)("function" == typeof s.redirectPath ? s.redirectPath() : s.redirectPath) : (0, r.openPage)(null !== (i = (0, r.getRedirectUrlFromResponse)(null == a ? void 0 : a.data, e.action.responseModel)) && void 0 !== i ? i : e.getRedirectUrl(n.router.currentRoute))
+                                t.instance.value.sandbox.markUnchanged(), t.fieldsErrors.value = {}, s.redirectPath ? (0, r.openPage)("function" == typeof s.redirectPath ? s.redirectPath() : s.redirectPath) : (0, r.openPage)(null !== (i = (0, r.getRedirectUrlFromResponse)(a.data, e.action.responseModel)) && void 0 !== i ? i : e.getRedirectUrl(n.router.currentRoute))
                             } catch (e) {
                                 e instanceof o.ModelValidationError ? t.fieldsErrors.value = e.toFieldsErrors() : console.warn(e)
                             }
                         }
                     }
                 };
             async function k(e) {
@@ -15637,40 +15653,34 @@
                 },
                 createUniqueIdGenerator: function() {
                     return Z
                 },
                 deepEqual: function() {
                     return a.vZ
                 },
-                defaultDownloadResponseHandler: function() {
-                    return L
-                },
                 deferredPromise: function() {
                     return w
                 },
                 downloadBase64File: function() {
                     return a.lS
                 },
-                downloadResponse: function() {
-                    return q
-                },
                 emptyInnerData: function() {
                     return k
                 },
                 emptyRepresentData: function() {
                     return F
                 },
                 escapeHtml: function() {
                     return a.Xv
                 },
                 findClosestPath: function() {
                     return a._q
                 },
                 formatPath: function() {
-                    return I
+                    return a.dI
                 },
                 generateBase32String: function() {
                     return a.fq
                 },
                 generatePassword: function() {
                     return a.F2
                 },
@@ -15689,15 +15699,15 @@
                 getRandomInt: function() {
                     return u
                 },
                 getRandomValues: function() {
                     return a.PP
                 },
                 getRedirectUrlFromResponse: function() {
-                    return O
+                    return a.xH
                 },
                 getTimeInUptimeFormat: function() {
                     return a.NN
                 },
                 getUniqueId: function() {
                     return A
                 },
@@ -15719,18 +15729,18 @@
                 isNotFoundView: function() {
                     return V
                 },
                 isObject: function() {
                     return a.Kn
                 },
                 iterFind: function() {
-                    return B
+                    return a.mF
                 },
                 joinPaths: function() {
-                    return M
+                    return a.RQ
                 },
                 loadImage: function() {
                     return y
                 },
                 lower: function() {
                     return a.zO
                 },
@@ -15767,18 +15777,15 @@
                 oneCharNumberToTwoChar: function() {
                     return a.MP
                 },
                 openPage: function() {
                     return T
                 },
                 openSublink: function() {
-                    return R
-                },
-                parseFileResponseName: function() {
-                    return N
+                    return a.Qb
                 },
                 parseResponseMessage: function() {
                     return a.MW
                 },
                 pathToArray: function() {
                     return a.NI
                 },
@@ -15808,17 +15815,14 @@
                 },
                 saveAllSettings: function() {
                     return P
                 },
                 saveHideMenuSettings: function() {
                     return a.Wu
                 },
-                setFileDownloadHandler: function() {
-                    return j
-                },
                 sleep: function() {
                     return a._v
                 },
                 sliceLongString: function() {
                     return a.TB
                 },
                 stopEnterPropagation: function() {
@@ -15838,15 +15842,15 @@
                 },
                 template: function() {
                     return a.XK
                 },
                 upper: function() {
                     return a.A2
                 }
-            }), n(57658), n(82472), n(48675), n(33105), n(63408), n(14590), n(3462), n(33824), n(8922), n(5835), n(23767), n(8585), n(8970), n(84444), n(68696), n(82801), n(33948), n(41637), n(81299), n(25387), n(2490), n(72608), n(15306), n(60285);
+            }), n(57658), n(82472), n(48675), n(33105), n(63408), n(14590), n(3462), n(33824), n(8922), n(5835), n(23767), n(8585), n(8970), n(84444), n(68696), n(82801), n(33948), n(41637), n(81299);
             var i = n(78345),
                 s = n(46509),
                 a = n(32465);
             const r = Symbol("EMPTY"),
                 o = {
                     GET: "get",
                     POST: "post",
@@ -15998,96 +16002,14 @@
                 return t
             }
             const E = "404";
 
             function V(e) {
                 return e.routeName === E
             }
-
-            function M() {
-                for (var e = arguments.length, t = new Array(e), n = 0; n < e; n++) t[n] = arguments[n];
-                return t.reduce(((e, t) => e + "/" + String(null != t ? t : "").replace(/^\/|\/$/g, "")), "") + "/"
-            }
-
-            function I(e, t, n) {
-                for (const [n, i] of Object.entries(t)) e = e.replace("{".concat(n, "}"), String(i));
-                return n ? e.replace(/{.+}/, String(n.getPkValue())) : e
-            }
-            async function R(e, t) {
-                const {
-                    router: n,
-                    api: i,
-                    error_handler: a
-                } = (0, s.M)();
-                let r = e.appendFragment ? M(n.currentRoute.path, e.appendFragment) : e.href;
-                if ("function" == typeof r && (r = r()), r = I(r, n.currentRoute.params, t), e.isFileResponse) try {
-                    const t = e.external ? await fetch(r) : await i.makeRequest({
-                        rawResponse: !0,
-                        method: "get",
-                        path: r
-                    });
-                    await q(t)
-                } catch (e) {
-                    a.defineErrorAndShow(e)
-                } else {
-                    if (!e.external) return n.push(r);
-                    window.open(r, "_blank")
-                }
-            }
-
-            function O(e, t) {
-                if (!e || "object" != typeof e || !t) return;
-                const n = (0, s.M)(),
-                    i = B(t.fields.values(), (e => e.redirect));
-                if (!i) return;
-                const a = i.redirect;
-                let r = "";
-                if (a.depend_field) {
-                    const t = e[a.depend_field],
-                        n = t ? String(t) : "";
-                    r += n.toLowerCase()
-                }
-                var o;
-                r && !a.concat_field_name || (r += null !== (o = a.operation_name) && void 0 !== o ? o : ""), r += "_get";
-                const l = n.viewsTree.findInAllPaths((e => e.operationId === r && e));
-                if (!l) return void console.warn("Can't find redirect view for operationId: ".concat(r), i, e);
-                const u = e[i.name];
-                return null != u ? I(l.path, {
-                    ...n.router.currentRoute.params,
-                    [l.pkParamName]: u
-                }) : void 0
-            }
-
-            function B(e, t) {
-                for (const n of e)
-                    if (t(n)) return n
-            }
-
-            function N(e) {
-                const t = e.headers.get("Content-Disposition");
-                if (!t) return "";
-                const n = /filename="(.+)"/.exec(t);
-                return n ? n[1] : ""
-            }
-            let D = L;
-
-            function j(e) {
-                D = e
-            }
-            async function L(e) {
-                const t = await e.blob(),
-                    n = URL.createObjectURL(t),
-                    i = N(e),
-                    s = document.createElement("a");
-                s.href = n, i && (s.download = i), document.body.appendChild(s), s.click(), document.body.removeChild(s), setTimeout((() => URL.revokeObjectURL(n)), 100)
-            }
-
-            function q(e) {
-                return D(e)
-            }
         },
         8905: function(e, t, n) {
             n.d(t, {
                 B4: function() {
                     return v
                 },
                 Bv: function() {
@@ -16188,15 +16110,15 @@
                         },
                         params: {
                             ...e.params
                         }
                     }
                 }
                 toRoute() {
-                    if (!this.hidden) return {
+                    return {
                         name: this.routeName,
                         path: this.getRoutePath(),
                         component: this.getComponent(),
                         props: this._propsFunc.bind(this),
                         meta: {
                             view: this
                         }
@@ -16218,24 +16140,23 @@
                 getRoutePath() {
                     var e, t;
                     return this.deepNestedParentView ? "{0}(/\\w+/{1})*/:{2}/{1}/".format([this.deepNestedParentView.getRoutePath().replace(/\/$/, ""), this.deepNestedParentView.deepNestedViewFragment, null === (e = this.deepNestedParentView.pageView) || void 0 === e ? void 0 : e.pkParamName]) : this.isDeepNested ? (0, r.joinPaths)(null === (t = this.parent) || void 0 === t ? void 0 : t.getRoutePath(), (0, r.pathToArray)(this.path).last) : super.getRoutePath()
                 }
                 openPageView(e) {
                     var t;
                     if (null !== (t = this.pageView) && void 0 !== t && t.hidden) return;
-                    const n = (0, r.getApp)().router,
-                        i = n.currentRoute;
-                    if (this.isDeepNested) return n.push((0, r.joinPaths)(i.path, e.getPkValue()));
-                    const s = this.pageView;
-                    s && (0, r.openSublink)({
-                        name: "",
-                        title: "",
-                        isFileResponse: s.isFileResponse,
-                        href: s.path
-                    }, e)
+                    const n = (0, r.getApp)(),
+                        i = (0, r.getApp)().router,
+                        s = i.currentRoute;
+                    if (this.isDeepNested) return i.push((0, r.joinPaths)(s.path, e.getPkValue()));
+                    const a = this.pageView;
+                    if (a) {
+                        const t = (0, r.formatPath)(a.path, s.params, e);
+                        a.isFileResponse ? window.open("".concat(n.api.baseURL, "/").concat(n.api.defaultVersion).concat(t)) : i.push(t)
+                    }
                 }
             }(0, i.Z)(h, "viewType", "LIST");
             class m extends p {
                 constructor() {
                     super(...arguments), (0, i.Z)(this, "hideReadonlyFields", !1), (0, i.Z)(this, "wrapperClasses", "col-12"), (0, i.Z)(this, "beforeFieldsGroups", void 0), (0, i.Z)(this, "afterFieldsGroups", void 0)
                 }
                 getFieldsGroups(e) {
@@ -16252,17 +16173,14 @@
                 }
                 getRoutePath() {
                     var e;
                     const t = null === (e = this.listView) || void 0 === e ? void 0 : e.deepNestedParentView;
                     var n, i, s;
                     return t ? "{0}/(\\w+/{1})*/:{3}/{1}/:{2}/".format([t.getRoutePath().replace(/\/$/, ""), t.deepNestedViewFragment, this.pkParamName, (null === (n = this.parent) || void 0 === n ? void 0 : n.parent).pkParamName]) : this.isDeepNested ? (0, r.joinPaths)(null === (i = this.parent) || void 0 === i ? void 0 : i.getRoutePath(), ":".concat(null !== (s = this.pkParamName) && void 0 !== s ? s : "")) : super.getRoutePath()
                 }
-                toRoute() {
-                    if (!this.isFileResponse) return super.toRoute()
-                }
                 getModel() {
                     return this.objects.getResponseModelClass(r.RequestTypes.RETRIEVE)
                 }
                 async resolveState(e) {
                     const {
                         route: t,
                         store: n
@@ -16314,16 +16232,15 @@
                 }
                 getModel() {
                     return this.objects.getRequestModelClass(this.isPartial ? r.RequestTypes.PARTIAL_UPDATE : r.RequestTypes.UPDATE)
                 }
             }(0, i.Z)(_, "viewType", "PAGE_EDIT");
             class b extends m {
                 constructor(e, t) {
-                    var n;
-                    super(e, t, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [l.Z]), (0, i.Z)(this, "hideReadonlyFields", !0), (0, i.Z)(this, "method", void 0), (0, i.Z)(this, "action", void 0), (0, i.Z)(this, "isFileResponse", void 0), this.method = e.method, this.action = e.action, this.isFileResponse = null !== (n = e.isFileResponse) && void 0 !== n && n
+                    super(e, t, arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : [l.Z]), (0, i.Z)(this, "hideReadonlyFields", !0), (0, i.Z)(this, "method", void 0), (0, i.Z)(this, "action", void 0), this.method = e.method, this.action = e.action
                 }
                 _createStore() {
                     return this._createStoreWithHook((0, u.createActionViewStore)(this))
                 }
                 getRoutePath() {
                     var e;
                     return (0, r.joinPaths)(null === (e = this.parent) || void 0 === e ? void 0 : e.getRoutePath(), (0, r.pathToArray)(this.path).last)
```

### Comparing `vstutils-5.5.0/vstutils/static/img/anonymous.png` & `vstutils-5.5.0a1/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/static_files.py` & `vstutils-5.5.0a1/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/tasks.py` & `vstutils-5.5.0a1/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/auth/base.html` & `vstutils-5.5.0a1/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/auth/language_selector.html` & `vstutils-5.5.0a1/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/auth/tfa.html` & `vstutils-5.5.0a1/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/base.html` & `vstutils-5.5.0a1/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/gui/base.html` & `vstutils-5.5.0a1/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/gui/offline.html` & `vstutils-5.5.0a1/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/gui/service-worker.js` & `vstutils-5.5.0a1/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/package.json.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/setup.py.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/test.py.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.5.0a1/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/registration/confirm_email.html` & `vstutils-5.5.0a1/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.5.0a1/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.5.0a1/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/registration/user_registration.html` & `vstutils-5.5.0a1/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/rest_framework/admin.html` & `vstutils-5.5.0a1/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.5.0a1/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.5.0a1/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templatetags/request_static.py` & `vstutils-5.5.0a1/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templatetags/translation.py` & `vstutils-5.5.0a1/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.5.0a1/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.5.0a1/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/templatetags/vstconfigs.py` & `vstutils-5.5.0a1/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/tests.py` & `vstutils-5.5.0a1/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/tools.py` & `vstutils-5.5.0a1/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/translations/cn.py` & `vstutils-5.5.0a1/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/translations/ru.py` & `vstutils-5.5.0a1/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/translations/vi.py` & `vstutils-5.5.0a1/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/urls.py` & `vstutils-5.5.0a1/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/utils.py` & `vstutils-5.5.0a1/vstutils/utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/web.ini` & `vstutils-5.5.0a1/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils/wsgi.py` & `vstutils-5.5.0a1/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils.egg-info/PKG-INFO` & `vstutils-5.5.0a1/vstutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.5.0
+Version: 5.5.0a1
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.5.0/vstutils.egg-info/SOURCES.txt` & `vstutils-5.5.0a1/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.5.0/vstutils.egg-info/requires.txt` & `vstutils-5.5.0a1/vstutils.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 django~=4.2.2
 configparser~=5.3.0
-configparserc~=1.4.1
+configparserc~=1.4.0
 Markdown==3.4.1
 django-environ~=0.10.0
 djangorestframework~=3.14.0
 drf-yasg==1.21.6
 MarkupSafe==2.0.1
 django-filter==23.2
 django-crispy-forms~=1.14.0
 drf_orjson_renderer~=1.7.1
 ormsgpack==1.2.6
-pyyaml~=5.4.1
 uvicorn~=0.22.0
 pyuwsgi==2.0.21
 fastapi==0.97.0
 cent~=4.1.0
 PyJWT~=2.7.0
 jsmin~=3.0.1
 django-htmlmin~=0.11.0
@@ -80,17 +79,17 @@
 
 [stubs]
 django-stubs[compatible-mypy]~=4.2.1
 djangorestframework-stubs[compatible-mypy]~=3.14.1
 celery-stubs~=0.1.3
 drf-yasg-stubs~=0.1.3
 django-filter-stubs~=0.1.2
-types-PyMySQL==1.0.19.7
-types-Markdown==3.4.2.9
-types-docutils==0.20.0.1
+types-PyMySQL~=1.0.19.6
+types-Markdown~=3.4.2.6
+types-docutils~=0.19.1.7
 
 [test]
 coverage~=7.2.7
 fakeldap==0.6.1
 tblib~=1.7.0
 beautifulsoup4~=4.12.2
 httpx~=0.24.1
```

