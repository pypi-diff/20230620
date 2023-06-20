# Comparing `tmp/ical-4.5.2.tar.gz` & `tmp/ical-4.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ical-4.5.2.tar", last modified: Sat Apr  1 16:47:27 2023, max compression
+gzip compressed data, was "ical-4.5.4.tar", last modified: Tue Jun 20 05:27:04 2023, max compression
```

## Comparing `ical-4.5.2.tar` & `ical-4.5.4.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 16:47:27.440767 ical-4.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-01 16:47:15.000000 ical-4.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-01 16:47:27.440767 ical-4.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-04-01 16:47:15.000000 ical-4.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 16:47:27.432767 ical-4.5.2/ical/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-01 16:47:15.000000 ical-4.5.2/ical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-04-01 16:47:15.000000 ical-4.5.2/ical/alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-04-01 16:47:15.000000 ical-4.5.2/ical/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-01 16:47:15.000000 ical-4.5.2/ical/calendar_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    11712 2023-04-01 16:47:15.000000 ical-4.5.2/ical/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-01 16:47:15.000000 ical-4.5.2/ical/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-04-01 16:47:15.000000 ical-4.5.2/ical/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-04-01 16:47:15.000000 ical-4.5.2/ical/freebusy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-04-01 16:47:15.000000 ical-4.5.2/ical/iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-01 16:47:15.000000 ical-4.5.2/ical/journal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 16:47:27.436767 ical-4.5.2/ical/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-01 16:47:15.000000 ical-4.5.2/ical/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-01 16:47:15.000000 ical-4.5.2/ical/parsing/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-01 16:47:15.000000 ical-4.5.2/ical/parsing/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-04-01 16:47:15.000000 ical-4.5.2/ical/parsing/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-04-01 16:47:15.000000 ical-4.5.2/ical/parsing/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-04-01 16:47:15.000000 ical-4.5.2/ical/parsing/unicode.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-01 16:47:15.000000 ical-4.5.2/ical/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-04-01 16:47:15.000000 ical-4.5.2/ical/store.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-01 16:47:15.000000 ical-4.5.2/ical/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-04-01 16:47:15.000000 ical-4.5.2/ical/timespan.py
--rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-04-01 16:47:15.000000 ical-4.5.2/ical/timezone.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-04-01 16:47:15.000000 ical-4.5.2/ical/todo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 16:47:27.436767 ical-4.5.2/ical/types/
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/cal_address.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/date_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/duration.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/float.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/period.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/priority.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/recur.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/request_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-01 16:47:15.000000 ical-4.5.2/ical/types/utc_offset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 16:47:27.436767 ical-4.5.2/ical/tzif/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-01 16:47:15.000000 ical-4.5.2/ical/tzif/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-01 16:47:15.000000 ical-4.5.2/ical/tzif/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-01 16:47:15.000000 ical-4.5.2/ical/tzif/timezoneinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-04-01 16:47:15.000000 ical-4.5.2/ical/tzif/tz_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-04-01 16:47:15.000000 ical-4.5.2/ical/tzif/tzif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-01 16:47:15.000000 ical-4.5.2/ical/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 16:47:27.436767 ical-4.5.2/ical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-04-01 16:47:27.000000 ical-4.5.2/ical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-01 16:47:27.000000 ical-4.5.2/ical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 16:47:27.000000 ical-4.5.2/ical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-01 16:47:27.000000 ical-4.5.2/ical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-01 16:47:27.000000 ical-4.5.2/ical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-01 16:47:27.440767 ical-4.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-01 16:47:15.000000 ical-4.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 16:47:27.440767 ical-4.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_alarm.py
--rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_calendar_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_freebusy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_journal.py
--rw-r--r--   0 runner    (1001) docker     (123)    32299 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_timezone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-01 16:47:15.000000 ical-4.5.2/tests/test_todo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:27:04.480605 ical-4.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 05:26:54.000000 ical-4.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-20 05:27:04.480605 ical-4.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-20 05:26:54.000000 ical-4.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:27:04.476605 ical-4.5.4/ical/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-20 05:26:54.000000 ical-4.5.4/ical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-20 05:26:54.000000 ical-4.5.4/ical/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4958 2023-06-20 05:26:54.000000 ical-4.5.4/ical/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-20 05:26:54.000000 ical-4.5.4/ical/calendar_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12558 2023-06-20 05:26:54.000000 ical-4.5.4/ical/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-20 05:26:54.000000 ical-4.5.4/ical/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16831 2023-06-20 05:26:54.000000 ical-4.5.4/ical/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-20 05:26:54.000000 ical-4.5.4/ical/freebusy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-06-20 05:26:54.000000 ical-4.5.4/ical/iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-06-20 05:26:54.000000 ical-4.5.4/ical/journal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:27:04.476605 ical-4.5.4/ical/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 05:26:54.000000 ical-4.5.4/ical/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-06-20 05:26:54.000000 ical-4.5.4/ical/parsing/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-20 05:26:54.000000 ical-4.5.4/ical/parsing/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-20 05:26:54.000000 ical-4.5.4/ical/parsing/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-20 05:26:54.000000 ical-4.5.4/ical/parsing/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-20 05:26:54.000000 ical-4.5.4/ical/parsing/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 05:26:54.000000 ical-4.5.4/ical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13344 2023-06-20 05:26:54.000000 ical-4.5.4/ical/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-20 05:26:54.000000 ical-4.5.4/ical/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-06-20 05:26:54.000000 ical-4.5.4/ical/timespan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-06-20 05:26:54.000000 ical-4.5.4/ical/timezone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-20 05:26:54.000000 ical-4.5.4/ical/todo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:27:04.476605 ical-4.5.4/ical/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/cal_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6003 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/date_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/duration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/recur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/request_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-20 05:26:54.000000 ical-4.5.4/ical/types/utc_offset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:27:04.480605 ical-4.5.4/ical/tzif/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 05:26:54.000000 ical-4.5.4/ical/tzif/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-20 05:26:54.000000 ical-4.5.4/ical/tzif/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-20 05:26:54.000000 ical-4.5.4/ical/tzif/timezoneinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-06-20 05:26:54.000000 ical-4.5.4/ical/tzif/tz_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-06-20 05:26:54.000000 ical-4.5.4/ical/tzif/tzif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-20 05:26:54.000000 ical-4.5.4/ical/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:27:04.480605 ical-4.5.4/ical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-20 05:27:04.000000 ical-4.5.4/ical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-20 05:27:04.000000 ical-4.5.4/ical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 05:27:04.000000 ical-4.5.4/ical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-20 05:27:04.000000 ical-4.5.4/ical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 05:27:04.000000 ical-4.5.4/ical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-20 05:27:04.480605 ical-4.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-20 05:26:54.000000 ical-4.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 05:27:04.480605 ical-4.5.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12945 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_calendar_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_freebusy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_journal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33623 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_timezone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-20 05:26:54.000000 ical-4.5.4/tests/test_todo.py
```

### Comparing `ical-4.5.2/LICENSE` & `ical-4.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/PKG-INFO` & `ical-4.5.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ical
-Version: 4.5.2
+Version: 4.5.4
 Summary: Python iCalendar implementation (rfc 2445)
 Home-page: https://github.com/allenporter/ical
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `ical-4.5.2/README.md` & `ical-4.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/alarm.py` & `ical-4.5.4/ical/alarm.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/calendar.py` & `ical-4.5.4/ical/calendar.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/calendar_stream.py` & `ical-4.5.4/ical/calendar_stream.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/component.py` & `ical-4.5.4/ical/component.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,42 @@
         or not (dtstart := values.get("dtstart"))
     ):
         return values
     rule.until = _adjust_recurrence_date(rule.until, dtstart)
     return values
 
 
+def _as_datetime(
+    date_value: datetime.datetime | datetime.date,
+    dtstart: datetime.datetime,
+) -> datetime.datetime:
+    if not isinstance(date_value, datetime.datetime):
+        return datetime.datetime.combine(date_value, dtstart.time())
+    return date_value
+
+
+def validate_recurrence_dates(
+    _cls: BaseModel, values: dict[str, Any]
+) -> dict[str, Any]:
+    """Verify the recurrence dates have the correct types."""
+    if (
+        not values.get("rrule")
+        or not (dtstart := values.get("dtstart"))
+        or not isinstance(dtstart, datetime.datetime)
+    ):
+        return values
+    for field in ("exdate", "rdate"):
+        if not (date_values := values.get(field)):
+            continue
+        values[field] = [
+            _as_datetime(date_value, dtstart) for date_value in date_values
+        ]
+    return values
+
+
 class ComponentModel(BaseModel):
     """Abstract class for rfc5545 component model."""
 
     @root_validator(pre=True, allow_reuse=True)
     def parse_extra_fields(
         cls, values: dict[str, list[ParsedProperty | ParsedComponent]]
     ) -> dict[str, Any]:
```

### Comparing `ical-4.5.2/ical/diagnostics.py` & `ical-4.5.4/ical/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/event.py` & `ical-4.5.4/ical/event.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import logging
 from collections.abc import Iterable
 from typing import Any, Optional, Union
 
 from pydantic import Field, root_validator
 
 from .alarm import Alarm
-from .component import ComponentModel, validate_until_dtstart
+from .component import ComponentModel, validate_until_dtstart, validate_recurrence_dates
 from .iter import RulesetIterable
 from .parsing.property import ParsedProperty
 from .timespan import Timespan
 from .types import (
     CalAddress,
     Classification,
     Geo,
@@ -359,25 +359,25 @@
         return RulesetIterable(
             self.start,
             [self.rrule.as_rrule(self.start)] if self.rrule else [],
             self.rdate,
             self.exdate,
         )
 
-    @root_validator(pre=True)
+    @root_validator(pre=True, allow_reuse=True)
     def _inspect_date_types(cls, values: dict[str, Any]) -> dict[str, Any]:
         """Debug the date and date/time values of the event."""
         dtstart = values.get("dtstart")
         dtend = values.get("dtend")
         if not dtstart or not dtend:
             return values
         _LOGGER.debug("Found initial values dtstart=%s, dtend=%s", dtstart, dtend)
         return values
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def _validate_date_types(cls, values: dict[str, Any]) -> dict[str, Any]:
         """Validate that start and end values are the same date or datetime type."""
         dtstart = values.get("dtstart")
         dtend = values.get("dtend")
 
         if not dtstart or not dtend:
             return values
@@ -392,15 +392,15 @@
             if isinstance(dtend, datetime.datetime):
                 raise ValueError(
                     f"Unexpected dtstart value '{dtstart}' was date but "
                     f"dtend value '{dtend}' was datetime"
                 )
         return values
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def _validate_datetime_timezone(cls, values: dict[str, Any]) -> dict[str, Any]:
         """Validate that start and end values have the same timezone information."""
         if (
             not (dtstart := values.get("dtstart"))
             or not (dtend := values.get("dtend"))
             or not isinstance(dtstart, datetime.datetime)
             or not isinstance(dtend, datetime.datetime)
@@ -410,28 +410,29 @@
             raise ValueError(
                 f"Expected end datetime value in localtime but was {dtend}"
             )
         if dtstart.tzinfo is not None and dtend.tzinfo is None:
             raise ValueError(f"Expected end datetime with timezone but was {dtend}")
         return values
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def _validate_one_end_or_duration(cls, values: dict[str, Any]) -> dict[str, Any]:
         """Validate that only one of duration or end date may be set."""
         if values.get("dtend") and values.get("duration"):
             raise ValueError("Only one of dtend or duration may be set." "")
         return values
 
-    @root_validator
+    @root_validator(allow_reuse=True)
     def _validate_duration_unit(cls, values: dict[str, Any]) -> dict[str, Any]:
         """Validate the duration is the appropriate units."""
         if not (duration := values.get("duration")):
             return values
         dtstart = values["dtstart"]
         if type(dtstart) == datetime.date:  # pylint: disable=unidiomatic-typecheck
             if duration.seconds != 0:
                 raise ValueError("Event with start date expects duration in days only")
         if duration < datetime.timedelta(seconds=0):
             raise ValueError(f"Expected duration to be positive but was {duration}")
         return values
 
     _validate_until_dtstart = root_validator(allow_reuse=True)(validate_until_dtstart)
+    _validate_recurrence_dates = root_validator(allow_reuse=True)(validate_recurrence_dates)
```

### Comparing `ical-4.5.2/ical/freebusy.py` & `ical-4.5.4/ical/freebusy.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/iter.py` & `ical-4.5.4/ical/iter.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/journal.py` & `ical-4.5.4/ical/journal.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import datetime
 import enum
 import logging
 from typing import Any, Optional, Union
 
 from pydantic import Field, root_validator
 
-from .component import ComponentModel, validate_until_dtstart
+from .component import ComponentModel, validate_until_dtstart, validate_recurrence_dates
 from .parsing.property import ParsedProperty
 from .types import CalAddress, Classification, Recur, RecurrenceId, RequestStatus, Uri
 from .util import dtstamp_factory, normalize_datetime, uid_factory
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -87,7 +87,8 @@
 
     @property
     def start_datetime(self) -> datetime.datetime:
         """Return the events start as a datetime."""
         return normalize_datetime(self.start).astimezone(tz=datetime.timezone.utc)
 
     _validate_until_dtstart = root_validator(allow_reuse=True)(validate_until_dtstart)
+    _validate_recurrence_dates = root_validator(allow_reuse=True)(validate_recurrence_dates)
```

### Comparing `ical-4.5.2/ical/parsing/component.py` & `ical-4.5.4/ical/parsing/component.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/parsing/parser.py` & `ical-4.5.4/ical/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/parsing/property.py` & `ical-4.5.4/ical/parsing/property.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/parsing/unicode.py` & `ical-4.5.4/ical/parsing/unicode.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/store.py` & `ical-4.5.4/ical/store.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/timeline.py` & `ical-4.5.4/ical/timeline.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/timespan.py` & `ical-4.5.4/ical/timespan.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/timezone.py` & `ical-4.5.4/ical/timezone.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/todo.py` & `ical-4.5.4/ical/todo.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import datetime
 import enum
 from typing import Any, Optional, Union
 
 from pydantic import Field, root_validator
 
 from .alarm import Alarm
-from .component import ComponentModel, validate_until_dtstart
+from .component import ComponentModel, validate_until_dtstart, validate_recurrence_dates
 from .parsing.property import ParsedProperty
 from .types import (
     CalAddress,
     Classification,
     Geo,
     Priority,
     Recur,
@@ -108,7 +108,8 @@
     def validate_duration_requires_start(cls, values: dict[str, Any]) -> dict[str, Any]:
         """Validate that only one of duration or end date may be set."""
         if values.get("duration") and not values.get("dtstart"):
             raise ValueError("Duration requires that dtstart is specified")
         return values
 
     _validate_until_dtstart = root_validator(allow_reuse=True)(validate_until_dtstart)
+    _validate_recurrence_dates = root_validator(allow_reuse=True)(validate_recurrence_dates)
```

### Comparing `ical-4.5.2/ical/types/__init__.py` & `ical-4.5.4/ical/types/__init__.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/boolean.py` & `ical-4.5.4/ical/types/boolean.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/cal_address.py` & `ical-4.5.4/ical/types/cal_address.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/data_types.py` & `ical-4.5.4/ical/types/data_types.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/date.py` & `ical-4.5.4/ical/types/date.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/date_time.py` & `ical-4.5.4/ical/types/date_time.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/duration.py` & `ical-4.5.4/ical/types/duration.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/geo.py` & `ical-4.5.4/ical/types/geo.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/integer.py` & `ical-4.5.4/ical/types/integer.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/parsing.py` & `ical-4.5.4/ical/types/parsing.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/period.py` & `ical-4.5.4/ical/types/period.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/priority.py` & `ical-4.5.4/ical/types/priority.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/recur.py` & `ical-4.5.4/ical/types/recur.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/request_status.py` & `ical-4.5.4/ical/types/request_status.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/text.py` & `ical-4.5.4/ical/types/text.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/uri.py` & `ical-4.5.4/ical/types/uri.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/types/utc_offset.py` & `ical-4.5.4/ical/types/utc_offset.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/tzif/model.py` & `ical-4.5.4/ical/tzif/model.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/tzif/timezoneinfo.py` & `ical-4.5.4/ical/tzif/timezoneinfo.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/tzif/tz_rule.py` & `ical-4.5.4/ical/tzif/tz_rule.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/tzif/tzif.py` & `ical-4.5.4/ical/tzif/tzif.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical/util.py` & `ical-4.5.4/ical/util.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/ical.egg-info/PKG-INFO` & `ical-4.5.4/ical.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ical
-Version: 4.5.2
+Version: 4.5.4
 Summary: Python iCalendar implementation (rfc 2445)
 Home-page: https://github.com/allenporter/ical
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.9
```

### Comparing `ical-4.5.2/ical.egg-info/SOURCES.txt` & `ical-4.5.4/ical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/setup.cfg` & `ical-4.5.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ical
-version = 4.5.2
+version = 4.5.4
 description = Python iCalendar implementation (rfc 2445)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/allenporter/ical
 author = Allen Porter
 author_email = allen.porter@gmail.com
 license = Apache-2.0
@@ -13,16 +13,16 @@
 	License :: OSI Approved :: Apache Software License
 
 [options]
 packages = find:
 python_requires = >= 3.9
 install_requires = 
 	python-dateutil>=2.8.2
-	tzdata>=2022.1
-	pydantic>=1.9.1
+	tzdata>=2023.3
+	pydantic>=1.9.1,<2.0a1
 	pyparsing>=3.0.9
 	emoji>=2.2.0
 include_package_data = True
 package_dir = 
 	= .
 
 [options.packages.find]
```

### Comparing `ical-4.5.2/tests/test_alarm.py` & `ical-4.5.4/tests/test_alarm.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_calendar.py` & `ical-4.5.4/tests/test_calendar.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_calendar_stream.py` & `ical-4.5.4/tests/test_calendar_stream.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_component.py` & `ical-4.5.4/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_diagnostics.py` & `ical-4.5.4/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_event.py` & `ical-4.5.4/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_freebusy.py` & `ical-4.5.4/tests/test_freebusy.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_iter.py` & `ical-4.5.4/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_journal.py` & `ical-4.5.4/tests/test_journal.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_store.py` & `ical-4.5.4/tests/test_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 
 
 def test_edit_event(
     store: EventStore,
     fetch_events: Callable[..., list[dict[str, Any]]],
     frozen_time: FrozenDateTimeFactory,
 ) -> None:
-    """Test adding an event to the store and retrieval."""
+    """Test editing an event."""
     store.add(
         Event(
             summary="Monday meeting",
             start="2022-08-29T09:00:00",
             end="2022-08-29T09:30:00",
         )
     )
@@ -517,21 +517,70 @@
 @pytest.mark.parametrize(
     "recur",
     [
         Recur.from_rrule("FREQ=WEEKLY;UNTIL=20220912T090000"),
         Recur.from_rrule("FREQ=WEEKLY;COUNT=3"),
     ],
 )
+def test_edit_recurring_all_day_event_instance(
+    store: EventStore,
+    fetch_events: Callable[..., list[dict[str, Any]]],
+    frozen_time: FrozenDateTimeFactory,
+    recur: Recur,
+) -> None:
+    """Test editing a single instance of a recurring all day event."""
+    store.add(
+        Event(
+            summary="Monday event",
+            start="2022-08-29",
+            end="2022-08-30",
+            rrule=recur,
+        )
+    )
+    frozen_time.tick(delta=datetime.timedelta(seconds=10))
+    store.edit(
+        "mock-uid-1",
+        Event(start="2022-09-06", summary="Tuesday event"),
+        recurrence_id="20220905",
+    )
+    assert fetch_events({"uid", "recurrence_id", "dtstart", "summary"}) == [
+        {
+            "uid": "mock-uid-1",
+            "recurrence_id": "20220829",
+            "dtstart": "2022-08-29",
+            "summary": "Monday event",
+        },
+        {
+            "uid": "mock-uid-2",
+            "dtstart": "2022-09-06",
+            "summary": "Tuesday event",
+        },
+        {
+            "uid": "mock-uid-1",
+            "recurrence_id": "20220912",
+            "dtstart": "2022-09-12",
+            "summary": "Monday event",
+        },
+    ]
+
+
+@pytest.mark.parametrize(
+    "recur",
+    [
+        Recur.from_rrule("FREQ=WEEKLY;UNTIL=20220912T090000"),
+        Recur.from_rrule("FREQ=WEEKLY;COUNT=3"),
+    ],
+)
 def test_edit_recurring_event_instance(
     store: EventStore,
     fetch_events: Callable[..., list[dict[str, Any]]],
     frozen_time: FrozenDateTimeFactory,
     recur: Recur,
 ) -> None:
-    """Test editing all instances of a recurring event."""
+    """Test editing a single instance of a recurring event."""
     store.add(
         Event(
             summary="Monday meeting",
             start="2022-08-29T09:00:00",
             end="2022-08-29T09:30:00",
             rrule=recur,
         )
@@ -742,18 +791,18 @@
             "recurrence_id": "20220912",
             "dtstart": "2022-09-12",
             "summary": "Mondays [edit]",
         },
     ]
 
 
-def test_add_and_delete_event_date(
+def test_delete_all_day_event(
     store: EventStore, fetch_events: Callable[..., list[dict[str, Any]]]
 ) -> None:
-    """Test adding an event to the store and retrieval."""
+    """Test deleting a single all day event."""
     store.add(
         Event(
             summary="Monday meeting",
             start="2022-08-29",
             end="2022-08-29",
         )
     )
@@ -768,18 +817,18 @@
             "sequence": 0,
         },
     ]
     store.delete("mock-uid-1")
     assert fetch_events() == []
 
 
-def test_delete_event_date_recurring(
+def test_delete_all_day_recurring(
     store: EventStore, fetch_events: Callable[..., list[dict[str, Any]]]
 ) -> None:
-    """Test adding an event to the store and retrieval."""
+    """Test deleting all instances of a recurring all day event."""
     store.add(
         Event(
             summary="Monday meeting",
             start="2022-08-29",
             end="2022-08-29",
             rrule=Recur.from_rrule("FREQ=WEEKLY;COUNT=3"),
         )
```

### Comparing `ical-4.5.2/tests/test_timeline.py` & `ical-4.5.4/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_timezone.py` & `ical-4.5.4/tests/test_timezone.py`

 * *Files identical despite different names*

### Comparing `ical-4.5.2/tests/test_todo.py` & `ical-4.5.4/tests/test_todo.py`

 * *Files identical despite different names*

