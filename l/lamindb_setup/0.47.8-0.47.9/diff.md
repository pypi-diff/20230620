# Comparing `tmp/lamindb_setup-0.47.8.tar.gz` & `tmp/lamindb_setup-0.47.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.47.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.47.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.47.8.tar` & `lamindb_setup-0.47.9.tar`

### file list

```diff
@@ -1,86 +1,86 @@
--rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.8/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.8/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.8/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.8/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.8/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.8/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.8/README.md
--rw-r--r--   0        0        0    54842 2023-06-15 00:40:24.498451 lamindb_setup-0.47.8/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.8/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.8/docs/faq/index.md
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.8/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.8/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.8/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.8/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.8/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.47.8/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.8/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.8/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.8/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.8/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.8/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.8/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.8/lamin-project.yaml
--rw-r--r--   0        0        0     2715 2023-06-15 00:40:15.342730 lamindb_setup-0.47.8/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.8/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.8/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.47.8/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.8/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.8/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.8/lamindb_setup/_info.py
--rw-r--r--   0        0        0     6662 2023-06-14 07:51:53.730520 lamindb_setup-0.47.8/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     5670 2023-06-11 19:14:24.008895 lamindb_setup-0.47.8/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1118 2023-06-15 00:10:45.075143 lamindb_setup-0.47.8/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.8/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.8/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.8/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.8/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.8/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.8/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.8/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.8/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.8/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.8/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.47.8/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.8/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0     9986 2023-06-14 14:20:23.627443 lamindb_setup-0.47.8/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.8/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     9359 2023-06-14 07:52:21.048065 lamindb_setup-0.47.8/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.8/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.8/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.8/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.8/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2455 2023-06-15 00:10:45.075595 lamindb_setup-0.47.8/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.8/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     5057 2023-06-04 11:49:29.989719 lamindb_setup-0.47.8/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.47.8/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      815 2023-06-15 00:10:32.815663 lamindb_setup-0.47.8/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.8/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.47.8/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.8/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.8/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    27342 2023-06-12 19:29:46.148924 lamindb_setup-0.47.8/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.8/lnschema-core/LICENSE
--rw-r--r--   0        0        0      308 2023-06-12 10:24:01.839064 lamindb_setup-0.47.8/lnschema-core/README.md
--rw-r--r--   0        0        0      608 2023-06-12 19:29:46.149107 lamindb_setup-0.47.8/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.8/lnschema-core/lnschema_core/_lookup.py
--rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.47.8/lnschema-core/lnschema_core/_queryset.py
--rw-r--r--   0        0        0     1644 2023-06-12 19:29:46.149255 lamindb_setup-0.47.8/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    12754 2023-06-12 19:29:46.149559 lamindb_setup-0.47.8/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.8/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    20627 2023-06-12 19:29:46.149767 lamindb_setup-0.47.8/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      591 2023-06-12 10:24:01.840710 lamindb_setup-0.47.8/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.47.8/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      184 2023-06-15 00:10:32.816080 lamindb_setup-0.47.8/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.8/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.8/noxfile.py
--rw-r--r--   0        0        0     1337 2023-06-11 19:14:24.010612 lamindb_setup-0.47.8/pyproject.toml
--rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.8/tests/test_bionty.py
--rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.8/tests/test_init_instance.py
--rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.47.8/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.8/tests/test_login.py
--rw-r--r--   0        0        0      420 2023-06-15 00:10:45.075855 lamindb_setup-0.47.8/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.8/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.8/tests/test_signup.py
--rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.8/PKG-INFO
+-rw-r--r--   0        0        0     4010 2023-06-04 10:03:32.188588 lamindb_setup-0.47.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.47.9/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.47.9/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.47.9/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.47.9/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.47.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.47.9/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.47.9/README.md
+-rw-r--r--   0        0        0    55000 2023-06-16 00:45:51.189658 lamindb_setup-0.47.9/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.47.9/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0       96 2023-06-04 10:03:32.190096 lamindb_setup-0.47.9/docs/faq/index.md
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.47.9/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.47.9/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     8164 2023-06-08 11:34:59.766816 lamindb_setup-0.47.9/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4362 2023-06-08 11:34:59.766951 lamindb_setup-0.47.9/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5750 2023-06-08 11:34:59.767059 lamindb_setup-0.47.9/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     3293 2023-06-11 19:14:24.006633 lamindb_setup-0.47.9/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.47.9/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.47.9/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.47.9/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.47.9/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.47.9/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.47.9/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.47.9/lamin-project.yaml
+-rw-r--r--   0        0        0     2715 2023-06-16 00:45:42.214821 lamindb_setup-0.47.9/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.47.9/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     1410 2023-06-05 07:31:40.592921 lamindb_setup-0.47.9/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      661 2023-06-11 19:14:24.008057 lamindb_setup-0.47.9/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.47.9/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.47.9/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.47.9/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     6662 2023-06-14 07:51:53.730520 lamindb_setup-0.47.9/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     5670 2023-06-11 19:14:24.008895 lamindb_setup-0.47.9/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1118 2023-06-15 00:10:45.075143 lamindb_setup-0.47.9/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1692 2023-06-03 14:40:15.909532 lamindb_setup-0.47.9/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      825 2023-06-04 19:41:00.163739 lamindb_setup-0.47.9/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.47.9/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     1891 2023-06-08 07:33:18.805466 lamindb_setup-0.47.9/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.47.9/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.47.9/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.47.9/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3548 2023-06-04 19:41:00.164398 lamindb_setup-0.47.9/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-06-04 19:41:00.164608 lamindb_setup-0.47.9/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.47.9/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5987 2023-06-11 19:14:24.009146 lamindb_setup-0.47.9/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.47.9/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10751 2023-06-15 12:55:29.507946 lamindb_setup-0.47.9/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.47.9/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     9359 2023-06-14 07:52:21.048065 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.47.9/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.47.9/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2140 2023-06-05 07:31:40.593368 lamindb_setup-0.47.9/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4812 2023-06-15 12:55:29.508183 lamindb_setup-0.47.9/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.47.9/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      815 2023-06-15 00:10:32.815663 lamindb_setup-0.47.9/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.47.9/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.47.9/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.47.9/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1836 2023-05-30 14:21:30.384687 lamindb_setup-0.47.9/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    27342 2023-06-12 19:29:46.148924 lamindb_setup-0.47.9/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.47.9/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      308 2023-06-12 10:24:01.839064 lamindb_setup-0.47.9/lnschema-core/README.md
+-rw-r--r--   0        0        0      608 2023-06-12 19:29:46.149107 lamindb_setup-0.47.9/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1560 2023-06-07 12:14:30.488867 lamindb_setup-0.47.9/lnschema-core/lnschema_core/_lookup.py
+-rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.47.9/lnschema-core/lnschema_core/_queryset.py
+-rw-r--r--   0        0        0     1644 2023-06-12 19:29:46.149255 lamindb_setup-0.47.9/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    12754 2023-06-12 19:29:46.149559 lamindb_setup-0.47.9/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.47.9/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0    20627 2023-06-15 15:27:51.637812 lamindb_setup-0.47.9/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      591 2023-06-12 10:24:01.840710 lamindb_setup-0.47.9/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.47.9/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      184 2023-06-15 00:10:32.816080 lamindb_setup-0.47.9/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      850 2023-06-07 12:14:30.490216 lamindb_setup-0.47.9/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0     1911 2023-06-07 16:31:43.467939 lamindb_setup-0.47.9/noxfile.py
+-rw-r--r--   0        0        0     1337 2023-06-15 18:22:44.771393 lamindb_setup-0.47.9/pyproject.toml
+-rw-r--r--   0        0        0      672 2023-06-04 11:49:29.990032 lamindb_setup-0.47.9/tests/test_bionty.py
+-rw-r--r--   0        0        0     3041 2023-06-01 11:33:10.508406 lamindb_setup-0.47.9/tests/test_init_instance.py
+-rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.47.9/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.47.9/tests/test_login.py
+-rw-r--r--   0        0        0      420 2023-06-15 00:10:45.075855 lamindb_setup-0.47.9/tests/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.47.9/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.47.9/tests/test_signup.py
+-rw-r--r--   0        0        0     1366 1970-01-01 00:00:00.000000 lamindb_setup-0.47.9/PKG-INFO
```

### Comparing `lamindb_setup-0.47.8/.github/workflows/build.yml` & `lamindb_setup-0.47.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.9/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/.gitignore` & `lamindb_setup-0.47.9/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/.pre-commit-config.yaml` & `lamindb_setup-0.47.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/LICENSE` & `lamindb_setup-0.47.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/docs/changelog.md` & `lamindb_setup-0.47.9/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🍱 Fix legacy data migration | [420](https://github.com/laminlabs/lamindb-setup/pull/420) | [falexwolf](https://github.com/falexwolf) | 2023-06-15 | 0.47.9
 ✨ Add ability to check for migrations | [419](https://github.com/laminlabs/lamindb-setup/pull/419) | [falexwolf](https://github.com/falexwolf) | 2023-06-14 | 0.47.8
 🎨 Updated bionty function imports | [418](https://github.com/laminlabs/lamindb-setup/pull/418) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-14 |
 ♻️ Different migr strategy | [417](https://github.com/laminlabs/lamindb-setup/pull/417) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.7
 🍱 Added migration script from legacy instances | [416](https://github.com/laminlabs/lamindb-setup/pull/416) | [falexwolf](https://github.com/falexwolf) | 2023-06-12 | 0.47.5
 🔥 Adapt locker to lock entire lamindb session | [415](https://github.com/laminlabs/lamindb-setup/pull/415) | [Koncopd](https://github.com/Koncopd) | 2023-06-11 |
 🚑 Only delete bionty sources when bionty is installed | [414](https://github.com/laminlabs/lamindb-setup/pull/414) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.4
 🚚 Rename source_key to source | [413](https://github.com/laminlabs/lamindb-setup/pull/413) | [sunnyosun](https://github.com/sunnyosun) | 2023-06-10 | 0.47.3
```

### Comparing `lamindb_setup-0.47.8/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.47.9/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.47.9/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.47.9/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.47.9/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.47.9/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.47.9/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.47.9/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/docs/guide/setup-user.md` & `lamindb_setup-0.47.9/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/__init__.py` & `lamindb_setup-0.47.9/lamindb_setup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.47.8"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.47.9"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.47.8/lamindb_setup/__main__.py` & `lamindb_setup-0.47.9/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.47.9/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_close.py` & `lamindb_setup-0.47.9/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_delete.py` & `lamindb_setup-0.47.9/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_docstrings.py` & `lamindb_setup-0.47.9/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_init_instance.py` & `lamindb_setup-0.47.9/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_load_instance.py` & `lamindb_setup-0.47.9/lamindb_setup/_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_migrate.py` & `lamindb_setup-0.47.9/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_notebook.py` & `lamindb_setup-0.47.9/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_register_instance.py` & `lamindb_setup-0.47.9/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_schema.py` & `lamindb_setup-0.47.9/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_set.py` & `lamindb_setup-0.47.9/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_settings.py` & `lamindb_setup-0.47.9/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_setup_user.py` & `lamindb_setup-0.47.9/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.47.9/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_django.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_django.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# flake8: noqa
 import builtins
 import os
 
 from lamin_logger import logger
 
 from ._settings_instance import InstanceSettings
 
@@ -57,21 +58,23 @@
     if django_table_exists:
         return False
     # otherwise, it's a legacy instance: it has the user table but not the django table
 
     datetime_str = "datetime" if isettings.dialect == "sqlite" else "timestamp"
 
     # now let's proceed
+    # fmt: off
     stmts = [
         f"alter table lnschema_core_run add column run_at {datetime_str}",
         "drop index if exists ix_core_run_transform_v",
         "drop index if exists ix_lnschema_core_run_transform_version",
         "drop index if exists ix_lnschema_core_file_transform_version",
         "alter table lnschema_core_run drop column transform_version",
         "alter table lnschema_core_file drop column transform_version",
+        "update lnschema_core_file set created_by_id = 'DzTjkKse' where created_by_id is null",
         "alter table lnschema_core_project add column external_id varchar(40)",
         "alter table lnschema_core_transform rename column name to short_name",
         "alter table lnschema_core_transform rename column title to name",
         "alter table lnschema_core_runinput add column id bigint",
         "update lnschema_core_transform set name = short_name where name is null",
         "alter table lnschema_core_transform add column stem_id varchar(12)",
         "update lnschema_core_transform set stem_id = id",
@@ -79,74 +82,63 @@
         f"alter table lnschema_core_featureset add column updated_at {datetime_str}",
         # now rename
         "alter table lnschema_core_user rename to lnschema_core_legacy_user",
         "alter table lnschema_core_storage rename to lnschema_core_legacy_storage",
         "alter table lnschema_core_project rename to lnschema_core_legacy_project",
         "alter table lnschema_core_transform rename to lnschema_core_legacy_transform",
         "alter table lnschema_core_run rename to lnschema_core_legacy_run",
-        "alter table lnschema_core_featureset rename to"
-        " lnschema_core_legacy_featureset",
+        "alter table lnschema_core_featureset rename to lnschema_core_legacy_featureset",
         "alter table lnschema_core_folder rename to lnschema_core_legacy_folder",
         "alter table lnschema_core_file rename to lnschema_core_legacy_file",
         "alter table lnschema_core_runinput rename to lnschema_core_legacy_runinput",
     ]
     if "bionty" in isettings.schema:
-        # fmt: off
         stmts += [
             "alter table lnschema_bionty_species rename to lnschema_bionty_legacy_species",  # noqa
             "alter table lnschema_bionty_gene rename to lnschema_bionty_legacy_gene",  # noqa
             "alter table lnschema_bionty_protein rename to lnschema_bionty_legacy_protein",  # noqa
             "alter table lnschema_bionty_cellmarker rename to lnschema_bionty_legacy_cellmarker",  # noqa
             "alter table lnschema_bionty_tissue rename to lnschema_bionty_legacy_tissue",  # noqa
             "alter table lnschema_bionty_celltype rename to lnschema_bionty_legacy_celltype",  # noqa
             "alter table lnschema_bionty_disease rename to lnschema_bionty_legacy_disease",  # noqa
             "alter table lnschema_bionty_cellline rename to lnschema_bionty_legacy_cellline",  # noqa
             "alter table lnschema_bionty_phenotype rename to lnschema_bionty_legacy_phenotype",  # noqa
             "alter table lnschema_bionty_pathway rename to lnschema_bionty_legacy_pathway",  # noqa
             "alter table lnschema_bionty_readout rename to lnschema_bionty_legacy_readout",  # noqa
         ]
-        # fmt: on
+    # fmt: on
     with engine.connect() as conn:
         for stmt in stmts:
             try:
                 conn.execute(sa.text(stmt))
             except Exception as e:
                 logger.warning(f"Failed to execute: {stmt} because of {e}")
     logger.success("Created legacy migration preparations")
     return True
 
 
 def insert_legacy_data(isettings: InstanceSettings):
     import sqlalchemy as sa
 
-    stmts = []
-    if isettings.dialect != "sqlite":
-        # problem is this list is still incomplete, we'd need it for all columns
-        stmts = [
-            "alter table lnschema_core_user alter column created_at drop not null",  # noqa
-            "alter table lnschema_core_transform alter column created_at drop not null",  # noqa
-            "alter table lnschema_core_run alter column created_by_id drop not null",  # noqa
-            "alter table lnschema_core_file alter column updated_at drop not null",  # noqa
-        ]
-
     engine = sa.create_engine(isettings.db)
+    # fmt: off
     stmts = [
-        "insert into lnschema_core_user select * from lnschema_core_legacy_user",
-        "insert into lnschema_core_storage select * from lnschema_core_legacy_storage",
+        # we use the handle instead of the name below to deal with SQLite's inability of changing nullability
+        "insert into lnschema_core_user (id, handle, email, name, created_at, updated_at) select id, handle, email, handle, created_at, created_at from lnschema_core_legacy_user",
+        "insert into lnschema_core_storage (id, root, type, region, created_at, updated_at, created_by_id) select id, root, type, region, created_at, created_at, created_by_id from lnschema_core_legacy_storage",
+        "update lnschema_core_legacy_project set updated_at = created_at",
         "insert into lnschema_core_project select * from lnschema_core_legacy_project",
-        "insert into lnschema_core_transform select * from"
-        " lnschema_core_legacy_transform",
-        "insert into lnschema_core_run select * from lnschema_core_legacy_run",
-        "insert into lnschema_core_featureset select * from"
-        " lnschema_core_legacy_featureset",
-        "insert into lnschema_core_folder select * from lnschema_core_legacy_folder",
-        "insert into lnschema_core_file select * from lnschema_core_legacy_file",
-        "insert into lnschema_core_runinput select * from"
-        " lnschema_core_legacy_runinput",
+        "insert into lnschema_core_transform (id, name, short_name, stem_id, version, type, reference, created_at, updated_at, created_by_id) select id, name, short_name, stem_id, version, type, reference, created_at, created_at, created_by_id from lnschema_core_legacy_transform",
+        "insert into lnschema_core_run (id, name, external_id, transform_id, created_at, run_at, created_by_id) select id, name, external_id, transform_id, created_at, created_at, created_by_id from lnschema_core_legacy_run",
+        "insert into lnschema_core_featureset (id, type, created_at, updated_at, created_by_id) select id, type, created_at, created_at, created_by_id from lnschema_core_legacy_featureset",
+        "insert into lnschema_core_folder (id, name, key, storage_id, created_at, updated_at, created_by_id) select id, name, key, storage_id, created_at, created_at, created_by_id from lnschema_core_legacy_folder",
+        "insert into lnschema_core_file (id, name, suffix, size, hash, key, run_id, transform_id, storage_id, created_at, updated_at, created_by_id) select id, name, suffix, size, hash, key, run_id, transform_id, storage_id, created_at, created_at, created_by_id from lnschema_core_legacy_file",
+        "insert into lnschema_core_runinput (run_id, file_id) select run_id, file_id from lnschema_core_legacy_runinput",
     ]
+    # fmt: on
     with engine.connect() as conn:
         for stmt in stmts:
             try:
                 conn.execute(sa.text(stmt))
             except Exception as e:
                 logger.warning(f"Failed to execute: {stmt} because of {e}")
```

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from django.db import transaction
-from lamin_logger import logger
 
 from ._settings_instance import InstanceSettings
 
 
 def write_bionty_sources(isettings: InstanceSettings):
     """Write bionty sources to BiontySource table."""
     if "bionty" in isettings.schema:
@@ -58,15 +57,14 @@
 
         try:  # this is only to deal with legacy instances
             active_records = (
                 BiontySource.objects.filter(currently_used=True).all().values()
             )
 
             write_yaml(parse_currently_used_sources(active_records), LAMINDB_SOURCES)
-            logger.hint("Configured default bionty sources from BiontySource table")
         except Exception:
             pass
 
 
 def delete_bionty_sources_yaml():
     """Delete LAMINDB_SOURCES_PATH in bionty."""
     try:
```

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/_storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,21 +47,15 @@
 
     @property
     def id(self) -> str:
         """Storage id."""
         if self._id is None:
             from lnschema_core.models import Storage
 
-            storage = Storage.objects.get(root=self.root_as_str)
-            if storage is None:
-                raise RuntimeError(
-                    f"{self.root_as_str} wasn't registered in the db! "
-                    "Check `ln.select(ln.Storage).df()`"
-                )
-            self._id = storage.id
+            self._id = Storage.objects.get(root=self.root_as_str).id
         return self._id
 
     @property
     def root(self) -> Union[Path, UPath]:
         """Root storage location."""
         return self._root
```

### Comparing `lamindb_setup-0.47.8/lamindb_setup/dev/upath.py` & `lamindb_setup-0.47.9/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.47.9/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.47.9/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/.gitignore` & `lamindb_setup-0.47.9/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.47.9/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.47.9/lnschema-core/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/LICENSE` & `lamindb_setup-0.47.9/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/lnschema_core/__init__.py` & `lamindb_setup-0.47.9/lnschema-core/lnschema_core/__init__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/lnschema_core/_lookup.py` & `lamindb_setup-0.47.9/lnschema-core/lnschema_core/_lookup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/lnschema_core/_queryset.py` & `lamindb_setup-0.47.9/lnschema-core/lnschema_core/_queryset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.47.9/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.47.9/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.47.9/lnschema-core/lnschema_core/models.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.47.9/lnschema-core/lnschema_core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/lnschema-core/pyproject.toml` & `lamindb_setup-0.47.9/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/noxfile.py` & `lamindb_setup-0.47.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/pyproject.toml` & `lamindb_setup-0.47.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/tests/test_bionty.py` & `lamindb_setup-0.47.9/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/tests/test_init_instance.py` & `lamindb_setup-0.47.9/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/tests/test_load_instance.py` & `lamindb_setup-0.47.9/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.47.8/PKG-INFO` & `lamindb_setup-0.47.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.47.8
+Version: 0.47.9
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnhub_rest==0.9.10
 Requires-Dist: sqlmodel
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
```

