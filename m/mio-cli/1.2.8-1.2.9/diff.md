# Comparing `tmp/mio-cli-1.2.8.tar.gz` & `tmp/mio-cli-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/homes/dpoulin/git/mio_cli_client/dist/tmp7kbm2oge/mio-cli-1.2.8.tar", last modified: Tue May 16 19:23:31 2023, max compression
+gzip compressed data, was "/homes/dpoulin/git/mio_cli_client/dist/tmpvn1mr1fj/mio-cli-1.2.9.tar", last modified: Tue Jun 20 07:15:24 2023, max compression
```

## Comparing `mio-cli-1.2.8.tar` & `mio-cli-1.2.9.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-05-16 19:23:31.000000 mio-cli-1.2.8/
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/data/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.2.8/src/data/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio-cli-1.2.8/src/data/doxygen-awesome-darkmode-toggle.js
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio-cli-1.2.8/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio-cli-1.2.8/src/data/doxygen-awesome-sidebar-only.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio-cli-1.2.8/src/data/doxygen-awesome.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio-cli-1.2.8/src/data/doxygen.awesome.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio-cli-1.2.8/src/data/doxygen.private.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio-cli-1.2.8/src/data/doxygen.public.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio-cli-1.2.8/src/data/doxygen_footer.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio-cli-1.2.8/src/data/doxygen_header.awesome.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio-cli-1.2.8/src/data/doxygen_header.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio-cli-1.2.8/src/data/doxygen_layout.xml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio-cli-1.2.8/src/data/doxygen_stylesheet.css
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio-cli-1.2.8/src/data/idv_doxyfilter_sv.pl
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio-cli-1.2.8/src/data/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio-cli-1.2.8/src/data/plantuml.jar
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/gen/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.2.8/src/gen/__init__.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    12700 2023-01-11 01:30:17.000000 mio-cli-1.2.8/src/gen/new_agent_parallel.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     7144 2023-01-11 01:30:21.000000 mio-cli-1.2.8/src/gen/new_agent_serial.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     6901 2023-01-11 01:30:24.000000 mio-cli-1.2.8/src/gen/new_block.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     5279 2023-01-11 01:30:27.000000 mio-cli-1.2.8/src/gen/new_lib.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     4690 2023-01-11 01:30:39.000000 mio-cli-1.2.8/src/gen/new_ral.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    16761 2023-01-11 01:30:43.000000 mio-cli-1.2.8/src/gen/new_singleton.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     7297 2023-01-11 01:30:47.000000 mio-cli-1.2.8/src/gen/new_ss.py
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/mio/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio-cli-1.2.8/src/mio/__init__.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio-cli-1.2.8/src/mio/__main__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49803 2023-03-28 19:31:34.000000 mio-cli-1.2.8/src/mio/cache.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9051 2023-05-16 18:43:34.000000 mio-cli-1.2.8/src/mio/cfg.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio-cli-1.2.8/src/mio/clean.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21719 2023-05-16 18:55:51.000000 mio-cli-1.2.8/src/mio/cli.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8094 2023-03-23 09:22:45.000000 mio-cli-1.2.8/src/mio/common.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio-cli-1.2.8/src/mio/cov.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio-cli-1.2.8/src/mio/doctor.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio-cli-1.2.8/src/mio/dox.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    88811 2023-04-02 00:57:55.000000 mio-cli-1.2.8/src/mio/eal.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12554 2023-05-16 18:58:16.000000 mio-cli-1.2.8/src/mio/help_text.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio-cli-1.2.8/src/mio/init.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio-cli-1.2.8/src/mio/install.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-02-20 21:32:41.000000 mio-cli-1.2.8/src/mio/main.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3031 2023-02-20 21:32:41.000000 mio-cli-1.2.8/src/mio/new.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16358 2023-03-14 00:06:11.000000 mio-cli-1.2.8/src/mio/publish.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35707 2023-04-02 01:22:56.000000 mio-cli-1.2.8/src/mio/regr.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio-cli-1.2.8/src/mio/results.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    27750 2023-04-02 01:23:04.000000 mio-cli-1.2.8/src/mio/sim.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio-cli-1.2.8/src/mio/user.py
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/mio_cli.egg-info/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3898 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/mio_cli.egg-info/PKG-INFO
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2018 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/mio_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/mio_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       34 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/mio_cli.egg-info/entry_points.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio-cli-1.2.8/src/mio_cli.egg-info/not-zip-safe
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      142 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/mio_cli.egg-info/requires.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       23 2023-05-16 19:23:30.000000 mio-cli-1.2.8/src/mio_cli.egg-info/top_level.txt
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-05-16 19:23:31.000000 mio-cli-1.2.8/src/templates/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio-cli-1.2.8/src/templates/LICENSE_solderpad_v2p1.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio-cli-1.2.8/src/templates/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio-cli-1.2.8/src/templates/dv_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio-cli-1.2.8/src/templates/interactive_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio-cli-1.2.8/src/templates/mdc.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio-cli-1.2.8/src/templates/mdc.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio-cli-1.2.8/src/templates/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio-cli-1.2.8/src/templates/project_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio-cli-1.2.8/src/templates/qst.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio-cli-1.2.8/src/templates/qst.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio-cli-1.2.8/src/templates/regression_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio-cli-1.2.8/src/templates/riv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio-cli-1.2.8/src/templates/riv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio-cli-1.2.8/src/templates/rtl_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio-cli-1.2.8/src/templates/sim_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio-cli-1.2.8/src/templates/ts.yml.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio-cli-1.2.8/src/templates/vcs.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio-cli-1.2.8/src/templates/vcs.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio-cli-1.2.8/src/templates/viv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio-cli-1.2.8/src/templates/viv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio-cli-1.2.8/src/templates/viv.prj.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio-cli-1.2.8/src/templates/vivado_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio-cli-1.2.8/src/templates/xcl.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio-cli-1.2.8/src/templates/xcl.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio-cli-1.2.8/LICENSE
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3089 2023-02-20 21:32:07.000000 mio-cli-1.2.8/README.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio-cli-1.2.8/pyproject.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2134 2023-05-16 19:23:31.000000 mio-cli-1.2.8/setup.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3898 2023-05-16 19:23:31.000000 mio-cli-1.2.8/PKG-INFO
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-06-20 07:15:24.000000 mio-cli-1.2.9/
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/data/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.2.9/src/data/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio-cli-1.2.9/src/data/doxygen-awesome-darkmode-toggle.js
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio-cli-1.2.9/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio-cli-1.2.9/src/data/doxygen-awesome-sidebar-only.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio-cli-1.2.9/src/data/doxygen-awesome.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio-cli-1.2.9/src/data/doxygen.awesome.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio-cli-1.2.9/src/data/doxygen.private.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio-cli-1.2.9/src/data/doxygen.public.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio-cli-1.2.9/src/data/doxygen_footer.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio-cli-1.2.9/src/data/doxygen_header.awesome.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio-cli-1.2.9/src/data/doxygen_header.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio-cli-1.2.9/src/data/doxygen_layout.xml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio-cli-1.2.9/src/data/doxygen_stylesheet.css
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio-cli-1.2.9/src/data/idv_doxyfilter_sv.pl
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio-cli-1.2.9/src/data/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio-cli-1.2.9/src/data/plantuml.jar
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/gen/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.2.9/src/gen/__init__.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    12700 2023-01-11 01:30:17.000000 mio-cli-1.2.9/src/gen/new_agent_parallel.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     7144 2023-01-11 01:30:21.000000 mio-cli-1.2.9/src/gen/new_agent_serial.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     6901 2023-01-11 01:30:24.000000 mio-cli-1.2.9/src/gen/new_block.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     5279 2023-01-11 01:30:27.000000 mio-cli-1.2.9/src/gen/new_lib.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     4690 2023-01-11 01:30:39.000000 mio-cli-1.2.9/src/gen/new_ral.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    16761 2023-01-11 01:30:43.000000 mio-cli-1.2.9/src/gen/new_singleton.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)     7297 2023-01-11 01:30:47.000000 mio-cli-1.2.9/src/gen/new_ss.py
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/mio/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio-cli-1.2.9/src/mio/__init__.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio-cli-1.2.9/src/mio/__main__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49803 2023-03-28 19:31:34.000000 mio-cli-1.2.9/src/mio/cache.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9051 2023-05-16 18:43:34.000000 mio-cli-1.2.9/src/mio/cfg.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio-cli-1.2.9/src/mio/clean.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21827 2023-06-20 04:20:39.000000 mio-cli-1.2.9/src/mio/cli.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8094 2023-03-23 09:22:45.000000 mio-cli-1.2.9/src/mio/common.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio-cli-1.2.9/src/mio/cov.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio-cli-1.2.9/src/mio/doctor.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio-cli-1.2.9/src/mio/dox.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    88811 2023-04-02 00:57:55.000000 mio-cli-1.2.9/src/mio/eal.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12554 2023-06-20 06:59:39.000000 mio-cli-1.2.9/src/mio/help_text.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio-cli-1.2.9/src/mio/init.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio-cli-1.2.9/src/mio/install.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-02-20 21:32:41.000000 mio-cli-1.2.9/src/mio/main.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2676 2023-06-20 06:56:36.000000 mio-cli-1.2.9/src/mio/new.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16358 2023-03-14 00:06:11.000000 mio-cli-1.2.9/src/mio/publish.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35707 2023-04-02 01:22:56.000000 mio-cli-1.2.9/src/mio/regr.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio-cli-1.2.9/src/mio/results.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    27750 2023-04-02 01:23:04.000000 mio-cli-1.2.9/src/mio/sim.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio-cli-1.2.9/src/mio/user.py
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/mio_cli.egg-info/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3898 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/mio_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2018 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/mio_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/mio_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       34 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/mio_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio-cli-1.2.9/src/mio_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      142 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/mio_cli.egg-info/requires.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       23 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/mio_cli.egg-info/top_level.txt
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-06-20 07:15:24.000000 mio-cli-1.2.9/src/templates/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio-cli-1.2.9/src/templates/LICENSE_solderpad_v2p1.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio-cli-1.2.9/src/templates/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio-cli-1.2.9/src/templates/dv_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio-cli-1.2.9/src/templates/interactive_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio-cli-1.2.9/src/templates/mdc.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio-cli-1.2.9/src/templates/mdc.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio-cli-1.2.9/src/templates/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio-cli-1.2.9/src/templates/project_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio-cli-1.2.9/src/templates/qst.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio-cli-1.2.9/src/templates/qst.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio-cli-1.2.9/src/templates/regression_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio-cli-1.2.9/src/templates/riv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio-cli-1.2.9/src/templates/riv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio-cli-1.2.9/src/templates/rtl_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio-cli-1.2.9/src/templates/sim_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio-cli-1.2.9/src/templates/ts.yml.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio-cli-1.2.9/src/templates/vcs.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio-cli-1.2.9/src/templates/vcs.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio-cli-1.2.9/src/templates/viv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio-cli-1.2.9/src/templates/viv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio-cli-1.2.9/src/templates/viv.prj.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio-cli-1.2.9/src/templates/vivado_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio-cli-1.2.9/src/templates/xcl.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio-cli-1.2.9/src/templates/xcl.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio-cli-1.2.9/LICENSE
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3089 2023-02-20 21:32:07.000000 mio-cli-1.2.9/README.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio-cli-1.2.9/pyproject.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2134 2023-06-20 07:15:24.000000 mio-cli-1.2.9/setup.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3898 2023-06-20 07:15:24.000000 mio-cli-1.2.9/PKG-INFO
```

### Comparing `mio-cli-1.2.8/src/data/doxygen-awesome-darkmode-toggle.js` & `mio-cli-1.2.9/src/data/doxygen-awesome-darkmode-toggle.js`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css` & `mio-cli-1.2.9/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen-awesome-sidebar-only.css` & `mio-cli-1.2.9/src/data/doxygen-awesome-sidebar-only.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen-awesome.css` & `mio-cli-1.2.9/src/data/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen.awesome.cfg` & `mio-cli-1.2.9/src/data/doxygen.awesome.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen.private.cfg` & `mio-cli-1.2.9/src/data/doxygen.private.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen.public.cfg` & `mio-cli-1.2.9/src/data/doxygen.public.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen_footer.html` & `mio-cli-1.2.9/src/data/doxygen_footer.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen_header.awesome.html` & `mio-cli-1.2.9/src/data/doxygen_header.awesome.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen_header.html` & `mio-cli-1.2.9/src/data/doxygen_header.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen_layout.xml` & `mio-cli-1.2.9/src/data/doxygen_layout.xml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/doxygen_stylesheet.css` & `mio-cli-1.2.9/src/data/doxygen_stylesheet.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/idv_doxyfilter_sv.pl` & `mio-cli-1.2.9/src/data/idv_doxyfilter_sv.pl`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/mio.toml` & `mio-cli-1.2.9/src/data/mio.toml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/data/plantuml.jar` & `mio-cli-1.2.9/src/data/plantuml.jar`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/gen/new_agent_parallel.py` & `mio-cli-1.2.9/src/gen/new_agent_parallel.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/gen/new_agent_serial.py` & `mio-cli-1.2.9/src/gen/new_agent_serial.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/gen/new_block.py` & `mio-cli-1.2.9/src/gen/new_block.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/gen/new_lib.py` & `mio-cli-1.2.9/src/gen/new_lib.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/gen/new_ral.py` & `mio-cli-1.2.9/src/gen/new_ral.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/gen/new_singleton.py` & `mio-cli-1.2.9/src/gen/new_singleton.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/gen/new_ss.py` & `mio-cli-1.2.9/src/gen/new_ss.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/cache.py` & `mio-cli-1.2.9/src/mio/cache.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/cfg.py` & `mio-cli-1.2.9/src/mio/cfg.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/clean.py` & `mio-cli-1.2.9/src/mio/clean.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/cli.py` & `mio-cli-1.2.9/src/mio/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,16 +89,32 @@
     log_cli_args_to_disk()
     cache.scan_and_load_ip_metadata()
     
     if cli_args.command == 'init':
         init.new_ip(cfg.pwd)
         common.exit()
     if cli_args.command == 'gen':
-        #new.menu(cfg.cli_args.template)
-        common.banner(f"The UVMx generator will come online Monday May 22nd 2023.  Please perform an update on that date: `pip3 install --upgrade mio-cli`")
+        type = ""
+        if cli_args.all:
+            type = "all"
+        elif cli_args.agents:
+            type = "agent"
+        elif cli_args.blocks:
+            type = "block"
+        elif cli_args.reg:
+            type = "reg"
+        elif cli_args.ss:
+            type = "ss"
+        elif cli_args.chip:
+            type = "chip"
+        else:
+            type = "all"
+        if len(cli_args.entities) == 0:
+            cli_args.entities = ["*"]
+        new.main(cli_args.entities, type)
         common.exit()
     if cli_args.command == 'install':
         if (cli_args.username != None) and (cli_args.username != ""):
             if (cli_args.password == None) or (cli_args.password == ""):
                 common.fatal("Must specify both username AND password")
             else:
                 user.login(cli_args.username, cli_args.password, True)
@@ -177,21 +193,22 @@
     parser_help.add_argument("cmd",  help='Command whose documentation to print', choices=commands)
     
     parser_doctor = subparsers.add_parser('doctor', description=help_text.doctor_help_text, add_help=False)
     
     parser_init = subparsers.add_parser('init', description=help_text.init_help_text, add_help=False)
     
     parser_new = subparsers.add_parser('gen', help=help_text.new_help_text, add_help=False)
-    parser_new.add_argument("-z", "--all"  , help="Generates all entities"       , action="store_true", default=False, required=False, dest="gen_all"   )
-    parser_new.add_argument("-a", "--agent", help="Generates all agents"         , action="store_true", default=False, required=False, dest="gen_agents")
-    parser_new.add_argument("-b", "--block", help="Generates all blocks"         , action="store_true", default=False, required=False, dest="gen_blocks")
-    parser_new.add_argument("-r", "--reg"  , help="Generates all register models", action="store_true", default=False, required=False, dest="gen_reg"   )
-    parser_new.add_argument("-s", "--ss"   , help="Generates all sub-systems"    , action="store_true", default=False, required=False, dest="gen_ss"    )
-    parser_new.add_argument("-c", "--chip" , help="Generates all chips"          , action="store_true", default=False, required=False, dest="gen_chips" )
-    parser_new.add_argument("entities"     , help='Entities to be generated'     , nargs='+', default=["*"])
+    parser_new_type = parser_new.add_mutually_exclusive_group(required=True)
+    parser_new_type.add_argument("-z", "--all"  , help="Generates all entities"       , action="store_true")
+    parser_new_type.add_argument("-a", "--agent", help="Generates all agents"         , action="store_true")
+    parser_new_type.add_argument("-b", "--block", help="Generates all blocks"         , action="store_true")
+    parser_new_type.add_argument("-r", "--reg"  , help="Generates all register models", action="store_true")
+    parser_new_type.add_argument("-s", "--ss"   , help="Generates all sub-systems"    , action="store_true")
+    parser_new_type.add_argument("-c", "--chip" , help="Generates all chips"          , action="store_true")
+    parser_new.add_argument     ("entities"     , help='Entities to be generated'     , nargs='*', default=[])
     
     parser_install = subparsers.add_parser('install', help=help_text.install_help_text, add_help=False)
     parser_install.add_argument('ip'              , help='Target IP'                                       )
     parser_install.add_argument("-g", "--global"  , help="Install dependencies under '~/.mio'." , action="store_true", default=False, required=False, dest="is_global")
     parser_install.add_argument('-u', "--username", help='Moore.io IP Marketplace username', required=False)
     parser_install.add_argument('-p', "--password", help='Moore.io IP Marketplace password', required=False)
```

### Comparing `mio-cli-1.2.8/src/mio/common.py` & `mio-cli-1.2.9/src/mio/common.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/cov.py` & `mio-cli-1.2.9/src/mio/cov.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/doctor.py` & `mio-cli-1.2.9/src/mio/doctor.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/dox.py` & `mio-cli-1.2.9/src/mio/dox.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/eal.py` & `mio-cli-1.2.9/src/mio/eal.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/help_text.py` & `mio-cli-1.2.9/src/mio/help_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2021-2023 Datum Technology Corporation
 # SPDX-License-Identifier: GPL-3.0
 ########################################################################################################################
 
 
-version = "1.2.8"
+version = "1.2.9"
 version_text = f"Moore.io CLI Client v{version}"
 
 
 
 main_help_text = f"""
                                  Moore.io (`mio`) Command Line Interface (CLI) - v{version}
                                       User Manual: https://mio-cli.readthedocs.io/
```

### Comparing `mio-cli-1.2.8/src/mio/init.py` & `mio-cli-1.2.9/src/mio/init.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/install.py` & `mio-cli-1.2.9/src/mio/install.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/publish.py` & `mio-cli-1.2.9/src/mio/publish.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/regr.py` & `mio-cli-1.2.9/src/mio/regr.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/results.py` & `mio-cli-1.2.9/src/mio/results.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/sim.py` & `mio-cli-1.2.9/src/mio/sim.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio/user.py` & `mio-cli-1.2.9/src/mio/user.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/mio_cli.egg-info/PKG-INFO` & `mio-cli-1.2.9/src/mio_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.2.8
+Version: 1.2.9
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
```

### Comparing `mio-cli-1.2.8/src/mio_cli.egg-info/SOURCES.txt` & `mio-cli-1.2.9/src/mio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/templates/LICENSE_solderpad_v2p1.md` & `mio-cli-1.2.9/src/templates/LICENSE_solderpad_v2p1.md`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/templates/dv_ip.yml` & `mio-cli-1.2.9/src/templates/dv_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/templates/interactive_results.html.j2` & `mio-cli-1.2.9/src/templates/interactive_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/templates/regression_results.html.j2` & `mio-cli-1.2.9/src/templates/regression_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/templates/rtl_ip.yml` & `mio-cli-1.2.9/src/templates/rtl_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/templates/ts.yml.j2` & `mio-cli-1.2.9/src/templates/ts.yml.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/src/templates/vivado_ip.yml` & `mio-cli-1.2.9/src/templates/vivado_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/LICENSE` & `mio-cli-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/README.md` & `mio-cli-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `mio-cli-1.2.8/setup.cfg` & `mio-cli-1.2.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mio-cli
-version = 1.2.8
+version = 1.2.9
 author = Datum Technology Corporation
 author_email = mio@datumtc.ca
 description = The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = SystemVerilog, UVM, DV, verilog, VHDL, hdl, rtl, synthesis, FPGA, simulation, Xilinx, Altera
 url = https://datum-technology-corporation.github.io/mio_cli_client/
```

### Comparing `mio-cli-1.2.8/PKG-INFO` & `mio-cli-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.2.8
+Version: 1.2.9
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
```

