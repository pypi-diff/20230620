# Comparing `tmp/vspreview-0.6.0.tar.gz` & `tmp/vspreview-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vspreview-0.6.0.tar", last modified: Sun Jun 11 01:40:35 2023, max compression
+gzip compressed data, was "vspreview-0.7.0.tar", last modified: Tue Jun 20 14:27:17 2023, max compression
```

## Comparing `vspreview-0.6.0.tar` & `vspreview-0.7.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.312761 vspreview-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-11 01:40:07.000000 vspreview-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-11 01:40:35.312761 vspreview-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-11 01:40:07.000000 vspreview-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-11 01:40:35.312761 vspreview-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-11 01:40:07.000000 vspreview-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.296761 vspreview-0.6.0/vspreview/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.300761 vspreview-0.6.0/vspreview/api/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/app.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/other.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/api/timecodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.300761 vspreview-0.6.0/vspreview/core/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.304761 vspreview-0.6.0/vspreview/core/custom/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/combobox.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/dragnavigator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/edits.py
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/graphicsview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/notch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/custom/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.304761 vspreview-0.6.0/vspreview/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    21900 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/video.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/types/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/core/vsenv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.304761 vspreview-0.6.0/vspreview/main/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    30658 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/main/window.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.304761 vspreview-0.6.0/vspreview/models/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/models/generalmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/models/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/models/scening.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/frame_props.ppy
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/split_view.ppy
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/plugins/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/benchmark/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/benchmark/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/comp/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/comp/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    30570 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/comp/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/debug/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/debug/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/debug/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/debug/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/main/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/main/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/misc/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/misc/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/pipette/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/pipette/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/pipette/colorview.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/pipette/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/pipette/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.308761 vspreview-0.6.0/vspreview/toolbars/playback/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/playback/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/playback/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    24791 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/playback/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.312761 vspreview-0.6.0/vspreview/toolbars/scening/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/scening/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/scening/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/scening/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    35867 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/toolbars/scening/toolbar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.312761 vspreview-0.6.0/vspreview/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/utils/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-11 01:40:07.000000 vspreview-0.6.0/vspreview/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 01:40:35.296761 vspreview-0.6.0/vspreview.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 01:40:25.000000 vspreview-0.6.0/vspreview.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-11 01:40:35.000000 vspreview-0.6.0/vspreview.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.439163 vspreview-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 14:26:50.000000 vspreview-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-20 14:27:17.439163 vspreview-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-20 14:26:50.000000 vspreview-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-20 14:27:17.439163 vspreview-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-20 14:26:50.000000 vspreview-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.427162 vspreview-0.7.0/vspreview/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.427162 vspreview-0.7.0/vspreview/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/api/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.427162 vspreview-0.7.0/vspreview/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16444 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/core/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/combobox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/dragnavigator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/edits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/graphicsview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4742 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/notch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/custom/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22099 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/types/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/core/vsenv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13718 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12902 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31241 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/main/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/models/generalmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/models/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14148 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/models/scening.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/frame_props.ppy
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/split_view.ppy
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/plugins/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.431163 vspreview-0.7.0/vspreview/toolbars/
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/benchmark/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9382 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/benchmark/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/comp/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/comp/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30482 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/comp/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/debug/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/debug/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/debug/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/debug/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/main/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/main/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/misc/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16070 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/misc/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/pipette/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/pipette/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/pipette/colorview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/pipette/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11751 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/pipette/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/playback/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/playback/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/playback/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25044 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/playback/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/toolbars/scening/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/scening/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/scening/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/scening/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35867 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/toolbars/scening/toolbar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.435163 vspreview-0.7.0/vspreview/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17975 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/utils/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-20 14:26:50.000000 vspreview-0.7.0/vspreview/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:27:17.427162 vspreview-0.7.0/vspreview.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:27:08.000000 vspreview-0.7.0/vspreview.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-20 14:27:17.000000 vspreview-0.7.0/vspreview.egg-info/top_level.txt
```

### Comparing `vspreview-0.6.0/LICENSE` & `vspreview-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/PKG-INFO` & `vspreview-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.6.0
+Version: 0.7.0
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
```

### Comparing `vspreview-0.6.0/README.md` & `vspreview-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/setup.cfg` & `vspreview-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/setup.py` & `vspreview-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/api/other.py` & `vspreview-0.7.0/vspreview/api/other.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/abstracts.py` & `vspreview-0.7.0/vspreview/core/abstracts.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/bases.py` & `vspreview-0.7.0/vspreview/core/bases.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/custom/combobox.py` & `vspreview-0.7.0/vspreview/core/custom/combobox.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/custom/dragnavigator.py` & `vspreview-0.7.0/vspreview/core/custom/dragnavigator.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/custom/edits.py` & `vspreview-0.7.0/vspreview/core/custom/edits.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/custom/graphicsview.py` & `vspreview-0.7.0/vspreview/core/custom/graphicsview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/custom/misc.py` & `vspreview-0.7.0/vspreview/core/custom/misc.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/custom/notch.py` & `vspreview-0.7.0/vspreview/core/custom/notch.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/custom/plotting.py` & `vspreview-0.7.0/vspreview/core/custom/plotting.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/logger.py` & `vspreview-0.7.0/vspreview/core/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,19 +48,22 @@
             )
 
         _logger_setup = True
 
 
 def set_log_level(main: int = LOG_LEVEL, engine: int = logging.ERROR) -> None:
     from vsengine import _hospice  # type: ignore[import]
+    from vsengine import policy
 
+    policy.logger.addFilter(lambda record: 'dead environment' not in record.msg)
     _hospice.logger.setLevel(engine)
     logging.getLogger().level = main
 
 
 def get_vs_logger() -> Callable[[MessageType, str], None]:
     setup_logger()
 
     def _logger(mType: MessageType, msg: str) -> None:
+        import logging
         return logging.log(_vsLogType_to_logging[mType], msg)
 
     return _logger
```

### Comparing `vspreview-0.6.0/vspreview/core/types/audio.py` & `vspreview-0.7.0/vspreview/core/types/audio.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
             vs_outputs = list(vs.get_outputs().values())
 
         self.index = vs_outputs.index(vs_output)
         self.source_vs_output = vs_output
         self.vs_output = self.source_vs_output
         self.is_mono = self.vs_output.num_channels == 1
 
+        self.info = self.main.user_output_info[vs.AudioNode].get(self.index, {})
+
         (self.arrayType, sampleTypeQ) = (
             'f', QAudioFormat.SampleFormat.Float
         ) if self.vs_output.sample_type == vs.FLOAT else (
             'I' if self.vs_output.bits_per_sample <= 16 else 'L', QAudioFormat.SampleFormat.Int16
         )
 
         sample_size = 8 * self.vs_output.bytes_per_sample
@@ -85,15 +87,15 @@
 
         self.audio_buffer = array(self.arrayType, [0] * self.SAMPLES_PER_FRAME * (self.vs_output.bytes_per_sample // 2))
 
         if not hasattr(self, 'name'):
             from ...models.outputs import AudioOutputs
 
             if vs_output in (vs_outputs := list(vs.get_outputs().values())):
-                self.name = self.main.user_output_names[vs.AudioNode].get(self.index, 'Track ' + str(self.index))
+                self.name = self.info.get('name', 'Track ' + str(self.index))
                 if isinstance(self.main.toolbars.playback.audio_outputs, AudioOutputs):
                     self.main.toolbars.playback.audio_outputs.setData(
                         self.main.toolbars.playback.audio_outputs.index(index), self.name
                     )
 
     def clear(self) -> None:
         self.source_vs_output = self.vs_output = None  # type: ignore
```

### Comparing `vspreview-0.6.0/vspreview/core/types/scene.py` & `vspreview-0.7.0/vspreview/core/types/scene.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/types/units.py` & `vspreview-0.7.0/vspreview/core/types/units.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/core/types/video.py` & `vspreview-0.7.0/vspreview/core/types/video.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 ]
 
 
 class PackingTypeInfo:
     _getid = iter_count()
 
     def __init__(
-        self, vs_format: VideoFormatT, qt_format: QImage.Format, shuffle: bool,
-        can_playback: bool = True
+        self, name: str, vs_format: VideoFormatT, qt_format: QImage.Format, shuffle: bool, can_playback: bool = True
     ):
         self.id = next(self._getid)
+        self.name = name
         self.vs_format = vs.core.get_video_format(vs_format)
         self.qt_format = qt_format
         self.shuffle = shuffle
         self.can_playback = can_playback
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, PackingTypeInfo):
@@ -41,48 +41,55 @@
         return self.id == other.id
 
     def __hash__(self) -> int:
         return int(self.id)
 
 
 class PackingType(PackingTypeInfo):
-    none_8bit = PackingTypeInfo(vs.RGB24, QImage.Format.Format_BGR30, False, False)
-    none_10bit = PackingTypeInfo(vs.RGB30, QImage.Format.Format_BGR30, False, False)
-    numpy_8bit = PackingTypeInfo(vs.RGB24, QImage.Format.Format_BGR30, True)
-    numpy_10bit = PackingTypeInfo(vs.RGB30, QImage.Format.Format_BGR30, True)
-    libp2p_8bit = PackingTypeInfo(vs.RGB24, QImage.Format.Format_RGB32, False)
-    libp2p_10bit = PackingTypeInfo(vs.RGB30, QImage.Format.Format_BGR30, True)
-    akarin_8bit = PackingTypeInfo(vs.RGB24, QImage.Format.Format_BGR30, False)
-    akarin_10bit = PackingTypeInfo(vs.RGB30, QImage.Format.Format_BGR30, False)
+    none_8bit = PackingTypeInfo('none-8bit', vs.RGB24, QImage.Format.Format_BGR30, False, False)
+    none_10bit = PackingTypeInfo('none-10bit', vs.RGB30, QImage.Format.Format_BGR30, False, False)
+    numpy_8bit = PackingTypeInfo('numpy-8bit', vs.RGB24, QImage.Format.Format_BGR30, True)
+    numpy_10bit = PackingTypeInfo('numpy-10bit', vs.RGB30, QImage.Format.Format_BGR30, True)
+    libp2p_8bit = PackingTypeInfo('libp2p-8bit', vs.RGB24, QImage.Format.Format_RGB32, False)
+    libp2p_10bit = PackingTypeInfo('libp2p-10bit', vs.RGB30, QImage.Format.Format_BGR30, True)
+    akarin_8bit = PackingTypeInfo('akarin-8bit', vs.RGB24, QImage.Format.Format_BGR30, False)
+    akarin_10bit = PackingTypeInfo('akarin-10bit', vs.RGB30, QImage.Format.Format_BGR30, False)
 
 
 PACKING_TYPE: PackingTypeInfo = None  # type: ignore
 
 
 class VideoOutput(AbstractYAMLObject):
     storable_attrs = (
-        'title', 'last_showed_frame', 'play_fps', 'crop_values'
+        'name', 'last_showed_frame', 'play_fps', 'crop_values'
     )
 
     __slots__ = (
         *storable_attrs, 'index', 'width', 'height', 'fps_num', 'fps_den',
         'total_frames', 'total_time',
         'end_frame', 'fps', 'source', 'prepared',
         'main', 'checkerboard', 'props', '_stateset'
     )
 
     source: VideoOutputNode
     prepared: VideoOutputNode
-    title: str | None
+    name: str
     last_showed_frame: Frame
     crop_values: CroppingInfo
     _stateset: bool
 
     def clear(self) -> None:
-        self.source = self.prepared = None  # type: ignore
+        if self.source:
+            del self.source.clip, self.source.alpha
+        if self.prepared:
+            del self.prepared.clip, self.prepared.alpha
+        if self.props:
+            self.props.clear()
+        del self.source, self.prepared, self.props
+        self.source = self.prepared = self.props = None
 
     def __init__(
         self, vs_output: vs.VideoOutputTuple, index: int, new_storage: bool = False
     ) -> None:
         self.setValue(vs_output, index, new_storage)
 
     def setValue(
@@ -112,17 +119,20 @@
         self.prepared.clip = self.prepare_vs_output(self.source.clip).std.CopyFrameProps(self.source.clip)
         self.width = self.prepared.clip.width
         self.height = self.prepared.clip.height
         self.fps_num = self.prepared.clip.fps.numerator
         self.fps_den = self.prepared.clip.fps.denominator
         self.fps = self.fps_num / self.fps_den
         self.total_frames = Frame(self.prepared.clip.num_frames)
-        self.title = self.main.user_output_names[vs.VideoNode].get(self.vs_index, None)  # type: ignore
+        self.info = self.main.user_output_info[vs.VideoNode].get(self.vs_index, {})  # type: ignore
+
+        self.name = self.info.get('name', 'Video Node %d' % self.vs_index)
+
         if self.main.outputs is not None:
-            self.main.outputs.setData(self.main.outputs.index(self.vs_index), self.title)
+            self.main.outputs.setData(self.main.outputs.index(self.vs_index), self.name)
 
         self.props = cast(vs.FrameProps, {})
 
         if self.source.alpha:
             self.checkerboard = self._generate_checkerboard()
 
         if not hasattr(self, 'last_showed_frame') or not (0 <= self.last_showed_frame < self.total_frames):
@@ -237,29 +247,14 @@
                 import numpy  # noqa: F401
                 PACKING_TYPE = PackingType.numpy_10bit if _default_10bits else PackingType.numpy_8bit
             except ModuleNotFoundError:
                 PACKING_TYPE = PackingType.none_10bit if _default_10bits else PackingType.none_8bit
 
         self.set_fmt_values()
 
-    @property
-    def name(self) -> str:
-        placeholder = 'Video Node %d' % self.index
-        if not hasattr(self, 'title') or self.title in {None, placeholder}:
-            if 'Name' in self.props:
-                self.title = cast(bytes, self.props['Name']).decode('utf-8')
-            elif not self.title:
-                self.title = placeholder
-
-        return self.title or placeholder
-
-    @name.setter
-    def name(self, newname: str) -> None:
-        self.title = newname
-
     def prepare_vs_output(self, clip: vs.VideoNode, is_alpha: bool = False) -> vs.VideoNode:
         from vstools import ChromaLocation, ColorRange, KwargsT, Matrix, Primaries, Transfer, video_heuristics
 
         assert clip.format
 
         heuristics = video_heuristics(clip, None)
 
@@ -298,21 +293,22 @@
 
         return self.pack_rgb_clip(clip)
 
     def pack_rgb_clip(self, clip: vs.VideoNode) -> vs.VideoNode:
         if PACKING_TYPE.shuffle:
             clip = clip.std.ShufflePlanes([2, 1, 0], vs.RGB)
 
+        shift = 2 ** (10 - PACKING_TYPE.vs_format.bits_per_sample)
+        r_shift, g_shift, b_shift = (x * shift for x in (1, 0x400, 0x100000))
+        high_bits_mask = 0xc0000000
+
         if PACKING_TYPE in {
             PackingType.none_8bit, PackingType.none_10bit, PackingType.numpy_8bit, PackingType.numpy_10bit
         }:
-            blank = vs.core.std.BlankClip(clip, None, None, vs.GRAY32, keep=True)
-
-            shift = 2 ** (10 - PACKING_TYPE.vs_format.bits_per_sample)
-            r_shift, g_shift, b_shift = (x * shift for x in (1, 1024, 1048576))
+            blank = vs.core.std.BlankClip(clip, None, None, vs.GRAY32, color=high_bits_mask, keep=True)
 
             if PACKING_TYPE in {PackingType.none_8bit, PackingType.none_10bit}:
                 from functools import partial
                 from multiprocessing.pool import ThreadPool
 
                 from vstools import ranges_product
 
@@ -321,15 +317,15 @@
                 pool = ThreadPool(self.main.settings.usable_cpus_count * 8)
 
                 def _packing_edarray(
                     bfp: vs.video_view, src_r: vs.video_view,
                     src_g: vs.video_view, src_b: vs.video_view,
                     idx: tuple[int, int]
                 ) -> None:
-                    bfp[idx] = (src_r[idx] * r_shift) + (src_g[idx] * g_shift) + (src_b[idx] * b_shift)
+                    bfp[idx] += (src_r[idx] * r_shift) + (src_g[idx] * g_shift) + (src_b[idx] * b_shift)
 
                 def _packrgb(n: int, f: list[vs.VideoFrame]) -> vs.VideoFrame:
                     bf = f[0].copy()
 
                     pool.map_async(partial(_packing_edarray, bf[0], f[1][0], f[1][1], f[1][2]), indices).wait()
 
                     return bf
@@ -337,54 +333,56 @@
                 import numpy as np
 
                 ein_shift = np.array([b_shift, g_shift, r_shift], np.uint32)
 
                 try:
                     import cupy as cp  # type: ignore
 
+                    self.__base_cupy_add = base_add = cp.asarray(blank.get_frame(0).copy()[0]).copy()
+
                     ein_shift = cp.asarray(ein_shift)
 
                     def _packrgb(n: int, f: list[vs.VideoFrame]) -> vs.VideoFrame:
                         bf = f[0].copy()
 
-                        cp.asnumpy(cp.einsum(
+                        cp.asnumpy(cp.add(cp.einsum(
                             'kji,k->ji', cp.asarray(f[1], cp.uint32), ein_shift, optimize='greedy'
-                        ), out=np.asarray(bf[0]))
+                        ), base_add), out=np.asarray(bf[0]))
 
                         return bf
                 except ModuleNotFoundError:
                     from numpy.core._multiarray_umath import c_einsum  # type: ignore
                     from numpy.core.numeric import tensordot
 
+                    self.__base_numpy_add = base_add = np.asarray(blank.get_frame(0).copy()[0]).copy()
+
                     def _packrgb(n: int, f: list[vs.VideoFrame]) -> vs.VideoFrame:
                         bf = f[0].copy()
 
-                        c_einsum(
-                            'ji->ji',
-                            tensordot(np.asarray(f[1], np.uint32), ein_shift, ((0,), (0,))),
-                            out=np.asarray(bf[0])
+                        np.add(
+                            c_einsum(
+                                'ji->ji', tensordot(np.asarray(f[1], np.uint32), ein_shift, ((0,), (0,)))
+                            ), base_add, np.asarray(bf[0])
                         )
 
                         return bf
 
             return blank.std.ModifyFrame([blank, clip], _packrgb)
 
         if PACKING_TYPE in {PackingType.libp2p_8bit, PackingType.libp2p_10bit}:
             return vs.core.libp2p.Pack(clip)
 
         if PACKING_TYPE in {PackingType.akarin_8bit, PackingType.akarin_10bit}:
             # x, y, z => b, g, r
             # we want a contiguous array, so we put in 0, 10 bits the R, 11 to 20 the G and 21 to 30 the B
-            # R stays like it is + shift if it's 8 bits (gets applied to all clips), then G gets shifted
+            # R stays like it is * shift if it's 8 bits (gets applied to all planes), then G gets shifted
             # by 10 bits, (we multiply by 2 ** 10) and same for B but by 20 bits and it all gets summed
-            shift = 2 ** (10 - PACKING_TYPE.vs_format.bits_per_sample)
-
             return vs.core.akarin.Expr(
                 clip.std.SplitPlanes(),
-                f'z {shift * 0x100000}  * y {shift * 0x400} * x {shift} * + + 0xc0000000 +', vs.GRAY32, True
+                f'z {b_shift} * y {g_shift} * x {r_shift} * + + {high_bits_mask} +', vs.GRAY32, True
             )
 
         return clip
 
     def frame_to_qimage(self, frame: vs.VideoFrame, is_alpha: bool = False) -> QImage:
         from ctypes import POINTER
         from ctypes import cast as ccast
@@ -561,13 +559,13 @@
 
         new_output.last_showed_frame = self.last_showed_frame
         new_output.name = self.name
 
         return new_output
 
     def __setstate__(self, state: Mapping[str, Any]) -> None:
-        try_load(state, 'title', str, self.__setattr__)
+        try_load(state, 'name', str, self.__setattr__)
         try_load(state, 'last_showed_frame', Frame, self.__setattr__)
         try_load(state, 'play_fps', Fraction, self.__setattr__)
         try_load(state, 'crop_values', CroppingInfo, self.__setattr__)
 
         self._stateset = True
```

### Comparing `vspreview-0.6.0/vspreview/core/types/yaml.py` & `vspreview-0.7.0/vspreview/core/types/yaml.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/init.py` & `vspreview-0.7.0/vspreview/init.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,34 +6,36 @@
 import sys
 from argparse import ArgumentParser
 from pathlib import Path
 from typing import Sequence
 
 from PyQt6.QtWidgets import QApplication
 
+from .core.logger import set_log_level, setup_logger
 # import vsenv as early as possible:
 # This is so other modules cannot accidentally use and lock us into a different policy.
 from .core.vsenv import set_vsengine_loop
-from .core.logger import set_log_level, setup_logger
 from .main import MainWindow
 from .plugins.install import install_plugins, plugins_commands, uninstall_plugins
 
 __all__ = [
     'main'
 ]
 
 
-def main(_args: Sequence[str] | None = None) -> None:
+def main(_args: Sequence[str] | None = None, no_exit: bool = False) -> None:
+    from .utils import exit_func
+
     parser = ArgumentParser(prog='VSPreview')
     parser.add_argument(
         'script_path_or_command', type=str, nargs='?',
         help=f'Path to Vapoursynth script or plugins command {",".join(plugins_commands)}'
     )
     parser.add_argument(
-        'plugins', type=str, nargs='+',
+        'plugins', type=str, nargs='*',
         help='Plugins to install/uninstall/update'
     )
     parser.add_argument(
         '--version', '-v', action='version', version='%(prog)s 0.2b'
     )
     parser.add_argument(
         '--preserve-cwd', '-c', action='store_true', help='do not chdir to script parent directory'
@@ -57,67 +59,85 @@
     )
 
     args = parser.parse_args(_args)
 
     setup_logger()
 
     if args.verbose:
+        from vstools import VSDebug
         set_log_level(logging.DEBUG, logging.DEBUG)
+        VSDebug(use_logging=True)
     else:
         set_log_level(logging.WARNING)
 
     if args.vscode_setup is not None:
         from .api.other import install_vscode_launch
 
         install_vscode_launch(args.vscode_setup)
 
-        sys.exit(0)
+        return exit_func(0, no_exit)
 
     script_path_or_command = args.script_path_or_command
 
     if not script_path_or_command and not (args.plugins and (script_path_or_command := next(iter(args.plugins)))):
         logging.error('Script path required.')
-        sys.exit(1)
+        return exit_func(1, no_exit)
 
     if (command := script_path_or_command) in plugins_commands:
         if not args.plugins:
             logging.error('You must provide at least one plugin!')
-            sys.exit(1)
+            return exit_func(1, no_exit)
 
         set_log_level(logging.INFO)
 
         plugins = list(args.plugins)
 
         if command == 'install':
             install_plugins(plugins, args.force, args.no_deps)
         elif command == 'uninstall':
             uninstall_plugins(plugins)
         elif command == 'update':
             uninstall_plugins(plugins, True)
             install_plugins(plugins, True, args.no_deps)
 
-        sys.exit(0)
+        return exit_func(0, no_exit)
 
     script_path = Path(script_path_or_command).resolve()
     if not script_path.exists():
         logging.error('Script path is invalid.')
-        sys.exit(1)
+        return exit_func(1, no_exit)
 
     if not args.preserve_cwd:
         os.chdir(script_path.parent)
 
-    app = QApplication(sys.argv)
-    set_vsengine_loop()
+    first_run = not hasattr(main, 'app')
+
+    if first_run:
+        main.app = QApplication(sys.argv)
+        set_vsengine_loop()
+    else:
+        from .core.vsenv import make_environment, get_current_environment
+        make_environment()
+        get_current_environment().use()
 
     signal.signal(signal.SIGINT, signal.SIG_DFL)
 
-    main_window = MainWindow(Path(os.getcwd()) if args.preserve_cwd else script_path.parent)
-    main_window.load_script(
+    main.main_window = MainWindow(Path(os.getcwd()) if args.preserve_cwd else script_path.parent, no_exit)
+    main.main_window.load_script(
         script_path, [tuple(a.split('=', maxsplit=1)) for a in args.arg or []], False, args.frame or None
     )
-    main_window.show()
+    main.main_window.show()
+
+    ret_code = main.app.exec()
+
+    if no_exit:
+        from .core.vsenv import _dispose
+
+        main.main_window.hide()
+
+        _dispose()
 
-    sys.exit(app.exec())
+    return exit_func(ret_code, no_exit)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `vspreview-0.6.0/vspreview/main/dialog.py` & `vspreview-0.7.0/vspreview/main/dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,16 @@
         self.hide()
         self.main.reload_script()
 
     def on_exit_clicked(self, clicked: bool | None = None) -> None:
         self.hide()
         self.script_exec_failed = True
 
-        sys.exit(1)
+        if not self.main.no_exit:
+            sys.exit(1)
 
     def closeEvent(self, event: QCloseEvent) -> None:
         self.on_exit_clicked()
 
 
 class SettingsDialog(ExtendedDialog):
     __slots__ = ('main', 'tab_widget',)
```

### Comparing `vspreview-0.6.0/vspreview/main/settings.py` & `vspreview-0.7.0/vspreview/main/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/main/timeline.py` & `vspreview-0.7.0/vspreview/main/timeline.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/main/window.py` & `vspreview-0.7.0/vspreview/main/window.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from PyQt6.QtCore import QEvent, QKeyCombination, QRectF, Qt, pyqtSignal
 from PyQt6.QtGui import QCloseEvent, QColorSpace, QKeySequence, QMoveEvent, QShortcut, QShowEvent
 from PyQt6.QtWidgets import QApplication, QLabel, QMainWindow, QSizePolicy, QSplitter, QTabWidget
 from vsengine import vpy  # type: ignore
 
 from ..core import (
     PRELOADED_MODULES, AbstractQItem, CroppingInfo, DragNavigator, ExtendedWidget, Frame, GraphicsImageItem,
-    GraphicsView, HBoxLayout, QAbstractYAMLObjectSingleton, StatusBar, Time, Timer, VBoxLayout, VideoOutput,
-    _monkey_runpy_dicts, get_current_environment, make_environment, MainVideoOutputGraphicsView
+    GraphicsView, HBoxLayout, MainVideoOutputGraphicsView, QAbstractYAMLObjectSingleton, StatusBar, Time, Timer,
+    VBoxLayout, VideoOutput, _monkey_runpy_dicts, dispose_environment, get_current_environment, make_environment
 )
 from ..models import GeneralModel, VideoOutputs
 from ..plugins import Plugins
 from ..toolbars import Toolbars
 from ..utils import fire_and_forget, set_status_label
 from .dialog import ScriptErrorDialog, SettingsDialog
 from .settings import MainSettings, WindowSettings
@@ -114,19 +114,21 @@
     toolbars: Toolbars
     plugins: Plugins
     app_settings: SettingsDialog
     window_settings = WindowSettings()
 
     autosave_timer: Timer
 
-    def __init__(self, config_dir: Path) -> None:
+    def __init__(self, config_dir: Path, no_exit: bool) -> None:
         from ..toolbars import MainToolbar
 
         super().__init__()
 
+        self.no_exit = no_exit
+
         self.settings = MainSettings(MainToolbar)
 
         self.current_config_dir = config_dir / self.VSP_DIR_NAME
         self.global_plugins_dir.mkdir(parents=True, exist_ok=True)
 
         self.app = cast(QApplication, QApplication.instance())
         assert self.app
@@ -159,16 +161,18 @@
         self.timecodes = dict[
             int, tuple[str | Path | dict[
                 tuple[int | None, int | None], float | tuple[int, int] | Fraction
             ] | list[Fraction], int | None]
         ]()
         self.norm_timecodes = dict[int, list[float]]()
 
-        self.user_output_names = {
-            vs.VideoNode: dict[int, str](), vs.AudioNode: dict[int, str](), vs.RawNode: dict[int, str]()
+        self.user_output_info = {
+            vs.VideoNode: dict[int, dict[str, Any]](),
+            vs.AudioNode: dict[int, dict[str, Any]](),
+            vs.RawNode: dict[int, dict[str, Any]]()
         }
 
         # global
         self.clipboard = self.app.clipboard()
         self.external_args = list[tuple[str, str]]()
         self.script_path = Path()
         self.script_exec_failed = False
@@ -215,17 +219,15 @@
 
         self.plugins_tab = QTabWidget(self.central_widget)
         self.plugins_tab.currentChanged.connect(lambda x: self.plugins.update())
 
         self.main_split = CentralSplitter(self, QtCore.Qt.Orientation.Horizontal)
         self.main_split.addWidget(self.graphics_view)
         self.main_split.addWidget(self.plugins_tab)
-        self.main_split.setSizePolicy(
-            QSizePolicy.Policy.Expanding, QSizePolicy.Policy.MinimumExpanding
-        )
+        self.main_split.setSizePolicy(QSizePolicy.Policy.Fixed, QSizePolicy.Policy.Fixed)
 
         HBoxLayout(self.main_layout, [self.main_split])
         self.main_layout.addWidget(self.timeline)
 
         # status bar
         self.statusbar = StatusBar(self.central_widget)
 
@@ -337,15 +339,15 @@
 
             self.env = vpy.variables(
                 dict(self.external_args),
                 environment=vs.get_current_environment(),
                 module_name="__vspreview__"
             ).result()
             self.env.module.__dict__['_monkey_runpy'] = random()
-            self.env = vpy.script(script_path, environment=self.env).result()
+            self.env = vpy.script(self.script_path, environment=self.env).result()
         except vpy.ExecutionFailed as e:
             from traceback import TracebackException
 
             logging.error(e.parent_error)
 
             te = TracebackException.from_exception(e.parent_error)
             logging.error(''.join(te.format()))
@@ -580,43 +582,57 @@
             return
 
         self.plugins.init_outputs()
 
         for graphics_view in self.graphics_views:
             graphics_view.graphics_scene.init_scenes()
 
-    def reload_script(self) -> None:
+    def clean_core_references(self) -> None:
         from vstools.utils.vs_proxy import clear_cache
 
-        self.reload_before_signal.emit()
+        for graphics_view in self.graphics_views:
+            graphics_view.graphics_scene.clear()
 
-        self.dump_storage()
+        self.timecodes.clear()
+        self.norm_timecodes.clear()
+
+        self.toolbars.pipette._curr_frame_cache.clear()
+        self.toolbars.pipette._curr_alphaframe_cache.clear()
+        self.toolbars.pipette.outputs.clear()
+
+        for v in self.user_output_info.values():
+            for k in v.values():
+                k.clear()
+            v.clear()
 
         try:
             with self.env:
                 clear_cache()
         except Exception:
             ...
 
         vs.clear_outputs()
-        for graphics_view in self.graphics_views:
-            graphics_view.graphics_scene.clear()
 
-        self.timecodes.clear()
-        self.norm_timecodes.clear()
-        for v in self.user_output_names.values():
-            v.clear()
         if self.outputs:
             self.outputs.clear()
+
         self.gc_collect()
+
+    def reload_script(self) -> None:
+        self.reload_before_signal.emit()
+
+        self.dump_storage()
+
+        self.clean_core_references()
+
         old_environment = get_current_environment()
 
         self.clear_monkey_runpy()
         make_environment()
-        old_environment.dispose()
+        dispose_environment(old_environment)
         self.gc_collect()
 
         try:
             self.load_script(self.script_path, reloading=True)
         finally:
             self.clear_monkey_runpy()
 
@@ -814,29 +830,36 @@
     def update_timecodes_info(
         self, index: int, timecodes: str | Path | dict[
             tuple[int | None, int | None], float | tuple[int, int] | Fraction
         ] | list[Fraction], den: int | None = None
     ) -> None:
         self.timecodes[index] = (timecodes, den)
 
-    def set_node_name(self, node_type: type, index: int, name: str) -> None:
-        self.user_output_names[node_type][index] = name
+    def set_node_info(self, node_type: type, index: int, **kwargs: Any) -> None:
+        base = self.user_output_info[node_type]
+
+        if index not in base:
+            base[index] = {**kwargs}
+        else:
+            base[index] |= kwargs
 
     def event(self, event: QEvent) -> bool:
         if event.type() == QEvent.Type.LayoutRequest:
             self.timeline.full_repaint()
 
         return super().event(event)
 
     # misc methods
     def showEvent(self, event: QShowEvent) -> None:
         super().showEvent(event)
         for graphics_view in self.graphics_views:
             graphics_view.setSizePolicy(self.EVENT_POLICY)
 
+        self.main_split.setSizePolicy(self.EVENT_POLICY)
+
     def closeEvent(self, event: QCloseEvent) -> None:
         if self.settings.autosave_control.value() != Time(seconds=0):
             self.dump_storage_async()
 
         self.reload_signal.emit()
 
     def moveEvent(self, _move_event: QMoveEvent) -> None:
```

### Comparing `vspreview-0.6.0/vspreview/models/generalmodel.py` & `vspreview-0.7.0/vspreview/models/generalmodel.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/models/outputs.py` & `vspreview-0.7.0/vspreview/models/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,14 @@
         local_storage, newstorage = (local_storage, False) if local_storage is not None else ({}, True)
 
         if main.storage_not_found:
             newstorage = False
 
         outputs = OrderedDict(sorted(vs.get_outputs().items()))
 
-        main.reload_signal.connect(self.clear_outputs)
-
         for i, vs_output in outputs.items():
             if not isinstance(vs_output, self.vs_type):
                 continue
 
             try:
                 output = local_storage[str(i)]
                 output.setValue(vs_output, i, newstorage)  # type: ignore
@@ -60,16 +58,16 @@
                 output = self.out_type(vs_output, i, newstorage)  # type: ignore
 
             self.items.append(output)
 
         self._items = list(self.items)
 
     def clear_outputs(self) -> None:
-        for o in self.items:
-            o.clear()
+        for output in (*self.items, *self._items):
+            output.clear()
 
     def __getitem__(self, i: int) -> T:
         return self.items[i]
 
     def __len__(self) -> int:
         return len(self.items)
 
@@ -84,14 +82,15 @@
         self.beginInsertRows(QModelIndex(), index, index)
         self.items.append(item)
         self.endInsertRows()
 
         return len(self.items) - 1
 
     def clear(self) -> None:
+        self.clear_outputs()
         self.beginRemoveRows(QModelIndex(), 0, len(self.items))
         self.items.clear()
         self._items.clear()
         self.endRemoveRows()
 
     def data(self, index: QModelIndex, role: int = Qt.ItemDataRole.UserRole) -> Any:
         if not index.isValid():
```

### Comparing `vspreview-0.6.0/vspreview/models/scening.py` & `vspreview-0.7.0/vspreview/models/scening.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/plugins/__init__.py` & `vspreview-0.7.0/vspreview/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/plugins/abstract.py` & `vspreview-0.7.0/vspreview/plugins/abstract.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/plugins/frame_props.ppy` & `vspreview-0.7.0/vspreview/plugins/frame_props.ppy`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/plugins/install.py` & `vspreview-0.7.0/vspreview/plugins/install.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/plugins/split_view.ppy` & `vspreview-0.7.0/vspreview/plugins/split_view.ppy`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/plugins/utils.py` & `vspreview-0.7.0/vspreview/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/__init__.py` & `vspreview-0.7.0/vspreview/toolbars/__init__.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/benchmark/settings.py` & `vspreview-0.7.0/vspreview/toolbars/benchmark/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/benchmark/toolbar.py` & `vspreview-0.7.0/vspreview/toolbars/benchmark/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/comp/settings.py` & `vspreview-0.7.0/vspreview/toolbars/comp/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/comp/toolbar.py` & `vspreview-0.7.0/vspreview/toolbars/comp/toolbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -792,17 +792,15 @@
             if not tmdb_id.startswith(suffix):
                 tmdb_id = f"{suffix}{tmdb_id}"
 
         tags = [self.tag_data.get(tag, tag) for tag in self.current_tags]
 
         filtered_outputs = []
         for output in self.main.outputs:
-            props = output.source.clip.get_frame(check_frame).props
-
-            if '_VSPDisableComp' in props and props._VSPDisableComp == 1:
+            if output.info.get('disable_comp', False):
                 continue
 
             filtered_outputs.append(output)
 
         return WorkerConfiguration(
             str(uuid4()), filtered_outputs, collection_name,
             self.is_public_checkbox.isChecked(), self.is_nsfw_checkbox.isChecked(),
```

### Comparing `vspreview-0.6.0/vspreview/toolbars/debug/toolbar.py` & `vspreview-0.7.0/vspreview/toolbars/debug/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/main/toolbar.py` & `vspreview-0.7.0/vspreview/toolbars/main/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/misc/toolbar.py` & `vspreview-0.7.0/vspreview/toolbars/misc/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/pipette/colorview.py` & `vspreview-0.7.0/vspreview/toolbars/pipette/colorview.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/pipette/toolbar.py` & `vspreview-0.7.0/vspreview/toolbars/pipette/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,33 +50,28 @@
         self.tracking = False
         self._curr_frame_cache = WeakKeyDictionary[VideoOutput, tuple[int, vs.VideoFrame]]()
         self._curr_alphaframe_cache = WeakKeyDictionary[VideoOutput, tuple[int, vs.VideoFrame]]()
         self._mouse_is_subscribed = False
 
         self.last_pos: tuple[VideoOutput, QPoint] | None = None
 
-        main.reload_signal.connect(self.clear_outputs)
-
         self.set_qobject_names()
 
         self.data_types = {
             vs.INTEGER: {
                 1: ctypes.c_uint8,
                 2: ctypes.c_uint16,
                 4: ctypes.c_uint32,
             },
             vs.FLOAT: {
                 2: ctypes.c_char,
                 4: ctypes.c_float,
             }
         }
 
-    def clear_outputs(self) -> None:
-        self.outputs.clear()
-
     def setup_ui(self) -> None:
         super().setup_ui()
 
         self.color_view = ColorView(self)
         self.color_view.setFixedSize(self.height() // 2, self.height() // 2)
 
         font = QFont('Consolas', 9)
```

### Comparing `vspreview-0.6.0/vspreview/toolbars/playback/settings.py` & `vspreview-0.7.0/vspreview/toolbars/playback/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/playback/toolbar.py` & `vspreview-0.7.0/vspreview/toolbars/playback/toolbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         qt_silent_call(self.seek_frame_control.setMaximum, self.main.current_output.total_frames)
         qt_silent_call(self.seek_time_control.setMaximum, self.main.current_output.total_time)
         qt_silent_call(self.seek_time_control.setMinimum, Time(Frame(1)))
         qt_silent_call(self.seek_time_control.setValue, Time(self.seek_frame_control.value()))
         qt_silent_call(self.fps_spinbox.setValue, float(self.main.current_output.play_fps))
 
     def rescan_outputs(self, outputs: AudioOutputs | None = None) -> None:
-        self.audio_outputs = outputs or AudioOutputs(self.main)
+        self.audio_outputs = outputs if isinstance(outputs, AudioOutputs) else AudioOutputs(self.main)
         self.audio_outputs_combobox.setModel(self.audio_outputs)
 
     def get_true_fps(self, n: int | Frame, frameprops: vs.FrameProps, force: bool = False) -> Fraction:
         if (
             hasattr(self.main.current_output, 'got_timecodes') and self.main.current_output.got_timecodes and not force
         ):
             return Fraction(self.main.current_output.timecodes[int(n)])
@@ -231,15 +231,22 @@
     @property
     def got_debug_fps(self) -> bool:
         return hasattr(self.main.toolbars, 'debug') and self.main.toolbars.debug.settings.DEBUG_PLAY_FPS
 
     def play(self, stop_at_frame: int | Frame | None = None) -> None:
         if (
             self.main.current_output.last_showed_frame > self.main.current_output.total_frames
-        ) or not video.PACKING_TYPE.can_playback:
+        ):
+            return
+
+        if not video.PACKING_TYPE.can_playback:
+            import logging
+            logging.warn(
+                f'The current backend ({video.PACKING_TYPE.name}) can\'t playback! Install akarin or libp2p plugins.'
+            )
             return
 
         if self.main.statusbar.label.text() == 'Ready':
             self.main.statusbar.label.setText('Playing')
 
         if self.main.current_output.prepared.alpha is None:
             self.allocate_buffer(False)
```

### Comparing `vspreview-0.6.0/vspreview/toolbars/scening/dialog.py` & `vspreview-0.7.0/vspreview/toolbars/scening/dialog.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/scening/settings.py` & `vspreview-0.7.0/vspreview/toolbars/scening/settings.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/toolbars/scening/toolbar.py` & `vspreview-0.7.0/vspreview/toolbars/scening/toolbar.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/utils/debug.py` & `vspreview-0.7.0/vspreview/utils/debug.py`

 * *Files identical despite different names*

### Comparing `vspreview-0.6.0/vspreview/utils/utils.py` & `vspreview-0.7.0/vspreview/utils/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from __future__ import annotations
 
+import sys
 from functools import partial, wraps
 from string import Template
 from typing import TYPE_CHECKING, Any, Callable
 
 from PyQt6.QtCore import QSignalBlocker
 
 if TYPE_CHECKING:
     from vstools import F, P, R, T
 
 from ..core import Time, main_window
 
 __all__ = [
+    'exit_func',
     'qt_silent_call',
     'strfdelta',
     'fire_and_forget',
     'set_status_label'
 ]
 
 
+def exit_func(ret_code: int, no_exit: bool) -> int:
+    if not no_exit:
+        sys.exit(ret_code)
+
+    return ret_code
+
+
 # it is a BuiltinMethodType at the same time
 def qt_silent_call(qt_method: Callable[P, R], *args: P.args, **kwargs: P.kwargs) -> R:
     block = QSignalBlocker(qt_method.__self__)  # type: ignore
     ret = qt_method(*args, **kwargs)
     del block
     return ret
```

### Comparing `vspreview-0.6.0/vspreview.egg-info/PKG-INFO` & `vspreview-0.7.0/vspreview.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vspreview
-Version: 0.6.0
+Version: 0.7.0
 Summary: Previewer for VapourSynth scripts
 Author: Endilll
 Author-email: 
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-preview
 Project-URL: Documentation, https://vspreview.encode.moe/en/latest/
```

### Comparing `vspreview-0.6.0/vspreview.egg-info/SOURCES.txt` & `vspreview-0.7.0/vspreview.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 vspreview.egg-info/entry_points.txt
 vspreview.egg-info/not-zip-safe
 vspreview.egg-info/requires.txt
 vspreview.egg-info/top_level.txt
 vspreview/api/__init__.py
 vspreview/api/app.py
 vspreview/api/info.py
+vspreview/api/nodes.py
 vspreview/api/other.py
 vspreview/api/output.py
-vspreview/api/timecodes.py
 vspreview/core/__init__.py
 vspreview/core/abstracts.py
 vspreview/core/bases.py
 vspreview/core/logger.py
 vspreview/core/vsenv.py
 vspreview/core/custom/__init__.py
 vspreview/core/custom/combobox.py
```

