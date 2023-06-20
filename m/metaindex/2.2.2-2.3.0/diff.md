# Comparing `tmp/metaindex-2.2.2.tar.gz` & `tmp/metaindex-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaindex-2.2.2.tar", last modified: Sat Jun  3 09:04:18 2023, max compression
+gzip compressed data, was "metaindex-2.3.0.tar", last modified: Tue Jun 20 19:53:14 2023, max compression
```

## Comparing `metaindex-2.2.2.tar` & `metaindex-2.3.0.tar`

### file list

```diff
@@ -1,171 +1,172 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/
--rw-r--r--   0 robert    (1000) robert    (1000)     6147 2023-06-03 09:03:31.000000 metaindex-2.2.2/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.2.2/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.2.2/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     4964 2023-06-03 09:04:18.100041 metaindex-2.2.2/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4141 2023-05-28 06:12:37.000000 metaindex-2.2.2/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.083375 metaindex-2.2.2/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.2.2/doc/Makefile
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.080041 metaindex-2.2.2/doc/build/
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.086708 metaindex-2.2.2/doc/build/doctrees/
--rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/addons.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/changelog.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/cmdoptions.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/cmdusage.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/configuration.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/description.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/environment.pickle
--rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/examples.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/extrametadata.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/index.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/indexers.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/install.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.2.2/doc/build/doctrees/license.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/reference.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/searchsyntax.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/synopsis.doctree
--rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/doctrees/usage.doctree
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.090041 metaindex-2.2.2/doc/build/html/
--rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/.buildinfo
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.093375 metaindex-2.2.2/doc/build/html/_sources/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.2.2/doc/build/html/_sources/addons.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.2.2/doc/build/html/_sources/changelog.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.2.2/doc/build/html/_sources/cmdoptions.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.2.2/doc/build/html/_sources/cmdusage.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.2.2/doc/build/html/_sources/configuration.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.2.2/doc/build/html/_sources/description.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.2.2/doc/build/html/_sources/examples.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.2.2/doc/build/html/_sources/extrametadata.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.2.2/doc/build/html/_sources/index.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.2.2/doc/build/html/_sources/indexers.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.2.2/doc/build/html/_sources/install.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.2.2/doc/build/html/_sources/license.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.2.2/doc/build/html/_sources/reference.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.2.2/doc/build/html/_sources/searchsyntax.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.2.2/doc/build/html/_sources/synopsis.rst.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.2.2/doc/build/html/_sources/usage.rst.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.096708 metaindex-2.2.2/doc/build/html/_static/
--rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/basic.css
--rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/doctools.js
--rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/documentation_options.js
--rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/file.png
--rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/jquery.js
--rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/language_data.js
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/minus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/nature.css
--rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/plus.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/_static/pygments.css
--rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/searchtools.js
--rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.2.2/doc/build/html/_static/underscore.js
--rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/addons.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/changelog.html
--rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/cmdusage.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/configuration.html
--rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/description.html
--rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/examples.html
--rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/extrametadata.html
--rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/genindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/index.html
--rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/indexers.html
--rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/install.html
--rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/license.html
--rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/objects.inv
--rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/reference.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/search.html
--rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/searchindex.js
--rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/searchsyntax.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/synopsis.html
--rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.2.2/doc/build/html/usage.html
--rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.2.2/doc/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.2.2/doc/make.bat
--rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.2.2/doc/metaindex.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.2.2/doc/requirements.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.096708 metaindex-2.2.2/doc/source/
--rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.2.2/doc/source/addons.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.2.2/doc/source/changelog.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     5307 2023-05-28 07:32:15.000000 metaindex-2.2.2/doc/source/cmdoptions.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.2.2/doc/source/cmdusage.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.2.2/doc/source/conf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8069 2023-05-18 15:06:36.000000 metaindex-2.2.2/doc/source/configuration.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.2.2/doc/source/description.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.2.2/doc/source/examples.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.2.2/doc/source/extrametadata.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.2.2/doc/source/index.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     8208 2023-05-28 07:47:46.000000 metaindex-2.2.2/doc/source/indexers.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.2.2/doc/source/install.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.2.2/doc/source/license.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.2.2/doc/source/reference.rst
--rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.2.2/doc/source/searchsyntax.rst
--rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.2.2/doc/source/synopsis.rst
--rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.2.2/doc/source/usage.rst
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.096708 metaindex-2.2.2/examples/
--rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.2.2/examples/indexing.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.096708 metaindex-2.2.2/man/
--rw-r--r--   0 robert    (1000) robert    (1000)    38113 2023-06-03 09:04:17.000000 metaindex-2.2.2/man/metaindex.1
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)      274 2023-05-16 17:26:33.000000 metaindex-2.2.2/metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)    16060 2023-05-27 16:53:24.000000 metaindex-2.2.2/metaindex/cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)    12461 2023-06-03 08:58:55.000000 metaindex-2.2.2/metaindex/cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-05-11 18:09:52.000000 metaindex-2.2.2/metaindex/client.py
--rw-r--r--   0 robert    (1000) robert    (1000)    24347 2023-05-27 19:11:56.000000 metaindex-2.2.2/metaindex/configuration.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/metaindex/docs/
--rw-r--r--   0 robert    (1000) robert    (1000)    13555 2023-06-03 09:04:17.000000 metaindex-2.2.2/metaindex/docs/cmdoptions.html
--rw-r--r--   0 robert    (1000) robert    (1000)    56492 2023-06-03 09:04:17.000000 metaindex-2.2.2/metaindex/docs/metaindex.html
--rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.2.2/metaindex/find.py
--rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.2.2/metaindex/fuse.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.2.2/metaindex/humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)    15319 2023-05-28 07:14:07.000000 metaindex-2.2.2/metaindex/indexer.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/metaindex/indexers/
--rw-r--r--   0 robert    (1000) robert    (1000)      512 2023-05-27 08:36:14.000000 metaindex-2.2.2/metaindex/indexers/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.2.2/metaindex/indexers/abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.2.2/metaindex/indexers/audio.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4956 2023-05-23 18:18:09.000000 metaindex-2.2.2/metaindex/indexers/collections.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6714 2023-05-27 16:39:21.000000 metaindex-2.2.2/metaindex/indexers/comicbook.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.2.2/metaindex/indexers/epub.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4742 2023-05-27 16:27:19.000000 metaindex-2.2.2/metaindex/indexers/filetags.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4435 2023-05-27 16:28:19.000000 metaindex-2.2.2/metaindex/indexers/gpx.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3061 2023-05-27 18:49:01.000000 metaindex-2.2.2/metaindex/indexers/html.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3801 2023-05-28 07:41:25.000000 metaindex-2.2.2/metaindex/indexers/images.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2788 2023-05-27 18:54:57.000000 metaindex-2.2.2/metaindex/indexers/ooxml.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2876 2023-05-27 18:56:00.000000 metaindex-2.2.2/metaindex/indexers/opendocument.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3353 2023-05-27 19:11:05.000000 metaindex-2.2.2/metaindex/indexers/pdf.py
--rw-r--r--   0 robert    (1000) robert    (1000)    10676 2023-05-19 08:45:31.000000 metaindex-2.2.2/metaindex/indexers/ruleindexer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4004 2023-05-28 07:13:11.000000 metaindex-2.2.2/metaindex/json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-19 08:54:45.000000 metaindex-2.2.2/metaindex/logger.py
--rw-r--r--   0 robert    (1000) robert    (1000)     9458 2023-05-28 07:33:08.000000 metaindex-2.2.2/metaindex/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)     7317 2023-05-28 07:42:39.000000 metaindex-2.2.2/metaindex/ocr.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2757 2023-05-27 16:14:29.000000 metaindex-2.2.2/metaindex/opf.py
--rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-06-03 08:59:37.000000 metaindex-2.2.2/metaindex/proto.py
--rw-r--r--   0 robert    (1000) robert    (1000)    27524 2023-05-27 08:10:45.000000 metaindex-2.2.2/metaindex/server.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6061 2023-06-03 08:58:47.000000 metaindex-2.2.2/metaindex/shared.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.2.2/metaindex/stores.py
--rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-06-03 09:03:39.000000 metaindex-2.2.2/metaindex/version.py
--rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.2.2/metaindex/xmlproxy.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4053 2023-05-28 07:02:39.000000 metaindex-2.2.2/metaindex/yaml.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/metaindex.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     4964 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     4390 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)      235 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-06-03 09:04:18.000000 metaindex-2.2.2/metaindex.egg-info/top_level.txt
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/misc/
--rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.2.2/misc/metaindex.conf
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/misc/ranger_metaindex/
--rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.2.2/misc/ranger_metaindex/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.2.2/misc/ranger_metaindex/linemode.py
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-03 09:04:18.100041 metaindex-2.2.2/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     3664 2023-05-21 10:28:55.000000 metaindex-2.2.2/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-03 09:04:18.100041 metaindex-2.2.2/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.2.2/tests/test_abc.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.2.2/tests/test_cache.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.2.2/tests/test_cacheentry.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.2.2/tests/test_cleanup.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.2.2/tests/test_collect.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.2.2/tests/test_humanizer.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.2.2/tests/test_indexers.py
--rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.2.2/tests/test_json.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.2.2/tests/test_ruleindexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.520248 metaindex-2.3.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)     6470 2023-06-20 19:52:13.000000 metaindex-2.3.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1107 2022-02-23 18:45:10.000000 metaindex-2.3.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      220 2021-09-01 18:34:21.000000 metaindex-2.3.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     4964 2023-06-20 19:53:14.520248 metaindex-2.3.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4141 2023-06-03 15:21:06.000000 metaindex-2.3.0/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.506914 metaindex-2.3.0/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)      638 2022-02-23 18:26:43.000000 metaindex-2.3.0/doc/Makefile
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.506914 metaindex-2.3.0/doc/build/
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.510248 metaindex-2.3.0/doc/build/doctrees/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14332 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/addons.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    32378 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/changelog.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    25916 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/cmdoptions.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6598 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/cmdusage.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    38700 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/configuration.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     5614 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/description.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    69762 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/doctrees/environment.pickle
+-rw-r--r--   0 robert    (1000) robert    (1000)    12145 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/examples.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    24665 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/extrametadata.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     8436 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/index.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    27055 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/indexers.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     9541 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/install.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     6122 2022-03-20 10:53:27.000000 metaindex-2.3.0/doc/build/doctrees/license.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)   177806 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/doctrees/reference.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    12666 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/doctrees/searchsyntax.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)     2656 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/doctrees/synopsis.doctree
+-rw-r--r--   0 robert    (1000) robert    (1000)    26715 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/doctrees/usage.doctree
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.513581 metaindex-2.3.0/doc/build/html/
+-rw-r--r--   0 robert    (1000) robert    (1000)      230 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/.buildinfo
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.513581 metaindex-2.3.0/doc/build/html/_sources/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.3.0/doc/build/html/_sources/addons.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.3.0/doc/build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-02-25 19:33:14.000000 metaindex-2.3.0/doc/build/html/_sources/cmdoptions.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      773 2022-02-25 21:17:37.000000 metaindex-2.3.0/doc/build/html/_sources/cmdusage.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     6605 2022-03-13 16:28:39.000000 metaindex-2.3.0/doc/build/html/_sources/configuration.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.3.0/doc/build/html/_sources/description.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.3.0/doc/build/html/_sources/examples.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.3.0/doc/build/html/_sources/extrametadata.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.3.0/doc/build/html/_sources/index.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     5934 2022-03-15 19:41:05.000000 metaindex-2.3.0/doc/build/html/_sources/indexers.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.3.0/doc/build/html/_sources/install.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.3.0/doc/build/html/_sources/license.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.3.0/doc/build/html/_sources/reference.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.3.0/doc/build/html/_sources/searchsyntax.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.3.0/doc/build/html/_sources/synopsis.rst.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.3.0/doc/build/html/_sources/usage.rst.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.516914 metaindex-2.3.0/doc/build/html/_static/
+-rw-r--r--   0 robert    (1000) robert    (1000)    14692 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/_static/basic.css
+-rw-r--r--   0 robert    (1000) robert    (1000)     9758 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/doctools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      350 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/_static/documentation_options.js
+-rw-r--r--   0 robert    (1000) robert    (1000)      286 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/file.png
+-rw-r--r--   0 robert    (1000) robert    (1000)   287630 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    89476 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/jquery.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    10854 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/_static/language_data.js
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/minus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     4181 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/_static/nature.css
+-rw-r--r--   0 robert    (1000) robert    (1000)       90 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/plus.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5432 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/_static/pygments.css
+-rw-r--r--   0 robert    (1000) robert    (1000)    16793 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/searchtools.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    68420 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    19530 2022-02-23 18:30:51.000000 metaindex-2.3.0/doc/build/html/_static/underscore.js
+-rw-r--r--   0 robert    (1000) robert    (1000)    11398 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/addons.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16853 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/changelog.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    12806 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6745 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/cmdusage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20977 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/configuration.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     4029 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/description.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    13768 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/examples.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    16741 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/extrametadata.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    18918 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/genindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     6742 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/index.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    20498 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/indexers.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     7101 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/install.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     5360 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/license.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     1235 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/objects.inv
+-rw-r--r--   0 robert    (1000) robert    (1000)    66164 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/reference.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3093 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/search.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    17128 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/searchindex.js
+-rw-r--r--   0 robert    (1000) robert    (1000)     9155 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/searchsyntax.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3970 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/synopsis.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    14783 2022-03-20 10:53:28.000000 metaindex-2.3.0/doc/build/html/usage.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     3334 2022-02-25 14:43:32.000000 metaindex-2.3.0/doc/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      804 2022-02-23 18:26:43.000000 metaindex-2.3.0/doc/make.bat
+-rw-r--r--   0 robert    (1000) robert    (1000)      901 2022-02-25 21:18:16.000000 metaindex-2.3.0/doc/metaindex.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       19 2022-02-23 18:30:21.000000 metaindex-2.3.0/doc/requirements.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.516914 metaindex-2.3.0/doc/source/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2736 2022-03-13 15:27:55.000000 metaindex-2.3.0/doc/source/addons.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       80 2022-02-23 18:39:36.000000 metaindex-2.3.0/doc/source/changelog.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     5307 2023-06-03 15:21:06.000000 metaindex-2.3.0/doc/source/cmdoptions.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      653 2023-05-11 18:09:52.000000 metaindex-2.3.0/doc/source/cmdusage.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1871 2022-02-23 18:29:41.000000 metaindex-2.3.0/doc/source/conf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8069 2023-06-03 15:21:06.000000 metaindex-2.3.0/doc/source/configuration.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      726 2022-03-10 18:16:36.000000 metaindex-2.3.0/doc/source/description.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1052 2022-03-20 09:25:44.000000 metaindex-2.3.0/doc/source/examples.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     4869 2022-02-25 20:09:22.000000 metaindex-2.3.0/doc/source/extrametadata.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      332 2022-03-13 15:16:59.000000 metaindex-2.3.0/doc/source/index.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     8208 2023-06-03 15:21:06.000000 metaindex-2.3.0/doc/source/indexers.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1151 2022-02-23 18:37:25.000000 metaindex-2.3.0/doc/source/install.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       58 2022-02-23 18:40:10.000000 metaindex-2.3.0/doc/source/license.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      664 2022-03-20 10:20:29.000000 metaindex-2.3.0/doc/source/reference.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)     1964 2022-03-13 16:29:46.000000 metaindex-2.3.0/doc/source/searchsyntax.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)      105 2022-02-25 19:48:09.000000 metaindex-2.3.0/doc/source/synopsis.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)       55 2022-02-25 19:48:15.000000 metaindex-2.3.0/doc/source/usage.rst
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.516914 metaindex-2.3.0/examples/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1223 2022-03-20 09:43:43.000000 metaindex-2.3.0/examples/indexing.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.516914 metaindex-2.3.0/man/
+-rw-r--r--   0 robert    (1000) robert    (1000)    38110 2023-06-20 19:53:14.000000 metaindex-2.3.0/man/metaindex.1
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.516914 metaindex-2.3.0/metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)      274 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    16060 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    12461 2023-06-03 15:22:29.000000 metaindex-2.3.0/metaindex/cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6631 2023-06-10 16:13:58.000000 metaindex-2.3.0/metaindex/cli.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1968 2023-06-11 10:21:34.000000 metaindex-2.3.0/metaindex/client.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    24285 2023-06-20 19:34:46.000000 metaindex-2.3.0/metaindex/configuration.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.516914 metaindex-2.3.0/metaindex/docs/
+-rw-r--r--   0 robert    (1000) robert    (1000)    13556 2023-06-20 19:53:14.000000 metaindex-2.3.0/metaindex/docs/cmdoptions.html
+-rw-r--r--   0 robert    (1000) robert    (1000)    56493 2023-06-20 19:53:14.000000 metaindex-2.3.0/metaindex/docs/metaindex.html
+-rw-r--r--   0 robert    (1000) robert    (1000)     2859 2023-05-11 18:09:52.000000 metaindex-2.3.0/metaindex/find.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    18409 2021-10-16 07:30:31.000000 metaindex-2.3.0/metaindex/fuse.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4287 2022-06-18 22:14:53.000000 metaindex-2.3.0/metaindex/humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    15319 2023-06-20 18:31:44.000000 metaindex-2.3.0/metaindex/indexer.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.520248 metaindex-2.3.0/metaindex/indexers/
+-rw-r--r--   0 robert    (1000) robert    (1000)      512 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1972 2022-08-21 19:12:49.000000 metaindex-2.3.0/metaindex/indexers/abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1157 2022-05-11 17:49:48.000000 metaindex-2.3.0/metaindex/indexers/audio.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4956 2023-06-20 18:37:32.000000 metaindex-2.3.0/metaindex/indexers/collections.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6714 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/comicbook.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1498 2022-06-27 12:23:51.000000 metaindex-2.3.0/metaindex/indexers/epub.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4742 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/filetags.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4435 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/gpx.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3061 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/html.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3801 2023-06-20 18:27:44.000000 metaindex-2.3.0/metaindex/indexers/images.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2788 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/ooxml.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2876 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/opendocument.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3353 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/pdf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    10676 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/indexers/ruleindexer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4004 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1566 2023-05-19 08:54:45.000000 metaindex-2.3.0/metaindex/logger.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     9597 2023-06-10 15:47:44.000000 metaindex-2.3.0/metaindex/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     7317 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/ocr.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2757 2023-06-03 15:21:06.000000 metaindex-2.3.0/metaindex/opf.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     8167 2023-06-11 10:21:34.000000 metaindex-2.3.0/metaindex/proto.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    27849 2023-06-20 19:50:59.000000 metaindex-2.3.0/metaindex/server.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6287 2023-06-20 19:01:33.000000 metaindex-2.3.0/metaindex/shared.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3198 2023-05-11 18:09:52.000000 metaindex-2.3.0/metaindex/stores.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-06-20 19:52:28.000000 metaindex-2.3.0/metaindex/version.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      734 2022-06-27 12:20:41.000000 metaindex-2.3.0/metaindex/xmlproxy.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4053 2023-06-20 19:02:16.000000 metaindex-2.3.0/metaindex/yaml.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.516914 metaindex-2.3.0/metaindex.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     4964 2023-06-20 19:53:14.000000 metaindex-2.3.0/metaindex.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     4407 2023-06-20 19:53:14.000000 metaindex-2.3.0/metaindex.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-20 19:53:14.000000 metaindex-2.3.0/metaindex.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       88 2023-06-20 19:53:14.000000 metaindex-2.3.0/metaindex.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)      235 2023-06-20 19:53:14.000000 metaindex-2.3.0/metaindex.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       29 2023-06-20 19:53:14.000000 metaindex-2.3.0/metaindex.egg-info/top_level.txt
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.520248 metaindex-2.3.0/misc/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2161 2023-05-11 18:09:52.000000 metaindex-2.3.0/misc/metaindex.conf
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.520248 metaindex-2.3.0/misc/ranger_metaindex/
+-rw-r--r--   0 robert    (1000) robert    (1000)       41 2021-09-01 18:34:21.000000 metaindex-2.3.0/misc/ranger_metaindex/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)      737 2023-05-11 18:09:16.000000 metaindex-2.3.0/misc/ranger_metaindex/linemode.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-20 19:53:14.520248 metaindex-2.3.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     3664 2023-06-03 15:21:06.000000 metaindex-2.3.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-20 19:53:14.520248 metaindex-2.3.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1072 2022-08-21 19:09:08.000000 metaindex-2.3.0/tests/test_abc.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4343 2023-05-11 18:09:52.000000 metaindex-2.3.0/tests/test_cache.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3043 2022-06-24 07:16:59.000000 metaindex-2.3.0/tests/test_cacheentry.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3933 2022-06-27 09:57:52.000000 metaindex-2.3.0/tests/test_cleanup.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2529 2022-02-26 17:13:44.000000 metaindex-2.3.0/tests/test_collect.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4866 2022-03-13 18:33:11.000000 metaindex-2.3.0/tests/test_humanizer.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1460 2022-03-15 17:55:22.000000 metaindex-2.3.0/tests/test_indexers.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     3895 2022-02-26 16:28:16.000000 metaindex-2.3.0/tests/test_json.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2549 2022-04-30 12:43:40.000000 metaindex-2.3.0/tests/test_ruleindexer.py
```

### Comparing `metaindex-2.2.2/CHANGELOG.md` & `metaindex-2.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,33 @@
 # Changelog
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
+
+## 2.3.0
+### Added
+- Very basic commandline interface. Try `metaindex cli`
+
+### Changed
+- Use `~/.local/state/metaindex/` instead of `~/.cache/metaindex/` for the database
+- Don't keep the fulltext in the `CacheEntry`s
+- Fix umask of the metaindex database
+
+### Fixed
+- YAML sidecar file with a date would cause errors
+
+
 ## 2.2.2
 ### Fixed
 - Fixed issues with `last_modified` and the new unified timestamp format
 
+
 ## 2.2.1
 ### Changed
 - `date` field in sidecar files will be split into `date` and `time` upon loading, if possible, and saved as a merged `date` field upon saving
 
 ### Fixed
 - Overriding values by setting them to `none`/`null` in the sidecar file was not actually doing anything
 - Language hinting for OCR was too demanding; now also short ISO 639 codes work
```

### Comparing `metaindex-2.2.2/LICENSE` & `metaindex-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/PKG-INFO` & `metaindex-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 2.2.2
+Version: 2.3.0
 Summary: Utilities to tag files
 Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `metaindex-2.2.2/README.md` & `metaindex-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/Makefile` & `metaindex-2.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/addons.doctree` & `metaindex-2.3.0/doc/build/doctrees/addons.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/changelog.doctree` & `metaindex-2.3.0/doc/build/doctrees/changelog.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/cmdoptions.doctree` & `metaindex-2.3.0/doc/build/doctrees/cmdoptions.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/cmdusage.doctree` & `metaindex-2.3.0/doc/build/doctrees/cmdusage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/configuration.doctree` & `metaindex-2.3.0/doc/build/doctrees/configuration.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/description.doctree` & `metaindex-2.3.0/doc/build/doctrees/description.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/environment.pickle` & `metaindex-2.3.0/doc/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/examples.doctree` & `metaindex-2.3.0/doc/build/doctrees/examples.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/extrametadata.doctree` & `metaindex-2.3.0/doc/build/doctrees/extrametadata.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/index.doctree` & `metaindex-2.3.0/doc/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/indexers.doctree` & `metaindex-2.3.0/doc/build/doctrees/indexers.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/install.doctree` & `metaindex-2.3.0/doc/build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/license.doctree` & `metaindex-2.3.0/doc/build/doctrees/license.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/reference.doctree` & `metaindex-2.3.0/doc/build/doctrees/reference.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/searchsyntax.doctree` & `metaindex-2.3.0/doc/build/doctrees/searchsyntax.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/synopsis.doctree` & `metaindex-2.3.0/doc/build/doctrees/synopsis.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/doctrees/usage.doctree` & `metaindex-2.3.0/doc/build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/addons.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/addons.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/cmdoptions.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/cmdoptions.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/cmdusage.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/cmdusage.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/configuration.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/configuration.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/description.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/description.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/examples.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/examples.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/extrametadata.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/extrametadata.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/indexers.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/indexers.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/install.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/reference.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/reference.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_sources/searchsyntax.rst.txt` & `metaindex-2.3.0/doc/build/html/_sources/searchsyntax.rst.txt`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/basic.css` & `metaindex-2.3.0/doc/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/doctools.js` & `metaindex-2.3.0/doc/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/jquery-3.5.1.js` & `metaindex-2.3.0/doc/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/jquery.js` & `metaindex-2.3.0/doc/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/language_data.js` & `metaindex-2.3.0/doc/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/nature.css` & `metaindex-2.3.0/doc/build/html/_static/nature.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/pygments.css` & `metaindex-2.3.0/doc/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/searchtools.js` & `metaindex-2.3.0/doc/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/underscore-1.13.1.js` & `metaindex-2.3.0/doc/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/_static/underscore.js` & `metaindex-2.3.0/doc/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/addons.html` & `metaindex-2.3.0/doc/build/html/addons.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/changelog.html` & `metaindex-2.3.0/doc/build/html/changelog.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/cmdoptions.html` & `metaindex-2.3.0/doc/build/html/cmdoptions.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/cmdusage.html` & `metaindex-2.3.0/doc/build/html/cmdusage.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/configuration.html` & `metaindex-2.3.0/doc/build/html/configuration.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/description.html` & `metaindex-2.3.0/doc/build/html/description.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/examples.html` & `metaindex-2.3.0/doc/build/html/examples.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/extrametadata.html` & `metaindex-2.3.0/doc/build/html/extrametadata.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/genindex.html` & `metaindex-2.3.0/doc/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/index.html` & `metaindex-2.3.0/doc/build/html/index.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/indexers.html` & `metaindex-2.3.0/doc/build/html/indexers.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/install.html` & `metaindex-2.3.0/doc/build/html/install.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/license.html` & `metaindex-2.3.0/doc/build/html/license.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/objects.inv` & `metaindex-2.3.0/doc/build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/reference.html` & `metaindex-2.3.0/doc/build/html/reference.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/search.html` & `metaindex-2.3.0/doc/build/html/search.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/searchindex.js` & `metaindex-2.3.0/doc/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/searchsyntax.html` & `metaindex-2.3.0/doc/build/html/searchsyntax.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/synopsis.html` & `metaindex-2.3.0/doc/build/html/synopsis.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/build/html/usage.html` & `metaindex-2.3.0/doc/build/html/usage.html`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/cmdoptions.rst` & `metaindex-2.3.0/doc/cmdoptions.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/make.bat` & `metaindex-2.3.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/metaindex.rst` & `metaindex-2.3.0/doc/metaindex.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/addons.rst` & `metaindex-2.3.0/doc/source/addons.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/cmdoptions.rst` & `metaindex-2.3.0/doc/source/cmdoptions.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/cmdusage.rst` & `metaindex-2.3.0/doc/source/cmdusage.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/conf.py` & `metaindex-2.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/configuration.rst` & `metaindex-2.3.0/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/description.rst` & `metaindex-2.3.0/doc/source/description.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/examples.rst` & `metaindex-2.3.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/extrametadata.rst` & `metaindex-2.3.0/doc/source/extrametadata.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/indexers.rst` & `metaindex-2.3.0/doc/source/indexers.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/install.rst` & `metaindex-2.3.0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/reference.rst` & `metaindex-2.3.0/doc/source/reference.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/doc/source/searchsyntax.rst` & `metaindex-2.3.0/doc/source/searchsyntax.rst`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/examples/indexing.py` & `metaindex-2.3.0/examples/indexing.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/man/metaindex.1` & `metaindex-2.3.0/man/metaindex.1`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "METAINDEX"  "" "" ""
+.TH "METAINDEX"  "" ""
 .SH NAME
 metaindex \- document search by metadata
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
```

### Comparing `metaindex-2.2.2/metaindex/cache.py` & `metaindex-2.3.0/metaindex/cache.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/cacheentry.py` & `metaindex-2.3.0/metaindex/cacheentry.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/client.py` & `metaindex-2.3.0/metaindex/client.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/configuration.py` & `metaindex-2.3.0/metaindex/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 HERE = pathlib.Path(__file__).parent
 
 HOME = pathlib.Path().home()
 PROGRAMNAME = 'metaindex'
 CONFFILENAME = PROGRAMNAME + os.path.extsep + 'conf'
 CONFIGFILE = HOME / ".config" / CONFFILENAME
-CACHEPATH = HOME / ".cache" / PROGRAMNAME
+CACHEPATH = HOME / ".local" / 'state' / PROGRAMNAME
 DATAPATH = HOME / ".local" / "share" / PROGRAMNAME
-SOCKETPATH = HOME / ".local" / "state"
+SOCKETPATH = HOME / ".local" / "state" / PROGRAMNAME
 
 IGNORE_DIRS = [".git", ".svn", ".hg", ".bzr",
                "System Volume Information",
                ".stfolder",
                "__pycache__",
                "__MACOSX"]
 IGNORE_FILES = ['*.aux', '*.toc', '*.out', '*.log', '*.nav',
@@ -142,15 +142,14 @@
                 },
             }
 
 
 try:
     from xdg import BaseDirectory
     CONFIGFILE = pathlib.Path(BaseDirectory.load_first_config(CONFFILENAME) or CONFIGFILE)
-    CACHEPATH = pathlib.Path(BaseDirectory.save_cache_path(PROGRAMNAME) or CACHEPATH)
     DATAPATH = pathlib.Path(BaseDirectory.save_data_path(PROGRAMNAME) or DATAPATH)
     SOCKETPATH = pathlib.Path(BaseDirectory.get_runtime_dir() or SOCKETPATH)
 except ImportError:
     BaseDirectory = None
 
 SOCKETPATH /= SOCKETPATH / (PROGRAMNAME + '.sock')
```

### Comparing `metaindex-2.2.2/metaindex/docs/cmdoptions.html` & `metaindex-2.3.0/metaindex/docs/cmdoptions.html`

 * *Files 0% similar despite different names*

#### Comparing `metaindex-2.2.2/metaindex/docs/cmdoptions.html` & `metaindex-2.3.0/metaindex/docs/cmdoptions.html`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/"/>
+    <meta name="generator" content="Docutils 0.20.1: https://docutils.sourceforge.io/"/>
     <title>Options</title>
     <style type="text/css">/*
 :Author: David Goodger (goodger@python.org)
 :Id: $Id: html4css1.css 8954 2022-01-20 10:10:25Z milde $
 :Copyright: This stylesheet has been placed in the public domain.
 
 Default cascading style sheet for the HTML output of Docutils.
```

### Comparing `metaindex-2.2.2/metaindex/docs/metaindex.html` & `metaindex-2.3.0/metaindex/docs/metaindex.html`

 * *Files 0% similar despite different names*

#### Comparing `metaindex-2.2.2/metaindex/docs/metaindex.html` & `metaindex-2.3.0/metaindex/docs/metaindex.html`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/"/>
+    <meta name="generator" content="Docutils 0.20.1: https://docutils.sourceforge.io/"/>
     <title>metaindex</title>
     <style type="text/css">/*
 :Author: David Goodger (goodger@python.org)
 :Id: $Id: html4css1.css 8954 2022-01-20 10:10:25Z milde $
 :Copyright: This stylesheet has been placed in the public domain.
 
 Default cascading style sheet for the HTML output of Docutils.
```

### Comparing `metaindex-2.2.2/metaindex/find.py` & `metaindex-2.3.0/metaindex/find.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/fuse.py` & `metaindex-2.3.0/metaindex/fuse.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/humanizer.py` & `metaindex-2.3.0/metaindex/humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexer.py` & `metaindex-2.3.0/metaindex/indexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/__init__.py` & `metaindex-2.3.0/metaindex/indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/abc.py` & `metaindex-2.3.0/metaindex/indexers/abc.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/audio.py` & `metaindex-2.3.0/metaindex/indexers/audio.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/collections.py` & `metaindex-2.3.0/metaindex/indexers/collections.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/comicbook.py` & `metaindex-2.3.0/metaindex/indexers/comicbook.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/epub.py` & `metaindex-2.3.0/metaindex/indexers/epub.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/filetags.py` & `metaindex-2.3.0/metaindex/indexers/filetags.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/gpx.py` & `metaindex-2.3.0/metaindex/indexers/gpx.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/html.py` & `metaindex-2.3.0/metaindex/indexers/html.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/images.py` & `metaindex-2.3.0/metaindex/indexers/images.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/ooxml.py` & `metaindex-2.3.0/metaindex/indexers/ooxml.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/opendocument.py` & `metaindex-2.3.0/metaindex/indexers/opendocument.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/pdf.py` & `metaindex-2.3.0/metaindex/indexers/pdf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/indexers/ruleindexer.py` & `metaindex-2.3.0/metaindex/indexers/ruleindexer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/json.py` & `metaindex-2.3.0/metaindex/json.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/logger.py` & `metaindex-2.3.0/metaindex/logger.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/main.py` & `metaindex-2.3.0/metaindex/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from metaindex import stores
 from metaindex import indexer
 from metaindex import indexers
 from metaindex import logger
 from metaindex import version
 from metaindex.cache import Cache
 from metaindex.find import find
+from metaindex.cli import CLI
 
 try:
     from metaindex.fuse import metaindex_fs
 except ImportError:
     metaindex_fs = None
 
 
@@ -130,14 +131,16 @@
                                  "links but extend with the new search result.")
 
     findparser.add_argument('query',
                             nargs='*',
                             help="The search query. If the query is - it will "
                                  "be read from stdin.")
 
+    cliparser = subparsers.add_parser('cli')
+
     if metaindex_fs is not None:
         fsparser = subparsers.add_parser('fs')
 
         fsparser.add_argument('action',
                               choices=('mount', 'unmount', 'umount'),
                               help="The command to control the filesystem")
         fsparser.add_argument('mountpoint',
@@ -259,11 +262,14 @@
                 print(feedback)
 
         return 0
 
     if args.command == "find":
         return find(cache, args)
 
+    if args.command == "cli":
+        return CLI(cache).run()
+
     if args.command == 'fs' and metaindex_fs is not None:
         return metaindex_fs(config, args)
 
     return -1
```

### Comparing `metaindex-2.2.2/metaindex/ocr.py` & `metaindex-2.3.0/metaindex/ocr.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/opf.py` & `metaindex-2.3.0/metaindex/opf.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/proto.py` & `metaindex-2.3.0/metaindex/proto.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/server.py` & `metaindex-2.3.0/metaindex/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import hashlib
 import threading
 import shutil
 import json
 import os
 import sys
 import signal
+from pathlib import Path
 
 import xapian
 
 from metaindex import configuration
 from metaindex import logger
 from metaindex import proto
 from metaindex import shared
@@ -423,16 +424,14 @@
 
                 for value in values:
                     indexer.index_text(value)
 
             if 'filename' in self.config.implicit_tags:
                 indexer.index_text(entry.path.stem)
 
-            doc.set_data(json.dumps(entry.as_dict()))
-
             doc.add_value(SLOT_FILEPATH, strpath)
             doc.add_value(SLOT_LASTMODIFIED, entry.last_modified.strftime(shared.TIMESTAMP_FORMAT))
             doc.add_boolean_term(ID_PREFIX + pathid)
             if entry.storage_label is not None:
                 doc.add_term(BASE_TAGS['storage'] + str(entry.storage_label))
             if entry.rel_path is None:
                 doc.add_term(BASE_TAGS['rel_path'] + strpath)
@@ -444,14 +443,21 @@
             doc.add_term(BASE_TAGS['file'] + str(entry.path.stem))
 
             suffix = entry.path.suffix
             if suffix.startswith('.'):
                 suffix = suffix[1:]
             doc.add_term(BASE_TAGS['extension'] + suffix)
 
+            # do not store the fulltext in the data blob
+            to_delete = {tag for tag, _ in entry if tag.endswith('.fulltext')}
+            for tag in to_delete:
+                entry.delete(tag)
+
+            doc.set_data(json.dumps(entry.as_dict()))
+
             if docid is None:
                 dbconn.add_document(doc)
             else:
                 dbconn.replace_document(docid, doc)
 
         dbconn.commit_transaction()
         dbconn.close()
@@ -762,15 +768,14 @@
         if pid > 0:
             return True
     except OSError:
         return False
 
     os.chdir('/')
     os.setsid()
-    os.umask(0)
 
     if os.fork() > 0:
         return True
 
     sys.stdout.flush()
     sys.stderr.flush()
 
@@ -788,20 +793,22 @@
     args = parse_args()
 
     config = configuration.load(args.config)
     another_server = False
     if not args.stop:
         another_server = is_server_running(config)
     if not args.stop and another_server:
-        logger.info("Another server is already running")
+        print("Another server is already running", file=sys.stderr)
         return 1
 
     loglevel = args.log_level or config.get(configuration.SECTION_SERVER, configuration.CONFIG_LOGLEVEL)
     logfile = args.log_file or config.get(configuration.SECTION_SERVER, configuration.CONFIG_LOGFILE)
 
+    if logfile != '-':
+        Path(logfile).expanduser().parent.mkdir(parents=True, exist_ok=True)
     logger.setup(level=loglevel.upper(), filename=logfile)
 
     if args.stop:
         stop_running_server(config)
     elif args.detach:
         daemonize(config)
     else:
```

### Comparing `metaindex-2.2.2/metaindex/shared.py` & `metaindex-2.3.0/metaindex/shared.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,25 +164,34 @@
 def split_date_time(entry):
     """Given a CacheEntry with a 'extra.date' field, attempt to split that into 'date' and 'time'
 
     Returns ``entry`` for convenience, but modifies ``entry`` in place.
     """
     timestamps = entry.get(EXTRA + 'date')
     for timestamp in timestamps:
-        try:
-            text = timestamp.raw_value
-            if len(text) == 16:
-                # it’s too short, but maybe just doesn’t have the seconds
-                text += ':00'
-            dt = strpdt(text)
-            entry.delete((EXTRA + 'date', timestamp))
-            entry.add(EXTRA + 'date', dt.date())
-            entry.add(EXTRA + 'time', dt.time())
-        except ValueError:
-            continue
+        raw = timestamp.raw_value
+        if isinstance(raw, str):
+            try:
+                text = str(raw)
+                if len(text) == 16:
+                    # it’s too short, but maybe just doesn’t have the seconds
+                    text += ':00'
+                raw = strpdt(text)
+            except ValueError:
+                continue
+
+        entry.delete((EXTRA + 'date', timestamp))
+
+        if isinstance(raw, datetime.datetime):
+            entry.add(EXTRA + 'time', raw.time())
+            entry.add(EXTRA + 'date', raw.date())
+
+        elif isinstance(raw, datetime.date):
+            entry.add(EXTRA + 'date', raw)
+
     return entry
 
 
 def to_utf8(raw):
     """Decode a blob of bytes into a UTF-8 string
     
     Attempts to determine the encoding automatically
```

### Comparing `metaindex-2.2.2/metaindex/stores.py` & `metaindex-2.3.0/metaindex/stores.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/xmlproxy.py` & `metaindex-2.3.0/metaindex/xmlproxy.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex/yaml.py` & `metaindex-2.3.0/metaindex/yaml.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/metaindex.egg-info/PKG-INFO` & `metaindex-2.3.0/metaindex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaindex
-Version: 2.2.2
+Version: 2.3.0
 Summary: Utilities to tag files
 Home-page: https://vonshednob.cc/metaindex
 Author: R
 Author-email: devel+metaindex@kakaomilchkuh.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `metaindex-2.2.2/metaindex.egg-info/SOURCES.txt` & `metaindex-2.3.0/metaindex.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 doc/source/synopsis.rst
 doc/source/usage.rst
 examples/indexing.py
 man/metaindex.1
 metaindex/__init__.py
 metaindex/cache.py
 metaindex/cacheentry.py
+metaindex/cli.py
 metaindex/client.py
 metaindex/configuration.py
 metaindex/find.py
 metaindex/fuse.py
 metaindex/humanizer.py
 metaindex/indexer.py
 metaindex/json.py
```

### Comparing `metaindex-2.2.2/misc/metaindex.conf` & `metaindex-2.3.0/misc/metaindex.conf`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/misc/ranger_metaindex/linemode.py` & `metaindex-2.3.0/misc/ranger_metaindex/linemode.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/setup.py` & `metaindex-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_abc.py` & `metaindex-2.3.0/tests/test_abc.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_cache.py` & `metaindex-2.3.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_cacheentry.py` & `metaindex-2.3.0/tests/test_cacheentry.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_cleanup.py` & `metaindex-2.3.0/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_collect.py` & `metaindex-2.3.0/tests/test_collect.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_humanizer.py` & `metaindex-2.3.0/tests/test_humanizer.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_indexers.py` & `metaindex-2.3.0/tests/test_indexers.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_json.py` & `metaindex-2.3.0/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `metaindex-2.2.2/tests/test_ruleindexer.py` & `metaindex-2.3.0/tests/test_ruleindexer.py`

 * *Files identical despite different names*

