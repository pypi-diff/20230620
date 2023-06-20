# Comparing `tmp/trackc-0.0.8.tar.gz` & `tmp/trackc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/yuanzan/Documents/github/seqyuan/trackc/dist/.tmp-q14gdtci/trackc-0.0.8.tar", last modified: Fri May 26 10:11:00 2023, max compression
+gzip compressed data, was "/Users/yuanzan/Documents/github/seqyuan/trackc/dist/.tmp-puolyzzf/trackc-0.0.9.tar", last modified: Tue Jun 20 04:38:29 2023, max compression
```

## Comparing `trackc-0.0.8.tar` & `trackc-0.0.9.tar`

### file list

```diff
@@ -1,105 +1,129 @@
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.902244 trackc-0.0.8/
--rw-r--r--   0 yuanzan    (501) staff       (20)       57 2023-05-23 15:00:45.000000 trackc-0.0.8/.gitignore
--rw-r--r--   0 yuanzan    (501) staff       (20)       25 2023-05-18 01:07:49.000000 trackc-0.0.8/.readthedocs.yml
--rw-r--r--   0 yuanzan    (501) staff       (20)     1064 2023-01-09 03:28:24.000000 trackc-0.0.8/LICENSE
--rw-r--r--   0 yuanzan    (501) staff       (20)      381 2023-05-26 10:11:00.898104 trackc-0.0.8/PKG-INFO
--rw-r--r--   0 yuanzan    (501) staff       (20)     1464 2023-05-26 10:10:21.000000 trackc-0.0.8/README.rst
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.477678 trackc-0.0.8/bin/
--rw-r--r--   0 yuanzan    (501) staff       (20)      129 2023-05-26 09:06:17.000000 trackc-0.0.8/bin/gtf2bed4trackc
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.537921 trackc-0.0.8/docs/
--rw-r--r--   0 yuanzan    (501) staff       (20)      645 2023-05-17 10:00:32.000000 trackc-0.0.8/docs/Makefile
--rw-r--r--   0 yuanzan    (501) staff       (20)       77 2023-05-23 15:39:03.000000 trackc-0.0.8/docs/_config.yml
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.549075 trackc-0.0.8/docs/_static/
--rw-r--r--   0 yuanzan    (501) staff       (20)   230273 2023-05-22 03:27:26.000000 trackc-0.0.8/docs/_static/demo.png
--rw-r--r--   0 yuanzan    (501) staff       (20)    15415 2023-05-22 03:27:26.000000 trackc-0.0.8/docs/_static/plotly_logo.png
--rw-r--r--   0 yuanzan    (501) staff       (20)      196 2023-05-22 03:27:26.000000 trackc-0.0.8/docs/_static/switcher.json
--rw-r--r--   0 yuanzan    (501) staff       (20)      628 2023-05-22 03:27:26.000000 trackc-0.0.8/docs/_static/theme_override.css
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.551547 trackc-0.0.8/docs/_templates/
--rw-r--r--   0 yuanzan    (501) staff       (20)      992 2023-05-22 03:27:26.000000 trackc-0.0.8/docs/_templates/module.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)      901 2023-05-22 06:05:37.000000 trackc-0.0.8/docs/api.rst
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.556043 trackc-0.0.8/docs/binder/
--rw-r--r--   0 yuanzan    (501) staff       (20)      167 2023-05-22 01:24:25.000000 trackc-0.0.8/docs/binder/requirements.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)    14672 2023-05-23 15:39:06.000000 trackc-0.0.8/docs/conf.py
--rw-r--r--   0 yuanzan    (501) staff       (20)    10978 2023-05-20 00:33:12.000000 trackc-0.0.8/docs/conf.py_bk
--rw-r--r--   0 yuanzan    (501) staff       (20)     2358 2023-05-19 07:42:13.000000 trackc-0.0.8/docs/custom-formats.pct.py
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.563717 trackc-0.0.8/docs/developer/
--rw-r--r--   0 yuanzan    (501) staff       (20)      631 2023-05-22 08:44:49.000000 trackc-0.0.8/docs/developer/about_us.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)     1094 2023-05-22 10:35:09.000000 trackc-0.0.8/docs/developer/history.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)      184 2023-05-22 09:10:50.000000 trackc-0.0.8/docs/developer/index.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)      187 2023-05-22 08:24:28.000000 trackc-0.0.8/docs/developer.rst
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.617461 trackc-0.0.8/docs/examples/
--rw-r--r--   0 yuanzan    (501) staff       (20)      777 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/examples/README.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)   704833 2023-05-24 03:22:31.000000 trackc-0.0.8/docs/examples/bw_track_tutorial.ipynb
--rw-r--r--   0 yuanzan    (501) staff       (20)   411933 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/examples/cmap-test-data.ipynb
--rw-r--r--   0 yuanzan    (501) staff       (20)   685187 2023-05-23 02:59:18.000000 trackc-0.0.8/docs/examples/mapc_eg.ipynb
--rw-r--r--   0 yuanzan    (501) staff       (20)   608023 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/examples/zoomin_heatmap.ipynb
--rw-r--r--   0 yuanzan    (501) staff       (20)   146859 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/examples/zoomin_heatmap.png
--rw-r--r--   0 yuanzan    (501) staff       (20)      176 2023-01-09 03:28:25.000000 trackc-0.0.8/docs/faq.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)      417 2023-05-23 01:46:30.000000 trackc-0.0.8/docs/gallary.rst
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.629551 trackc-0.0.8/docs/images/
--rw-r--r--   0 yuanzan    (501) staff       (20)   481183 2023-05-25 09:33:34.000000 trackc-0.0.8/docs/images/trackc_dynamic_2022.png
--rw-r--r--   0 yuanzan    (501) staff       (20)    13078 2023-05-17 02:08:38.000000 trackc-0.0.8/docs/images/trackc_logo.png
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.635805 trackc-0.0.8/docs/images/tutorials/
--rw-r--r--   0 yuanzan    (501) staff       (20)    89978 2023-05-22 05:54:42.000000 trackc-0.0.8/docs/images/tutorials/grid_spec_01.png
--rw-r--r--   0 yuanzan    (501) staff       (20)   146859 2023-05-22 02:49:56.000000 trackc-0.0.8/docs/images/tutorials/zoomin_heatmap.png
--rw-r--r--   0 yuanzan    (501) staff       (20)     1735 2023-05-25 09:30:13.000000 trackc-0.0.8/docs/index.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)      764 2023-05-17 09:57:58.000000 trackc-0.0.8/docs/make.bat
--rw-r--r--   0 yuanzan    (501) staff       (20)       49 2023-05-17 15:35:25.000000 trackc-0.0.8/docs/modules.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)     1029 2023-05-25 06:54:10.000000 trackc-0.0.8/docs/quick_start.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)     3501 2023-05-25 09:45:26.000000 trackc-0.0.8/docs/references.bib
--rw-r--r--   0 yuanzan    (501) staff       (20)       52 2023-05-18 01:26:56.000000 trackc-0.0.8/docs/references.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)        0 2023-05-17 07:21:56.000000 trackc-0.0.8/docs/releases.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)      597 2023-05-23 02:00:50.000000 trackc-0.0.8/docs/requirements.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)     7789 2023-05-22 01:25:34.000000 trackc-0.0.8/docs/source
--rw-r--r--   0 yuanzan    (501) staff       (20)      450 2023-05-17 15:35:14.000000 trackc-0.0.8/docs/trackc.pa.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)     1411 2023-05-17 15:35:14.000000 trackc-0.0.8/docs/trackc.pl.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)      375 2023-05-17 15:35:14.000000 trackc-0.0.8/docs/trackc.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)      150 2023-05-17 15:35:14.000000 trackc-0.0.8/docs/trackc.tl.rst
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.757140 trackc-0.0.8/docs/tutorials/
--rw-r--r--   0 yuanzan    (501) staff       (20)      386 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/tutorials/README.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)   708712 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/tutorials/bw_track_tutorial.ipynb
--rw-r--r--   0 yuanzan    (501) staff       (20)   411911 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/tutorials/cmap-test-data.ipynb
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.771371 trackc-0.0.8/docs/tutorials/fileformats/
--rw-r--r--   0 yuanzan    (501) staff       (20)     1562 2023-05-26 06:07:18.000000 trackc-0.0.8/docs/tutorials/fileformats/GRCh38.84.gtf.bed12
--rw-r--r--   0 yuanzan    (501) staff       (20)     1104 2023-05-26 06:15:29.000000 trackc-0.0.8/docs/tutorials/fileformats/bed12.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)   526486 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/tutorials/mapc_eg.ipynb
--rw-r--r--   0 yuanzan    (501) staff       (20)   607928 2023-05-23 01:13:11.000000 trackc-0.0.8/docs/tutorials/zoomin_heatmap.ipynb
--rw-r--r--   0 yuanzan    (501) staff       (20)     1258 2023-05-26 00:38:40.000000 trackc-0.0.8/docs/tutorials.rst
--rw-r--r--   0 yuanzan    (501) staff       (20)     1931 2023-05-19 09:33:48.000000 trackc-0.0.8/docs/utils.py
--rw-r--r--   0 yuanzan    (501) staff       (20)      112 2023-05-26 09:19:01.000000 trackc-0.0.8/pypi.sh
--rw-r--r--   0 yuanzan    (501) staff       (20)       18 2023-01-09 05:16:57.000000 trackc-0.0.8/requirements.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)       38 2023-05-26 10:11:00.902487 trackc-0.0.8/setup.cfg
--rw-r--r--   0 yuanzan    (501) staff       (20)     1257 2023-05-26 10:10:28.000000 trackc-0.0.8/setup.py
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.467332 trackc-0.0.8/src/
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.779422 trackc-0.0.8/src/trackc/
--rw-r--r--   0 yuanzan    (501) staff       (20)      395 2023-05-17 15:12:16.000000 trackc-0.0.8/src/trackc/__init__.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     2172 2023-05-19 09:43:28.000000 trackc-0.0.8/src/trackc/_utils.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     3479 2023-05-15 11:51:00.000000 trackc-0.0.8/src/trackc/gs.py
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.856131 trackc-0.0.8/src/trackc/pa/
--rw-r--r--   0 yuanzan    (501) staff       (20)      211 2023-05-17 15:15:18.000000 trackc-0.0.8/src/trackc/pa/__init__.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     1566 2023-05-15 07:22:37.000000 trackc-0.0.8/src/trackc/pa/cmaps.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     4362 2023-05-10 01:28:12.000000 trackc-0.0.8/src/trackc/pa/palettes.py
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.888376 trackc-0.0.8/src/trackc/pl/
--rw-r--r--   0 yuanzan    (501) staff       (20)     4528 2023-05-23 09:06:04.000000 trackc-0.0.8/src/trackc/pl/Virtual4C.py
--rw-r--r--   0 yuanzan    (501) staff       (20)      813 2023-05-17 15:16:06.000000 trackc-0.0.8/src/trackc/pl/__init__.py
--rw-r--r--   0 yuanzan    (501) staff       (20)    10770 2023-05-23 14:20:20.000000 trackc-0.0.8/src/trackc/pl/bed.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     6516 2023-05-23 14:21:24.000000 trackc-0.0.8/src/trackc/pl/bigwig.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     5878 2023-05-23 14:15:48.000000 trackc-0.0.8/src/trackc/pl/gene.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     6493 2023-05-23 14:15:59.000000 trackc-0.0.8/src/trackc/pl/links.py
--rw-r--r--   0 yuanzan    (501) staff       (20)    14755 2023-05-23 14:12:51.000000 trackc-0.0.8/src/trackc/pl/mapc.py
--rw-r--r--   0 yuanzan    (501) staff       (20)    11947 2023-05-23 09:04:24.000000 trackc-0.0.8/src/trackc/pl/mapc_markline.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     2645 2023-05-15 12:53:14.000000 trackc-0.0.8/src/trackc/pl/mapc_xylim.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)     7694 2023-05-23 08:58:13.000000 trackc-0.0.8/src/trackc/pl/scale.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     2812 2023-05-19 08:34:47.000000 trackc-0.0.8/src/trackc/pl/zoomin.py
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.891790 trackc-0.0.8/src/trackc/scripts/
--rw-r--r--   0 yuanzan    (501) staff       (20)        0 2023-05-26 09:03:49.000000 trackc-0.0.8/src/trackc/scripts/__init__.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     6217 2023-05-26 09:06:01.000000 trackc-0.0.8/src/trackc/scripts/gtf2bed12.py
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.896209 trackc-0.0.8/src/trackc/tl/
--rw-r--r--   0 yuanzan    (501) staff       (20)      126 2023-05-17 15:16:25.000000 trackc-0.0.8/src/trackc/tl/__init__.py
--rw-r--r--   0 yuanzan    (501) staff       (20)     8848 2023-05-15 07:09:40.000000 trackc-0.0.8/src/trackc/tl/_getRegionsCmat.py
-drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-05-26 10:11:00.838439 trackc-0.0.8/src/trackc.egg-info/
--rw-r--r--   0 yuanzan    (501) staff       (20)      381 2023-05-26 10:10:59.000000 trackc-0.0.8/src/trackc.egg-info/PKG-INFO
--rw-r--r--   0 yuanzan    (501) staff       (20)     2046 2023-05-26 10:11:00.000000 trackc-0.0.8/src/trackc.egg-info/SOURCES.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)        1 2023-05-26 10:10:59.000000 trackc-0.0.8/src/trackc.egg-info/dependency_links.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)       18 2023-05-26 10:10:59.000000 trackc-0.0.8/src/trackc.egg-info/requires.txt
--rw-r--r--   0 yuanzan    (501) staff       (20)        7 2023-05-26 10:10:59.000000 trackc-0.0.8/src/trackc.egg-info/top_level.txt
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.526247 trackc-0.0.9/
+-rw-r--r--   0 yuanzan    (501) staff       (20)       57 2023-05-23 15:00:45.000000 trackc-0.0.9/.gitignore
+-rw-r--r--   0 yuanzan    (501) staff       (20)       25 2023-05-18 01:07:49.000000 trackc-0.0.9/.readthedocs.yml
+-rw-r--r--   0 yuanzan    (501) staff       (20)     1064 2023-01-09 03:28:24.000000 trackc-0.0.9/LICENSE
+-rw-r--r--   0 yuanzan    (501) staff       (20)      378 2023-06-20 04:38:29.525719 trackc-0.0.9/PKG-INFO
+-rw-r--r--   0 yuanzan    (501) staff       (20)     1464 2023-05-26 10:10:21.000000 trackc-0.0.9/README.rst
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.184977 trackc-0.0.9/bin/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      180 2023-05-26 10:28:57.000000 trackc-0.0.9/bin/gtf2bed4trackc
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.239820 trackc-0.0.9/docs/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      645 2023-05-17 10:00:32.000000 trackc-0.0.9/docs/Makefile
+-rw-r--r--   0 yuanzan    (501) staff       (20)       77 2023-05-23 15:39:03.000000 trackc-0.0.9/docs/_config.yml
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.250108 trackc-0.0.9/docs/_static/
+-rw-r--r--   0 yuanzan    (501) staff       (20)   230273 2023-05-22 03:27:26.000000 trackc-0.0.9/docs/_static/demo.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)    15415 2023-05-22 03:27:26.000000 trackc-0.0.9/docs/_static/plotly_logo.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)      196 2023-05-22 03:27:26.000000 trackc-0.0.9/docs/_static/switcher.json
+-rw-r--r--   0 yuanzan    (501) staff       (20)      628 2023-05-22 03:27:26.000000 trackc-0.0.9/docs/_static/theme_override.css
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.257473 trackc-0.0.9/docs/_templates/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      992 2023-05-22 03:27:26.000000 trackc-0.0.9/docs/_templates/module.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      901 2023-05-22 06:05:37.000000 trackc-0.0.9/docs/api.rst
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.259766 trackc-0.0.9/docs/binder/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      167 2023-05-22 01:24:25.000000 trackc-0.0.9/docs/binder/requirements.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)    14678 2023-06-12 03:38:12.000000 trackc-0.0.9/docs/conf.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     2358 2023-05-19 07:42:13.000000 trackc-0.0.9/docs/custom-formats.pct.py
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.267999 trackc-0.0.9/docs/developer/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      629 2023-05-27 04:08:57.000000 trackc-0.0.9/docs/developer/about_us.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)     1141 2023-06-11 10:19:10.000000 trackc-0.0.9/docs/developer/history.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      184 2023-05-22 09:10:50.000000 trackc-0.0.9/docs/developer/index.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      187 2023-05-22 08:24:28.000000 trackc-0.0.9/docs/developer.rst
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.310548 trackc-0.0.9/docs/examples/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      777 2023-05-23 01:13:11.000000 trackc-0.0.9/docs/examples/README.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)   704833 2023-05-24 03:22:31.000000 trackc-0.0.9/docs/examples/bw_track_tutorial.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)   411933 2023-05-23 01:13:11.000000 trackc-0.0.9/docs/examples/cmap-test-data.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)   685114 2023-06-11 08:32:38.000000 trackc-0.0.9/docs/examples/mapc_eg.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)    39232 2023-06-11 14:12:08.000000 trackc-0.0.9/docs/examples/neotad.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)  1645307 2023-06-11 14:11:22.000000 trackc-0.0.9/docs/examples/rearranged_interactions.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)   146859 2023-05-23 01:13:11.000000 trackc-0.0.9/docs/examples/zoomin_heatmap.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)      176 2023-01-09 03:28:25.000000 trackc-0.0.9/docs/faq.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      570 2023-06-11 14:59:06.000000 trackc-0.0.9/docs/gallery.rst
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.352140 trackc-0.0.9/docs/images/
+-rw-r--r--   0 yuanzan    (501) staff       (20)   109859 2023-06-11 11:09:52.000000 trackc-0.0.9/docs/images/trackc-brand-board-your-branding-colors-and-fonts.zip
+-rw-r--r--   0 yuanzan    (501) staff       (20)    27234 2023-06-11 11:09:01.000000 trackc-0.0.9/docs/images/trackc-high-resolution-color-logo.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)    33743 2023-06-11 11:09:11.000000 trackc-0.0.9/docs/images/trackc-high-resolution-logo-color-on-transparent-background.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)    35406 2023-06-11 11:09:19.000000 trackc-0.0.9/docs/images/trackc-high-resolution-logo-white-on-transparent-background.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)   289772 2023-06-11 11:09:40.000000 trackc-0.0.9/docs/images/trackc-logo-zip-file.zip
+-rw-r--r--   0 yuanzan    (501) staff       (20)    27618 2023-06-11 11:07:36.000000 trackc-0.0.9/docs/images/trackc-low-resolution-color-logo.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)    22793 2023-06-11 11:08:51.000000 trackc-0.0.9/docs/images/trackc-low-resolution-logo-black-on-transparent-background.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)    29367 2023-06-11 11:08:38.000000 trackc-0.0.9/docs/images/trackc-low-resolution-logo-color-on-transparent-background.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)    23498 2023-06-11 11:08:45.000000 trackc-0.0.9/docs/images/trackc-low-resolution-logo-white-on-transparent-background.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)   481183 2023-05-25 09:33:34.000000 trackc-0.0.9/docs/images/trackc_dynamic_2022.png
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.364962 trackc-0.0.9/docs/images/tutorials/
+-rw-r--r--   0 yuanzan    (501) staff       (20)    89978 2023-05-22 05:54:42.000000 trackc-0.0.9/docs/images/tutorials/grid_spec_01.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)    39914 2023-06-06 01:57:36.000000 trackc-0.0.9/docs/images/tutorials/quick_start.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)   146859 2023-05-22 02:49:56.000000 trackc-0.0.9/docs/images/tutorials/zoomin_heatmap.png
+-rw-r--r--   0 yuanzan    (501) staff       (20)     1313 2023-06-11 15:04:45.000000 trackc-0.0.9/docs/index.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      532 2023-06-11 15:05:49.000000 trackc-0.0.9/docs/install.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      764 2023-05-17 09:57:58.000000 trackc-0.0.9/docs/make.bat
+-rw-r--r--   0 yuanzan    (501) staff       (20)       49 2023-05-17 15:35:25.000000 trackc-0.0.9/docs/modules.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)     4277 2023-05-29 04:28:52.000000 trackc-0.0.9/docs/references.bib
+-rw-r--r--   0 yuanzan    (501) staff       (20)       52 2023-05-18 01:26:56.000000 trackc-0.0.9/docs/references.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)        0 2023-05-17 07:21:56.000000 trackc-0.0.9/docs/releases.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      597 2023-05-23 02:00:50.000000 trackc-0.0.9/docs/requirements.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)     7789 2023-05-22 01:25:34.000000 trackc-0.0.9/docs/source
+-rw-r--r--   0 yuanzan    (501) staff       (20)      450 2023-05-17 15:35:14.000000 trackc-0.0.9/docs/trackc.pa.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)     1411 2023-05-17 15:35:14.000000 trackc-0.0.9/docs/trackc.pl.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      375 2023-05-17 15:35:14.000000 trackc-0.0.9/docs/trackc.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      150 2023-05-17 15:35:14.000000 trackc-0.0.9/docs/trackc.tl.rst
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.465857 trackc-0.0.9/docs/tutorials/
+-rw-r--r--   0 yuanzan    (501) staff       (20)  1358247 2023-05-30 00:44:19.000000 trackc-0.0.9/docs/tutorials/ENCFF041XLP.bedpe
+-rw-r--r--   0 yuanzan    (501) staff       (20)      386 2023-05-23 01:13:11.000000 trackc-0.0.9/docs/tutorials/README.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)   214570 2023-05-29 06:47:34.000000 trackc-0.0.9/docs/tutorials/Virtual4C.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)     4366 2023-06-11 11:27:50.000000 trackc-0.0.9/docs/tutorials/bed.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)    15450 2023-05-29 10:29:41.000000 trackc-0.0.9/docs/tutorials/bigwig.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)   708712 2023-05-23 01:13:11.000000 trackc-0.0.9/docs/tutorials/bw_track_tutorial.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)   411911 2023-05-23 01:13:11.000000 trackc-0.0.9/docs/tutorials/cmap-test-data.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)   292254 2023-06-03 05:05:29.000000 trackc-0.0.9/docs/tutorials/contactmap.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)   190781 2023-05-29 02:47:50.000000 trackc-0.0.9/docs/tutorials/datas.ipynb
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.473626 trackc-0.0.9/docs/tutorials/fileformats/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      427 2023-05-26 11:16:19.000000 trackc-0.0.9/docs/tutorials/fileformats/GRCh38.84.bed12
+-rw-r--r--   0 yuanzan    (501) staff       (20)      375 2023-05-26 11:16:36.000000 trackc-0.0.9/docs/tutorials/fileformats/GRCh38.84.gtf.bed12
+-rw-r--r--   0 yuanzan    (501) staff       (20)     1910 2023-05-27 13:15:20.000000 trackc-0.0.9/docs/tutorials/fileformats/bed12.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)      169 2023-06-01 01:14:22.000000 trackc-0.0.9/docs/tutorials/fileformats/mcool.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)    39757 2023-06-11 07:28:56.000000 trackc-0.0.9/docs/tutorials/gene.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)    40716 2023-05-27 06:49:51.000000 trackc-0.0.9/docs/tutorials/gene_track.pdf
+-rw-r--r--   0 yuanzan    (501) staff       (20)    40004 2023-06-11 07:52:28.000000 trackc-0.0.9/docs/tutorials/grid_spec.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)    30777 2023-05-31 08:23:43.000000 trackc-0.0.9/docs/tutorials/links.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)   526486 2023-05-23 01:13:11.000000 trackc-0.0.9/docs/tutorials/mapc_eg.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)    52779 2023-06-11 11:26:38.000000 trackc-0.0.9/docs/tutorials/mapc_markline.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)    37530 2023-06-11 10:45:07.000000 trackc-0.0.9/docs/tutorials/scalebar.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)     9394 2023-05-27 10:30:06.000000 trackc-0.0.9/docs/tutorials/trackc_scale.pdf
+-rw-r--r--   0 yuanzan    (501) staff       (20)    36245 2023-05-29 07:34:23.000000 trackc-0.0.9/docs/tutorials/zoomin.ipynb
+-rw-r--r--   0 yuanzan    (501) staff       (20)     3208 2023-06-11 12:23:26.000000 trackc-0.0.9/docs/tutorials.rst
+-rw-r--r--   0 yuanzan    (501) staff       (20)     1931 2023-05-19 09:33:48.000000 trackc-0.0.9/docs/utils.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)      112 2023-05-26 09:19:01.000000 trackc-0.0.9/pypi.sh
+-rw-r--r--   0 yuanzan    (501) staff       (20)       18 2023-01-09 05:16:57.000000 trackc-0.0.9/requirements.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)       38 2023-06-20 04:38:29.526419 trackc-0.0.9/setup.cfg
+-rw-r--r--   0 yuanzan    (501) staff       (20)     1258 2023-05-26 10:22:37.000000 trackc-0.0.9/setup.py
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.173150 trackc-0.0.9/src/
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.480007 trackc-0.0.9/src/trackc/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      551 2023-05-27 15:57:45.000000 trackc-0.0.9/src/trackc/__init__.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     2172 2023-05-19 09:43:28.000000 trackc-0.0.9/src/trackc/_utils.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     7415 2023-06-11 07:51:13.000000 trackc-0.0.9/src/trackc/gs.py
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.489750 trackc-0.0.9/src/trackc/pa/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      240 2023-06-11 11:25:24.000000 trackc-0.0.9/src/trackc/pa/__init__.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     2008 2023-06-11 11:23:52.000000 trackc-0.0.9/src/trackc/pa/cmaps.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     4362 2023-05-10 01:28:12.000000 trackc-0.0.9/src/trackc/pa/palettes.py
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.516857 trackc-0.0.9/src/trackc/pl/
+-rw-r--r--   0 yuanzan    (501) staff       (20)     7070 2023-05-31 16:04:18.000000 trackc-0.0.9/src/trackc/pl/Virtual4C.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)      813 2023-05-17 15:16:06.000000 trackc-0.0.9/src/trackc/pl/__init__.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)    11635 2023-06-04 09:25:33.000000 trackc-0.0.9/src/trackc/pl/bed.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     7720 2023-05-29 10:32:11.000000 trackc-0.0.9/src/trackc/pl/bigwig.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     8856 2023-06-11 07:28:04.000000 trackc-0.0.9/src/trackc/pl/gene.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     7721 2023-06-01 01:14:14.000000 trackc-0.0.9/src/trackc/pl/links.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)    17500 2023-06-01 07:57:57.000000 trackc-0.0.9/src/trackc/pl/mapc.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)    13594 2023-06-11 09:42:15.000000 trackc-0.0.9/src/trackc/pl/mapc_markline.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     2920 2023-05-29 03:23:29.000000 trackc-0.0.9/src/trackc/pl/mapc_xylim.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)    10471 2023-06-04 12:01:16.000000 trackc-0.0.9/src/trackc/pl/scale.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     4516 2023-05-29 10:17:44.000000 trackc-0.0.9/src/trackc/pl/zoomin.py
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.519347 trackc-0.0.9/src/trackc/scripts/
+-rw-r--r--   0 yuanzan    (501) staff       (20)        0 2023-05-26 09:03:49.000000 trackc-0.0.9/src/trackc/scripts/__init__.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     6207 2023-05-26 11:03:26.000000 trackc-0.0.9/src/trackc/scripts/gtf2bed12.py
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.523604 trackc-0.0.9/src/trackc/tl/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      126 2023-05-17 15:16:25.000000 trackc-0.0.9/src/trackc/tl/__init__.py
+-rw-r--r--   0 yuanzan    (501) staff       (20)     9962 2023-06-01 08:17:07.000000 trackc-0.0.9/src/trackc/tl/_getRegionsCmat.py
+drwxr-xr-x   0 yuanzan    (501) staff       (20)        0 2023-06-20 04:38:29.485426 trackc-0.0.9/src/trackc.egg-info/
+-rw-r--r--   0 yuanzan    (501) staff       (20)      378 2023-06-20 04:38:28.000000 trackc-0.0.9/src/trackc.egg-info/PKG-INFO
+-rw-r--r--   0 yuanzan    (501) staff       (20)     3108 2023-06-20 04:38:29.000000 trackc-0.0.9/src/trackc.egg-info/SOURCES.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)        1 2023-06-20 04:38:28.000000 trackc-0.0.9/src/trackc.egg-info/dependency_links.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)       18 2023-06-20 04:38:28.000000 trackc-0.0.9/src/trackc.egg-info/requires.txt
+-rw-r--r--   0 yuanzan    (501) staff       (20)        7 2023-06-20 04:38:28.000000 trackc-0.0.9/src/trackc.egg-info/top_level.txt
```

### Comparing `trackc-0.0.8/LICENSE` & `trackc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/README.rst` & `trackc-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/Makefile` & `trackc-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/_static/demo.png` & `trackc-0.0.9/docs/_static/demo.png`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/_static/plotly_logo.png` & `trackc-0.0.9/docs/_static/plotly_logo.png`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/_static/theme_override.css` & `trackc-0.0.9/docs/_static/theme_override.css`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/_templates/module.rst` & `trackc-0.0.9/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/api.rst` & `trackc-0.0.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/conf.py` & `trackc-0.0.9/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,34 +125,35 @@
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 
 # The theme is set by the make target
 
-project = 'TrackC'
+#project = 'TrackC'
 master_doc = 'index'
 html_theme = 'pydata_sphinx_theme'
 autosummary_generate = True
 html_show_sphinx =  False
 pygments_style = 'sphinx'
 highlight_language = 'python3'
 
 
 
 # bibliography
 bibtex_bibfiles = ["references.bib"]
 bibtex_reference_style = "author_year"
 bibtex_default_style = "alpha"
 
+"""
 nbsphinx_thumbnails = {
     'thumbnail_size': '400x300',
-    'examples/zoomin_heatmap': 'examples/zoomin_heatmap.png',
-    'tutorials/bw_track_tutorial': 'examples/zoomin_heatmap.png',
+    'examples/rearranged_interactions': 'examples/neotad.png',
 }
+"""
 
 def setup(app):
     """Sphinx setup function."""
     app.add_css_file('theme_override.css')
     app.add_object_type('confval', 'confval',
                         objname='configuration value',
                         indextemplate='pair: %s; configuration value')
@@ -164,15 +165,15 @@
 
 html_theme_options = {
     'navbar_center': ['navbar-nav'],
     'show_toc_level': 2,
     'show_nav_level': 2,
     #'navbar_end': ['theme-switcher', 'version-switcher', 'navbar-icon-links'],
     'logo': {
-        'text': 'TrackC',
+        'text': None,
     },
     #'switcher': dict(
     #    json_url='https://sphinx-gallery.github.io/dev/_static/switcher.json',
     #    version_match='dev' if 'dev' in version else 'stable',
     #),
     "github_url": "https://github.com/seqyuan/trackc",
     "icon_links": [
@@ -192,15 +193,15 @@
 #html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 #html_short_title = None
 
 # The name of an image file (relative to this directory) to place at the top
 # of the sidebar.
-#html_logo = None
+html_logo = 'images/trackc-low-resolution-logo-color-on-transparent-background.png'
 
 # The name of an image file (within the static path) to use as favicon of the
 # docs.  This file should be a Windows icon file (.ico) being 16x16 or 32x32
 # pixels large.
 #html_favicon = None
```

### Comparing `trackc-0.0.8/docs/custom-formats.pct.py` & `trackc-0.0.9/docs/custom-formats.pct.py`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/developer/about_us.rst` & `trackc-0.0.9/docs/developer/about_us.rst`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 TrackC was originally written by Zan Yuan, and has been developed with the help 
 of many others. Thanks to everyone who has improved TrackC by contributing code, 
 bug reports (and fixes), documentation, and input on design, features, and the future of TrackC.
 
 Contributors
 ------------
 
-If you are a NetworkX contributor, please feel free to
+If you are a TrackC contributor, please feel free to
 open an `issue <https://github.com/seqyuan/trackc/issues/new>`_ or
 submit a `pull request <https://github.com/seqyuan/trackc/compare/>`_
 to add your name to the bottom of the list.
 
 - Zan Yuan, GitHub: `seqyuan <https://github.com/seqyuan>`_
 - Jiaying Yao
 - Xinyu Tong
```

### Comparing `trackc-0.0.8/docs/developer/history.rst` & `trackc-0.0.9/docs/developer/history.rst`

 * *Files 4% similar despite different names*

```diff
@@ -11,11 +11,11 @@
 pcolormesh to implement the triangular heatmap instead of the original layered method from the Hi-C mode. 
 The implementation method for the triangular heatmap from HiTC was initially converted to Python by Lixiang Ma 
 one our team member.
 
 which project uses trackc
 -------------------------
 
-- PIBF1
+- https://doi.org/10.1016/j.jare.2023.04.015
 - pseudogene
 - zhongshan eye
-- muxu
+- muxu 3D genome
```

### Comparing `trackc-0.0.8/docs/examples/README.txt` & `trackc-0.0.9/docs/examples/README.txt`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/examples/bw_track_tutorial.ipynb` & `trackc-0.0.9/docs/examples/bw_track_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/examples/cmap-test-data.ipynb` & `trackc-0.0.9/docs/examples/cmap-test-data.ipynb`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/examples/mapc_eg.ipynb` & `trackc-0.0.9/docs/examples/mapc_eg.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9875595238095238%*

 * *Differences: {"'cells'": "{0: {'source': ['# Cis contact heatmap\\n', 'In this section, we demonstrate how to "*

 * *            "generate various types of Hi-C cis contact heatmaps'], delete: ['attachments']}, 4: "*

 * *            "{'source': {insert: [(0, 'fig, axs = tc.make_spec(figsize=(6, 8), "*

 * *            "height_ratios=[1,1,1,1,2,2,2], hspace=0.3)\\n')], delete: [0]}}, 6: {'source': "*

 * *            "{insert: [(0, 'fig, axs = tc.make_spec(figsize=(12,7), width_ratios=[1,1,1,1,2,2,2], "*

 * *            "wspace=0.6)\\n')], delete: […]*

```diff
@@ -1,24 +1,15 @@
 {
     "cells": [
         {
-            "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "# cis contact mapc examples"
-            ]
-        },
-        {
-            "attachments": {},
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": [
-                "blabla\n",
-                "## all mapc types"
+                "# Cis contact heatmap\n",
+                "In this section, we demonstrate how to generate various types of Hi-C cis contact heatmaps"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {},
             "outputs": [
@@ -109,15 +100,15 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "fig, axs = tc.make_spec(width=6, height=8, height_ratios=[1,1,1,1,2,2,2], hspace=0.3)\n",
+                "fig, axs = tc.make_spec(figsize=(6, 8), height_ratios=[1,1,1,1,2,2,2], hspace=0.3)\n",
                 "\n",
                 "tc.pl.mapC(ax=axs[0], mat=normal, label='triangle\\nmat', \n",
                 "           map_type='triangle',  height=50)\n",
                 "tc.pl.mapC(ax=axs[1], mat2=normal, label='triangle\\nmat2', \n",
                 "           map_type='triangle',  height=50)\n",
                 "\n",
                 "tc.pl.mapC(ax=axs[2], mat=tumor, label='rectangle\\nmat2', \n",
@@ -180,15 +171,15 @@
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 }
             ],
             "source": [
-                "fig, axs = tc.make_spec(width=12, height=7, width_ratios=[1,1,1,1,2,2,2], wspace=0.6)\n",
+                "fig, axs = tc.make_spec(figsize=(12,7), width_ratios=[1,1,1,1,2,2,2], wspace=0.6)\n",
                 "\n",
                 "\n",
                 "tc.pl.mapC(ax=axs[0], mat2=normal, label='triangle\\ntrans_ax=True\\nmat2', \n",
                 "           map_type='triangle',  height=50, trans_ax=True)\n",
                 "tc.pl.mapC(ax=axs[1], mat=normal, label='triangle\\ntrans_ax=True\\nmat', \n",
                 "           map_type='triangle',  height=50, trans_ax=True)\n",
                 "\n",
```

### Comparing `trackc-0.0.8/docs/examples/zoomin_heatmap.png` & `trackc-0.0.9/docs/examples/zoomin_heatmap.png`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/images/trackc_dynamic_2022.png` & `trackc-0.0.9/docs/images/trackc_dynamic_2022.png`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/images/tutorials/grid_spec_01.png` & `trackc-0.0.9/docs/images/tutorials/grid_spec_01.png`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/images/tutorials/zoomin_heatmap.png` & `trackc-0.0.9/docs/images/tutorials/zoomin_heatmap.png`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/index.rst` & `trackc-0.0.9/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,43 @@
 trackc - track view of chromosome conformation and multi-omics data
 ===================================================================
 
 **trackc** is a Python Package to Flexible Visualization of 3D Genome and Multiomics.
-It builds on top of `matplotlib`, from which it allow for flexible adjustments.
+It builds on top of `matplotlib`, from which it allows for flexible adjustments.
 
-
-.. image:: https://raw.githubusercontent.com/seqyuan/trackc/main/docs/images/trackc_logo.png
-    :alt: trackc title figure
-    :width: 100px
-    :align: center
-    :target: https://doi.org/1xxxx.1358-2
-
-Manuscript
-----------
-Please see our manuscript :cite:`Palla:22` in **Bioinformatics** to learn more.
-
-Trackc's key applications
+TrackC's key applications
 --------------------------
 - Mark the abnormal interaction formed by the structural variation of the genome.
 - Show the three-dimensional genome interaction and multi-omics data after rearrangement.
 - Flexible and convenient layout for multi-track 
 
 Getting started with trackc
 ----------------------------
-- Browse :doc:`quick start </quick_start>`, :doc:`available tracks types </available_track_types>` and :doc:`gallary </gallary>`.
-- Discuss usage on `discourse`_ and development on `github`_.
+- Browse :doc:`quick start </quick_start>`, :doc:`available tracks types </available_track_types>` and :doc:`gallery </gallery>`.
+
 
 Contributing to trackc
 -----------------------
-We are happy about any contributions! Before you start, check out our `contributing guide`_.
-
+We are happy about any contributions! Welcome to talk at github issue.
 
 .. toctree::
    :caption: General:
    :maxdepth: 1
 
-   quick_start
+   install
    tutorials
-   gallary
+   gallery
    api
    developer/index
    
 
 .. _github: https://github.com/seqyuan/trackc
 
 
-
 Citation
 ---------
 
 Please cite trackc as follows:
 
 Zan Yuan, Guoliang Li, Yang Chen.
-**trackc: a Package for Flexible Visualization of rearrangement 3D Genome and Multi-omics**, Bioinformatics, Volume 48, Issue W1, 1 July 2023, Pages W177–W184, https://doi.org/10.1093/nar/gkaa220
+**trackc: a Package for Flexible Visualization of rearrangement 3D Genome and Multi-omics**, xxx, Volume 48, Issue W1, 1 July 2023, Pages xxx, https://doi.org/xxx/xxx/xxx
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `trackc-0.0.8/docs/make.bat` & `trackc-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/references.bib` & `trackc-0.0.9/docs/references.bib`

 * *Files 10% similar despite different names*

```diff
@@ -60,7 +60,22 @@
 	journaltitle = {Nature},
 	shortjournal = {Nature},
 	author = {Xu, Jie and Song, Fan and Lyu, Huijue and Kobayashi, Mikoto and Zhang, Baozhen and Zhao, Ziyu and Hou, Ye and Wang, Xiaotao and Luan, Yu and Jia, Bei and Stasiak, Lena and Wong, Josiah Hiu-yuen and Wang, Qixuan and Jin, Qi and Jin, Qiushi and Fu, Yihao and Yang, Hongbo and Hardison, Ross C. and Dovat, Sinisa and Platanias, Leonidas C. and Diao, Yarui and Yang, Yue and Yamada, Tomoko and Viny, Aaron D. and Levine, Ross L. and Claxton, David and Broach, James. R. and Zheng, Hong and Yue, Feng},
 	urldate = {2022-11-01},
 	date = {2022-10-26},
 	langid = {english},
 }
+@article{xu_structural_2022,
+	title = {Structural variants drive context-dependent oncogene activation in cancer},
+	volume = {612},
+	issn = {0028-0836, 1476-4687},
+	url = {https://www.nature.com/articles/s41586-022-05504-4},
+	doi = {10.1038/s41586-022-05504-4},
+	pages = {564--572},
+	number = {7940},
+	journaltitle = {Nature},
+	shortjournal = {Nature},
+	author = {Xu, Zhichao and Lee, Dong-Sung and Chandran, Sahaana and Le, Victoria T. and Bump, Rosalind and Yasis, Jean and Dallarda, Sofia and Marcotte, Samantha and Clock, Benjamin and Haghani, Nicholas and Cho, Chae Yun and Akdemir, Kadir C. and Tyndale, Selene and Futreal, P. Andrew and {McVicker}, Graham and Wahl, Geoffrey M. and Dixon, Jesse R.},
+	urldate = {2023-01-05},
+	date = {2022-12-15},
+	langid = {english},
+}
```

### Comparing `trackc-0.0.8/docs/requirements.txt` & `trackc-0.0.9/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/source` & `trackc-0.0.9/docs/source`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/trackc.pl.rst` & `trackc-0.0.9/docs/trackc.pl.rst`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/tutorials/bw_track_tutorial.ipynb` & `trackc-0.0.9/docs/tutorials/bw_track_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/tutorials/cmap-test-data.ipynb` & `trackc-0.0.9/docs/tutorials/cmap-test-data.ipynb`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/tutorials/mapc_eg.ipynb` & `trackc-0.0.9/docs/tutorials/mapc_eg.ipynb`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/docs/utils.py` & `trackc-0.0.9/docs/utils.py`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/setup.py` & `trackc-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     scripts=['bin/gtf2bed4trackc'],
     #include_package_data=True,
     #package_dir={'trackc': 'src/trackc'},
     #package_data={'trackc': ['qc_template.html']},
     url='http://trackc.readthedocs.io',
     description="Track view of chromosome conformation and multi-omics data",
     #long_description=open('README.rst').read(),
-    long_description='x',
+    #long_description='x',
     #url="https://github.com/seqyuan/trackc",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `trackc-0.0.8/src/trackc/_utils.py` & `trackc-0.0.9/src/trackc/_utils.py`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/src/trackc/pa/cmaps.py` & `trackc-0.0.9/src/trackc/pa/cmaps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import seaborn as sns
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.cm import get_cmap
+from matplotlib.colors import ListedColormap, LinearSegmentedColormap
 
 def hex2rgb(value):
     # convert hex to rgb
     value = value.lstrip('#')
     lv = len(value)
     rgb = tuple(int(value[i:i + lv // 3], 16) for i in range(0, lv, lv // 3))
     return np.array([rgb[0]/255, rgb[1]/255, rgb[2]/255, 1])
@@ -40,14 +41,19 @@
     newcmap = ListedColormap(newcolors)
 
     return newcmap
 
 fruitpunch = sns.blend_palette(['white', 'red'], as_cmap=True)
 #fruitpunch2 = sns.blend_palette(['white', 'blue'], as_cmap=True)
 fruitpunch2 = sns.blend_palette(['white', 'purple'], as_cmap=True)
-
+washu = sns.blend_palette(['white', '#B9378A'], as_cmap=True)
+fruitpunch3 = LinearSegmentedColormap.from_list('fruitpunch3', 
+                                             [(0, 'white'),
+                                              (0.03, 'w'),
+                                              (0.4, 'r'),
+                                              (1, '#CF3F35')], N=100)
 
 
 
 
 #-----------------------------------------------------------------
```

### Comparing `trackc-0.0.8/src/trackc/pa/palettes.py` & `trackc-0.0.9/src/trackc/pa/palettes.py`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/src/trackc/pl/__init__.py` & `trackc-0.0.9/src/trackc/pl/__init__.py`

 * *Files identical despite different names*

### Comparing `trackc-0.0.8/src/trackc/pl/bed.py` & `trackc-0.0.9/src/trackc/pl/bed.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,62 +7,69 @@
 from matplotlib import cm
 import pandas as pd
 import numpy as np
 from trackc.tl._getRegionsCmat import GenomeRegion
 from .bigwig import _make_multi_region_ax
 
 def bed_track(ax: Optional[Axes] = None,
-              bed: pd.DataFrame = None,
+              bed: Union[pd.DataFrame, str, None]  = None,
               regions: Union[Sequence[str], str, None] = None,
               track_style: Union[str, None] = 'bar',
               color: Union[Sequence[str], None] = 'tab:blue',
-              cmap: Union[Sequence[Colormap], str, None] = None,
+              cmap: Union[Colormap, str, None] = None,
               intervals: Union[int, None] = 1,
               #show_names: Union[bool, None] = False,
               alpha: Union[float, None] = 1,
               label: Union[str, None] = None,
-              label_fontsize: Union[int, None] = 5,
+              label_fontsize: Union[int, None] = 12,
               label_rotation: Union[int, None] = 0,
               ymin: Optional[float] = None,
               ymax: Optional[float] = None,
               tick_fontsize: Optional[int] = 8,
               tick_fl: Optional[str] ='%0.2f',
               score_label_size: Union[int, None] = 7,
               ):
-    """
+    """\
+    Plot bed track, support for multiple or reverse genome regions.
+    support bed3 and bed5, the fields after the column5 will be ignored, 
+        should be sorted py chromStart if ``track_style`` is `line`
+
     Parameters
     ----------
-    bed
-        ``pd.DataFrame``: 6th columns dataframe
-            should be sorted py chromStart if track_style is line
-            column1: chrom
-                The name of the chromosome (e.g. chr3, chrY, chr2_random) or scaffold (e.g. scaffold10671).
-            column2: chromStart
-                The starting position of the feature in the chromosome or scaffold. The first base in a chromosome is numbered 0.
-            column3: chromEnd
-                The ending position of the feature in the chromosome or scaffold.
-            column4: name
-                Defines the name of the BED line. Either "." (=no name), or other string
-            column5: score
-                Defines the name of the BED line. if nessasary, can be set as ``.``,
-                if track_type/style is one of bar/line/heatmap 
-            column6: strand 
-                Defines the strand. Either "." (=no strand) or "+" or "-".
-    track_style
-        ``str``: bed blocks style, 
-            line
-            bar
-            heatmap
-            triangle
-            rec
-                rectangle
-            arrow
-            
-    color
-        ``str`` or list: the color of line/triangle/rectangle, if color is color list, the block will 
+    ax: :class:`matplotlib.axes.Axes` object
+    bed: `pd.DataFrame` | `str`
+        If ``bed`` if a filepath, the file should have no headers
+        Here is bed formats:
+        column1: chrom
+            The name of the chromosome (e.g. chr3, chrY, chr2_random) or scaffold (e.g. scaffold10671).
+        column2: chromStart
+            The starting position of the feature in the chromosome or scaffold. The first base in a chromosome is numbered 0.
+        column3: chromEnd
+            The ending position of the feature in the chromosome or scaffold.
+        column4: name
+            Defines the name of the BED line. Either "." (=no name), or other string
+        column5: score
+            Defines the name of the BED line. if nessasary, can be set as ``.``,
+            if track_type/style is one of bar/line
+        column6: strand 
+            Defines the strand. Either "." (=no strand) or "+" or "-".
+    regions: `str` | `str list`
+        The genome regions to plot
+        e.g. ``"chr6:1000000-2000000"`` or ``["chr6:1000000-2000000", "chr3:5000000-4000000"]``
+        The start can be larger than the end (eg. ``"chr6:2000000-1000000"``), 
+            which means you want to get the reverse region
+    track_style: `str`
+        bed blocks style,  opions in ['line', 'bar', 'triangle', 'rec']
+    color: `str` or `list`
+        the color of line/triangle/rectangle, if color is color list, the block will set by regions
+    cmap: `str` | `matplotlib.colors.Colormap`
+        the colormap of the plot except track_style:line
+    intervals: 
+
+
     intervals
         ``int``: if track_style is one of [triangle, rec], the row number distribution for triangle/rectangle blocks
     """
     if isinstance(regions, list):
         line_GenomeRegions = pd.concat([GenomeRegion(i).GenomeRegion2df() for i in regions])
     else:
         line_GenomeRegions = GenomeRegion(regions).GenomeRegion2df()
@@ -97,59 +104,65 @@
         bed.columns = ['chrom', 'start', 'end', 'name']
     if bed.shape[1] == 5:
         score_label = bed.columns[4]
         bed.columns = ['chrom', 'start', 'end', 'name', 'score']
     if bed.shape[1] == 6:
         score_label = bed.columns[4]
         bed.columns = ['chrom', 'start', 'end', 'name', 'score', 'strand']
+    bed['chrom'] = bed['chrom'].astype(str)
 
     min_y = None
     max_y = None
     max_len = 0
+    
     for ix, row in line_GenomeRegions.iterrows(): 
         bed2plot = bed[(bed['chrom']==row['chrom']) & (bed['end']>=row['fetch_start']) & (bed['start']<=row['fetch_end'])]
         if track_style in ['line', 'bar'] or bed.shape[1]>=5:
             if min_y==None:
-                min_y = bed2plot['score'].min()
+                min_y = bed2plot['score'].min(skipna=True, numeric_only=True)
             else:
-                if min_y < bed2plot['score'].min():
-                    min_y = bed2plot['score'].min()
+                if min_y < bed2plot['score'].min(skipna=True, numeric_only=True):
+                    min_y = bed2plot['score'].min(skipna=True, numeric_only=True)
         
             if max_y==None:
-                max_y = bed2plot['score'].max()
+                max_y = bed2plot['score'].max(skipna=True, numeric_only=True)
             else:
-                if max_y > bed2plot['score'].max():
-                    max_y = bed2plot['score'].max()
+                if max_y > bed2plot['score'].max(skipna=True, numeric_only=True):
+                    max_y = bed2plot['score'].max(skipna=True, numeric_only=True)
 
-        maxlength = (bed2plot['end']-bed2plot['start']).max()
+        maxlength = (bed2plot['end']-bed2plot['start']).max(skipna=True, numeric_only=True)
         if max_len < maxlength:
             max_len = maxlength
 
     if ymin == None:
         ymin = min_y
     if ymax == None:
         ymax = max_y
 
+    
     for ix, row in line_GenomeRegions.iterrows(): 
         bed2plot = bed[(bed['chrom']==row['chrom']) & (bed['end']>=row['fetch_start']) & (bed['start']<=row['fetch_end'])].copy()
+        if bed2plot.shape[0] == 0:
+            continue
         if track_style == "line":
-            plot_bed_bar_l(axs[ix], bed2plot, row['fetch_start'], row['fetch_end'], needReverse=row['isReverse'], style='line', color=color[ix], alpha=alpha)    
+            _plot_bed_bar_l(axs[ix], bed2plot, row['fetch_start'], row['fetch_end'], needReverse=row['isReverse'], style='line', color=color[ix], alpha=alpha)    
         if track_style == "bar":
             _plot_bed_bar_l(axs[ix], bed2plot, row['fetch_start'], row['fetch_end'], needReverse=row['isReverse'], style='bar', color=color[ix], alpha=alpha)
         if track_style == "rec":
             _plot_bed_rec(ax, axs[ix], bed2plot, row['fetch_start'], row['fetch_end'], 
                          needReverse=row['isReverse'], color=color[ix], cname=cmap[ix], 
                          alpha=alpha, min=ymin, max=ymax, score_label=score_label, intervals=intervals, score_label_size=score_label_size)
         if track_style == "triangle":
             _plot_bed_tri(ax, axs[ix], bed2plot, row['fetch_start'], row['fetch_end'], 
                          needReverse=row['isReverse'], color=color[ix], cname=cmap[ix], 
                          alpha=alpha, min=ymin, max=ymax, score_label=score_label, score_label_size=score_label_size)
             
             axs[ix].set_ylim(0, max_len/2)
 
+
     if track_style in ['line', 'bar']:
         for axi in axs:
             axi.set_ylim(ymin, ymax)
         ax.set_ylim(ymin, ymax)
         ax.text(0, ymax, " [{0}, {1}]".format(tick_fl % ymin, tick_fl % ymax), va='top', fontsize=tick_fontsize)
 
 
@@ -254,9 +267,7 @@
         ax.spines[i].set_color('none')
         ax.spines[i].set_linewidth(0)
     ax.spines["bottom"].set_color('black')
     ax.spines["bottom"].set_linewidth(1)
     #ax.tick_params(bottom =True,top=False,left=False,right=False)
     #ax.set_xticklabels("")
     #ax.set_yticklabels("")
-
-
```

### Comparing `trackc-0.0.8/src/trackc/pl/bigwig.py` & `trackc-0.0.9/src/trackc/pl/bigwig.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from matplotlib.axes import Axes
 #import pyBigWig
 from typing import Union, Optional, Sequence, Any, Mapping, List, Tuple, Callable
 import pandas as pd
 from trackc.tl._getRegionsCmat import GenomeRegion
+import numpy as np
 
 def _make_multi_region_ax(ax, lineGenomeRegions):
     lineGenomeRegions['len'] = lineGenomeRegions['fetch_end']-lineGenomeRegions['fetch_start']
     lineGenomeRegions['ax_ratio'] = lineGenomeRegions['len']/lineGenomeRegions['len'].sum()
     lineGenomeRegions['ax_x'] = lineGenomeRegions['ax_ratio'].cumsum(axis=0) - lineGenomeRegions['ax_ratio']
     axs = [ax.inset_axes([row['ax_x'], 0, row['ax_ratio'], 1]) for i, row in lineGenomeRegions.iterrows()]
     for axi in axs:
@@ -14,49 +15,79 @@
     
     return axs
 
 def bw_track(bw,
              ax: Optional[Axes] = None,
              regions: Union[Sequence[str], str, None] = None, 
              binsize: Optional[int] = 50000,
-             averagetype: Union[str, None] = 'mean',
-             ymin: Optional[float] = None,
-             ymax: Optional[float] = None,
+             summary_type: Union[str, None] = 'mean',
+             minrange: Optional[float] = None,
+             maxrange: Optional[float] = None,
              color: Union[Sequence[str], None] = '#827DBB',
              invert_y: Optional[bool] = False,
              label: Optional[str] = None,
              label_rotation: Union[int, None] = 0,
              label_fontsize: Optional[int] = 12,
              tick_fontsize: Optional[int] = 8,
-             tick_fl: Optional[str] ='%0.2f', 
+             tick_fl: Optional[str] = '%0.2f', 
+             ax_on: bool = False,
             ):
     """\
-    Plot multi-regions bigwig signal tracks.
+    Plot bigwig signal track, support for multiple or reverse genome regions.
     
     Parameters
     ----------
-    ax 
-        ``cooler.Cooler``: cool format Hi-C matrix (https://github.com/open2c/cooler)
-    ylabel
-        ``str``: The ``'balance'`` parameters of ``coolMat.matrix(balance=False).fetch('chr6:119940450-123940450')``
-    regions: bool, optional
-        Force balancing weights to be interpreted as divisive (True) or
-        multiplicativ
-
-    binsize
-        ``chrom region`` list: or ``chrom region`` or None. 
-        The subset matrix row genome regions
-        eg. ``"chr6:1000000-2000000"``, eg. ``["chr6:1000000-2000000", "chr3:5000000-4000000", "chr5"]``
+    bw: `pyBigWig.open` query object
+    ax: :class:`matplotlib.axes.Axes` object
+    regions: `str` | `str list`
+        The genome regions to show the signal.
+        e.g. ``"chr6:1000000-2000000"`` or ``["chr6:1000000-2000000", "chr3:5000000-4000000", "chr5"]``
         The start can be larger than the end (eg. ``"chr6:2000000-1000000"``), 
-            which means you want to get the reverse region contact matrix
-
-    averagetype
-        ``chrom region`` list: or ``chrom region`` or None. 
-        The subset matrix col genome regions, default is ``None``, which means the sample region as ``row_regions``
+            which means the reverse region
+    binsize: `int`
+        binsize divided to computing signal summary statistics
+    summary_type: `str`
+        Summary type (mean, min, max, coverage, std), default 'mean'.
+    minrange: `float`
+        the minimum range of values used to define the ylim
+    maxrange: `float`
+        the maximum range of values used to define the ylim
+    color: `str`
+        the signal bar color
+    invert_y: `bool`
+        whether reverse the y-axis
+    label: `str`
+        the title of the track, will show on the left
+    label_rotation: `int`
+        the label text rotation
+    label_fontsize: `int`
+        the label text fontsize
+    tick_fontsize: `int`
+        values range ticks text fontsize
+    tick_fl: `str`  
+        values range ticks retains a few decimal places
+    ax_on: `bool`
+        whether show the spines
+
+    Example
+    -------
+    >>> import trackc as tc
+    >>> import pyBigWig
+    >>> H3K27ac = pyBigWig.open('./GSM4604189.bigwig')
+    
+    >>> ten = tc.tenon(width=8, height=1)
+    >>> ten.add(pos='bottom', height=1, hspace=0.1)
+    >>> ten.add(pos='bottom', height=1, hspace=0.2)
+
+    >>> regions = ['chr8:127000000-129200000', 'chr14:96500000-99300000']
+    >>> tc.pl.bw_track(H3K27ac, ten.axs(0), regions=regions, maxrange=20, label='H3K27ac', binsize=10000, color='tab:blue')
+    >>> tc.pl.bw_track(H3K27ac, ten.axs(1), regions=regions, maxrange=5, label='H3K27ac', binsize=10000, invert_y=True, ax_on=True)
+    >>> tc.savefig('trackc_bigwig_track.pdf')
     """
+    
     if isinstance(regions, list):
         line_GenomeRegions = pd.concat([GenomeRegion(i).GenomeRegion2df() for i in regions])
     else:
         line_GenomeRegions = GenomeRegion(regions).GenomeRegion2df()
 
     axs = _make_multi_region_ax(ax, line_GenomeRegions)
     line_GenomeRegions = line_GenomeRegions.reset_index()
@@ -68,15 +99,15 @@
         color = (color * repeat_times)[:line_GenomeRegions.shape[0]]
     
     min_y = 0
     max_y = 0
     
     for i, row in line_GenomeRegions.iterrows():    
         bins = int(row['len']/binsize)
-        plot_list = bw.stats(row['chrom'], row['fetch_start'], row['fetch_end'], type=averagetype, nBins=bins)
+        plot_list = bw.stats(row['chrom'], row['fetch_start'], row['fetch_end'], type=summary_type, nBins=bins)
         plot_list = [0 if v is None else v  for v in plot_list]
 
         axs[i].bar(x=range(0, bins), height=plot_list, width=1, bottom=[0]*(bins),color=color[i],align="edge",edgecolor=color[i])    
         
         right, left = bins, 0
         if row['isReverse'] == True:
             left, right = bins, 0
@@ -84,43 +115,44 @@
         
         if min_y < min(plot_list):
             min_y = min(plot_list)
             
         if max_y < max(plot_list):
             max_y = max(plot_list)
         
-    if ymin == None:
-        ymin = min_y
-    if ymax == None:
-        ymax = max_y
+    if minrange == None:
+        minrange = min_y
+    if maxrange == None:
+        maxrange = max_y
         
-    if invert_y == True:
-        ymin = max_y
-        ymax = min_y
-
     for axi in axs:
-        axi.set_ylim(ymin, ymax)
-        
-    ax.set_ylim(ymin, ymax)
-    
+        if invert_y:
+            axi.set_ylim(maxrange, minrange)
+        else:
+            axi.set_ylim(minrange, maxrange)
     va = 'top'
-    if invert_y == True:
+    if invert_y:
         va='bottom'
-    ax.text(0, ymax, " [{0}, {1}]".format(tick_fl % min_y, tick_fl % ymax), verticalalignment=va, fontsize=tick_fontsize)
+        ax.set_ylim(maxrange, minrange)
+    else:
+        ax.set_ylim(minrange, maxrange)
+     
+    ax.text(0, maxrange, " [{0}, {1}]".format(tick_fl % minrange, tick_fl % maxrange), verticalalignment=va, fontsize=tick_fontsize)
     
     ax.set_ylabel(label, fontsize=label_fontsize, rotation=label_rotation, 
                   horizontalalignment='right', verticalalignment='center')
      
-    spines = ['top', 'bottom', 'left', 'right']
-    if invert_y == True:
-        del spines[0]
-    else:
-        del spines[1]
-    for i in spines:
-        ax.spines[i].set_visible(False)
+    if ax_on == False:
+        spines = ['top', 'bottom', 'left', 'right']
+        if invert_y == True:
+            del spines[0]
+        else:
+            del spines[1]
+        for i in spines:
+            ax.spines[i].set_visible(False)
     ax.set_xticks([])
     ax.set_xticklabels('')
     ax.set_yticks([])
     ax.set_yticklabels('')
     
 def bw_compartment(compartment_bw, ax, chrom, start, end, ylabel, xticklabel=False, Acolor="#3271B2", Bcolor="#FBD23C", binsize=100000):
     chrsize = compartment_bw.chroms()[chrom]
```

### Comparing `trackc-0.0.8/src/trackc/pl/links.py` & `trackc-0.0.9/src/trackc/pl/links.py`

 * *Files 19% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     for i in range(dots_num):
         x = x_dots12[i] + (x_dots23[i]-x_dots12[i])*i / (dots_num-1)
         y = y_dots12[i] + (y_dots23[i]-y_dots12[i])*i / (dots_num-1)
         xt.append(x)
         yt.append(y)
     return (xt, yt)
 
-def _plot_loop(ax, loop_df, color, max_extend, invert_y, start, end, left_anchor, right_anchor):
+def _plot_loop_arc(ax, loop_df, color, max_extend, invert_y, start, end, left_anchor, right_anchor):
     if loop_df.shape[0] == 0:
         return
     
     top_y = 0
 
     for i, row in loop_df.iterrows():
         top = row['length']/max_extend
@@ -48,59 +48,84 @@
             
     ax.set_xlim(start, end)
     if invert_y==True:
         ax.set_ylim(0.5, 0)
     else:
         ax.set_ylim(0, 0.5)
 
+
+
 def links_track(
         ax: Optional[Axes] = None,
-        links_df: pd.DataFrame = None, 
+        data: pd.DataFrame = None, 
         regions: Union[Sequence[str], str, None] = None,
-        links_type: Union[str, None] = 'loop',
+        links_type: Union[str, None] = 'arc',
         color: Union[Sequence[str], None] = '#66AC84',
         maxrange: Union[int, None] = 3000000,
         invert_y: Optional[bool] = False,
         anchor: Union[str, None] = 'inside',
-
         label: Optional[str] = None,
         label_rotation: Union[int, None] = 0,
         label_fontsize: Optional[int] = 12,
+        ax_on: bool = False,
         ):
     """\
-    Plot multi-regions loop or TAD links.
+    Plot loop arc, support for multiple or reverse genome regions.
     
     Parameters
     ----------
-    loop_bed
-        ``pd.DataFrame``: the file format for links is (tab separated), column names:
-            chr1 x1 x2 chr2 y1 y2 (score ...)
-        The score field is optional
-        The fields after the y2 score will be ignored, score column is useless right now
-        for example:
-            chr1 100 200 chr1 250 300 1
-
-    ax 
-        ``cooler.Cooler``: cool format Hi-C matrix (https://github.com/open2c/cooler)
-    ylabel
-        ``str``: The ``'balance'`` parameters of ``coolMat.matrix(balance=False).fetch('chr6:119940450-123940450')``
-    regions:
-        bool, optional
-        Force balancing weights to be interpreted as divisive (True) or
-        multiplicativ
-    links_type: 
-        ``str``: links type, either 'loop' or 'triangle'
-    
-    
-    anchor:
-        ``str``: links type, either 'loop' or 'triangle'
-            the link coordinates type for loop and triangle, by default: inside
-                inside: link x2 and y1
-                mid: link the middle of x1 and x2 and the middle of y1 and y2, (x1+x2)/2 and (y1+y2)/2
-                outside: link x1 and y2
+    ax: :class:`matplotlib.axes.Axes` object
+    data: `pd.DataFrame`
+        the file format expected is like this:
+        chr1 x1 x2 chr2 y1 y2
+        the fields after the y2 will be ignored,
+        recommend the result of juicer loop calling
+    regions: `str` | `str list`
+        The genome regions to show the arc.
+        e.g. ``"chr6:1000000-2000000"`` or ``["chr6:1000000-2000000", "chr3:5000000-4000000", "chr5"]``
+        The start can be larger than the end (eg. ``"chr6:2000000-1000000"``), 
+            which means the reverse region
+    links_type: `str`
+        Optional is ['arc']
+    color: `str` or `str list`
+        the color of the arc links, if multiple regions, color para can  set as list
+    maxrange: `int`
+        The maximum distance between two anchor of loop, to filter loops
+        if value is None, all loop will bed plotted 
+    invert_y: `bool`
+        whether reverse the y-axis
+    anchor: `str`
+        Optional is ['inside', 'outside']
+        inside: arc link x2 y1
+        outside: arc link x2 y1
+    label: `str`
+        the title of the track, will show on the left
+    label_rotation: `int`
+        the label text rotation
+    label_fontsize: `int`
+        the label text fontsize
+    ax_on: `bool`
+        whether show the spines
+        
+    Example
+    -------
+    >>> import trackc as tc
+    >>> regions = ['chr7:153000000-151000000', 'chr11:118500000-116500000']
+
+    >>> ten = tc.tenon(width=8, height=1)
+    >>> ten.add(pos='bottom', height=1)
+    >>> ten.add(pos='bottom', height=1, hspace=0.1)
+    >>> ten.add(pos='bottom', height=0.4, hspace=0.1)
+
+    >>> tc.pl.links_track(ax=ten.axs(0), data=loops, label='GM12878', regions=regions, 
+                color=['#66AC84', 'tab:purple'], maxrange=3000000, anchor='inside')
+    >>> tc.pl.links_track(ax=ten.axs(1), data=loops, label='GM12878', regions=regions, 
+                color='tab:purple', invert_y=True, anchor='outside', ax_on=True)
+    >>> tc.pl.multi_scale_track(ten.axs(2), regions=regions, scale_adjust='Mb', intervals=1, tick_rotation=0, tick_fontsize=10, colors=['#66AC84', 'tab:purple'])
+    >>> tc.savefig('trackc_links_track.pdf')
     """
 
     if isinstance(regions, list):
         line_GenomeRegions = pd.concat([GenomeRegion(i).GenomeRegion2df() for i in regions])
     else:
         line_GenomeRegions = GenomeRegion(regions).GenomeRegion2df()
 
@@ -109,44 +134,47 @@
 
     if isinstance(color, list)==False:
         color = [color]
     if len(color) < line_GenomeRegions.shape[0]:
         repeat_times = (line_GenomeRegions.shape[0] + len(color) - 1) // len(color)
         color = (color * repeat_times)[:line_GenomeRegions.shape[0]]
     
+    data = data.iloc[:,[0,1,2,3,4,5]]
+    data.columns = ['chr1', 'x1', 'x2', 'chr2', 'y1', 'y2']
+
     if anchor == "mid":
         left_anchor = 'left_mid'
         right_anchor = 'right_mid'
 
     if anchor == "inside":
         left_anchor = 'x2'
         right_anchor = 'y1'
     if anchor == "outside":
         left_anchor = 'x1'
         right_anchor = 'y2'
 
     max_extend = 0
     links_df_list = []
 
-    links_df = links_df[['chr1', 'x1', 'x2', 'chr2', 'y1', 'y2']]
-    links_df['chr1'] = links_df['chr1'].astype(str)
-    links_df['chr2'] = links_df['chr2'].astype(str)
+    data['chr1'] = data['chr1'].astype(str)
+    data['chr2'] = data['chr2'].astype(str)
 
     for ix, row in line_GenomeRegions.iterrows(): 
-        loop_bed_plot = links_df[links_df['chr1']==row['chrom']]
+        loop_bed_plot = data[data['chr1']==row['chrom']]
         
 
         loop_bed_plot['length'] = loop_bed_plot["y2"] - loop_bed_plot["x1"]
         
         loop_bed_plot = loop_bed_plot[((loop_bed_plot['x1'] >= row['fetch_start']) & (loop_bed_plot['x1'] <= row['fetch_end'])) | \
                                 ((loop_bed_plot['x2'] >= row['fetch_start']) & (loop_bed_plot['x2'] <= row['fetch_end']) |\
                                 (loop_bed_plot['y1'] >= row['fetch_start']) & (loop_bed_plot['y1'] <= row['fetch_end'])) | \
                                     ((loop_bed_plot['y2'] >= row['fetch_start']) & (loop_bed_plot['y2'] <= row['fetch_end']))]
-
-        loop_bed_plot = loop_bed_plot[(loop_bed_plot["y2"] - loop_bed_plot["x1"])<maxrange] 
+        
+        if isinstance(maxrange, int):
+            loop_bed_plot = loop_bed_plot[(loop_bed_plot["y2"] - loop_bed_plot["x1"])<maxrange] 
         #print('looop num:', loop_bed_plot.shape)
         if loop_bed_plot.shape[0] == 0:
             #for i in ['top', 'right', "left", "bottom"]:
             #    ax.spines[i].set_color('none')
             #    ax.spines[i].set_linewidth(0)
             next
 
@@ -155,27 +183,30 @@
 
         links_df_list.append(loop_bed_plot)
         if loop_bed_plot.shape[0] >0:
             if max_extend < max(loop_bed_plot['length']):
                 max_extend = max(loop_bed_plot['length'])
    
     for ix, row in line_GenomeRegions.iterrows(): 
-        if links_type == 'loop':
-            _plot_loop(axs[ix], links_df_list[ix], color[ix], max_extend, invert_y, row['start'], row['end'], left_anchor, right_anchor)
+        if links_type == 'arc':
+            _plot_loop_arc(axs[ix], links_df_list[ix], color[ix], max_extend, invert_y, row['start'], row['end'], left_anchor, right_anchor)
         #if links_type == 'loop':
             #plot_triangle()
 
     ax.set_ylabel(label, fontsize=label_fontsize, rotation=label_rotation, 
                   horizontalalignment='right',verticalalignment='center')
     
-    spines = ['top', 'bottom', 'left', 'right']
-    if invert_y == True:
-        del spines[0]
-    else:
-        del spines[1]
-    for i in spines:
-        ax.spines[i].set_visible(False)
+    
+    if ax_on == False:
+        spines = ['top', 'bottom', 'left', 'right']
+        if invert_y == True:
+            del spines[0]
+        else:
+            del spines[1]
+        for i in spines:
+            ax.spines[i].set_visible(False)
+
     ax.set_xticks([])
     ax.set_xticklabels('')
     ax.set_yticks([])
     ax.set_yticklabels('')
```

### Comparing `trackc-0.0.8/src/trackc/pl/mapc.py` & `trackc-0.0.9/src/trackc/pl/mapc.py`

 * *Files 23% similar despite different names*

```diff
@@ -270,46 +270,91 @@
         label: Union[Sequence[str], str, None] = None,
         label_fontsize: Union[Sequence[int], int] = 10,
         label_color: Union[Sequence[str], str, None] = 'k',
         
         logdata: Union[Sequence[bool], bool] = False, 
         maxrange: Union[Sequence[float], float]=None,
         minrange: Union[Sequence[float], float]=None,
-        trim_range: Union[Sequence[float], float]=0.99,
+        trim_range: Union[Sequence[float], float]=0.98,
         
         map_type: Union[str, None] = 'triangle',
         height: int = 0,
         trans_ax: bool = False,
         symmetric: bool = False,
         ax_on: bool =True,
         aspect: Union[str, float]='auto'
         ):
     """\
-    Draw triangle view of the C data
-
+    Plot contact map, support for multiple or reverse genome regions.
+    This function implements the plot method for `np.ndarray`,
+    which could get from trackc.tl.extractCisContact or trackc.tl.extractContactRegions
+    By default, the trim_range value is fixed so that the 98th percentile (resp. 2th percentile) of each
+    interaction matrix is discarded. It therefore allow to remove the extreme values from the matrix,  
+    mat or mat2 is plotted independently
+    If the maxrange parameter is set, data higher that this threshold will be fixed to the maxrange value.
+    
+    cmap, label, label_fontsize, label_color, logdata, minrange, maxrange, trim_range, those parameters can be set as a list, 
+    mat and mat2 will set to the first two values. If those parameters are one single value or the length of list is one,
+    then mat and mat2 both set the same value
+   
     Parameters
-    mat:
-
-    cmap
-    map_type
-        contact heatmap type, can be one of ``['square', 'triangle', 'rectangle']``,
-        if select ``rectangle`` the ``mapHeight`` parameter should be set.
-    mapHeight: int or None
-        Parameter for ``map_type: rectangle'``, ``map_type: triangle'`` also can be set.
-        it means the heapmap hight bin number
-    symmetric: bool
-        If there is one of ``mat`` and ``mat2`` para is None, 
-        value ``True`` means the  symmetric heatmap
-    aspect: 'auto' or 1
+    ----------
+    ax: :class:`matplotlib.axes.Axes` object
+    mat: `np.ndarray`
+        matrix for plot upper or right of heatmap
+    mat2: `np.ndarray`
+        matrix for plot bottom or left of heatmap
+    cmap: `str` | `matplotlib.colors.Colormap` | `list`
+        colormap for continuous annotations, if set as list, mat and mat2 will set to the first two values
+    label: `str`
+        the title of the track, will show on the left
+    label_fontsize: `int`
+        the label text fontsize
+    label_color: `int`
+        the label text color
+    logdata: `bool` | `bool list`
+        do you want to log the data before plotting the heatmap
+    minrange: `float` | `float list`
+        the minimum range of values used to define the color palette
+    maxrange: `float` | `float list` 
+        the maximum range of values used to define the color palette
+    trim_range: `float` | `float list` 
+        remove the extreme values by trimming the counts.[0,1]
+        define the maxrange and minrange values using the percentile of the interaction matrix
+    map_type: `str`
+        optional is ['square', 'triangle', 'rectangle'], default is square
+        triangle and rectangle default is flip the image 45 degrees to the left.
+        for rectangle type, the corresponding length of ``height`` will be truncated 
+        from both ends of the input matrix.
+    height: `int`
+        if map_type is one of ['triangle', 'rectangle'], `height` indicates the longest interaction bin interval you want to show
+    trans_ax: `bool`
+        whether flip the image 45 degrees to the right
+    symmetric: `bool`
+        whether to display a symmetrical heatmap when only one of mat and mat2 is set
+    ax_on: `bool`
+        whether show the spines
+    aspect: `str` | `float`
+        optional is 'auto' or 1
+        length-width ratio of heatmap
+    
+    Example
+    -------
+    >>> import trackc as tc
+    >>> import cooler
+    >>> BxPC3 = cooler.Cooler('./BxPC3.chr18.mcool::/resolutions/25000')
+    >>> neo_domain_regions = ['18:47950000-48280000', '18:75280000-74850000']
+    >>> tumor_zoom = tc.tl.extractContactRegions(clr=BxPC3, row_regions=neo_domain_regions)
+    >>> ten = tc.tenon(width=6, height=1)
+    >>> ten.add(pos='bottom', height=0.7, hspace=0.05)
+    >>> tc.pl.mapC(ax=ten.axs(0), mat=tumor_zoom.cmat, map_type='triangle',
+            maxrange=200, minrange=10, label='tumor res=25k', ax_on=False, height=40)
+    >>> tc.savefig('trackc_mapc.pdf')
     """
 
-    #cmap = copy(get_cmap(cmap))
-    #cmap.set_bad(na_color)
-    #cmap2 = copy(get_cmap(cmap2))
-    #cmap2.set_bad(na_color)
     cmap = _paraPair(cmap)
     label = _paraPair(label)
     label_fontsize = _paraPair(label_fontsize)
     label_color = _paraPair(label_color)
     logdata = _paraPair(logdata)
     maxrange = _paraPair(maxrange)
     minrange = _paraPair(minrange)
@@ -408,28 +453,27 @@
         _mapC_label(ax2, label[1], trans_ax, 1, map_type, height, fontsize=label_fontsize[1], color=label_color[1], Pair_mat=Pair_mat)
 
 def set_xylim(axs, conf, map_type, map_order, symmetric, trans_ax, pair_mat, matx, height):
     conf = conf[(conf['map_type']==map_type) & (conf['map_order']==map_order) & (conf['symmetric']==symmetric) & (conf['trans_ax']==trans_ax) & (conf['pair_mat']==pair_mat)]
     if height == 0:
         height = matx.shape[0]
     
-    conf_values = {'mat_w': matx.shape[0], 'mat_h': matx.shape[1], 'height': height, 'height_m': -height, 
-                   'mat_w_height': matx.shape[0]-height, '0':0}
+    conf_values = {'mat_w': matx.shape[1], 'mat_h': matx.shape[0], 'height': height, 'height_m': -height, 
+                   'mat_w_height': matx.shape[1]-height, '0':0, '-0.5':-0.5, 'mat_w_0.5m':matx.shape[1]-0.5, 'mat_h_0.5m':matx.shape[0]-0.5}
     
     if conf.shape[0] == 0:
         print('type not set xylim')
     else:
         ix = conf.index[0]
         xmin = conf_values[conf.loc[ix, 'xlim_left']]
         xmax = conf_values[conf.loc[ix, 'xlim_right']]
         ymin = conf_values[conf.loc[ix, 'ylim_bottom']]
         ymax = conf_values[conf.loc[ix, 'ylim_top']]
         axs.set_xlim([xmin, xmax])
         axs.set_ylim([ymin, ymax])
-
     
     axs.set_xticklabels([])
     axs.set_xticks([])
     axs.set_yticklabels([])
     axs.set_yticks([])
```

### Comparing `trackc-0.0.8/src/trackc/pl/scale.py` & `trackc-0.0.9/src/trackc/pl/scale.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,46 +14,76 @@
     else:
         return ticks
     return ticks
 def scale_track(ax: Optional[Axes] = None,
                 region: Union[str, None] = None,
                 tick_pos: str = 'bottom',
                 ratio2ax: float = 0.5,
-                chrom_fontsize: Union[int, None] = 10,
+                label_fontsize: Union[int, None] = 10,
                 scale_adjust: Union[str, None] = 'kb',
                 tick_fl: Union[str, None] ='%0.2f',
                 tick_fontsize: Union[int, None] = 8,
                 tick_rotation: Union[int, None] = 0,
                 space: float = 0.1,
                 ):
-    """
+    """\
+    Plot one region scale bar track
+
     Parameters
     ----------
+    ax: :class:`matplotlib.axes.Axes` object
+    region: `str`
+        one genome region, format: `chrom:start-end`
+        examples: "chr18:45000000-78077248"
+        if the start is bigger than end, the genome region will be reversed
+    tick_pos: `str`
+        ticks position, can be one of ['top', 'bottom']
+    ratio2ax: `float`
+        the height ratio refer to the given `ax`'s height
+    label_fontsize: `int`
+        the region text fontsize
+    scale_adjust: `str`
+        adjust the scale unit to make it pretty, can be one of ['kb', 'Mb']   
+    tick_fl: `str`  
+        ticks retains a few decimal places
+    tick_fontsize: `int`
+        ticks text fontsize
+    tick_rotation: `int`
+        ticks text rotation
+    space: `float`
+        space relative to the ax
     
-    scale_adjust
-        ``str``: should be one of [kb, Mb, bp]
-            adjust the scale unit to make it pretty
-    tick_fl
-        ``str``: The position label retains the number of decimal places  
-    tick_pos
-        one of ['top', 'bottom', 'left', 'right']                   
-
+    Example
+    -------
+    >>> import trackc as tc
+    >>> region = 'chr7:153000000-151000000'
+    
+    >>> ten = tc.tenon(width=8, height=1.2)
+    >>> ten.add(pos='bottom', height=0.5)
+    >>> ten.axs(0).axis('off')
+
+    >>> tc.pl.scale_track(ax=ten.axs(0), region=region, scale_adjust='Mb', tick_pos='bottom', ratio2ax=1.2)
+    >>> tc.pl.scale_track(ax=ten.axs(0), region=region, scale_adjust='Mb', tick_pos='top', ratio2ax=1.2)
+    >>> tc.savefig('trackc_scalebar_track.pdf')
     """
+
     line_GenomeRegions = None
     if isinstance(region, list):
         print('scale_track is only for one region')
         return
     else:
         line_GenomeRegions = GenomeRegion(region).GenomeRegion2df()
 
+    line_GenomeRegions['raw_region'] = line_GenomeRegions.index
     line_GenomeRegions = line_GenomeRegions.reset_index()
 
     chrom = line_GenomeRegions.loc[0, "chrom"]
     start = line_GenomeRegions.loc[0, "start"]
     end = line_GenomeRegions.loc[0, "end"]
+    raw_region = line_GenomeRegions.loc[0, 'raw_region']
 
     pos_dic = {
         'left': [-ratio2ax,	0, ratio2ax, 1],
         'right': [1, 0,	ratio2ax, 1],
         'top': [0, 1+space, 1, ratio2ax],
         'bottom': [0, -ratio2ax-space, 1, ratio2ax]
     }
@@ -62,50 +92,55 @@
     ax = ax2
     
     if tick_pos in ['top', 'bottom']:
         ax.set_xlim([start, end])
 
         xticks = ax.get_xticks()
         xtick_labels = xticks
+
         if scale_adjust == 'Mb':
             xtick_labels = xtick_labels/1000000
             xtick_labels = ["{0}".format(tick_fl % i) for i in xtick_labels]
             ax.set_xticks(xticks, xtick_labels, fontsize=tick_fontsize, rotation=tick_rotation)
             ax.spines['bottom'].set_position(('data', 0))
             #ax.text(end-(abs(end-start)*0.05), -1, 'Mb', fontsize=chrom_fontsize)
         elif scale_adjust == 'kb':
             xtick_labels = xtick_labels/1000
             xtick_labels = ["{0}".format(tick_fl % i) for i in xtick_labels]
-            ax.set_xticks(xticks, xtick_labels, fontsize=tick_fontsize, rotation=tick_rotation)
+            ax.set_xticks(xticks, xtick_labels)
             #ax.text(end-(abs(end-start)*0.05), -1, 'kb', fontsize=chrom_fontsize)
             ax.spines['bottom'].set_position(('data', 0))
         else:
             pass
 
         spines = ['bottom', 'top', 'right', 'left']
-        chrom_x = start + (end-start)/2
+        #chrom_x = start + (end-start)/2
+        chrom_x = start
         chrom_y = 1
         va = 'top'
-        
+        ha2  = 'right'
         if tick_pos=='bottom':
             del spines[1]
             ax.tick_params(top=True, labeltop=True, bottom=False, labelbottom=False)
             chrom_y = 0
             va = 'bottom'
             
         if tick_pos=='top':
+            ha2  = 'left'
             del spines[0]
             ax.tick_params(top=False, labeltop=False, bottom=True, labelbottom=True)
         for i in spines:
             ax.spines[i].set_visible(False)
+        if tick_rotation == 0:
+            ha2 = 'center'
 
-        ax.text(chrom_x, chrom_y, chrom, fontsize=chrom_fontsize, ha='center', va=va)
+        ax.text(chrom_x, chrom_y, raw_region, fontsize=label_fontsize, ha='left', va=va)
         labels = [label.get_text() for label in ax.get_xticklabels()]
         labels[-1] += '({0})'.format(scale_adjust)
-        ax.set_xticklabels(labels)
+        ax.set_xticklabels(labels, fontsize=tick_fontsize, rotation=tick_rotation, va='center', ha=ha2)
 
         ax.tick_params(which='major', direction='in', pad=-16) 
         ax.set_yticks([])
         ax.set_yticklabels('')  
     
 
 
@@ -116,14 +151,45 @@
                       intervals: Union[int, None] = 1,
                       scale_adjust: Union[str, None] = 'kb',
                       tick_fl: Union[str, None] ='%0.2f',
                       tick_fontsize: Union[int, None] = 8,
                       tick_rotation: Union[int, None] = 0,
                 ):
     """\
+    Plot region scale bar, support for multiple or reverse genome regions.
+
+    Parameters
+    ----------
+    ax: :class:`matplotlib.axes.Axes` object
+    regions: `str list` | `str`
+        e.g. ``"chr6:1000000-2000000"`` or ``["chr6:1000000-2000000", "chr3:5000000-4000000"]``
+        The start can be larger than the end (eg. ``"chr6:2000000-1000000"``), 
+            which means you want to get the reverse region
+    colors: `str list`
+        scale bar colors
+    alpha: `float`
+        scale bar alpha
+    intervals: `int`
+        rows of the scale bar by region
+    scale_adjust: `str`
+        options in ['kb', 'Mb']
+    tick_fl: `str`  
+        ticks retains a few decimal places
+    tick_fontsize: `int`
+        ticks text fontsize
+    tick_rotation: `int`
+        ticks text rotation
+
+    Example
+    -------
+    >>> import trackc as tc
+    >>> regions = ['7:153000000-151000000', '11:118500000-116500000']
+    >>> ten = tc.tenon(width=8, height=1)
+    >>> ten.add(pos='bottom', height=1)
+    >>> tc.pl.multi_scale_track(ten.axs(0), regions=regions, scale_adjust='Mb', intervals=2)
     """
 
     if colors != None:
         track_colors  = colors
     else:
         track_colors = trackcl_11
 
@@ -151,41 +217,46 @@
     else:
         bottom = bottom[:line_GenomeRegions.shape[0]]
     line_GenomeRegions.loc[:, 'bottom'] = bottom
 
     line_GenomeRegions['tick_s'] = _scale_ticks(line_GenomeRegions['start'], scale=scale_adjust, tick_fl=tick_fl)
     line_GenomeRegions['tick_e'] = _scale_ticks(line_GenomeRegions['end'], scale=scale_adjust, tick_fl=tick_fl)
     if scale_adjust in ['Mb', 'kb']:
-        line_GenomeRegions.loc[line_GenomeRegions.index[-1], "tick_e"] = line_GenomeRegions.loc[line_GenomeRegions.index[-1], "tick_e"] + "(" + scale_adjust + ")"
+        if intervals > 1:
+            line_GenomeRegions.loc[line_GenomeRegions.index[-1], "tick_e"] = line_GenomeRegions.loc[line_GenomeRegions.index[-1], "tick_e"] + "(" + scale_adjust + ")"
+        else:
+            line_GenomeRegions['tick_e'] = line_GenomeRegions['tick_e'] + "(" + scale_adjust + ")"
 
     for i, row in line_GenomeRegions.iterrows():
         arrow_s = row['acum'] - row['len']
         dx = row['len']
         if row["isReverse"] == True:
             arrow_s = row['acum']
             dx = -1 * row['len']
             
         ax.arrow(arrow_s, row['bottom'], dx, 0, 
-            overhang=1, width=0.01,
-            head_width=0.25,
-            head_length=sum_len/170,
+            overhang=1, width=0.02,
+            head_width=0.3,
+            head_length=sum_len/100,
             length_includes_head=True,
             color=row['color'],
             linewidth=1,
             alpha = alpha
             )
         
         tick_ha = 'center'
         if tick_rotation != 0:
             tick_ha = 'right'
-
-        ax.text(row['acum'] - row['len']/2, row['bottom']+0.1, row['chrom'], ha='center', va='bottom', fontsize=tick_fontsize, color=row['color'])
-        ax.text(row['acum'] - row['len'], row['bottom']-0.1, row['tick_s'], ha=tick_ha, va='top', fontsize=tick_fontsize, rotation=tick_rotation, color=row['color'])
-        ax.text(row['acum'], row['bottom']-0.1, row['tick_e'], ha=tick_ha, va='top', fontsize=tick_fontsize, rotation=tick_rotation, color=row['color'])
-
+        if intervals > 1:
+            ax.text(row['acum'] - row['len']/2, row['bottom']+0.1, row['chrom'], ha='center', va='bottom', fontsize=tick_fontsize, color=row['color'])
+            ax.text(row['acum'] - row['len'], row['bottom']-0.1, row['tick_s'], ha=tick_ha, va='top', fontsize=tick_fontsize, rotation=tick_rotation, color=row['color'])
+            ax.text(row['acum'], row['bottom']-0.1, row['tick_e'], ha=tick_ha, va='top', fontsize=tick_fontsize, rotation=tick_rotation, color=row['color'])
+        else:
+            ax.text(row['acum'] - row['len']/2, row['bottom']-0.2, '{0}:{1}-{2}'.format(row['chrom'], row['tick_s'], row['tick_e']), ha='center', va='top', fontsize=tick_fontsize, color=row['color'])
+            
 
     ax.set_xlim([0, sum_len])
     ax.set_ylim([-0.7, intervals-0.3])
 
     for i in ['bottom', 'top','right', 'left']:
         ax.spines[i].set_color('none')
         ax.spines[i].set_linewidth(0)
```

### Comparing `trackc-0.0.8/src/trackc/scripts/gtf2bed12.py` & `trackc-0.0.9/src/trackc/scripts/gtf2bed12.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,29 +53,21 @@
 
 def _bedcol9_2dic(bedcol9, split=";"):
     tmp = bedcol9.split(split)
     col9dic = {}
     for i in tmp:
         i = i.strip()
         ii = i.split(" ")
+        if len(ii) < 2:
+            continue
         val = ii[1].strip("\"")
         col9dic[ii[0]] = val
     return col9dic
 
 
-
-gene = None
-#gene_id="gene_id"
-gene_name_tag="gene_name"
-gene_id_tag="gene_id"
-gene_biotype_tag="gene_biotype"
-split = ";"
-biotype2bed13 = True
-
-
 def _parse_arguments(args=None):
     """
     get command line arguments
     """
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         add_help=False,
@@ -89,41 +81,42 @@
                                 required=True)
 
     parserRequired.add_argument('--outFileName', '-o',
                                 help='File name of gene annotation bed12 format.',
                                 required=True)
 
     parserOpt = parser.add_argument_group('Optional arguments')
-    parserOpt.add_argument('--splitby', '-s',
-                           help='tags of GTF split by which str',
+    parserOpt.add_argument('--sep', '-s',
+                           help='tags of GTF sepration by which str',
                            default=";")
     parserOpt.add_argument('--gene_name_tag', '-nt',
                            help='tags of GTF gene_name',
                            default="gene_name")
     parserOpt.add_argument('--gene_id_tag', '-it',
                            help='tags of GTF gene_id',
                            default="gene_id")
     parserOpt.add_argument('--gene_biotype_tag', '-bt',
                            help='tags of GTF gene_biotype',
                            default="gene_biotype")
     parserOpt.add_argument('--biotype2bed13', '-bed13',
                            help='if this arg is set, the out file columns 13 will add gene\'s biotype',
                            action='store_true')
+    parserOpt.add_argument("-h", "--help", action="help", help="show this help message and exit")
 
     return parser
 
 
 def _main(args=None):
 
     args = _parse_arguments().parse_args(args)
     gene_name_tag = args.gene_name_tag
     gene_id_tag = args.gene_id_tag
     gene_biotype_tag = args.gene_biotype_tag
-    split = args.splitby
-    biotype2bed13 = args.outFileName
+    sep = args.sep
+    biotype2bed13 = args.biotype2bed13
 
     gene = None
     gtf_hand = open(args.gtf, "r")
     gtf2bed = open(args.outFileName,'w')
 
     for line in gtf_hand:
         bedtab = line.rstrip().split('\t')
@@ -142,15 +135,15 @@
         if bedtab[2] == "gene":
             if gene != None:
                 gtf2bed.write(gene.tostr(biotype2bed13) + "\n")
             Gene_name = 'xx'
             Gene_biotype = "yy"
             
             
-            col9dic = _bedcol9_2dic(bedtab[8], split=split)
+            col9dic = _bedcol9_2dic(bedtab[8], split=sep)
             if gene_name_tag in col9dic.keys():
                 Gene_name = col9dic[gene_name_tag]
             elif gene_id_tag in col9dic.keys():
                 Gene_name = col9dic[gene_id_tag]
             else:
                 print(bedtab[8], ' have no {0}, xx instead'.format(gene_name_tag))
```

### Comparing `trackc-0.0.8/src/trackc/tl/_getRegionsCmat.py` & `trackc-0.0.9/src/trackc/tl/_getRegionsCmat.py`

 * *Files 15% similar despite different names*

```diff
@@ -66,52 +66,65 @@
         self.cmat = cmat
         self.row_regions = row_regions
         self.col_regions = col_regions
 
 # import extractContactRegions as subsetContactRegions
 
 def extractContactRegions(
-        clr: cooler.Cooler, 
+        clr: Union[cooler.Cooler, str], 
         balance: bool = False,
         #divisive_weights = None,
         row_regions: Union[Sequence[str], str, None] = None,
         col_regions: Union[Sequence[str], str, None] = None, 
         ) -> RegionsCmat:
     """\
     Extract a set of regions matrix from the cool format Hi-C matrix.
 
-    The extracted matrix will splice intra and Inter region interaction according to 
+    The extracted matrix will splice intra and inter region interaction according to 
         the given order and direction of the regions.
+
     Parameters
     ----------
-    coolMat 
-        ``cooler.Cooler``: cool format Hi-C matrix (https://github.com/open2c/cooler)
-    balance
-        ``bool``: The ``'balance'`` parameters of ``coolMat.matrix(balance=False).fetch('chr6:119940450-123940450')``
-    divisive_weights: bool, optional
-        Force balancing weights to be interpreted as divisive (True) or
-        multiplicative (False). Weights are always assumed to be
-        multiplicative by default unless named KR, VC or SQRT_VC, in which
-        case they are assumed to be divisive by default.
+    clr: `cooler.Cooler` | `str`
+        cool format Hi-C matrix (https://github.com/open2c/cooler) or cool file path
+        `cooler.Cooler` e.g. GM12878=cooler.Cooler('./GM12878.chr18.mcool::/resolutions/50000')
+        `str` e.g. 'GM12878.chr18.mcool::/resolutions/50000' or 'GM12878.chr18.cool'
 
-    row_regions
-        ``chrom region`` list: or ``chrom region`` or None. 
+    balance: `bool`
+        The ``'balance'`` parameters of ``coolMat.matrix(balance=False).fetch('chr6:119940450-123940450')``
+    row_regions: `str` | `str list` | None. 
         The subset matrix row genome regions
-        eg. ``"chr6:1000000-2000000"``, eg. ``["chr6:1000000-2000000", "chr3:5000000-4000000", "chr5"]``
-        The start can be larger than the end (eg. ``"chr6:2000000-1000000"``), 
+        e.g. ``"chr6:1000000-2000000"``, e.g. ``["chr6:1000000-2000000", "chr3:5000000-4000000", "chr5"]``
+        The start can be larger than the end (e.g. ``"chr6:2000000-1000000"``), 
             which means you want to get the reverse region contact matrix
-
-    col_regions
-        ``chrom region`` list: or ``chrom region`` or None. 
+    col_regions: `str` | `str list` | None. 
         The subset matrix col genome regions, default is ``None``, which means the sample region as ``row_regions``
         
     Returns:
-        :class:`~trackc.RegionsCmat`
+    --------
+        :class:`~trackc.tl.RegionsCmat`
             row_regions and col_regions contact matrix object
+
+    Example
+    -------
+    >>> import trackc as tc
+    >>> import cooler
+    >>> mat1 = tc.tl.extractContactRegions(clr='GM12878.chr18.mcool::/resolutions/50000', row_regions="18:45000000-78077248")
+    >>> GM12878 = cooler.Cooler('./GM12878.chr18.mcool::/resolutions/50000')
+    >>> mat2 = tc.tl.extractContactRegions(clr=GM12878, row_regions=["18:61140000-63630000", "18:74030000-77560000"], col_regions="18:47340000-50370000")
+    >>> print(mat2.cmap.shape)
+    >>> print(mat2.row_regions)
+    >>> print(mat2.col_regions)
     """
+    #divisive_weights: bool, optional
+    #    Force balancing weights to be interpreted as divisive (True) or
+    #    multiplicative (False). Weights are always assumed to be
+    #    multiplicative by default unless named KR, VC or SQRT_VC, in which
+    #    case they are assumed to be divisive by default.
+
     # -------
     if isinstance(row_regions, list):
         row_GenomeRegions = pd.concat([GenomeRegion(i).GenomeRegion2df() for i in row_regions])
     else:
         row_GenomeRegions = GenomeRegion(row_regions).GenomeRegion2df()
 
     if col_regions == None:
@@ -119,14 +132,17 @@
     else:
         if isinstance(col_regions, list):
             col_GenomeRegions = pd.concat([GenomeRegion(i).GenomeRegion2df() for i in col_regions])
         else:
             col_GenomeRegions = GenomeRegion(col_regions).GenomeRegion2df()
     
     # ------
+    if isinstance(clr, str):
+        clr = cooler.Cooler(clr)
+
     region_mat_dic = {}
     for _, row_row in row_GenomeRegions.iterrows():
         for _, col_row in col_GenomeRegions.iterrows():
             row_col_region_cmat = clr.matrix(balance=balance).fetch(row_row['region4coolFetch'], col_row['region4coolFetch'])
             if row_row['isReverse'] == True:
                 row_col_region_cmat = np.flip(row_col_region_cmat, 0)
             if col_row['isReverse'] == True:
@@ -174,47 +190,56 @@
     r_l_regions_cMat = RegionsCmat(cmat=cMat, row_regions=row_GenomeRegions, col_regions=col_GenomeRegions)
     
     return r_l_regions_cMat
         
 # import extractCisRegion as subsetCisRegion
 
 def extractCisContact(
-        clr: cooler.Cooler,
+        clr: Union[cooler.Cooler, str],
         region: str,
         extend: int = 0,
         balance: bool = False,
-        divisive_weights = None,
+        #divisive_weights = None,
         ) -> np.array:
     """\
-    Extract cis contact matrix from the cool format Hi-C matrix.
+    Extract cis contact matrix from the cool or mcool format Hi-C matrix.
 
     Parameters
     ----------
-    clr: ``cooler.Cooler``
-        cool format Hi-C matrix (https://github.com/open2c/cooler)
-    region: ``str``
+    clr: `cooler.Cooler` | `str`
+        cool format Hi-C matrix (https://github.com/open2c/cooler) or cool file path
+        `cooler.Cooler` e.g. GM12878=cooler.Cooler('./GM12878.chr18.mcool::/resolutions/50000')
+        `str` e.g. 'GM12878.chr18.mcool::/resolutions/50000' or 'GM12878.chr18.cool'
+    region: `str`
         The subset matrix row genome regions
         eg. ``"chr6:1000000-2000000"`` or ``chr6``
 
-    extend: ``int``
+    extend: `int`
         contact map extend to start and end position
-    balance: ``bool``
+    balance: `bool`
         The ``'balance'`` parameters of ``coolMat.matrix(balance=False).fetch('chr6:119940450-123940450')``
-    divisive_weights: bool, optional
-        Force balancing weights to be interpreted as divisive (True) or
-        multiplicative (False). Weights are always assumed to be
-        multiplicative by default unless named KR, VC or SQRT_VC, in which
-        case they are assumed to be divisive by default.
 
     Returns:
-    ----------
+    --------
     contact matrix: np.array
-        matrix sstart with top-left
+        matrix start with top-left
+
+    Example
+    -------
+    >>> import trackc as tc
+    >>> import cooler
+    >>> mat1 = tc.tl.extractCisContact(clr='GM12878.chr18.mcool::/resolutions/50000', region="18:45000000-78077248")
+    >>> GM12878 = cooler.Cooler('./GM12878.chr18.mcool::/resolutions/50000')
+    >>> mat2 = tc.tl.extractCisContact(clr=GM12878, region="18:45000000-78077248")
+    >>> print(mat2.shape)
     """
 
+    if isinstance(clr, str):
+        clr = cooler.Cooler(clr)
+
     resolution = clr.binsize
     genome_region = GenomeRegion(region)
 
     if genome_region.chrom not in clr.chromsizes:
          logging.error(genome_region.chrom, ' is not a chrom in the cool matrix') 
 
     maxChromL = clr.chromsizes[genome_region.chrom]
```

### Comparing `trackc-0.0.8/src/trackc.egg-info/SOURCES.txt` & `trackc-0.0.9/src/trackc.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -6,23 +6,22 @@
 requirements.txt
 setup.py
 bin/gtf2bed4trackc
 docs/Makefile
 docs/_config.yml
 docs/api.rst
 docs/conf.py
-docs/conf.py_bk
 docs/custom-formats.pct.py
 docs/developer.rst
 docs/faq.rst
-docs/gallary.rst
+docs/gallery.rst
 docs/index.rst
+docs/install.rst
 docs/make.bat
 docs/modules.rst
-docs/quick_start.rst
 docs/references.bib
 docs/references.rst
 docs/releases.rst
 docs/requirements.txt
 docs/source
 docs/trackc.pa.rst
 docs/trackc.pl.rst
@@ -39,27 +38,52 @@
 docs/developer/about_us.rst
 docs/developer/history.rst
 docs/developer/index.rst
 docs/examples/README.txt
 docs/examples/bw_track_tutorial.ipynb
 docs/examples/cmap-test-data.ipynb
 docs/examples/mapc_eg.ipynb
-docs/examples/zoomin_heatmap.ipynb
+docs/examples/neotad.png
+docs/examples/rearranged_interactions.ipynb
 docs/examples/zoomin_heatmap.png
+docs/images/trackc-brand-board-your-branding-colors-and-fonts.zip
+docs/images/trackc-high-resolution-color-logo.png
+docs/images/trackc-high-resolution-logo-color-on-transparent-background.png
+docs/images/trackc-high-resolution-logo-white-on-transparent-background.png
+docs/images/trackc-logo-zip-file.zip
+docs/images/trackc-low-resolution-color-logo.png
+docs/images/trackc-low-resolution-logo-black-on-transparent-background.png
+docs/images/trackc-low-resolution-logo-color-on-transparent-background.png
+docs/images/trackc-low-resolution-logo-white-on-transparent-background.png
 docs/images/trackc_dynamic_2022.png
-docs/images/trackc_logo.png
 docs/images/tutorials/grid_spec_01.png
+docs/images/tutorials/quick_start.png
 docs/images/tutorials/zoomin_heatmap.png
+docs/tutorials/ENCFF041XLP.bedpe
 docs/tutorials/README.txt
+docs/tutorials/Virtual4C.ipynb
+docs/tutorials/bed.ipynb
+docs/tutorials/bigwig.ipynb
 docs/tutorials/bw_track_tutorial.ipynb
 docs/tutorials/cmap-test-data.ipynb
+docs/tutorials/contactmap.ipynb
+docs/tutorials/datas.ipynb
+docs/tutorials/gene.ipynb
+docs/tutorials/gene_track.pdf
+docs/tutorials/grid_spec.ipynb
+docs/tutorials/links.ipynb
 docs/tutorials/mapc_eg.ipynb
-docs/tutorials/zoomin_heatmap.ipynb
+docs/tutorials/mapc_markline.ipynb
+docs/tutorials/scalebar.ipynb
+docs/tutorials/trackc_scale.pdf
+docs/tutorials/zoomin.ipynb
+docs/tutorials/fileformats/GRCh38.84.bed12
 docs/tutorials/fileformats/GRCh38.84.gtf.bed12
 docs/tutorials/fileformats/bed12.rst
+docs/tutorials/fileformats/mcool.rst
 src/trackc/__init__.py
 src/trackc/_utils.py
 src/trackc/gs.py
 src/trackc.egg-info/PKG-INFO
 src/trackc.egg-info/SOURCES.txt
 src/trackc.egg-info/dependency_links.txt
 src/trackc.egg-info/requires.txt
```

