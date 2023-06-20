# Comparing `tmp/garpix_user-3.6.1.tar.gz` & `tmp/garpix_user-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garpix_user-3.6.1.tar", last modified: Fri Jun  9 06:24:49 2023, max compression
+gzip compressed data, was "garpix_user-3.7.0.tar", last modified: Tue Jun 20 12:40:58 2023, max compression
```

## Comparing `garpix_user-3.6.1.tar` & `garpix_user-3.7.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.477300 garpix_user-3.6.1/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-06-09 06:24:49.000000 garpix_user-3.6.1/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10220 2023-06-09 06:24:49.476890 garpix_user-3.6.1/PKG-INFO
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.448022 garpix_user-3.6.1/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5255 2023-06-09 06:24:25.000000 garpix_user-3.6.1/garpix_user/CHANGELOG.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/CONTRIBUTING.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.6.1/garpix_user/MANIFEST.in
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9556 2023-06-09 06:24:25.000000 garpix_user-3.6.1/garpix_user/README.md
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/README.rst
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.6.1/garpix_user/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.453750 garpix_user-3.6.1/garpix_user/admin/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/admin/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/admin/referral_type.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.6.1/garpix_user/admin/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/admin/user_session.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.6.1/garpix_user/apps.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.6.1/garpix_user/exceptions.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.455522 garpix_user-3.6.1/garpix_user/forms/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/forms/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1009 2023-05-31 03:44:48.000000 garpix_user-3.6.1/garpix_user/forms/login.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.443465 garpix_user-3.6.1/garpix_user/locale/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.443518 garpix_user-3.6.1/garpix_user/locale/ru/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.456273 garpix_user-3.6.1/garpix_user/locale/ru/LC_MESSAGES/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7138 2023-06-09 06:24:25.000000 garpix_user-3.6.1/garpix_user/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9523 2023-06-09 06:24:25.000000 garpix_user-3.6.1/garpix_user/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.456638 garpix_user-3.6.1/garpix_user/mixins/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/mixins/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.456990 garpix_user-3.6.1/garpix_user/mixins/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/mixins/models/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.458159 garpix_user-3.6.1/garpix_user/mixins/models/confirm/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/mixins/models/confirm/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.6.1/garpix_user/mixins/models/confirm/code_length_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5477 2023-05-10 13:07:30.000000 garpix_user-3.6.1/garpix_user/mixins/models/confirm/email_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3562 2023-05-10 13:07:30.000000 garpix_user-3.6.1/garpix_user/mixins/models/confirm/phone_confirm.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5511 2023-05-31 09:44:39.000000 garpix_user-3.6.1/garpix_user/mixins/models/restore_password.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.460921 garpix_user-3.6.1/garpix_user/mixins/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/mixins/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.6.1/garpix_user/mixins/serializers/password_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.6.1/garpix_user/mixins/serializers/to_lower.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.463212 garpix_user-3.6.1/garpix_user/models/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/models/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.6.1/garpix_user/models/access_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/models/refferal.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.6.1/garpix_user/models/refresh_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.6.1/garpix_user/models/user.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4986 2023-04-24 07:29:27.000000 garpix_user-3.6.1/garpix_user/models/user_session.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.463461 garpix_user-3.6.1/garpix_user/rest/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/rest/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-01 07:20:35.000000 garpix_user-3.6.1/garpix_user/rest/authentication.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.465978 garpix_user-3.6.1/garpix_user/serializers/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      769 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/serializers/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.6.1/garpix_user/serializers/auth_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/serializers/email_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1584 2023-05-31 09:44:39.000000 garpix_user-3.6.1/garpix_user/serializers/passwrod_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/serializers/phone_confirmation_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/serializers/refresh_token_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.6.1/garpix_user/serializers/registration_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.6.1/garpix_user/serializers/user_session_serializer.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-09 06:24:25.000000 garpix_user-3.6.1/garpix_user/setup.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.466741 garpix_user-3.6.1/garpix_user/tasks/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.6.1/garpix_user/tasks/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.6.1/garpix_user/tasks/delete_unconfirmed_users.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.444222 garpix_user-3.6.1/garpix_user/templates/
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.467060 garpix_user-3.6.1/garpix_user/templates/garpix_user/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/templates/garpix_user/send_confirm.html
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.467362 garpix_user-3.6.1/garpix_user/tests/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/tests/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.467847 garpix_user-3.6.1/garpix_user/tests/test_api/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/tests/test_api/__init__.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.468059 garpix_user-3.6.1/garpix_user/tests/test_api/_trial_temp/
--rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/tests/test_api/_trial_temp/_trial_marker
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.6.1/garpix_user/tests/test_api/_trial_temp/test.log
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/tests/test_api/api_login.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/tests/test_api/api_registration.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.6.1/garpix_user/tests/test_api/api_user_session_restore_password.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/tests/test_views.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.468393 garpix_user-3.6.1/garpix_user/tests/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/tests/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/tests/utils/settings.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/tests/utils/test_case_mixin.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2581 2023-03-07 13:05:56.000000 garpix_user-3.6.1/garpix_user/urls.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.469159 garpix_user-3.6.1/garpix_user/utils/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.6.1/garpix_user/utils/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-03-20 15:00:08.000000 garpix_user-3.6.1/garpix_user/utils/backends.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/utils/current_date.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.6.1/garpix_user/utils/drf_spectacular.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/utils/get_token_from_request.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.6.1/garpix_user/utils/repluralize.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.473005 garpix_user-3.6.1/garpix_user/views/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/views/__init__.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/views/change_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.6.1/garpix_user/views/email_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2376 2023-06-09 06:24:25.000000 garpix_user-3.6.1/garpix_user/views/login_views.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.6.1/garpix_user/views/logout_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1610 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/views/obtain_auth_token.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.6.1/garpix_user/views/phone_confirmation_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/views/referral_links_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.6.1/garpix_user/views/refresh_token_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/views/registration_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3452 2023-05-31 09:44:39.000000 garpix_user-3.6.1/garpix_user/views/restore_password_view.py
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.6.1/garpix_user/views/user_session_view.py
-drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-09 06:24:49.450054 garpix_user-3.6.1/garpix_user.egg-info/
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10220 2023-06-09 06:24:49.000000 garpix_user-3.6.1/garpix_user.egg-info/PKG-INFO
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3140 2023-06-09 06:24:49.000000 garpix_user-3.6.1/garpix_user.egg-info/SOURCES.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-09 06:24:49.000000 garpix_user-3.6.1/garpix_user.egg-info/dependency_links.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-09 06:24:49.000000 garpix_user-3.6.1/garpix_user.egg-info/not-zip-safe
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)      279 2023-06-09 06:24:49.000000 garpix_user-3.6.1/garpix_user.egg-info/requires.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-06-09 06:24:49.000000 garpix_user-3.6.1/garpix_user.egg-info/top_level.txt
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-09 06:24:49.477378 garpix_user-3.6.1/setup.cfg
--rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-09 06:24:49.000000 garpix_user-3.6.1/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.687886 garpix_user-3.7.0/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2023-06-20 12:40:58.000000 garpix_user-3.7.0/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10251 2023-06-20 12:40:58.687690 garpix_user-3.7.0/PKG-INFO
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.679576 garpix_user-3.7.0/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5315 2023-06-20 12:38:59.000000 garpix_user-3.7.0/garpix_user/CHANGELOG.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1020 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/CONTRIBUTING.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       31 2022-10-05 13:12:08.000000 garpix_user-3.7.0/garpix_user/MANIFEST.in
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9587 2023-06-20 12:33:35.000000 garpix_user-3.7.0/garpix_user/README.md
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3261 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/README.rst
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       57 2022-10-05 13:12:08.000000 garpix_user-3.7.0/garpix_user/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.680671 garpix_user-3.7.0/garpix_user/admin/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      238 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/admin/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      204 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/admin/referral_type.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1113 2023-03-06 08:48:05.000000 garpix_user-3.7.0/garpix_user/admin/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      260 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/admin/user_session.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      128 2022-10-05 13:12:08.000000 garpix_user-3.7.0/garpix_user/apps.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1782 2023-04-11 08:24:40.000000 garpix_user-3.7.0/garpix_user/exceptions.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.680878 garpix_user-3.7.0/garpix_user/forms/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       35 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/forms/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1009 2023-05-31 03:44:48.000000 garpix_user-3.7.0/garpix_user/forms/login.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.676608 garpix_user-3.7.0/garpix_user/locale/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.676656 garpix_user-3.7.0/garpix_user/locale/ru/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.681095 garpix_user-3.7.0/garpix_user/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     7138 2023-06-09 06:24:25.000000 garpix_user-3.7.0/garpix_user/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     9523 2023-06-09 06:24:25.000000 garpix_user-3.7.0/garpix_user/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.681198 garpix_user-3.7.0/garpix_user/mixins/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/mixins/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.681392 garpix_user-3.7.0/garpix_user/mixins/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       58 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/mixins/models/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.681810 garpix_user-3.7.0/garpix_user/mixins/models/confirm/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      114 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/mixins/models/confirm/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      637 2022-11-03 14:31:02.000000 garpix_user-3.7.0/garpix_user/mixins/models/confirm/code_length_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5477 2023-05-10 13:07:30.000000 garpix_user-3.7.0/garpix_user/mixins/models/confirm/email_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3562 2023-05-10 13:07:30.000000 garpix_user-3.7.0/garpix_user/mixins/models/confirm/phone_confirm.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5511 2023-05-31 09:44:39.000000 garpix_user-3.7.0/garpix_user/mixins/models/restore_password.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.682119 garpix_user-3.7.0/garpix_user/mixins/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      103 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/mixins/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2505 2023-02-24 11:10:07.000000 garpix_user-3.7.0/garpix_user/mixins/serializers/password_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      369 2022-10-24 09:55:11.000000 garpix_user-3.7.0/garpix_user/mixins/serializers/to_lower.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.682733 garpix_user-3.7.0/garpix_user/models/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      237 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/models/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      881 2022-11-07 08:16:45.000000 garpix_user-3.7.0/garpix_user/models/access_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      968 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/models/refferal.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      885 2022-11-07 08:16:45.000000 garpix_user-3.7.0/garpix_user/models/refresh_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3225 2023-03-01 08:01:40.000000 garpix_user-3.7.0/garpix_user/models/user.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4986 2023-04-24 07:29:27.000000 garpix_user-3.7.0/garpix_user/models/user_session.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.682921 garpix_user-3.7.0/garpix_user/rest/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/rest/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1709 2023-03-01 07:20:35.000000 garpix_user-3.7.0/garpix_user/rest/authentication.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.683788 garpix_user-3.7.0/garpix_user/serializers/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      769 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/serializers/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1393 2023-02-07 14:13:30.000000 garpix_user-3.7.0/garpix_user/serializers/auth_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      469 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/serializers/email_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1584 2023-05-31 09:44:39.000000 garpix_user-3.7.0/garpix_user/serializers/passwrod_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      434 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/serializers/phone_confirmation_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      219 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/serializers/refresh_token_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     4248 2023-03-07 08:55:10.000000 garpix_user-3.7.0/garpix_user/serializers/registration_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      387 2023-01-18 14:28:54.000000 garpix_user-3.7.0/garpix_user/serializers/user_session_serializer.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2090 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-20 12:38:59.000000 garpix_user-3.7.0/garpix_user/setup.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.684005 garpix_user-3.7.0/garpix_user/tasks/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       63 2023-03-06 10:42:24.000000 garpix_user-3.7.0/garpix_user/tasks/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1074 2023-03-15 14:13:43.000000 garpix_user-3.7.0/garpix_user/tasks/delete_unconfirmed_users.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.677295 garpix_user-3.7.0/garpix_user/templates/
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.684112 garpix_user-3.7.0/garpix_user/templates/garpix_user/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      269 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/templates/garpix_user/send_confirm.html
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.684320 garpix_user-3.7.0/garpix_user/tests/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       77 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/tests/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.684756 garpix_user-3.7.0/garpix_user/tests/test_api/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      176 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/tests/test_api/__init__.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.684963 garpix_user-3.7.0/garpix_user/tests/test_api/_trial_temp/
+-rwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/tests/test_api/_trial_temp/_trial_marker
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       41 2022-10-26 15:07:44.000000 garpix_user-3.7.0/garpix_user/tests/test_api/_trial_temp/test.log
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     8303 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/tests/test_api/api_login.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    14883 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/tests/test_api/api_registration.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     5000 2023-04-07 13:05:13.000000 garpix_user-3.7.0/garpix_user/tests/test_api/api_user_session_restore_password.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2122 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/tests/test_views.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.685364 garpix_user-3.7.0/garpix_user/tests/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        0 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/tests/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      681 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/tests/utils/settings.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1294 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/tests/utils/test_case_mixin.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2662 2023-06-20 12:32:44.000000 garpix_user-3.7.0/garpix_user/urls.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.686137 garpix_user-3.7.0/garpix_user/utils/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       67 2022-10-27 08:16:59.000000 garpix_user-3.7.0/garpix_user/utils/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      855 2023-03-20 15:00:08.000000 garpix_user-3.7.0/garpix_user/utils/backends.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      181 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/utils/current_date.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      406 2022-10-26 12:08:38.000000 garpix_user-3.7.0/garpix_user/utils/drf_spectacular.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      226 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/utils/get_token_from_request.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      542 2023-02-24 11:10:07.000000 garpix_user-3.7.0/garpix_user/utils/repluralize.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.687506 garpix_user-3.7.0/garpix_user/views/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      603 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/views/__init__.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1154 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/views/change_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3914 2023-04-19 13:51:11.000000 garpix_user-3.7.0/garpix_user/views/email_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     2376 2023-06-09 06:24:25.000000 garpix_user-3.7.0/garpix_user/views/login_views.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1211 2022-10-05 12:27:45.000000 garpix_user-3.7.0/garpix_user/views/logout_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1610 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/views/obtain_auth_token.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3292 2023-02-24 11:10:07.000000 garpix_user-3.7.0/garpix_user/views/phone_confirmation_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      710 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/views/referral_links_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1781 2023-03-17 09:50:52.000000 garpix_user-3.7.0/garpix_user/views/refresh_token_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      739 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/views/registration_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3452 2023-05-31 09:44:39.000000 garpix_user-3.7.0/garpix_user/views/restore_password_view.py
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1261 2023-01-19 12:18:01.000000 garpix_user-3.7.0/garpix_user/views/user_session_view.py
+drwxr-xr-x   0 viktoriaresetova   (501) staff       (20)        0 2023-06-20 12:40:58.680257 garpix_user-3.7.0/garpix_user.egg-info/
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)    10251 2023-06-20 12:40:58.000000 garpix_user-3.7.0/garpix_user.egg-info/PKG-INFO
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     3140 2023-06-20 12:40:58.000000 garpix_user-3.7.0/garpix_user.egg-info/SOURCES.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-20 12:40:58.000000 garpix_user-3.7.0/garpix_user.egg-info/dependency_links.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)        1 2023-06-20 12:40:58.000000 garpix_user-3.7.0/garpix_user.egg-info/not-zip-safe
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)      279 2023-06-20 12:40:58.000000 garpix_user-3.7.0/garpix_user.egg-info/requires.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       12 2023-06-20 12:40:58.000000 garpix_user-3.7.0/garpix_user.egg-info/top_level.txt
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)       38 2023-06-20 12:40:58.687930 garpix_user-3.7.0/setup.cfg
+-rw-r--r--   0 viktoriaresetova   (501) staff       (20)     1557 2023-06-20 12:40:58.000000 garpix_user-3.7.0/setup.py
```

### Comparing `garpix_user-3.6.1/PKG-INFO` & `garpix_user-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix_user
-Version: 3.6.1
+Version: 3.7.0
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -392,14 +392,15 @@
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
     'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
     'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
     'CONFIRMATION_DELAY': 10,  # in days
     # restore password
     'USE_RESTORE_PASSWORD': True,
     # registration
+    'USE_REGISTRATION': False,
     'REGISTRATION_SERIALIZER': 'app.serializers.RegistrationCustSerializer',
     'MIN_LENGTH_PASSWORD': 8,
     'MIN_DIGITS_PASSWORD': 2,
     'MIN_CHARS_PASSWORD': 2,
     'MIN_UPPERCASE_PASSWORD': 1,
     # response messages
     'WAIT_RESPONSE': 'Не прошло 1 мин с момента предыдущего запроса',
```

### Comparing `garpix_user-3.6.1/garpix_user/CHANGELOG.md` & `garpix_user-3.7.0/garpix_user/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+### 3.7.0 (20.06.2023)
+
+- `USE_REGISTRATION` setting added
+
 ### 3.6.1 (08.06.2023)
 
 - `LoginView` fixed
 
 ### 3.6.0 (31.05.2023)
 
 - `username` field added to `restore_password. step 2` endpoint
```

### Comparing `garpix_user-3.6.1/garpix_user/CONTRIBUTING.md` & `garpix_user-3.7.0/garpix_user/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/README.md` & `garpix_user-3.7.0/garpix_user/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -373,14 +373,15 @@
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
     'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
     'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
     'CONFIRMATION_DELAY': 10,  # in days
     # restore password
     'USE_RESTORE_PASSWORD': True,
     # registration
+    'USE_REGISTRATION': False,
     'REGISTRATION_SERIALIZER': 'app.serializers.RegistrationCustSerializer',
     'MIN_LENGTH_PASSWORD': 8,
     'MIN_DIGITS_PASSWORD': 2,
     'MIN_CHARS_PASSWORD': 2,
     'MIN_UPPERCASE_PASSWORD': 1,
     # response messages
     'WAIT_RESPONSE': 'Не прошло 1 мин с момента предыдущего запроса',
```

### Comparing `garpix_user-3.6.1/garpix_user/README.rst` & `garpix_user-3.7.0/garpix_user/README.rst`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/admin/user.py` & `garpix_user-3.7.0/garpix_user/admin/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/exceptions.py` & `garpix_user-3.7.0/garpix_user/exceptions.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/forms/login.py` & `garpix_user-3.7.0/garpix_user/forms/login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/locale/ru/LC_MESSAGES/django.mo` & `garpix_user-3.7.0/garpix_user/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/locale/ru/LC_MESSAGES/django.po` & `garpix_user-3.7.0/garpix_user/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/mixins/models/confirm/code_length_mixin.py` & `garpix_user-3.7.0/garpix_user/mixins/models/confirm/code_length_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/mixins/models/confirm/email_confirm.py` & `garpix_user-3.7.0/garpix_user/mixins/models/confirm/email_confirm.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/mixins/models/confirm/phone_confirm.py` & `garpix_user-3.7.0/garpix_user/mixins/models/confirm/phone_confirm.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/mixins/models/restore_password.py` & `garpix_user-3.7.0/garpix_user/mixins/models/restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/mixins/serializers/password_mixin.py` & `garpix_user-3.7.0/garpix_user/mixins/serializers/password_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/models/access_token.py` & `garpix_user-3.7.0/garpix_user/models/access_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/models/refferal.py` & `garpix_user-3.7.0/garpix_user/models/refferal.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/models/refresh_token.py` & `garpix_user-3.7.0/garpix_user/models/refresh_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/models/user.py` & `garpix_user-3.7.0/garpix_user/models/user.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/models/user_session.py` & `garpix_user-3.7.0/garpix_user/models/user_session.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/rest/authentication.py` & `garpix_user-3.7.0/garpix_user/rest/authentication.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/serializers/__init__.py` & `garpix_user-3.7.0/garpix_user/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/serializers/auth_token_serializer.py` & `garpix_user-3.7.0/garpix_user/serializers/auth_token_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/serializers/passwrod_serializer.py` & `garpix_user-3.7.0/garpix_user/serializers/passwrod_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/serializers/registration_serializer.py` & `garpix_user-3.7.0/garpix_user/serializers/registration_serializer.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/settings.py` & `garpix_user-3.7.0/garpix_user/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/setup.py` & `garpix_user-3.7.0/garpix_user/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.6.1',
+    version='3.7.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

### Comparing `garpix_user-3.6.1/garpix_user/tasks/delete_unconfirmed_users.py` & `garpix_user-3.7.0/garpix_user/tasks/delete_unconfirmed_users.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/tests/test_api/api_login.py` & `garpix_user-3.7.0/garpix_user/tests/test_api/api_login.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/tests/test_api/api_registration.py` & `garpix_user-3.7.0/garpix_user/tests/test_api/api_registration.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/tests/test_api/api_user_session_restore_password.py` & `garpix_user-3.7.0/garpix_user/tests/test_api/api_user_session_restore_password.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/tests/test_views.py` & `garpix_user-3.7.0/garpix_user/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/tests/utils/settings.py` & `garpix_user-3.7.0/garpix_user/tests/utils/settings.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/tests/utils/test_case_mixin.py` & `garpix_user-3.7.0/garpix_user/tests/utils/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/urls.py` & `garpix_user-3.7.0/garpix_user/urls.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,22 +30,24 @@
 if GARPIX_USER_SETTINGS.get('USE_RESTORE_PASSWORD', False):
     router.register(r'restore_password', RestorePasswordView, basename='api_restore_password')
 
 api_urlpatterns = [
     path('login/', obtain_auth_token, name='api_login'),
     path('refresh/', refresh_token_view, name='api_refresh'),
     path('logout/', logout_view, name='api_logout'),
-    path('register/', registration_view, name='api_registration'),
     path(r'', include(router.urls))
 ]
 
 urlpatterns = [
     path(f'{settings.API_URL}/garpix_user/', include((api_urlpatterns, 'garpix_user'), namespace='garpix_user_api')),
 ]
 
+if GARPIX_USER_SETTINGS.get('USE_REGISTRATIONS', False):
+    api_urlpatterns.append(path('register/', registration_view, name='api_registration'))
+
 if GARPIX_USER_SETTINGS.get('USE_REFERRAL_LINKS', False):
     urlpatterns += [
         re_path(r'invite_link/(?P<hash>.*?)/$', ReferralLinkView.as_view(), name='referral_link'),
         re_path(r'invite_link/(?P<hash>.*?)$', ReferralLinkView.as_view(), name='referral_link')
     ]
 
 if GARPIX_USER_SETTINGS.get('USE_EMAIL_CONFIRMATION', False) and GARPIX_USER_SETTINGS.get('USE_EMAIL_LINK_CONFIRMATION',
```

### Comparing `garpix_user-3.6.1/garpix_user/utils/backends.py` & `garpix_user-3.7.0/garpix_user/utils/backends.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/utils/repluralize.py` & `garpix_user-3.7.0/garpix_user/utils/repluralize.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/__init__.py` & `garpix_user-3.7.0/garpix_user/views/__init__.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/change_password_view.py` & `garpix_user-3.7.0/garpix_user/views/change_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/email_confirmation_view.py` & `garpix_user-3.7.0/garpix_user/views/email_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/login_views.py` & `garpix_user-3.7.0/garpix_user/views/login_views.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/logout_view.py` & `garpix_user-3.7.0/garpix_user/views/logout_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/obtain_auth_token.py` & `garpix_user-3.7.0/garpix_user/views/obtain_auth_token.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/phone_confirmation_view.py` & `garpix_user-3.7.0/garpix_user/views/phone_confirmation_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/referral_links_view.py` & `garpix_user-3.7.0/garpix_user/views/referral_links_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/refresh_token_view.py` & `garpix_user-3.7.0/garpix_user/views/refresh_token_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/registration_view.py` & `garpix_user-3.7.0/garpix_user/views/registration_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/restore_password_view.py` & `garpix_user-3.7.0/garpix_user/views/restore_password_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user/views/user_session_view.py` & `garpix_user-3.7.0/garpix_user/views/user_session_view.py`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/garpix_user.egg-info/PKG-INFO` & `garpix_user-3.7.0/garpix_user.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garpix-user
-Version: 3.6.1
+Version: 3.7.0
 Home-page: https://github.com/garpixcms/garpix_user
 Author: Garpix LTD
 Author-email: info@garpix.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
@@ -392,14 +392,15 @@
     'CONFIRM_EMAIL_CODE_LIFE_TIME': 2,  # in days
     'PHONE_CONFIRMATION_LIFE_TIME': 2, # in days
     'EMAIL_CONFIRMATION_LIFE_TIME': 2, # in days
     'CONFIRMATION_DELAY': 10,  # in days
     # restore password
     'USE_RESTORE_PASSWORD': True,
     # registration
+    'USE_REGISTRATION': False,
     'REGISTRATION_SERIALIZER': 'app.serializers.RegistrationCustSerializer',
     'MIN_LENGTH_PASSWORD': 8,
     'MIN_DIGITS_PASSWORD': 2,
     'MIN_CHARS_PASSWORD': 2,
     'MIN_UPPERCASE_PASSWORD': 1,
     # response messages
     'WAIT_RESPONSE': 'Не прошло 1 мин с момента предыдущего запроса',
```

### Comparing `garpix_user-3.6.1/garpix_user.egg-info/SOURCES.txt` & `garpix_user-3.7.0/garpix_user.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garpix_user-3.6.1/setup.py` & `garpix_user-3.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.join(path.abspath(path.dirname(__file__)), 'garpix_user')
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='garpix_user',
-    version='3.6.1',
+    version='3.7.0',
     description='',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/garpixcms/garpix_user',
     author='Garpix LTD',
     author_email='info@garpix.com',
     license='MIT',
```

