# Comparing `tmp/h5py-3.7.0.tar.gz` & `tmp/h5py-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5py-3.7.0.tar", last modified: Tue May 24 08:53:09 2022, max compression
+gzip compressed data, was "h5py-3.8.0.tar", last modified: Mon Jan 23 10:21:36 2023, max compression
```

## Comparing `h5py-3.7.0.tar` & `h5py-3.8.0.tar`

### file list

```diff
@@ -1,246 +1,249 @@
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.585142 h5py-3.7.0/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      407 2022-02-16 12:39:33.000000 h5py-3.7.0/.gitignore
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1520 2021-05-09 11:55:36.000000 h5py-3.7.0/LICENSE
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1037 2022-02-16 12:39:33.000000 h5py-3.7.0/MANIFEST.in
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1825 2022-05-24 08:53:09.584141 h5py-3.7.0/PKG-INFO
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1703 2022-02-16 12:39:33.000000 h5py-3.7.0/README.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10725 2022-03-21 15:18:18.000000 h5py-3.7.0/api_gen.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6858 2021-05-09 11:55:36.000000 h5py-3.7.0/asv.conf.json
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.504141 h5py-3.7.0/benchmarks/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2021-05-09 11:55:36.000000 h5py-3.7.0/benchmarks/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7089 2021-05-09 11:55:36.000000 h5py-3.7.0/benchmarks/benchmark_slicing.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1669 2021-05-09 11:55:36.000000 h5py-3.7.0/benchmarks/benchmarks.py
--rwxrwxr-x   0 takluyver  (1000) takluyver  (1000)      375 2022-02-16 12:39:33.000000 h5py-3.7.0/dev-install.sh
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.510141 h5py-3.7.0/docs/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6757 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/Makefile
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     9040 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/build.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8508 2022-05-24 08:44:52.000000 h5py-3.7.0/docs/conf.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2942 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/config.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16441 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/contributing.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10190 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/faq.rst
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.513141 h5py-3.7.0/docs/high/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3972 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/high/attr.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    24127 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/high/dataset.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3729 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/high/dims.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    21806 2022-05-23 15:29:34.000000 h5py-3.7.0/docs/high/file.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    18603 2022-05-23 15:29:34.000000 h5py-3.7.0/docs/high/group.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1363 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/high/lowlevel.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1375 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/index.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11708 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/licenses.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5131 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/mpi.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5733 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/quick.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3985 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/refs.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1201 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/release_guide.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       71 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/requirements-rtd.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     7866 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/special.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     5962 2022-02-09 11:00:47.000000 h5py-3.7.0/docs/strings.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6987 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/swmr.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5811 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/vds.rst
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.518141 h5py-3.7.0/docs/whatsnew/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7122 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.0.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1832 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.1.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5438 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.10.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2625 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.2.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2608 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.3.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1436 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.4.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2460 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/whatsnew/2.5.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2591 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/whatsnew/2.6.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1753 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.7.1.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4493 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/whatsnew/2.7.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3916 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.8.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1843 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/2.9.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10020 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/3.0.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      750 2021-05-09 11:55:36.000000 h5py-3.7.0/docs/whatsnew/3.1.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2043 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/whatsnew/3.2.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1928 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/whatsnew/3.3.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      639 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/whatsnew/3.4.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2040 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/whatsnew/3.5.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1060 2022-02-16 12:39:33.000000 h5py-3.7.0/docs/whatsnew/3.6.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2723 2022-05-24 08:44:52.000000 h5py-3.7.0/docs/whatsnew/3.7.rst
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      333 2022-05-24 08:44:52.000000 h5py-3.7.0/docs/whatsnew/index.rst
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.524141 h5py-3.7.0/docs_api/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6814 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/Makefile
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.524141 h5py-3.7.0/docs_api/_static/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/_static/.keep
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7563 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/automod.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8479 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/conf.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      639 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      428 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5a.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      114 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5ac.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      867 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5d.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       65 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5ds.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1298 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5f.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1204 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5fd.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      621 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5g.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      351 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5i.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      222 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5l.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      918 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5o.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1777 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5p.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       65 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5pl.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      521 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5r.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      933 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5s.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3796 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5t.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1099 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/h5z.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      663 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/index.rst
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)       96 2021-05-09 11:55:36.000000 h5py-3.7.0/docs_api/objects.rst
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.529141 h5py-3.7.0/examples/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      380 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/bytesio.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1831 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/collective_io.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1431 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/dataset_concatenation.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      903 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/dual_pco_edge.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      971 2022-05-23 15:29:34.000000 h5py-3.7.0/examples/eiger_use_case.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1308 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/excalibur_detector_modules.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1344 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/multiblockslice_interleave.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3539 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/multiprocessing_example.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1107 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/percival_use_case.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1339 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/store_and_retrieve_units_example.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      244 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/store_datetimes.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2673 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/swmr_inotify_example.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3865 2022-02-16 12:39:33.000000 h5py-3.7.0/examples/swmr_multiprocess.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10795 2022-02-16 12:39:33.000000 h5py-3.7.0/examples/threading_example.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1175 2021-05-09 11:55:36.000000 h5py-3.7.0/examples/vds_simple.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1260 2022-02-16 12:39:33.000000 h5py-3.7.0/examples/write-direct-compressed.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.549141 h5py-3.7.0/h5py/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3740 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/_conv.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    35396 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/_conv.pyx
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    20367 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/_errors.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     7513 2022-03-15 16:29:32.000000 h5py-3.7.0/h5py/_errors.pyx
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.559141 h5py-3.7.0/h5py/_hl/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      457 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/_hl/__init__.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10666 2022-04-05 12:41:30.000000 h5py-3.7.0/h5py/_hl/attrs.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    15669 2022-03-21 15:18:18.000000 h5py-3.7.0/h5py/_hl/base.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1375 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/_hl/compat.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    40933 2022-05-23 15:29:34.000000 h5py-3.7.0/h5py/_hl/dataset.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1548 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/_hl/datatype.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5422 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/_hl/dims.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    22505 2022-03-21 15:18:18.000000 h5py-3.7.0/h5py/_hl/files.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    13857 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/_hl/filters.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    25709 2022-05-23 15:29:34.000000 h5py-3.7.0/h5py/_hl/group.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    14478 2022-03-15 16:29:32.000000 h5py-3.7.0/h5py/_hl/selections.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2723 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/_hl/selections2.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     9353 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/_hl/vds.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4571 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/_locks.pxi
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      760 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/_objects.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10107 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/_objects.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      538 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/_proxy.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10834 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/_proxy.pyx
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    16151 2022-04-29 10:50:55.000000 h5py-3.7.0/h5py/_selector.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1431 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/api_compat.h
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    33917 2022-05-23 15:29:34.000000 h5py-3.7.0/h5py/api_functions.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1712 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/api_types_ext.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    30190 2022-03-21 15:18:18.000000 h5py-3.7.0/h5py/api_types_hdf5.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      688 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6842 2022-03-21 15:18:18.000000 h5py-3.7.0/h5py/h5.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      388 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5a.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    12817 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5a.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      383 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5ac.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5961 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5ac.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      406 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5d.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    21714 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5d.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5ds.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4802 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5ds.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      413 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5f.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    18888 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/h5f.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      448 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5fd.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     8309 2022-03-21 15:18:18.000000 h5py-3.7.0/h5py/h5fd.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      412 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5g.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    15721 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/h5g.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      394 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5i.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4053 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5i.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      358 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5l.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10000 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5l.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5o.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10381 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5o.pyx
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2072 2022-05-23 15:29:34.000000 h5py-3.7.0/h5py/h5p.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    57412 2022-05-23 15:29:34.000000 h5py-3.7.0/h5py/h5p.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      667 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5pl.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2354 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/h5pl.pyx
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      523 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/h5py_warnings.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      822 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5r.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5946 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5r.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      395 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5s.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18189 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5s.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1466 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5t.pxd
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    57093 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/h5t.pyx
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5z.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2970 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/h5z.pyx
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3642 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/ipy_completer.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.573141 h5py-3.7.0/h5py/tests/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      668 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/__init__.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6845 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/common.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      143 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/conftest.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.575141 h5py-3.7.0/h5py/tests/data_files/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      193 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/data_files/__init__.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6304 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/data_files/vlen_string_dset.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)   169904 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/data_files/vlen_string_dset_utc.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9008 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/data_files/vlen_string_s390x.h5
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2865 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_attribute_create.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     9577 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_attrs.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7646 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_attrs_data.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3816 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_base.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1445 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_big_endian_file.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1473 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_completions.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    68867 2022-05-23 15:29:34.000000 h5py-3.7.0/h5py/tests/test_dataset.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    18885 2022-04-29 10:50:55.000000 h5py-3.7.0/h5py/tests/test_dataset_getitem.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5825 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_dataset_swmr.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1007 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_datatype.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7942 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_dimension_scales.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      601 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_dims_dimensionproxy.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    17927 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_dtype.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2247 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_errors.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    33263 2022-03-21 15:18:18.000000 h5py-3.7.0/h5py/tests/test_file.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8854 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_file2.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4375 2022-03-15 16:25:38.000000 h5py-3.7.0/h5py/tests/test_file_alignment.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1524 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_file_image.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     3302 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_filters.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    35178 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_group.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1216 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_h5.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5358 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_h5d_direct_chunk.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4018 2022-03-21 15:18:18.000000 h5py-3.7.0/h5py/tests/test_h5f.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      508 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_h5o.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     7265 2022-05-23 15:29:34.000000 h5py-3.7.0/h5py/tests/test_h5p.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1999 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_h5pl.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6582 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_h5t.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      911 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_objects.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4564 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_selections.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    13874 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_slicing.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.578141 h5py-3.7.0/h5py/tests/test_vds/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      103 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_vds/__init__.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    17262 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_vds/test_highlevel_vds.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    12319 2022-02-16 12:39:33.000000 h5py-3.7.0/h5py/tests/test_vds/test_lowlevel_vds.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5932 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/tests/test_vds/test_virtual_source.py
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      870 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/utils.pxd
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5396 2021-05-09 11:55:36.000000 h5py-3.7.0/h5py/utils.pyx
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1910 2022-05-24 08:44:52.000000 h5py-3.7.0/h5py/version.py
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.550141 h5py-3.7.0/h5py.egg-info/
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     1825 2022-05-24 08:53:09.000000 h5py-3.7.0/h5py.egg-info/PKG-INFO
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4710 2022-05-24 08:53:09.000000 h5py-3.7.0/h5py.egg-info/SOURCES.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        1 2022-05-24 08:53:09.000000 h5py-3.7.0/h5py.egg-info/dependency_links.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       14 2022-05-24 08:53:09.000000 h5py-3.7.0/h5py.egg-info/requires.txt
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        5 2022-05-24 08:53:09.000000 h5py-3.7.0/h5py.egg-info/top_level.txt
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.580141 h5py-3.7.0/licenses/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3766 2021-05-09 11:55:36.000000 h5py-3.7.0/licenses/hdf5.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1739 2021-05-09 11:55:36.000000 h5py-3.7.0/licenses/license.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1640 2021-05-09 11:55:36.000000 h5py-3.7.0/licenses/pytables.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2503 2021-05-09 11:55:36.000000 h5py-3.7.0/licenses/python.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1394 2021-05-09 11:55:36.000000 h5py-3.7.0/licenses/stdint.txt
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.582141 h5py-3.7.0/lzf/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1556 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/LICENSE.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3328 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/README.txt
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2729 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/example.c
-drwxrwxr-x   0 takluyver  (1000) takluyver  (1000)        0 2022-05-24 08:53:09.583141 h5py-3.7.0/lzf/lzf/
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4406 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/lzf/lzf.h
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5445 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/lzf/lzfP.h
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9002 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/lzf/lzf_c.c
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4415 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/lzf/lzf_d.c
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7239 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/lzf_filter.c
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      861 2021-05-09 11:55:36.000000 h5py-3.7.0/lzf/lzf_filter.h
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11803 2021-05-09 11:55:36.000000 h5py-3.7.0/pylintrc
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)      386 2022-02-16 12:39:33.000000 h5py-3.7.0/pyproject.toml
--rw-r--r--   0 takluyver  (1000) takluyver  (1000)      109 2021-05-09 11:55:36.000000 h5py-3.7.0/pytest.ini
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       38 2022-05-24 08:53:09.585142 h5py-3.7.0/setup.cfg
--rwxrwxr-x   0 takluyver  (1000) takluyver  (1000)     4460 2022-05-24 08:44:52.000000 h5py-3.7.0/setup.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     6147 2022-04-05 12:41:30.000000 h5py-3.7.0/setup_build.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)    10525 2022-04-05 12:41:30.000000 h5py-3.7.0/setup_configure.py
--rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2341 2022-02-16 12:39:33.000000 h5py-3.7.0/tox.ini
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.019553 h5py-3.8.0/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      407 2022-12-21 16:13:47.000000 h5py-3.8.0/.gitignore
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1520 2021-05-09 11:55:36.000000 h5py-3.8.0/LICENSE
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1037 2022-12-21 16:13:47.000000 h5py-3.8.0/MANIFEST.in
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2442 2023-01-23 10:21:36.018553 h5py-3.8.0/PKG-INFO
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1712 2023-01-20 16:24:30.000000 h5py-3.8.0/README.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10725 2022-12-21 16:13:47.000000 h5py-3.8.0/api_gen.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6858 2021-05-09 11:55:36.000000 h5py-3.8.0/asv.conf.json
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.956553 h5py-3.8.0/benchmarks/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2021-05-09 11:55:36.000000 h5py-3.8.0/benchmarks/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7089 2021-05-09 11:55:36.000000 h5py-3.8.0/benchmarks/benchmark_slicing.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1669 2021-05-09 11:55:36.000000 h5py-3.8.0/benchmarks/benchmarks.py
+-rwxr-xr-x   0 takluyver  (1000) takluyver  (1000)      375 2022-12-21 16:13:47.000000 h5py-3.8.0/dev-install.sh
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.963553 h5py-3.8.0/docs/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6835 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/Makefile
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9459 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/build.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8513 2023-01-23 10:18:46.000000 h5py-3.8.0/docs/conf.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1224 2023-01-20 16:24:30.000000 h5py-3.8.0/docs/config.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    16467 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/contributing.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10212 2023-01-20 16:24:30.000000 h5py-3.8.0/docs/faq.rst
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.965553 h5py-3.8.0/docs/high/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3972 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/high/attr.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    24278 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/high/dataset.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3729 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/high/dims.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    23568 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/high/file.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    20381 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/high/group.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1363 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/high/lowlevel.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1382 2023-01-20 16:24:30.000000 h5py-3.8.0/docs/index.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11708 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/licenses.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5131 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/mpi.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5733 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/quick.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3985 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/refs.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4424 2023-01-20 16:24:30.000000 h5py-3.8.0/docs/related_projects.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1201 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/release_guide.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       71 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/requirements-rtd.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7866 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/special.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6041 2023-01-04 17:26:33.000000 h5py-3.8.0/docs/strings.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6987 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/swmr.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5811 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/vds.rst
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.970553 h5py-3.8.0/docs/whatsnew/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7122 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.0.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1832 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.1.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5438 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.10.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2625 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.2.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2608 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.3.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1436 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.4.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2460 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/2.5.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2591 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/2.6.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1753 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.7.1.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4493 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/2.7.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3916 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.8.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1843 2021-05-09 11:55:36.000000 h5py-3.8.0/docs/whatsnew/2.9.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10020 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.0.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      750 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.1.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2043 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.2.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1928 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.3.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      639 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.4.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2040 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.5.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1060 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.6.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2723 2022-12-21 16:13:47.000000 h5py-3.8.0/docs/whatsnew/3.7.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3016 2023-01-23 10:18:46.000000 h5py-3.8.0/docs/whatsnew/3.8.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      341 2023-01-23 10:18:46.000000 h5py-3.8.0/docs/whatsnew/index.rst
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.974553 h5py-3.8.0/docs_api/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6814 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/Makefile
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.974553 h5py-3.8.0/docs_api/_static/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)        0 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/_static/.keep
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7563 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/automod.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8479 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/conf.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      639 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      428 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5a.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      114 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5ac.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      867 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/h5d.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       65 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/h5ds.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1298 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5f.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1204 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/h5fd.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      621 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5g.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      351 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5i.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      222 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5l.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      918 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5o.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1777 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/h5p.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       65 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5pl.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      521 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5r.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      933 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5s.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3796 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5t.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1099 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/h5z.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      663 2022-12-21 16:13:47.000000 h5py-3.8.0/docs_api/index.rst
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       96 2021-05-09 11:55:36.000000 h5py-3.8.0/docs_api/objects.rst
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.977553 h5py-3.8.0/examples/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      380 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/bytesio.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1831 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/collective_io.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1431 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/dataset_concatenation.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      903 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/dual_pco_edge.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      971 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/eiger_use_case.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1308 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/excalibur_detector_modules.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1344 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/multiblockslice_interleave.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3539 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/multiprocessing_example.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1107 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/percival_use_case.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1339 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/store_and_retrieve_units_example.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      244 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/store_datetimes.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2673 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/swmr_inotify_example.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3865 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/swmr_multiprocess.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10795 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/threading_example.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1175 2021-05-09 11:55:36.000000 h5py-3.8.0/examples/vds_simple.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1260 2022-12-21 16:13:47.000000 h5py-3.8.0/examples/write-direct-compressed.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.995553 h5py-3.8.0/h5py/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3740 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/_conv.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    35396 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_conv.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    20382 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_errors.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7528 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_errors.pyx
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.999553 h5py-3.8.0/h5py/_hl/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      457 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/_hl/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10694 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/attrs.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    15669 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/base.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1375 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/compat.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    42162 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/dataset.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1548 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/datatype.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5407 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/dims.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    23981 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/files.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    13857 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/filters.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    27646 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_hl/group.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    14478 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/selections.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2723 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/selections2.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9353 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_hl/vds.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4571 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/_locks.pxi
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      760 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/_objects.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10107 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/_objects.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      538 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_proxy.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10834 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/_proxy.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    16418 2023-01-20 16:24:30.000000 h5py-3.8.0/h5py/_selector.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1431 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/api_compat.h
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    34257 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/api_functions.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1712 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/api_types_ext.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    33446 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/api_types_hdf5.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      688 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6842 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      388 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5a.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    12817 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5a.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      383 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5ac.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5961 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5ac.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      406 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5d.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    24596 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/h5d.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5ds.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4802 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5ds.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      413 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5f.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18888 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5f.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      448 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5fd.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8378 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/h5fd.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      412 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5g.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    15721 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5g.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      394 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5i.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4053 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5i.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      358 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5l.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10000 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5l.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5o.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10381 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5o.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2072 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5p.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    58333 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/h5p.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      667 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5pl.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2354 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5pl.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      523 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/h5py_warnings.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      822 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5r.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5946 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5r.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      389 2023-01-05 09:43:23.000000 h5py-3.8.0/h5py/h5s.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18189 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5s.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1460 2023-01-05 09:43:23.000000 h5py-3.8.0/h5py/h5t.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    57174 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/h5t.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      316 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5z.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2970 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/h5z.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3642 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/ipy_completer.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.011553 h5py-3.8.0/h5py/tests/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      668 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6845 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/common.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      547 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/conftest.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.012553 h5py-3.8.0/h5py/tests/data_files/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      193 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/data_files/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6304 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/data_files/vlen_string_dset.h5
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)   169904 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/data_files/vlen_string_dset_utc.h5
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9008 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/data_files/vlen_string_s390x.h5
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2865 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_attribute_create.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9577 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_attrs.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7646 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_attrs_data.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3816 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_base.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1445 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_big_endian_file.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1473 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_completions.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    73292 2023-01-10 17:06:37.000000 h5py-3.8.0/h5py/tests/test_dataset.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    18885 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_dataset_getitem.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5825 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_dataset_swmr.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1007 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_datatype.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     8307 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_dimension_scales.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      601 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_dims_dimensionproxy.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    17927 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_dtype.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2247 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_errors.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    32636 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_file.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    10340 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_file2.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4404 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_file_alignment.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1524 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_file_image.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3302 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_filters.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    36053 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_group.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1216 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_h5.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5358 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_h5d_direct_chunk.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4018 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_h5f.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      508 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_h5o.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7265 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_h5p.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1999 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_h5pl.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6582 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_h5t.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      911 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_objects.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1503 2023-01-04 17:26:33.000000 h5py-3.8.0/h5py/tests/test_ros3.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4852 2023-01-20 16:24:30.000000 h5py-3.8.0/h5py/tests/test_selections.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    13874 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_slicing.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.014553 h5py-3.8.0/h5py/tests/test_vds/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      103 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_vds/__init__.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    17262 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_vds/test_highlevel_vds.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    12319 2022-12-21 16:13:47.000000 h5py-3.8.0/h5py/tests/test_vds/test_lowlevel_vds.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5932 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/tests/test_vds/test_virtual_source.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      870 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/utils.pxd
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5396 2021-05-09 11:55:36.000000 h5py-3.8.0/h5py/utils.pyx
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1910 2023-01-23 10:18:46.000000 h5py-3.8.0/h5py/version.py
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:35.995553 h5py-3.8.0/h5py.egg-info/
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     2442 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/PKG-INFO
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)     4782 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/SOURCES.txt
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        1 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/dependency_links.txt
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)       14 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/requires.txt
+-rw-rw-r--   0 takluyver  (1000) takluyver  (1000)        5 2023-01-23 10:21:35.000000 h5py-3.8.0/h5py.egg-info/top_level.txt
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.015553 h5py-3.8.0/licenses/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3766 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/hdf5.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1739 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/license.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1640 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/pytables.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2503 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/python.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1394 2021-05-09 11:55:36.000000 h5py-3.8.0/licenses/stdint.txt
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.016553 h5py-3.8.0/lzf/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     1556 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/LICENSE.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     3330 2022-12-21 16:13:47.000000 h5py-3.8.0/lzf/README.txt
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2729 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/example.c
+drwxr-xr-x   0 takluyver  (1000) takluyver  (1000)        0 2023-01-23 10:21:36.018553 h5py-3.8.0/lzf/lzf/
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4406 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf/lzf.h
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     5445 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf/lzfP.h
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     9002 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf/lzf_c.c
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     4415 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf/lzf_d.c
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     7239 2022-12-21 16:13:47.000000 h5py-3.8.0/lzf/lzf_filter.c
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      861 2021-05-09 11:55:36.000000 h5py-3.8.0/lzf/lzf_filter.h
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11803 2021-05-09 11:55:36.000000 h5py-3.8.0/pylintrc
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2831 2023-01-20 16:24:30.000000 h5py-3.8.0/pyproject.toml
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)      171 2023-01-04 17:26:33.000000 h5py-3.8.0/pytest.ini
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)       38 2023-01-23 10:21:36.019553 h5py-3.8.0/setup.cfg
+-rwxr-xr-x   0 takluyver  (1000) takluyver  (1000)     2699 2023-01-23 10:18:46.000000 h5py-3.8.0/setup.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     6357 2023-01-04 17:26:33.000000 h5py-3.8.0/setup_build.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)    11595 2023-01-04 17:26:33.000000 h5py-3.8.0/setup_configure.py
+-rw-r--r--   0 takluyver  (1000) takluyver  (1000)     2807 2023-01-20 16:24:30.000000 h5py-3.8.0/tox.ini
```

### Comparing `h5py-3.7.0/LICENSE` & `h5py-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/MANIFEST.in` & `h5py-3.8.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/PKG-INFO` & `h5py-3.8.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 Metadata-Version: 2.1
 Name: h5py
-Version: 3.7.0
+Version: 3.8.0
 Summary: Read and write HDF5 files from Python
-Home-page: http://www.h5py.org
-Author: Andrew Collette
-Author-email: andrew.collette@gmail.com
-Maintainer: Andrew Collette
-Maintainer-email: andrew.collette@gmail.com
-License: BSD
-Download-URL: https://pypi.python.org/pypi/h5py
+Author-email: Andrew Collette <andrew.collette@gmail.com>
+Maintainer-email: Thomas Kluyver <thomas@kluyver.me.uk>, Thomas A Caswell <tcaswell@bnl.gov>
+License: BSD-3-Clause
+Project-URL: Homepage, https://www.h5py.org/
 Project-URL: Source, https://github.com/h5py/h5py
-Platform: UNKNOWN
+Project-URL: Documentation, https://docs.h5py.org/en/stable/
+Project-URL: Release notes, https://docs.h5py.org/en/stable/whatsnew/index.html
+Project-URL: Discussion forum, https://forum.hdfgroup.org/c/hdf-tools/h5py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
 The h5py package provides both a high- and low-level interface to the HDF5
 library from Python. The low-level interface is intended to be a complete
 wrapping of the HDF5 API, while the high-level component supports  access to
 HDF5 files, datasets and groups using established Python and NumPy concepts.
 
 A strong emphasis on automatic conversion between Python (Numpy) datatypes and
 data structures and their HDF5 equivalents vastly simplifies the process of
 reading and writing data from Python.
 
-Supports HDF5 versions 1.8.4 and higher.  On Windows, HDF5 is included with
-the installer.
-
+Wheels are provided for several popular platforms, with an included copy of
+the HDF5 library (usually the latest version when h5py is released).
 
+You can also `build h5py from source
+<https://docs.h5py.org/en/stable/build.html#source-installation>`_
+with any HDF5 stable release from version 1.8.4 onwards, although naturally new
+HDF5 versions released after this version of h5py may not work.
+Odd-numbered minor versions of HDF5 (e.g. 1.13) are experimental, and may not
+be supported.
```

### Comparing `h5py-3.7.0/README.rst` & `h5py-3.8.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -4,30 +4,30 @@
    :target: https://ci.appveyor.com/project/h5py/h5py/branch/master
 .. image:: https://dev.azure.com/h5pyappveyor/h5py/_apis/build/status/h5py.h5py?branchName=master
    :target: https://dev.azure.com/h5pyappveyor/h5py/_build/latest?definitionId=1&branchName=master
 
 HDF5 for Python
 ===============
 `h5py` is a thin, pythonic wrapper around `HDF5 <https://portal.hdfgroup.org/display/HDF5/>`_,
-which runs on Python 3 (3.6+).
+which runs on Python 3 (3.7+).
 
 Websites
 --------
 
 * Main website: https://www.h5py.org
 * Source code: https://github.com/h5py/h5py
-* Mailing list: https://groups.google.com/d/forum/h5py
+* Discussion forum: https://forum.hdfgroup.org/c/hdf-tools/h5py
 
 Installation
 ------------
 
 Pre-build `h5py` can either be installed via your Python Distribution (e.g.
 `Continuum Anaconda`_, `Enthought Canopy`_) or from `PyPI`_ via `pip`_.
 `h5py` is also distributed in many Linux Distributions (e.g. Ubuntu, Fedora),
-and in the MacOS package managers `Homebrew <https://brew.sh/>`_,
+and in the macOS package managers `Homebrew <https://brew.sh/>`_,
 `Macports <https://www.macports.org/>`_, or `Fink <http://finkproject.org/>`_.
 
 More detailed installation instructions, including how to install `h5py` with
 MPI support, can be found at: https://docs.h5py.org/en/latest/build.html.
 
 
 Reporting bugs
```

### Comparing `h5py-3.7.0/api_gen.py` & `h5py-3.8.0/api_gen.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/asv.conf.json` & `h5py-3.8.0/asv.conf.json`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/benchmarks/benchmark_slicing.py` & `h5py-3.8.0/benchmarks/benchmark_slicing.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/benchmarks/benchmarks.py` & `h5py-3.8.0/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/Makefile` & `h5py-3.8.0/docs/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -171,7 +171,10 @@
 	@echo
 	@echo "Build finished. The XML files are in $(BUILDDIR)/xml."
 
 pseudoxml:
 	$(SPHINXBUILD) -b pseudoxml $(ALLSPHINXOPTS) $(BUILDDIR)/pseudoxml
 	@echo
 	@echo "Build finished. The pseudo-XML files are in $(BUILDDIR)/pseudoxml."
+
+show:
+	@python -m webbrowser -t "file://$(shell pwd)/_build/html/index.html"
```

### Comparing `h5py-3.7.0/docs/build.rst` & `h5py-3.8.0/docs/build.rst`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,19 @@
 
 Source installation
 -------------------
 To install h5py from source, you need:
 
 * A supported Python version with development headers
 * HDF5 1.8.4 or newer with development headers
+
+  * HDF5 versions newer than the h5py version you're using might not work.
+  * Odd minor versions of HDF5 (e.g. 1.13) are experimental, and might not work.
+    Use a 'maintenance' version like 1.12.x if possible.
+
 * A C compiler
 
 On Unix platforms, you also need ``pkg-config`` unless you explicitly specify
 a path for HDF5 as described in :ref:`custom_install`.
 
 There are notes below on installing HDF5, Python and a C compiler on different
 platforms.
@@ -234,7 +239,11 @@
 
     $ export CC=mpicc
     $ export HDF5_MPI="ON"
     $ pip install --no-binary=h5py h5py
 
 You will need a shared-library build of Parallel HDF5 as well, i.e. built with
 ``./configure --enable-shared --enable-parallel``.
+
+On Windows, MS-MPI is usually used which does not have an ``mpicc`` wrapper.
+Instead, you may use the ``H5PY_MSMPI`` environment variable to ``ON`` in
+order to query the system for MS-MPI's information.
```

### Comparing `h5py-3.7.0/docs/conf.py` & `h5py-3.8.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,18 @@
         'sphinx.ext.extlinks',
         'sphinx.ext.mathjax',
 ]
 
 intersphinx_mapping = {'low': ('https://api.h5py.org', None)}
 
 extlinks = {
-    'issue': ('https://github.com/h5py/h5py/issues/%s', 'GH'),
-    'pr': ('https://github.com/h5py/h5py/pull/%s', 'PR '),
+    'issue': ('https://github.com/h5py/h5py/issues/%s', 'GH%s'),
+    'pr': ('https://github.com/h5py/h5py/pull/%s', 'PR %s'),
 }
+
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = '.rst'
 
 # The encoding of source files.
@@ -57,15 +58,15 @@
 copyright = '2014, Andrew Collette and contributors'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
-release = '3.7.0'
+release = '3.8.0'
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
```

### Comparing `h5py-3.7.0/docs/contributing.rst` & `h5py-3.8.0/docs/contributing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 
 Contributions and bug reports are welcome from anyone!  Some of the best
 features in h5py, including thread support, dimension scales, and the
 scale-offset filter, came from user code contributions.
 
 Since we use GitHub, the workflow will be familiar to many people.
 If you have questions about the process or about the details of implementing
-your feature, always feel free to ask on the Google Groups list, either
-by emailing:
+your feature, feel free to ask on Github itself, or on the h5py section of the
+HDF5 forum:
 
-     h5py@googlegroups.com
+    https://forum.hdfgroup.org/c/hdf-tools/h5py
 
-or via the web interface at:
-
-    https://groups.google.com/forum/#!forum/h5py
+Posting on this forum requires registering for a free account with HDF group.
 
 Anyone can post to this list. Your first message will be approved by a
 moderator, so don't worry if there's a brief delay.
 
 This guide is divided into three sections.  The first describes how to file
 a bug report.
```

### Comparing `h5py-3.7.0/docs/faq.rst` & `h5py-3.8.0/docs/faq.rst`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
 sec2                                Standard optimized driver                   Default on UNIX/Windows
 stdio                               Buffered I/O using stdio.h
 core                                In-memory file (optionally backed to disk)
 family                              Multi-file driver
 mpio                                Parallel HDF5 file access
 =================================== =========================================== ============================
 
+.. _h5py_pytable_cmp:
 
 What's the difference between h5py and PyTables?
 ------------------------------------------------
 
 The two projects have different design goals. PyTables presents a database-like
 approach to data storage, providing features like indexing and fast "in-kernel"
 queries on dataset contents. It also has a custom system to represent data types.
```

### Comparing `h5py-3.7.0/docs/high/attr.rst` & `h5py-3.8.0/docs/high/attr.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/high/dataset.rst` & `h5py-3.8.0/docs/high/dataset.rst`

 * *Files 1% similar despite different names*

```diff
@@ -658,14 +658,19 @@
 
        True if this dataset is a :doc:`virtual dataset </vds>`, otherwise False.
 
     .. attribute:: dims
 
         Access to :ref:`dimension_scales`.
 
+    .. attribute:: is_scale
+
+        Return ``True`` if the dataset is also a :ref:`dimension scale <dimension_scales>`,
+        ``False`` otherwise.
+
     .. attribute:: attrs
 
         :ref:`attributes` for this dataset.
 
     .. attribute:: id
 
         The dataset's low-level identifier; an instance of
```

### Comparing `h5py-3.7.0/docs/high/dims.rst` & `h5py-3.8.0/docs/high/dims.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/high/file.rst` & `h5py-3.8.0/docs/high/file.rst`

 * *Files 4% similar despite different names*

```diff
@@ -92,26 +92,32 @@
         meta_ext:
           Metadata filename extension. Default is '-m.h5'.
 
         raw_ext:
           Raw data filename extension. Default is '-r.h5'.
 
     'ros3'
-        Allows read only access to HDF5 files on S3. Keywords:
+        Allows read-only access to HDF5 files in AWS S3 or S3 compatible object
+        stores. HDF5 file name must be one of \http://, \https://, or s3://
+        resource location. An s3:// location will be translated into an AWS
+        `path-style <https://docs.aws.amazon.com/AmazonS3/latest/userguide/VirtualHosting.html#path-style-access>`_
+        location. Keywords:
 
         aws_region:
-          Name of the AWS "region" where the S3 bucket with the file is, e.g. ``b"us-east-1"``. Default is ``b''``.
+          AWS region of the S3 bucket with the file, e.g. ``b"us-east-1"``.
+          Default is ``b''``. Required for s3:// locations.
 
         secret_id:
-          "Access ID" for the resource. Default is ``b''``.
+          AWS access key ID. Default is ``b''``.
 
         secret_key:
-          "Secret Access Key" associated with the ID and resource. Default is ``b''``.
+          AWS secret access key. Default is ``b''``.
 
-        The argument values must be ``bytes`` objects.
+        The argument values must be ``bytes`` objects. All three arguments are
+        required to activate AWS authentication.
 
 
 .. _file_fileobj:
 
 Python file-like objects
 ------------------------
 
@@ -323,18 +329,18 @@
 possible those chunks are cached in memory, so that if the user requests a
 different part of a chunk that has already been read, the data can be copied
 directly from memory rather than reading the file again.  The details of a
 given dataset's chunks are controlled when creating the dataset, but it is
 possible to adjust the behavior of the chunk *cache* when opening the file.
 
 The parameters controlling this behavior are prefixed by ``rdcc``, for *raw data
-chunk cache*.
+chunk cache*. They apply to all datasets unless specifically changed for each one.
 
 * ``rdcc_nbytes`` sets the total size (measured in bytes) of the raw data chunk
-  cache for each dataset.  The default size is 1 MB.
+  cache for each dataset.  The default size is 1 MiB.
   This should be set to the size of each chunk times the number of
   chunks that are likely to be needed in cache.
 * ``rdcc_w0`` sets the policy for chunks to be
   removed from the cache when more space is needed.  If the value is set to 0,
   then the library will always evict the least recently used chunk in cache.  If
   the value is set to 1, the library will always evict the least recently used
   chunk which has been fully read or written, and if none have been fully read
@@ -382,14 +388,29 @@
 constructor help control the threshold in bytes where the data alignment policy
 takes effect and the alignment in bytes within the file. The alignment is
 measured from the end of the user block.
 
 For more information, see the official HDF5 documentation `H5P_SET_ALIGNMENT
 <https://portal.hdfgroup.org/display/HDF5/H5P_SET_ALIGNMENT>`_.
 
+.. _file_meta_block_size:
+
+Meta block size
+---------------
+
+Space for metadata is allocated in blocks within the HDF5 file. The argument
+``meta_block_size`` of the :class:`File` constructor sets the minimum size of
+these blocks.  Setting a large value can consolidate metadata into a small
+number of regions. Setting a small value can reduce the overall file size,
+especially in combination with the ``libver`` option. This controls how the
+overall data and metadata are laid out within the file.
+
+For more information, see the offical HDF5 documentation `H5P_SET_META_BLOCK_SIZE
+<https://portal.hdfgroup.org/display/HDF5/H5P_SET_META_BLOCK_SIZE>`_.
+
 Reference
 ---------
 
 .. note::
 
     Unlike Python file objects, the attribute :attr:`File.name` gives the
     HDF5 name of the root group, "``/``". To access the on-disk name, use
@@ -427,42 +448,55 @@
     :param rdcc_nslots:  Number of chunk slots in the raw data chunk cache for
                     this file.  Default value is 521.
     :param track_order:  Track dataset/group/attribute creation order under
                     root group if ``True``.  Default is
                     ``h5.get_config().track_order``.
     :param fs_strategy: The file space handling strategy to be used.
             Only allowed when creating a new file. One of "fsm", "page",
-            "aggregate", "none", or None (to use the HDF5 default).
+            "aggregate", "none", or ``None`` (to use the HDF5 default).
     :param fs_persist: A boolean to indicate whether free space should be
             persistent or not. Only allowed when creating a new file. The
             default is False.
+    :param fs_page_size: File space page size in bytes. Only use when
+            fs_strategy="page". If ``None`` use the HDF5 default (4096 bytes).
     :param fs_threshold: The smallest free-space section size that the free
             space manager will track. Only allowed when creating a new file.
             The default is 1.
     :param page_buf_size: Page buffer size in bytes. Only allowed for HDF5 files
             created with fs_strategy="page". Must be a power of two value and
             greater or equal than the file space page size when creating the
             file. It is not used by default.
     :param min_meta_keep: Minimum percentage of metadata to keep in the page
             buffer before allowing pages containing metadata to be evicted.
             Applicable only if ``page_buf_size`` is set. Default value is zero.
     :param min_raw_keep: Minimum percentage of raw data to keep in the page
             buffer before allowing pages containing raw data to be evicted.
             Applicable only if ``page_buf_size`` is set. Default value is zero.
-    :param locking: The file locking behavior. One of False (or "false"), True
-            (or "true"), "best-effort", or None. Warning: The
-            HDF5_USE_FILE_LOCKING environment variable can override this
-            parameter. Only available with HDF5 >= 1.12.1 or 1.10.x >= 1.10.7.
+    :param locking: The file locking behavior. One of:
+
+            - False (or "false") --  Disable file locking
+            - True (or "true")   --  Enable file locking
+            - "best-effort"      --  Enable file locking but ignore some errors
+            - None               --  Use HDF5 defaults
+
+            .. warning::
+
+                The HDF5_USE_FILE_LOCKING environment variable can override
+                this parameter.
+
+            Only available with HDF5 >= 1.12.1 or 1.10.x >= 1.10.7.
     :param alignment_threshold: Together with ``alignment_interval``, this
             property ensures that any file object greater than or equal
             in size to the alignement threshold (in bytes) will be
             aligned on an address which is a multiple of alignment interval.
     :param alignment_interval: This property should be used in conjunction with
             ``alignment_threshold``. See the description above. For more
             details, see :ref:`file_alignment`.
+    :param meta_block_size: Determines the current minimum size, in bytes, of
+            new metadata block allocations. See :ref:`file_meta_block_size`.
     :param kwds:    Driver-specific keywords; see :ref:`file_driver`.
 
     .. method:: __bool__()
 
         Check that the file descriptor is valid and the file open:
 
             >>> f = h5py.File(filename)
@@ -508,7 +542,12 @@
     .. attribute:: libver
 
         2-tuple with library version settings.  See :ref:`file_version`.
 
     .. attribute:: userblock_size
 
         Size of user block (in bytes).  Generally 0.  See :ref:`file_userblock`.
+
+    .. attribute:: meta_block_size
+
+        Minimum size, in bytes, of metadata block allocations. Default: 2048.
+        See :ref`file_meta_block_size`.
```

### Comparing `h5py-3.7.0/docs/high/group.rst` & `h5py-3.8.0/docs/high/group.rst`

 * *Files 5% similar despite different names*

```diff
@@ -380,32 +380,63 @@
             ``(name, offset, size)`` to store data from ``offset`` to
             ``offset + size`` in the named file. Each name must be a str,
             bytes, or os.PathLike; each offset and size, an integer. The last
             file in the sequence may have size ``h5py.h5f.UNLIMITED`` to let
             it grow as needed. If only a name is given instead of an iterable
             of tuples, it is equivalent to
             ``[(name, 0, h5py.h5f.UNLIMITED)]``.
+
         :keyword allow_unknown_filter: Do not check that the requested filter is
             available for use (T/F). This should only be set if you will
             write any data with ``write_direct_chunk``, compressing the
             data before passing it to h5py.
 
-    .. method:: require_dataset(name, shape=None, dtype=None, exact=None, **kwds)
+        :keyword rdcc_nbytes: Total size of the dataset's chunk cache in bytes.
+            The default size is 1024**2 (1 MiB).
+
+        :keyword rdcc_w0: The chunk preemption policy for this dataset. This
+            must be between 0 and 1 inclusive and indicates the weighting
+            according to which chunks which have been fully read or written are
+            penalized when determining which chunks to flush from cache. A value
+            of 0 means fully read or written chunks are treated no differently
+            than other chunks (the preemption is strictly LRU) while a value of
+            1 means fully read or written chunks are always preempted before
+            other chunks. If your application only reads or writes data once,
+            this can be safely set to 1. Otherwise, this should be set lower
+            depending on how often you re-read or re-write the same data. The
+            default value is 0.75.
+
+        :keyword rdcc_nslots: The number of chunk slots in the dataset's chunk
+            cache. Increasing this value reduces the number of cache collisions,
+            but slightly increases the memory used. Due to the hashing strategy,
+            this value should ideally be a prime number. As a rule of thumb,
+            this value should be at least 10 times the number of chunks that can
+            fit in rdcc_nbytes bytes. For maximum performance, this value should
+            be set approximately 100 times that number of chunks. The default
+            value is 521.
+
+    .. method:: require_dataset(name, shape, dtype, exact=False, **kwds)
 
         Open a dataset, creating it if it doesn't exist.
 
         If keyword "exact" is False (default), an existing dataset must have
         the same shape and a conversion-compatible dtype to be returned.  If
         True, the shape and dtype must match exactly.
 
+        If keyword "maxshape" is given, the maxshape and dtype must match
+        instead.
+
+        If any of the keywords "rdcc_nslots", "rdcc_nbytes", or "rdcc_w0" are
+        given, they will be used to configure the dataset's chunk cache.
+
         Other dataset keywords (see create_dataset) may be provided, but are
         only used if a new dataset is to be created.
 
         Raises TypeError if an incompatible object already exists, or if the
-        shape or dtype don't match according to the above rules.
+        shape, maxshape or dtype don't match according to the above rules.
 
         :keyword exact:     Require shape and type to match exactly (T/**F**)
 
 
     .. method:: create_dataset_like(name, other, **kwds)
 
         Create a dataset similar to `other`, much like numpy's `_like` functions.
```

### Comparing `h5py-3.7.0/docs/high/lowlevel.rst` & `h5py-3.8.0/docs/high/lowlevel.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/index.rst` & `h5py-3.8.0/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 * :ref:`Installation <install>`
 
 
 Other resources
 ---------------
 
 * `Python and HDF5 O'Reilly book <https://shop.oreilly.com/product/0636920030249.do>`_
-* `Ask questions on the mailing list at Google Groups <http://groups.google.com/d/forum/h5py>`_
+* `Ask questions on the HDF forum <https://forum.hdfgroup.org/c/hdf-tools/h5py>`_
 * `GitHub project <https://github.com/h5py/h5py>`_
 
 
 Introductory info
 -----------------
 
 .. toctree::
@@ -57,14 +57,15 @@
     config
     special
     strings
     refs
     mpi
     swmr
     vds
+    related_projects
 
 
 Meta-info about the h5py project
 --------------------------------
 
 .. toctree::
     :maxdepth: 1
```

### Comparing `h5py-3.7.0/docs/licenses.rst` & `h5py-3.8.0/docs/licenses.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/mpi.rst` & `h5py-3.8.0/docs/mpi.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/quick.rst` & `h5py-3.8.0/docs/quick.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/refs.rst` & `h5py-3.8.0/docs/refs.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/release_guide.rst` & `h5py-3.8.0/docs/release_guide.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/special.rst` & `h5py-3.8.0/docs/special.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/strings.rst` & `h5py-3.8.0/docs/strings.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 ---------------
 
 String data in HDF5 datasets is read as bytes by default: ``bytes`` objects
 for variable-length strings, or numpy bytes arrays (``'S'`` dtypes) for
 fixed-length strings. Use :meth:`.Dataset.asstr` to retrieve ``str`` objects.
 
 Variable-length strings in attributes are read as ``str`` objects. These are
-decoded as UTF-8 with surrogate escaping for unrecognised bytes.
+decoded as UTF-8 with surrogate escaping for unrecognised bytes. Fixed-length
+strings are read as numpy bytes arrays, the same as for datasets.
 
 Storing strings
 ---------------
 
 When creating a new dataset or attribute, Python ``str`` or ``bytes`` objects
 will be treated as variable-length strings, marked as UTF-8 and ASCII respectively.
 Numpy bytes arrays (``'S'`` dtypes) make fixed-length strings.
```

### Comparing `h5py-3.7.0/docs/swmr.rst` & `h5py-3.8.0/docs/swmr.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/vds.rst` & `h5py-3.8.0/docs/vds.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.0.rst` & `h5py-3.8.0/docs/whatsnew/2.0.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.1.rst` & `h5py-3.8.0/docs/whatsnew/2.1.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.10.rst` & `h5py-3.8.0/docs/whatsnew/2.10.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.2.rst` & `h5py-3.8.0/docs/whatsnew/2.2.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.3.rst` & `h5py-3.8.0/docs/whatsnew/2.3.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.4.rst` & `h5py-3.8.0/docs/whatsnew/2.4.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.5.rst` & `h5py-3.8.0/docs/whatsnew/2.5.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.6.rst` & `h5py-3.8.0/docs/whatsnew/2.6.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.7.1.rst` & `h5py-3.8.0/docs/whatsnew/2.7.1.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.7.rst` & `h5py-3.8.0/docs/whatsnew/2.7.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.8.rst` & `h5py-3.8.0/docs/whatsnew/2.8.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/2.9.rst` & `h5py-3.8.0/docs/whatsnew/2.9.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/3.0.rst` & `h5py-3.8.0/docs/whatsnew/3.0.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/3.1.rst` & `h5py-3.8.0/docs/whatsnew/3.1.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/3.2.rst` & `h5py-3.8.0/docs/whatsnew/3.2.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/3.3.rst` & `h5py-3.8.0/docs/whatsnew/3.3.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/3.4.rst` & `h5py-3.8.0/docs/whatsnew/3.4.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/3.5.rst` & `h5py-3.8.0/docs/whatsnew/3.5.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/3.6.rst` & `h5py-3.8.0/docs/whatsnew/3.6.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs/whatsnew/3.7.rst` & `h5py-3.8.0/docs/whatsnew/3.7.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/Makefile` & `h5py-3.8.0/docs_api/Makefile`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/automod.py` & `h5py-3.8.0/docs_api/automod.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/conf.py` & `h5py-3.8.0/docs_api/conf.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5.rst` & `h5py-3.8.0/docs_api/h5.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5d.rst` & `h5py-3.8.0/docs_api/h5d.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5f.rst` & `h5py-3.8.0/docs_api/h5f.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5fd.rst` & `h5py-3.8.0/docs_api/h5fd.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5g.rst` & `h5py-3.8.0/docs_api/h5g.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5o.rst` & `h5py-3.8.0/docs_api/h5o.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5p.rst` & `h5py-3.8.0/docs_api/h5p.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5r.rst` & `h5py-3.8.0/docs_api/h5r.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5s.rst` & `h5py-3.8.0/docs_api/h5s.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5t.rst` & `h5py-3.8.0/docs_api/h5t.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/h5z.rst` & `h5py-3.8.0/docs_api/h5z.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/docs_api/index.rst` & `h5py-3.8.0/docs_api/index.rst`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/collective_io.py` & `h5py-3.8.0/examples/collective_io.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/dataset_concatenation.py` & `h5py-3.8.0/examples/dataset_concatenation.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/dual_pco_edge.py` & `h5py-3.8.0/examples/dual_pco_edge.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/eiger_use_case.py` & `h5py-3.8.0/examples/eiger_use_case.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/excalibur_detector_modules.py` & `h5py-3.8.0/examples/excalibur_detector_modules.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/multiblockslice_interleave.py` & `h5py-3.8.0/examples/multiblockslice_interleave.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/multiprocessing_example.py` & `h5py-3.8.0/examples/multiprocessing_example.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/percival_use_case.py` & `h5py-3.8.0/examples/percival_use_case.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/store_and_retrieve_units_example.py` & `h5py-3.8.0/examples/store_and_retrieve_units_example.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/swmr_inotify_example.py` & `h5py-3.8.0/examples/swmr_inotify_example.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/swmr_multiprocess.py` & `h5py-3.8.0/examples/swmr_multiprocess.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/threading_example.py` & `h5py-3.8.0/examples/threading_example.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/vds_simple.py` & `h5py-3.8.0/examples/vds_simple.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/examples/write-direct-compressed.py` & `h5py-3.8.0/examples/write-direct-compressed.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/__init__.py` & `h5py-3.8.0/h5py/__init__.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_conv.pyx` & `h5py-3.8.0/h5py/_conv.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_errors.pxd` & `h5py-3.8.0/h5py/_errors.pxd`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
 
     ctypedef herr_t (*H5E_auto_t)(void *client_data)
     herr_t    H5Eset_auto(hid_t estack_id, H5E_auto_t func, void *client_data) nogil
     herr_t    H5Eget_auto(hid_t estack_id, H5E_auto_t *func, void** client_data)
 
     herr_t    H5Eprint(hid_t estack_id, void *stream)
 
-    ctypedef herr_t (*H5E_walk_t)(int n, H5E_error_t *err_desc, void* client_data)
+    ctypedef herr_t (*H5E_walk_t)(unsigned int n, const H5E_error_t *err_desc, void* client_data)
     herr_t    H5Ewalk(hid_t estack_id, H5E_direction_t direction, H5E_walk_t func, void* client_data)
 
 # --- Functions for managing the HDF5 error callback mechanism ---
 
 ctypedef struct err_cookie:
     # Defines the error handler state (callback and callback data)
     H5E_auto_t func
```

### Comparing `h5py-3.7.0/h5py/_errors.pyx` & `h5py-3.8.0/h5py/_errors.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     _minor_table[H5E_BADID] = ValueError  # Unable to find ID information
     _exact_table[(H5E_SYM, H5E_CANTCREATE)] = ValueError  # Object already exists
 
 cdef struct err_data_t:
     H5E_error_t err
     int n
 
-cdef herr_t walk_cb(int n, H5E_error_t *desc, void *e) nogil:
+cdef herr_t walk_cb(unsigned int n, const H5E_error_t *desc, void *e) nogil:
 
     cdef err_data_t *ee = <err_data_t*>e
 
     ee[0].err.maj_num = desc[0].maj_num
     ee[0].err.min_num = desc[0].min_num
     ee[0].err.desc = desc[0].desc
     ee[0].n = n
```

### Comparing `h5py-3.7.0/h5py/_hl/attrs.py` & `h5py-3.8.0/h5py/_hl/attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,21 @@
         self._id = parent.id
 
     @with_phil
     def __getitem__(self, name):
         """ Read the value of an attribute.
         """
         attr = h5a.open(self._id, self._e(name))
+        shape = attr.shape
 
-        if is_empty_dataspace(attr):
+        # shape is None for empty dataspaces
+        if shape is None:
             return Empty(attr.dtype)
 
         dtype = attr.dtype
-        shape = attr.shape
 
         # Do this first, as we'll be fiddling with the dtype for top-level
         # array types
         htype = h5t.py_create(dtype)
 
         # NumPy doesn't support top-level array types, so we have to "fake"
         # the correct type and shape for the array.  For example, consider
@@ -79,15 +80,15 @@
         string_info = h5t.check_string_dtype(dtype)
         if string_info and (string_info.length is None):
             # Vlen strings: convert bytes to Python str
             arr = numpy.array([
                 b.decode('utf-8', 'surrogateescape') for b in arr.flat
             ], dtype=dtype).reshape(arr.shape)
 
-        if len(arr.shape) == 0:
+        if arr.ndim == 0:
             return arr[()]
         return arr
 
     def get_id(self, name):
         """Get a low-level AttrID object for the named attribute.
         """
         return h5a.open(self._id, self._e(name))
```

### Comparing `h5py-3.7.0/h5py/_hl/base.py` & `h5py-3.8.0/h5py/_hl/base.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_hl/compat.py` & `h5py-3.8.0/h5py/_hl/compat.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_hl/dataset.py` & `h5py-3.8.0/h5py/_hl/dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 
 def make_new_dset(parent, shape=None, dtype=None, data=None, name=None,
                   chunks=None, compression=None, shuffle=None,
                   fletcher32=None, maxshape=None, compression_opts=None,
                   fillvalue=None, scaleoffset=None, track_times=False,
                   external=None, track_order=None, dcpl=None, dapl=None,
-                  efile_prefix=None, virtual_prefix=None,
-                  allow_unknown_filter=False):
+                  efile_prefix=None, virtual_prefix=None, allow_unknown_filter=False,
+                  rdcc_nslots=None, rdcc_nbytes=None, rdcc_w0=None):
     """ Return a new low-level dataset identifier """
 
     # Convert data to a C-contiguous ndarray
     if data is not None and not isinstance(data, Empty):
         from . import base
         data = base.array_for_new_object(data, specified_dtype=dtype)
 
@@ -134,54 +134,74 @@
         dcpl.set_attr_creation_order(0)
     elif track_order is not None:
         raise TypeError("track_order must be either True or False")
 
     if maxshape is not None:
         maxshape = tuple(m if m is not None else h5s.UNLIMITED for m in maxshape)
 
-    if efile_prefix is not None or virtual_prefix is not None:
+    if any([efile_prefix, virtual_prefix, rdcc_nbytes, rdcc_nslots, rdcc_w0]):
         dapl = dapl or h5p.create(h5p.DATASET_ACCESS)
 
     if efile_prefix is not None:
         dapl.set_efile_prefix(efile_prefix)
 
     if virtual_prefix is not None:
         dapl.set_virtual_prefix(virtual_prefix)
 
+    if rdcc_nbytes or rdcc_nslots or rdcc_w0:
+        cache_settings = list(dapl.get_chunk_cache())
+        if rdcc_nslots is not None:
+            cache_settings[0] = rdcc_nslots
+        if rdcc_nbytes is not None:
+            cache_settings[1] = rdcc_nbytes
+        if rdcc_w0 is not None:
+            cache_settings[2] = rdcc_w0
+        dapl.set_chunk_cache(*cache_settings)
+
     if isinstance(data, Empty):
         sid = h5s.create(h5s.NULL)
     else:
         sid = h5s.create_simple(shape, maxshape)
 
-
     dset_id = h5d.create(parent.id, name, tid, sid, dcpl=dcpl, dapl=dapl)
 
     if (data is not None) and (not isinstance(data, Empty)):
         dset_id.write(h5s.ALL, h5s.ALL, data)
 
     return dset_id
 
-def open_dset(parent, name, dapl=None, efile_prefix=None, virtual_prefix=None, **kwds):
+
+def open_dset(parent, name, dapl=None, efile_prefix=None, virtual_prefix=None,
+              rdcc_nslots=None, rdcc_nbytes=None, rdcc_w0=None, **kwds):
     """ Return an existing low-level dataset identifier """
 
-    if efile_prefix is not None or virtual_prefix is not None:
+    if any([efile_prefix, virtual_prefix, rdcc_nbytes, rdcc_nslots, rdcc_w0]):
         dapl = dapl or h5p.create(h5p.DATASET_ACCESS)
-    else:
-        dapl = dapl or None
 
     if efile_prefix is not None:
         dapl.set_efile_prefix(efile_prefix)
 
     if virtual_prefix is not None:
         dapl.set_virtual_prefix(virtual_prefix)
 
+    if rdcc_nbytes or rdcc_nslots or rdcc_w0:
+        cache_settings = list(dapl.get_chunk_cache())
+        if rdcc_nslots is not None:
+            cache_settings[0] = rdcc_nslots
+        if rdcc_nbytes is not None:
+            cache_settings[1] = rdcc_nbytes
+        if rdcc_w0 is not None:
+            cache_settings[2] = rdcc_w0
+        dapl.set_chunk_cache(*cache_settings)
+
     dset_id = h5d.open(parent.id, name, dapl=dapl)
 
     return dset_id
 
+
 class AstypeWrapper:
     """Wrapper to convert data on reading from a dataset.
     """
     def __init__(self, dset, dtype):
         self._dset = dset
         self._dtype = numpy.dtype(dtype)
 
@@ -249,14 +269,20 @@
     def __init__(self, dset, prior_dtype, names):
         self._dset = dset
         if isinstance(names, str):
             self.extract_field = names
             names = [names]
         self.read_dtype = readtime_dtype(prior_dtype, names)
 
+    def __array__(self, dtype=None):
+        data = self[:]
+        if dtype is not None:
+            data = data.astype(dtype)
+        return data
+
     def __getitem__(self, args):
         data = self._dset.__getitem__(args, new_dtype=self.read_dtype)
         if self.extract_field is not None:
             data = data[self.extract_field]
         return data
 
     def __len__(self):
@@ -269,15 +295,15 @@
 
 def readtime_dtype(basetype, names):
     """Make a NumPy compound dtype with a subset of available fields"""
     if basetype.names is None:  # Names provided, but not compound
         raise ValueError("Field names only allowed for compound types")
 
     for name in names:  # Check all names are legal
-        if not name in basetype.names:
+        if name not in basetype.names:
             raise ValueError("Field %s does not appear in this type." % name)
 
     return numpy.dtype([(name, basetype.fields[name][0]) for name in names])
 
 
 if MPI:
     class CollectiveContext:
@@ -367,14 +393,15 @@
 
             if dim > 0:
                 # reset to the start and continue iterating with higher dimension
                 self._chunk_index[dim] = 0
             dim -= 1
         return tuple(slices)
 
+
 class Dataset(HLObject):
 
     """
         Represents an HDF5 dataset
     """
 
     def astype(self, dtype):
@@ -1110,7 +1137,16 @@
         You can then attach it to dimensions of other datasets like this::
 
             other_ds.dims[0].attach_scale(ds)
 
         You can optionally pass a name to associate with this scale.
         """
         h5ds.set_scale(self._id, self._e(name))
+
+    @property
+    @with_phil
+    def is_scale(self):
+        """Return ``True`` if this dataset is also a dimension scale.
+
+        Return ``False`` otherwise.
+        """
+        return h5ds.is_scale(self._id)
```

### Comparing `h5py-3.7.0/h5py/_hl/datatype.py` & `h5py-3.8.0/h5py/_hl/datatype.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_hl/dims.py` & `h5py-3.8.0/h5py/_hl/dims.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
         if index > len(self) - 1:
             raise IndexError('Index out of range')
         return DimensionProxy(self._id, index)
 
     @with_phil
     def __len__(self):
         """ Number of dimensions associated with the dataset. """
-        return len(Dataset(self._id).shape)
+        return self._id.rank
 
     @with_phil
     def __iter__(self):
         """ Iterate over the dimensions. """
         for i in range(len(self)):
             yield self[i]
```

### Comparing `h5py-3.7.0/h5py/_hl/files.py` & `h5py-3.8.0/h5py/_hl/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,16 @@
     """Return a frozenset of the names of all of the registered drivers.
     """
     return frozenset(_drivers)
 
 
 def make_fapl(driver, libver, rdcc_nslots, rdcc_nbytes, rdcc_w0, locking,
               page_buf_size, min_meta_keep, min_raw_keep,
-              alignment_threshold, alignment_interval, **kwds):
+              alignment_threshold, alignment_interval, meta_block_size,
+              **kwds):
     """ Set up a file access property list """
     plist = h5p.create(h5p.FILE_ACCESS)
 
     if libver is not None:
         if libver in libver_dict:
             low = libver_dict[libver]
             high = h5f.LIBVER_LATEST
@@ -138,18 +139,22 @@
     if rdcc_w0 is not None:
         cache_settings[3] = rdcc_w0
     plist.set_cache(*cache_settings)
 
     if page_buf_size:
         plist.set_page_buffer_size(int(page_buf_size), int(min_meta_keep),
                                    int(min_raw_keep))
+
+    if meta_block_size is not None:
+        plist.set_meta_block_size(int(meta_block_size))
+
     if locking is not None:
         if hdf5_version < (1, 12, 1) and (hdf5_version[:2] != (1, 10) or hdf5_version[2] < 7):
             raise ValueError(
-                "HDF version >= 1.12.1 or 1.10.x >= 1.10.7 required for file locking.")
+                "HDF5 version >= 1.12.1 or 1.10.x >= 1.10.7 required for file locking.")
 
         if locking in ("false", False):
             plist.set_file_locking(False, ignore_when_disabled=False)
         elif locking in ("true", True):
             plist.set_file_locking(True, ignore_when_disabled=False)
         elif locking == "best-effort":
             plist.set_file_locking(True, ignore_when_disabled=True)
@@ -323,14 +328,21 @@
     @property
     @with_phil
     def userblock_size(self):
         """ User block size (in bytes) """
         fcpl = self.id.get_create_plist()
         return fcpl.get_userblock()
 
+    @property
+    @with_phil
+    def meta_block_size(self):
+        """ Meta block size (in bytes) """
+        fapl = self.id.get_access_plist()
+        return fapl.get_meta_block_size()
+
     if mpi and hdf5_version >= (1, 8, 9):
 
         @property
         @with_phil
         def atomic(self):
             """ Set/get MPI-IO atomic mode
             """
@@ -360,15 +372,15 @@
         else:
             raise RuntimeError('SWMR support is not available in HDF5 version {}.{}.{}.'.format(*hdf5_version))
 
     def __init__(self, name, mode='r', driver=None, libver=None, userblock_size=None, swmr=False,
                  rdcc_nslots=None, rdcc_nbytes=None, rdcc_w0=None, track_order=None,
                  fs_strategy=None, fs_persist=False, fs_threshold=1, fs_page_size=None,
                  page_buf_size=None, min_meta_keep=0, min_raw_keep=0, locking=None,
-                 alignment_threshold=1, alignment_interval=1, **kwds):
+                 alignment_threshold=1, alignment_interval=1, meta_block_size=None, **kwds):
         """Create a new file object.
 
         See the h5py user guide for a detailed explanation of the options.
 
         name
             Name of the file on disk, or file-like object.  Note: for files
             created with the 'core' driver, HDF5 still requires this be
@@ -388,37 +400,37 @@
             options can only be specified with the HDF5 1.10.2 library or later.
         userblock_size
             Desired size of user block.  Only allowed when creating a new
             file (mode w, w- or x).
         swmr
             Open the file in SWMR read mode. Only used when mode = 'r'.
         rdcc_nbytes
-            Total size of the raw data chunk cache in bytes. The default size
-            is 1024**2 (1 MB) per dataset.
+            Total size of the dataset chunk cache in bytes. The default size
+            is 1024**2 (1 MiB) per dataset. Applies to all datasets unless individually changed.
         rdcc_w0
             The chunk preemption policy for all datasets.  This must be
             between 0 and 1 inclusive and indicates the weighting according to
             which chunks which have been fully read or written are penalized
             when determining which chunks to flush from cache.  A value of 0
             means fully read or written chunks are treated no differently than
             other chunks (the preemption is strictly LRU) while a value of 1
             means fully read or written chunks are always preempted before
             other chunks.  If your application only reads or writes data once,
             this can be safely set to 1.  Otherwise, this should be set lower
             depending on how often you re-read or re-write the same data.  The
-            default value is 0.75.
+            default value is 0.75. Applies to all datasets unless individually changed.
         rdcc_nslots
             The number of chunk slots in the raw data chunk cache for this
             file. Increasing this value reduces the number of cache collisions,
             but slightly increases the memory used. Due to the hashing
             strategy, this value should ideally be a prime number. As a rule of
             thumb, this value should be at least 10 times the number of chunks
             that can fit in rdcc_nbytes bytes. For maximum performance, this
             value should be set approximately 100 times that number of
-            chunks. The default value is 521.
+            chunks. The default value is 521. Applies to all datasets unless individually changed.
         track_order
             Track dataset/group/attribute creation order under root group
             if True. If None use global default h5.get_config().track_order.
         fs_strategy
             The file space handling strategy to be used.  Only allowed when
             creating a new file (mode w, w- or x).  Defined as:
             "fsm"        FSM, Aggregators, VFD
@@ -448,50 +460,71 @@
             page_buf_size is set. Default value is zero.
         min_raw_keep
             Minimum percentage of raw data to keep in the page buffer before
             allowing pages containing raw data to be evicted. Applicable only if
             page_buf_size is set. Default value is zero.
         locking
             The file locking behavior. Defined as:
-            False (or "false")  Disable file locking
-            True (or "true")    Enable file locking
-            "best-effort"       Enable file locking but ignore some errors
-            None                Use HDF5 defaults
-            Warning: The HDF5_USE_FILE_LOCKING environment variable can override
-            this parameter.
+
+            - False (or "false") --  Disable file locking
+            - True (or "true")   --  Enable file locking
+            - "best-effort"      --  Enable file locking but ignore some errors
+            - None               --  Use HDF5 defaults
+
+            .. warning::
+
+                The HDF5_USE_FILE_LOCKING environment variable can override
+                this parameter.
+
             Only available with HDF5 >= 1.12.1 or 1.10.x >= 1.10.7.
 
         alignment_threshold
             Together with ``alignment_interval``, this property ensures that
             any file object greater than or equal in size to the alignement
             threshold (in bytes) will be aligned on an address which is a
             multiple of alignment interval.
 
         alignment_interval
             This property should be used in conjunction with
             ``alignment_threshold``. See the description above. For more
             details, see
             https://portal.hdfgroup.org/display/HDF5/H5P_SET_ALIGNMENT
 
+        meta_block_size
+            Set the current minimum size, in bytes, of new metadata block allocations.
+            See https://portal.hdfgroup.org/display/HDF5/H5P_SET_META_BLOCK_SIZE
+
         Additional keywords
             Passed on to the selected file driver.
         """
         if (fs_strategy or page_buf_size) and hdf5_version < (1, 10, 1):
-            raise ValueError("HDF version 1.10.1 or greater required for file space strategy or page buffering support.")
+            raise ValueError("HDF5 version 1.10.1 or greater required for file space strategy or page buffering support.")
 
         if swmr and not swmr_support:
             raise ValueError("The SWMR feature is not available in this version of the HDF5 library")
 
-        if driver == 'ros3' and not ros3:
-            raise ValueError(
-                "h5py was built without ROS3 support, can't use ros3 driver")
+        if driver == 'ros3':
+            if ros3:
+                from urllib.parse import urlparse
+                url = urlparse(name)
+                if url.scheme == 's3':
+                    aws_region = kwds.get('aws_region', b'').decode('ascii')
+                    if len(aws_region) == 0:
+                        raise ValueError('AWS region required for s3:// location')
+                    name = f'https://s3.{aws_region}.amazonaws.com/{url.netloc}{url.path}'
+                elif url.scheme not in ('https', 'http'):
+                    raise ValueError(f'{name}: S3 location must begin with '
+                                     'either "https://", "http://", or "s3://"')
+            else:
+                raise ValueError(
+                    "h5py was built without ROS3 support, can't use ros3 driver")
 
         if locking is not None and hdf5_version < (1, 12, 1) and (
                 hdf5_version[:2] != (1, 10) or hdf5_version[2] < 7):
-            raise ValueError("HDF version >= 1.12.1 or 1.10.x >= 1.10.7 required for file locking options.")
+            raise ValueError("HDF5 version >= 1.12.1 or 1.10.x >= 1.10.7 required for file locking options.")
 
         if isinstance(name, _objects.ObjectID):
             if fs_strategy:
                 raise ValueError("Unable to set file space strategy of an existing file")
 
             with phil:
                 fid = h5i.get_file_id(name)
@@ -522,14 +555,15 @@
                 )
 
             with phil:
                 fapl = make_fapl(driver, libver, rdcc_nslots, rdcc_nbytes, rdcc_w0,
                                  locking, page_buf_size, min_meta_keep, min_raw_keep,
                                  alignment_threshold=alignment_threshold,
                                  alignment_interval=alignment_interval,
+                                 meta_block_size=meta_block_size,
                                  **kwds)
                 fcpl = make_fcpl(track_order=track_order, fs_strategy=fs_strategy,
                                  fs_persist=fs_persist, fs_threshold=fs_threshold,
                                  fs_page_size=fs_page_size)
                 fid = make_fid(name, mode, userblock_size, fapl, fcpl, swmr=swmr)
 
             if isinstance(libver, tuple):
```

### Comparing `h5py-3.7.0/h5py/_hl/filters.py` & `h5py-3.8.0/h5py/_hl/filters.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_hl/group.py` & `h5py-3.8.0/h5py/_hl/group.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,22 +35,20 @@
         """ Create a new Group object by binding to a low-level GroupID.
         """
         with phil:
             if not isinstance(bind, h5g.GroupID):
                 raise ValueError("%s is not a GroupID" % bind)
             super().__init__(bind)
 
-
     _gcpl_crt_order = h5p.create(h5p.GROUP_CREATE)
     _gcpl_crt_order.set_link_creation_order(
         h5p.CRT_ORDER_TRACKED | h5p.CRT_ORDER_INDEXED)
     _gcpl_crt_order.set_attr_creation_order(
         h5p.CRT_ORDER_TRACKED | h5p.CRT_ORDER_INDEXED)
 
-
     def create_group(self, name, track_order=None):
         """ Create and return a new subgroup.
 
         Name may be absolute or relative.  Fails if the target name already
         exists.
 
         track_order
@@ -136,14 +134,38 @@
         virtual_prefix
             (String) Virtual dataset file prefix for dataset access property
             list. Does not persist in the file.
         allow_unknown_filter
             (T/F) Do not check that the requested filter is available for use.
             This should only be used with ``write_direct_chunk``, where the caller
             compresses the data before handing it to h5py.
+        rdcc_nbytes
+            Total size of the dataset's chunk cache in bytes. The default size
+            is 1024**2 (1 MiB).
+        rdcc_w0
+            The chunk preemption policy for this dataset.  This must be
+            between 0 and 1 inclusive and indicates the weighting according to
+            which chunks which have been fully read or written are penalized
+            when determining which chunks to flush from cache.  A value of 0
+            means fully read or written chunks are treated no differently than
+            other chunks (the preemption is strictly LRU) while a value of 1
+            means fully read or written chunks are always preempted before
+            other chunks.  If your application only reads or writes data once,
+            this can be safely set to 1.  Otherwise, this should be set lower
+            depending on how often you re-read or re-write the same data.  The
+            default value is 0.75.
+        rdcc_nslots
+            The number of chunk slots in the dataset's chunk cache. Increasing
+            this value reduces the number of cache collisions, but slightly
+            increases the memory used. Due to the hashing strategy, this value
+            should ideally be a prime number. As a rule of thumb, this value
+            should be at least 10 times the number of chunks that can fit in
+            rdcc_nbytes bytes. For maximum performance, this value should be set
+            approximately 100 times that number of chunks. The default value is
+            521.
         """
         if 'track_order' not in kwds:
             kwds['track_order'] = h5.get_config().track_order
 
         if 'efile_prefix' in kwds:
             kwds['efile_prefix'] = self._e(kwds['efile_prefix'])
 
@@ -226,47 +248,54 @@
     def require_dataset(self, name, shape, dtype, exact=False, **kwds):
         """ Open a dataset, creating it if it doesn't exist.
 
         If keyword "exact" is False (default), an existing dataset must have
         the same shape and a conversion-compatible dtype to be returned.  If
         True, the shape and dtype must match exactly.
 
+        If keyword "maxshape" is given, the maxshape and dtype must match
+        instead.
+
+        If any of the keywords "rdcc_nslots", "rdcc_nbytes", or "rdcc_w0" are
+        given, they will be used to configure the dataset's chunk cache.
+
         Other dataset keywords (see create_dataset) may be provided, but are
         only used if a new dataset is to be created.
 
         Raises TypeError if an incompatible object already exists, or if the
-        shape or dtype don't match according to the above rules.
+        shape, maxshape or dtype don't match according to the above rules.
         """
         if 'efile_prefix' in kwds:
             kwds['efile_prefix'] = self._e(kwds['efile_prefix'])
 
         if 'virtual_prefix' in kwds:
             kwds['virtual_prefix'] = self._e(kwds['virtual_prefix'])
 
         with phil:
-            if not name in self:
+            if name not in self:
                 return self.create_dataset(name, *(shape, dtype), **kwds)
 
             if isinstance(shape, int):
                 shape = (shape,)
 
             try:
                 dsid = dataset.open_dset(self, self._e(name), **kwds)
                 dset = dataset.Dataset(dsid)
             except KeyError:
                 dset = self[name]
                 raise TypeError("Incompatible object (%s) already exists" % dset.__class__.__name__)
-            except:
-                raise
 
-            if not shape == dset.shape:
-                raise TypeError("Shapes do not match (existing %s vs new %s)" % (dset.shape, shape))
+            if shape != dset.shape:
+                if "maxshape" not in kwds:
+                    raise TypeError("Shapes do not match (existing %s vs new %s)" % (dset.shape, shape))
+                elif kwds["maxshape"] != dset.maxshape:
+                    raise TypeError("Max shapes do not match (existing %s vs new %s)" % (dset.maxshape, kwds["maxshape"]))
 
             if exact:
-                if not dtype == dset.dtype:
+                if dtype != dset.dtype:
                     raise TypeError("Datatypes do not exactly match (existing %s vs new %s)" % (dset.dtype, dtype))
             elif not numpy.can_cast(dtype, dset.dtype):
                 raise TypeError("Datatypes cannot be safely cast (existing %s vs new %s)" % (dset.dtype, dtype))
 
             return dset
 
     def create_dataset_like(self, name, other, **kwupdate):
@@ -305,15 +334,15 @@
         # TODO: support kwargs like require_dataset
         """Return a group, creating it if it doesn't exist.
 
         TypeError is raised if something with that name already exists that
         isn't a group.
         """
         with phil:
-            if not name in self:
+            if name not in self:
                 return self.create_group(name)
             grp = self[name]
             if not isinstance(grp, Group):
                 raise TypeError("Incompatible object (%s) already exists" % grp.__class__.__name__)
             return grp
 
     @with_phil
@@ -324,15 +353,15 @@
             oid = h5r.dereference(name, self.id)
             if oid is None:
                 raise ValueError("Invalid HDF5 object reference")
         elif isinstance(name, (bytes, str)):
             oid = h5o.open(self.id, self._e(name), lapl=self._lapl)
         else:
             raise TypeError("Accessing a group is done with bytes or str, "
-                            " not {}".format(type(name)))
+                            "not {}".format(type(name)))
 
         otype = h5i.get_type(oid)
         if otype == h5i.GROUP:
             return Group(oid)
         elif otype == h5i.DATASET:
             return dataset.Dataset(oid, readonly=(self.file.mode == 'r'))
         elif otype == h5i.DATATYPE:
@@ -368,15 +397,15 @@
         with phil:
             if not (getclass or getlink):
                 try:
                     return self[name]
                 except KeyError:
                     return default
 
-            if not name in self:
+            if name not in self:
                 return default
 
             elif getclass and not getlink:
                 typecode = h5o.get_info(self.id, self._e(name)).type
 
                 try:
                     return {h5o.TYPE_GROUP: Group,
@@ -435,16 +464,15 @@
         with phil:
             name, lcpl = self._e(name, lcpl=True)
 
             if isinstance(obj, HLObject):
                 h5o.link(obj.id, self.id, name, lcpl=lcpl, lapl=self._lapl)
 
             elif isinstance(obj, SoftLink):
-                self.id.links.create_soft(name, self._e(obj.path),
-                              lcpl=lcpl, lapl=self._lapl)
+                self.id.links.create_soft(name, self._e(obj.path), lcpl=lcpl, lapl=self._lapl)
 
             elif isinstance(obj, ExternalLink):
                 fn = filename_encode(obj.filename)
                 self.id.links.create_external(name, fn, self._e(obj.path),
                                               lcpl=lcpl, lapl=self._lapl)
 
             elif isinstance(obj, numpy.dtype):
```

### Comparing `h5py-3.7.0/h5py/_hl/selections.py` & `h5py-3.8.0/h5py/_hl/selections.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_hl/selections2.py` & `h5py-3.8.0/h5py/_hl/selections2.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_hl/vds.py` & `h5py-3.8.0/h5py/_hl/vds.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_locks.pxi` & `h5py-3.8.0/h5py/_locks.pxi`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_objects.pxd` & `h5py-3.8.0/h5py/_objects.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_objects.pyx` & `h5py-3.8.0/h5py/_objects.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_proxy.pxd` & `h5py-3.8.0/h5py/_proxy.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_proxy.pyx` & `h5py-3.8.0/h5py/_proxy.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/_selector.pyx` & `h5py-3.8.0/h5py/_selector.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -168,57 +168,63 @@
                     self.block[dim_ix],
                 ) = a.indices(l)
                 self.scalar[dim_ix] = False
 
                 continue
 
             # [[0, 2, 10]] - list/array of indices ('fancy indexing')
-            if isinstance(a, (list, np.ndarray)):
-                if isinstance(a, list) and len(a) == 0:
-                    a = np.asarray(a, dtype=np.intp)
-                else:
-                    a = np.asarray(a)
+            if isinstance(a, np.ndarray):
                 if a.ndim != 1:
                     raise TypeError("Only 1D arrays allowed for fancy indexing")
-                if a.dtype.kind == 'b':
-                    if a.size != l:
-                        raise TypeError("boolean index did not match indexed array")
-                    a = a.nonzero()[0]
-                if not np.issubdtype(a.dtype, np.integer):
-                    raise TypeError("Indexing arrays must have integer dtypes")
-                if array_ix != -1:
-                    raise TypeError("Only one indexing vector or array is currently allowed for fancy indexing")
-
-                # Convert negative indices to positive
-                if np.any(a < 0):
-                    a = a.copy()
-                    a[a < 0] += l
-
-                # Bounds check
-                if np.any((a < 0) | (a > l)):
-                    if l == 0:
-                        msg = "Fancy indexing out of range for empty dimension"
-                    else:
-                        msg = f"Fancy indexing out of range for (0-{l-1})"
-                    raise IndexError(msg)
-
-                if np.any(np.diff(a) <= 0):
-                    raise TypeError("Indexing elements must be in increasing order")
-
-                array_ix = dim_ix
-                array_arg = a
-                self.start[dim_ix] = 0
-                self.stride[dim_ix] = 1
-                self.count[dim_ix] = a.shape[0]
-                self.block[dim_ix] = 1
-                self.scalar[dim_ix] = False
+            else:
+                arr = np.asarray(a)
+                if arr.ndim != 1:
+                    raise TypeError("Selection can't process %r" % a)
+                a = arr
+                if a.size == 0:
+                    # asarray([]) gives float dtype by default
+                    a = a.astype(np.intp)
+
+            if a.dtype.kind == 'b':
+                if self.rank == 1:
+                    # The dataset machinery should fall back to a faster
+                    # alternative (using PointSelection) in this case.
+                    # https://github.com/h5py/h5py/issues/2189
+                    raise TypeError("Use other code for boolean selection on 1D dataset")
+                if a.size != l:
+                    raise TypeError("boolean index did not match indexed array")
+                a = a.nonzero()[0]
+            if not np.issubdtype(a.dtype, np.integer):
+                raise TypeError("Indexing arrays must have integer dtypes")
+            if array_ix != -1:
+                raise TypeError("Only one indexing vector or array is currently allowed for fancy indexing")
+
+            # Convert negative indices to positive
+            if np.any(a < 0):
+                a = a.copy()
+                a[a < 0] += l
+
+            # Bounds check
+            if np.any((a < 0) | (a > l)):
+                if l == 0:
+                    msg = "Fancy indexing out of range for empty dimension"
+                else:
+                    msg = f"Fancy indexing out of range for (0-{l-1})"
+                raise IndexError(msg)
 
-                continue
+            if np.any(np.diff(a) <= 0):
+                raise TypeError("Indexing elements must be in increasing order")
 
-            raise TypeError("Simple selection can't process %r" % a)
+            array_ix = dim_ix
+            array_arg = a
+            self.start[dim_ix] = 0
+            self.stride[dim_ix] = 1
+            self.count[dim_ix] = a.shape[0]
+            self.block[dim_ix] = 1
+            self.scalar[dim_ix] = False
 
         if nargs < self.rank:
             # Fill in ellipsis or trailing dimensions
             ellipsis_end = ellipsis_ix + (self.rank - nargs)
             for dim_ix in range(ellipsis_ix, ellipsis_end):
                 self.start[dim_ix] = 0
                 self.stride[dim_ix] = 1
```

### Comparing `h5py-3.7.0/h5py/api_compat.h` & `h5py-3.8.0/h5py/api_compat.h`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/api_functions.txt` & `h5py-3.8.0/h5py/api_functions.txt`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,16 @@
   1.10.2    herr_t H5DOread_chunk(hid_t dset_id, hid_t dxpl_id, const hsize_t *offset, uint32_t *filters, void *buf) nogil
   1.10.3    herr_t H5Dread_chunk(hid_t dset_id, hid_t dxpl_id, const hsize_t *offset, uint32_t *filters, void *buf) nogil
 
   # Chunk query functions
   1.10.5    herr_t H5Dget_num_chunks(hid_t dset_id, hid_t fspace_id, hsize_t *nchunks)
   1.10.5    herr_t H5Dget_chunk_info(hid_t dset_id, hid_t fspace_id, hsize_t chk_idx, hsize_t *offset, unsigned *filter_mask, haddr_t *addr, hsize_t *size)
   1.10.5    herr_t H5Dget_chunk_info_by_coord(hid_t dset_id, const hsize_t *offset, unsigned *filter_mask, haddr_t *addr, hsize_t *size)
+  1.10.10-1.10.99 herr_t H5Dchunk_iter(hid_t dset_id, hid_t dxpl_id, H5D_chunk_iter_op_t cb, void *op_data)
+  1.12.3    herr_t H5Dchunk_iter(hid_t dset_id, hid_t dxpl_id, H5D_chunk_iter_op_t cb, void *op_data)
 
 
   # === H5E - Minimal error-handling interface ================================
 
   # The error interfaces used by h5py are exposed directly through Cython
   # code in h5py._errors, so wrappers are not autogenerated for them.
 
@@ -313,14 +315,16 @@
   herr_t    H5Pset_fapl_stdio(hid_t fapl_id)
   herr_t    H5Pset_fapl_split(hid_t fapl_id, const char *meta_ext, hid_t meta_plist_id, const char *raw_ext, hid_t raw_plist_id)
   herr_t    H5Pset_driver(hid_t plist_id, hid_t driver_id, void *driver_info)
   hid_t     H5Pget_driver(hid_t fapl_id)
   void*     H5Pget_driver_info(hid_t plist_id)
   herr_t    H5Pget_mdc_config(hid_t plist_id, H5AC_cache_config_t *config_ptr)
   herr_t    H5Pset_mdc_config(hid_t plist_id, H5AC_cache_config_t *config_ptr)
+  herr_t    H5Pset_meta_block_size(hid_t fapl_id, hsize_t size)
+  herr_t    H5Pget_meta_block_size(hid_t fapl_id, hsize_t * size)
   1.8.9 herr_t H5Pset_file_image(hid_t plist_id, void *buf_ptr, size_t buf_len)
   1.10.1 herr_t H5Pset_page_buffer_size(hid_t plist_id, size_t buf_size, unsigned min_meta_per, unsigned min_raw_per)
   1.10.1 herr_t H5Pget_page_buffer_size(hid_t plist_id, size_t *buf_size, unsigned *min_meta_per, unsigned *min_raw_per)
   1.10.7-1.10.99 herr_t H5Pget_file_locking(hid_t fapl_id, hbool_t *use_file_locking, hbool_t *ignore_when_disabled)
   1.12.1 herr_t H5Pget_file_locking(hid_t fapl_id, hbool_t *use_file_locking, hbool_t *ignore_when_disabled)
   1.10.7-1.10.99 herr_t H5Pset_file_locking(hid_t fapl_id, hbool_t use_file_locking, hbool_t ignore_when_disabled)
   1.12.1 herr_t H5Pset_file_locking(hid_t fapl_id, hbool_t use_file_locking, hbool_t ignore_when_disabled)
```

### Comparing `h5py-3.7.0/h5py/api_types_ext.pxd` & `h5py-3.8.0/h5py/api_types_ext.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/api_types_hdf5.pxd` & `h5py-3.8.0/h5py/api_types_hdf5.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,19 @@
     H5D_FILL_VALUE_UNDEFINED    =0,
     H5D_FILL_VALUE_DEFAULT      =1,
     H5D_FILL_VALUE_USER_DEFINED =2
 
   ctypedef  herr_t (*H5D_operator_t)(void *elem, hid_t type_id, unsigned ndim,
                     hsize_t *point, void *operator_data) except -1
 
+
+  IF HDF5_VERSION >= (1, 12, 3) or (HDF5_VERSION >= (1, 10, 10) and HDF5_VERSION < (1, 10, 99)):
+    ctypedef int (*H5D_chunk_iter_op_t)(const hsize_t *offset, unsigned filter_mask,
+                                        haddr_t addr, hsize_t size, void *op_data) except -1
+
 # === H5F - File API ==========================================================
 
   # File constants
   cdef enum:
     H5F_ACC_TRUNC
     H5F_ACC_RDONLY
     H5F_ACC_RDWR
@@ -149,24 +154,24 @@
     ctypedef enum H5F_libver_t:
       H5F_LIBVER_EARLIEST = 0,        # Use the earliest possible format for storing objects
       H5F_LIBVER_V18 = 1,
       H5F_LIBVER_V110 = 2,
       H5F_LIBVER_NBOUNDS
     int H5F_LIBVER_LATEST  # Use the latest possible format available for storing objects
 
-  IF HDF5_VERSION >= (1, 11, 4) and HDF5_VERSION < (1, 13, 0):
+  IF HDF5_VERSION >= (1, 11, 4) and HDF5_VERSION < (1, 14, 0):
     ctypedef enum H5F_libver_t:
       H5F_LIBVER_EARLIEST = 0,        # Use the earliest possible format for storing objects
       H5F_LIBVER_V18 = 1,
       H5F_LIBVER_V110 = 2,
       H5F_LIBVER_V112 = 3,
       H5F_LIBVER_NBOUNDS
     int H5F_LIBVER_LATEST  # Use the latest possible format available for storing objects
 
-  IF HDF5_VERSION >= (1, 13, 0):
+  IF HDF5_VERSION >= (1, 14, 0):
     ctypedef enum H5F_libver_t:
       H5F_LIBVER_EARLIEST = 0,        # Use the earliest possible format for storing objects
       H5F_LIBVER_V18 = 1,
       H5F_LIBVER_V110 = 2,
       H5F_LIBVER_V112 = 3,
       H5F_LIBVER_V114 = 4,
       H5F_LIBVER_NBOUNDS
@@ -231,48 +236,108 @@
   int H5FD_LOG_ALLOC      # 0x4000
   int H5FD_LOG_ALL        # (H5FD_LOG_ALLOC|H5FD_LOG_TIME_IO|H5FD_LOG_NUM_IO|H5FD_LOG_FLAVOR|H5FD_LOG_FILE_IO|H5FD_LOG_LOC_IO)
 
   ctypedef enum H5FD_mpio_xfer_t:
     H5FD_MPIO_INDEPENDENT = 0,
     H5FD_MPIO_COLLECTIVE
 
+  # File driver identifier type and values
+  IF HDF5_VERSION >= (1, 14, 0):
+    ctypedef int H5FD_class_value_t
+
+    H5FD_class_value_t H5_VFD_INVALID      # -1
+    H5FD_class_value_t H5_VFD_SEC2         # 0
+    H5FD_class_value_t H5_VFD_CORE         # 1
+    H5FD_class_value_t H5_VFD_LOG          # 2
+    H5FD_class_value_t H5_VFD_FAMILY       # 3
+    H5FD_class_value_t H5_VFD_MULTI        # 4
+    H5FD_class_value_t H5_VFD_STDIO        # 5
+    H5FD_class_value_t H5_VFD_SPLITTER     # 6
+    H5FD_class_value_t H5_VFD_MPIO         # 7
+    H5FD_class_value_t H5_VFD_DIRECT       # 8
+    H5FD_class_value_t H5_VFD_MIRROR       # 9
+    H5FD_class_value_t H5_VFD_HDFS         # 10
+    H5FD_class_value_t H5_VFD_ROS3         # 11
+    H5FD_class_value_t H5_VFD_SUBFILING    # 12
+    H5FD_class_value_t H5_VFD_IOC          # 13
+    H5FD_class_value_t H5_VFD_ONION        # 14
+
   # Class information for each file driver
-  ctypedef struct H5FD_class_t:
-    const char *name
-    haddr_t maxaddr
-    H5F_close_degree_t fc_degree
-    herr_t  (*terminate)()
-    hsize_t (*sb_size)(H5FD_t *file)
-    herr_t  (*sb_encode)(H5FD_t *file, char *name, unsigned char *p)
-    herr_t  (*sb_decode)(H5FD_t *f, const char *name, const unsigned char *p)
-    size_t  fapl_size
-    void *  (*fapl_get)(H5FD_t *file)
-    void *  (*fapl_copy)(const void *fapl)
-    herr_t  (*fapl_free)(void *fapl)
-    size_t  dxpl_size
-    void *  (*dxpl_copy)(const void *dxpl)
-    herr_t  (*dxpl_free)(void *dxpl)
-    H5FD_t *(*open)(const char *name, unsigned flags, hid_t fapl, haddr_t maxaddr)
-    herr_t  (*close)(H5FD_t *file)
-    int     (*cmp)(const H5FD_t *f1, const H5FD_t *f2)
-    herr_t  (*query)(const H5FD_t *f1, unsigned long *flags)
-    herr_t  (*get_type_map)(const H5FD_t *file, H5FD_mem_t *type_map)
-    haddr_t (*alloc)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl_id, hsize_t size)
-    herr_t  (*free)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl_id, haddr_t addr, hsize_t size)
-    haddr_t (*get_eoa)(const H5FD_t *file, H5FD_mem_t type)
-    herr_t  (*set_eoa)(H5FD_t *file, H5FD_mem_t type, haddr_t addr)
-    haddr_t (*get_eof)(const H5FD_t *file, H5FD_mem_t type)
-    herr_t  (*get_handle)(H5FD_t *file, hid_t fapl, void**file_handle)
-    herr_t  (*read)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl, haddr_t addr, size_t size, void *buffer)
-    herr_t  (*write)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl, haddr_t addr, size_t size, const void *buffer)
-    herr_t  (*flush)(H5FD_t *file, hid_t dxpl_id, hbool_t closing)
-    herr_t  (*truncate)(H5FD_t *file, hid_t dxpl_id, hbool_t closing)
-    herr_t  (*lock)(H5FD_t *file, hbool_t rw)
-    herr_t  (*unlock)(H5FD_t *file)
-    H5FD_mem_t fl_map[<int>H5FD_MEM_NTYPES]
+  IF HDF5_VERSION < (1, 14, 0):
+    ctypedef struct H5FD_class_t:
+      const char *name
+      haddr_t maxaddr
+      H5F_close_degree_t fc_degree
+      herr_t  (*terminate)()
+      hsize_t (*sb_size)(H5FD_t *file)
+      herr_t  (*sb_encode)(H5FD_t *file, char *name, unsigned char *p)
+      herr_t  (*sb_decode)(H5FD_t *f, const char *name, const unsigned char *p)
+      size_t  fapl_size
+      void *  (*fapl_get)(H5FD_t *file)
+      void *  (*fapl_copy)(const void *fapl)
+      herr_t  (*fapl_free)(void *fapl)
+      size_t  dxpl_size
+      void *  (*dxpl_copy)(const void *dxpl)
+      herr_t  (*dxpl_free)(void *dxpl)
+      H5FD_t *(*open)(const char *name, unsigned flags, hid_t fapl, haddr_t maxaddr)
+      herr_t  (*close)(H5FD_t *file)
+      int     (*cmp)(const H5FD_t *f1, const H5FD_t *f2)
+      herr_t  (*query)(const H5FD_t *f1, unsigned long *flags)
+      herr_t  (*get_type_map)(const H5FD_t *file, H5FD_mem_t *type_map)
+      haddr_t (*alloc)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl_id, hsize_t size)
+      herr_t  (*free)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl_id, haddr_t addr, hsize_t size)
+      haddr_t (*get_eoa)(const H5FD_t *file, H5FD_mem_t type)
+      herr_t  (*set_eoa)(H5FD_t *file, H5FD_mem_t type, haddr_t addr)
+      haddr_t (*get_eof)(const H5FD_t *file, H5FD_mem_t type)
+      herr_t  (*get_handle)(H5FD_t *file, hid_t fapl, void**file_handle)
+      herr_t  (*read)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl, haddr_t addr, size_t size, void *buffer)
+      herr_t  (*write)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl, haddr_t addr, size_t size, const void *buffer)
+      herr_t  (*flush)(H5FD_t *file, hid_t dxpl_id, hbool_t closing)
+      herr_t  (*truncate)(H5FD_t *file, hid_t dxpl_id, hbool_t closing)
+      herr_t  (*lock)(H5FD_t *file, hbool_t rw)
+      herr_t  (*unlock)(H5FD_t *file)
+      H5FD_mem_t fl_map[<int>H5FD_MEM_NTYPES]
+  ELSE:
+    unsigned H5FD_CLASS_VERSION  # File driver struct version
+
+    ctypedef struct H5FD_class_t:
+      unsigned version  # File driver class struct version number
+      H5FD_class_value_t value
+      const char *name
+      haddr_t maxaddr
+      H5F_close_degree_t fc_degree
+      herr_t  (*terminate)()
+      hsize_t (*sb_size)(H5FD_t *file)
+      herr_t  (*sb_encode)(H5FD_t *file, char *name, unsigned char *p)
+      herr_t  (*sb_decode)(H5FD_t *f, const char *name, const unsigned char *p)
+      size_t  fapl_size
+      void *  (*fapl_get)(H5FD_t *file)
+      void *  (*fapl_copy)(const void *fapl)
+      herr_t  (*fapl_free)(void *fapl)
+      size_t  dxpl_size
+      void *  (*dxpl_copy)(const void *dxpl)
+      herr_t  (*dxpl_free)(void *dxpl)
+      H5FD_t *(*open)(const char *name, unsigned flags, hid_t fapl, haddr_t maxaddr)
+      herr_t  (*close)(H5FD_t *file)
+      int     (*cmp)(const H5FD_t *f1, const H5FD_t *f2)
+      herr_t  (*query)(const H5FD_t *f1, unsigned long *flags)
+      herr_t  (*get_type_map)(const H5FD_t *file, H5FD_mem_t *type_map)
+      haddr_t (*alloc)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl_id, hsize_t size)
+      herr_t  (*free)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl_id, haddr_t addr, hsize_t size)
+      haddr_t (*get_eoa)(const H5FD_t *file, H5FD_mem_t type)
+      herr_t  (*set_eoa)(H5FD_t *file, H5FD_mem_t type, haddr_t addr)
+      haddr_t (*get_eof)(const H5FD_t *file, H5FD_mem_t type)
+      herr_t  (*get_handle)(H5FD_t *file, hid_t fapl, void**file_handle)
+      herr_t  (*read)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl, haddr_t addr, size_t size, void *buffer)
+      herr_t  (*write)(H5FD_t *file, H5FD_mem_t type, hid_t dxpl, haddr_t addr, size_t size, const void *buffer)
+      herr_t  (*flush)(H5FD_t *file, hid_t dxpl_id, hbool_t closing)
+      herr_t  (*truncate)(H5FD_t *file, hid_t dxpl_id, hbool_t closing)
+      herr_t  (*lock)(H5FD_t *file, hbool_t rw)
+      herr_t  (*unlock)(H5FD_t *file)
+      H5FD_mem_t fl_map[<int>H5FD_MEM_NTYPES]
 
   # The main datatype for each driver
   ctypedef struct H5FD_t:
     hid_t driver_id             # driver ID for this file
     const H5FD_class_t cls      # constant class info
     unsigned long fileno        # File 'serial' number
     unsigned access_flags       # File access flags (from create or open)
```

### Comparing `h5py-3.7.0/h5py/h5.pxd` & `h5py-3.8.0/h5py/h5.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5.pyx` & `h5py-3.8.0/h5py/h5.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5a.pyx` & `h5py-3.8.0/h5py/h5a.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5ac.pyx` & `h5py-3.8.0/h5py/h5ac.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5d.pyx` & `h5py-3.8.0/h5py/h5d.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,62 @@
     VDS_FIRST_MISSING   = H5D_VDS_FIRST_MISSING
     VDS_LAST_AVAILABLE  = H5D_VDS_LAST_AVAILABLE
 
 IF HDF5_VERSION >= (1, 10, 5):
     StoreInfo = namedtuple('StoreInfo',
                            'chunk_offset, filter_mask, byte_offset, size')
 
+# === Dataset chunk iterator ==================================================
+
+IF HDF5_VERSION >= (1, 12, 3) or (HDF5_VERSION >= (1, 10, 10) and HDF5_VERSION < (1, 10, 99)):
+
+    cdef class _ChunkVisitor:
+        cdef int rank
+        cdef object func
+        cdef object retval
+
+        def __init__(self, rank, func):
+            self.rank = rank
+            self.func = func
+            self.retval = None
+
+
+    cdef int _cb_chunk_info(const hsize_t *offset, unsigned filter_mask, haddr_t addr, hsize_t size, void *op_data) except -1 with gil:
+        """Callback function for chunk iteration. (Not to be used directly.)
+
+        This function is called for every chunk with the following information:
+            * offset - Logical position of the chunk’s first element in units of dataset elements
+            * filter_mask - Bitmask indicating the filters used when the chunk was written
+            * addr - Chunk file address
+            * size - Chunk size in bytes, 0 if the chunk does not exist
+
+        Chunk information is converted to a StoreInfo namedtuple and passed as input
+        to the user-supplied callback object in the "op_data".
+
+        Feature requires: HDF5 1.10.10 or any later 1.10
+                          HDF5 1.12.3 or later
+
+        .. versionadded:: 3.8
+        """
+        cdef _ChunkVisitor visit
+        cdef object chunk_info
+        cdef tuple cot
+
+        visit = <_ChunkVisitor>op_data
+        if addr != HADDR_UNDEF:
+            cot = convert_dims(offset, <hsize_t>visit.rank)
+            chunk_info = StoreInfo(cot, filter_mask, addr, size)
+        else:
+            chunk_info = StoreInfo(None, filter_mask, None, size)
+
+        visit.retval = visit.func(chunk_info)
+        if visit.retval is not None:
+            return 1
+        return 0
+
 # === Dataset operations ======================================================
 
 @with_phil
 def create(ObjectID loc not None, object name, TypeID tid not None,
            SpaceID space not None, PropID dcpl=None, PropID lcpl=None,
            PropID dapl = None):
     """ (objectID loc, STRING name or None, TypeID tid, SpaceID space,
@@ -615,7 +663,34 @@
                                        &size)
             efree(co)
 
             return StoreInfo(chunk_offset if byte_offset != HADDR_UNDEF else None,
                              filter_mask,
                              byte_offset if byte_offset != HADDR_UNDEF else None,
                              size)
+
+    IF HDF5_VERSION >= (1, 12, 3) or (HDF5_VERSION >= (1, 10, 10) and HDF5_VERSION < (1, 10, 99)):
+
+        @with_phil
+        def chunk_iter(self, object func, PropID dxpl=None):
+            """(CALLABLE func, PropDXID dxpl=None) => <Return value from func>
+
+            Iterate over each chunk and invoke user-supplied "func" callable object.
+            The "func" receives chunk information: logical offset, filter mask,
+            file location, and size. Any not-None return value from "func" ends iteration.
+
+            Feature requires: HDF5 1.10.10 or any later 1.10
+                            HDF5 1.12.3 or later
+
+            .. versionadded:: 3.8
+            """
+            cdef int rank
+            cdef hid_t space_id
+            cdef _ChunkVisitor visit
+
+            space_id = H5Dget_space(self.id)
+            rank = H5Sget_simple_extent_ndims(space_id)
+            H5Sclose(space_id)
+            visit = _ChunkVisitor(rank, func)
+            H5Dchunk_iter(self.id, pdefault(dxpl), <H5D_chunk_iter_op_t>_cb_chunk_info, <void*>visit)
+
+            return visit.retval
```

### Comparing `h5py-3.7.0/h5py/h5ds.pyx` & `h5py-3.8.0/h5py/h5ds.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5f.pyx` & `h5py-3.8.0/h5py/h5f.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5fd.pyx` & `h5py-3.8.0/h5py/h5fd.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -212,9 +212,11 @@
                H5FD_MEM_SUPER,  # super
                H5FD_MEM_SUPER,  # btree
                H5FD_MEM_DRAW,   # draw
                H5FD_MEM_DRAW,   # gheap
                H5FD_MEM_SUPER,  # lheap
                H5FD_MEM_SUPER   # ohdr
 	       ]
+IF HDF5_VERSION >= (1, 14, 0):
+    info.version = H5FD_CLASS_VERSION
 
 fileobj_driver = H5FDregister(&info)
```

### Comparing `h5py-3.7.0/h5py/h5g.pyx` & `h5py-3.8.0/h5py/h5g.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5i.pyx` & `h5py-3.8.0/h5py/h5i.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5l.pyx` & `h5py-3.8.0/h5py/h5l.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5o.pyx` & `h5py-3.8.0/h5py/h5o.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5p.pxd` & `h5py-3.8.0/h5py/h5p.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5p.pyx` & `h5py-3.8.0/h5py/h5p.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -543,14 +543,22 @@
 
         # check for vlen strings
         # create correct typeID and convert from c_str pointer to string
         string_info = check_string_dtype(value.dtype)
         if string_info is not None and string_info.length is None:
             tid = py_create(value.dtype, logical=1)
             ret = H5Pget_fill_value(self.id, tid.id, &c_ptr)
+            if c_ptr == NULL:
+                # If the pointer is NULL (either the value did not get changed,
+                # or maybe the 0 length string, it's unclear currently), if
+                # PyBytes_FromString is called on the pointer, we get a
+                # segfault. If we set the value to empty bytes, then we
+                # shouldn't segfault.
+                value[0] = b""
+                return
             fill_value = c_ptr
             value[0] = fill_value
             return
 
         tid = py_create(value.dtype)
         H5Pget_fill_value(self.id, tid.id, value.data)
 
@@ -1086,15 +1094,15 @@
                           char* secret_key=""):
             """(STRING aws_region, STRING secret_id, STRING secret_key)
 
             Set up the ros3 driver.
             """
             cdef H5FD_ros3_fapl_t config
             config.version = H5FD_CURR_ROS3_FAPL_T_VERSION
-            if len(aws_region) or len(secret_id) or len(secret_key):
+            if len(aws_region) and len(secret_id) and len(secret_key):
                 config.authenticate = <hbool_t>1
             else:
                 config.authenticate = <hbool_t>0
             config.aws_region = aws_region
             config.secret_id = secret_id
             config.secret_key = secret_key
             H5Pset_fapl_ros3(self.id, &config)
@@ -1283,14 +1291,31 @@
         - h5f.LIBVER_V110 (HDF5 1.10.2 or later)
         - h5f.LIBVER_V112 (HDF5 1.11.4 or later)
         - h5f.LIBVER_V114 (HDF5 1.13.0 or later)
         - h5f.LIBVER_LATEST
         """
         H5Pset_libver_bounds(self.id, <H5F_libver_t>low, <H5F_libver_t>high)
 
+    @with_phil
+    def set_meta_block_size(self, size_t size):
+        """ (UINT size)
+
+        Set the current minimum size, in bytes, of new metadata block allocations.
+        """
+        H5Pset_meta_block_size(self.id, size)
+
+    @with_phil
+    def get_meta_block_size(self):
+        """ () => UINT size
+
+        Get the current minimum size, in bytes, of new metadata block allocations.
+        """
+        cdef hsize_t size
+        H5Pget_meta_block_size(self.id, &size)
+        return size
 
     @with_phil
     def get_libver_bounds(self):
         """ () => (INT low, INT high)
 
         Get the compatibility level for file format. Returned values are from:
```

### Comparing `h5py-3.7.0/h5py/h5pl.pxd` & `h5py-3.8.0/h5py/h5pl.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5pl.pyx` & `h5py-3.8.0/h5py/h5pl.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5py_warnings.py` & `h5py-3.8.0/h5py/h5py_warnings.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5r.pxd` & `h5py-3.8.0/h5py/h5r.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5r.pyx` & `h5py-3.8.0/h5py/h5r.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5s.pyx` & `h5py-3.8.0/h5py/h5s.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/h5t.pxd` & `h5py-3.8.0/h5py/h5t.pxd`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Copyright 2008-2013 Andrew Collette and contributors
 #
 # License:  Standard 3-clause BSD; see "license.txt" for full license terms
 #           and contributor agreement.
 
 from .defs cimport *
 
-from ._objects cimport class ObjectID
+from ._objects cimport ObjectID
 
 cdef class TypeID(ObjectID):
 
     cdef object py_dtype(self)
 
 # --- Top-level classes ---
```

### Comparing `h5py-3.7.0/h5py/h5t.pyx` & `h5py-3.8.0/h5py/h5t.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1219,15 +1219,16 @@
             field_offsets.append(self.get_member_offset(i))
 
 
         # 1. Check if it should be converted to a complex number
         if len(field_names) == 2                                and \
             tuple(field_names) == (cfg._r_name, cfg._i_name)    and \
             field_types[0] == field_types[1]                    and \
-            field_types[0].kind == 'f':
+            field_types[0].kind == 'f'                          and \
+            field_types[0].itemsize in (4, 8, 16):
 
             bstring = field_types[0].str
             blen = int(bstring[2:])
             nstring = bstring[0] + "c" + str(2*blen)
             typeobj = np.dtype(nstring)
 
         # 2. Otherwise, read all fields of the compound type, in HDF5 order.
```

### Comparing `h5py-3.7.0/h5py/h5z.pyx` & `h5py-3.8.0/h5py/h5z.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/ipy_completer.py` & `h5py-3.8.0/h5py/ipy_completer.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/__init__.py` & `h5py-3.8.0/h5py/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/common.py` & `h5py-3.8.0/h5py/tests/common.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/data_files/vlen_string_dset.h5` & `h5py-3.8.0/h5py/tests/data_files/vlen_string_dset.h5`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/data_files/vlen_string_dset_utc.h5` & `h5py-3.8.0/h5py/tests/data_files/vlen_string_dset_utc.h5`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/data_files/vlen_string_s390x.h5` & `h5py-3.8.0/h5py/tests/data_files/vlen_string_s390x.h5`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_attribute_create.py` & `h5py-3.8.0/h5py/tests/test_attribute_create.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_attrs.py` & `h5py-3.8.0/h5py/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_attrs_data.py` & `h5py-3.8.0/h5py/tests/test_attrs_data.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_base.py` & `h5py-3.8.0/h5py/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_big_endian_file.py` & `h5py-3.8.0/h5py/tests/test_big_endian_file.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_completions.py` & `h5py-3.8.0/h5py/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_dataset.py` & `h5py-3.8.0/h5py/tests/test_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,14 +472,33 @@
     def test_exc(self):
         """ Bogus fill value raises ValueError """
         with self.assertRaises(ValueError):
             dset = self.f.create_dataset('foo', (10,),
                     dtype=[('a', 'i'), ('b', 'f')], fillvalue=42)
 
 
+@pytest.mark.parametrize('dt,expected', [
+    (int, 0),
+    (np.int32, 0),
+    (np.int64, 0),
+    (float, 0.0),
+    (np.float32, 0.0),
+    (np.float64, 0.0),
+    (h5py.string_dtype(encoding='utf-8', length=5), b''),
+    (h5py.string_dtype(encoding='ascii', length=5), b''),
+    (h5py.string_dtype(encoding='utf-8'), b''),
+    (h5py.string_dtype(encoding='ascii'), b''),
+    (h5py.string_dtype(), b''),
+
+])
+def test_get_unset_fill_value(dt, expected, writable_file):
+    dset = writable_file.create_dataset('foo', (10,), dtype=dt)
+    assert dset.fillvalue == expected
+
+
 class TestCreateNamedType(BaseDataset):
 
     """
         Feature: Datasets created from an existing named type
     """
 
     def test_named(self):
@@ -1033,14 +1052,21 @@
     """
 
     def test_dtype(self):
         """ Retrieve dtype from dataset """
         dset = self.f.create_dataset('foo', (5,), '|S10')
         self.assertEqual(dset.dtype, np.dtype('|S10'))
 
+    def test_dtype_complex32(self):
+        """ Retrieve dtype from complex float16 dataset (gh-2156) """
+        # No native support in numpy as of v1.23.3, so expect compound type.
+        complex32 = np.dtype([('r', np.float16), ('i', np.float16)])
+        dset = self.f.create_dataset('foo', (5,), complex32)
+        self.assertEqual(dset.dtype, complex32)
+
 
 class TestLen(BaseDataset):
 
     """
         Feature: Size of first axis is available via Python's len
     """
 
@@ -1137,14 +1163,23 @@
         self.assertFalse(tid.is_variable_str())
         self.assertEqual(tid.get_size(), 10)
         self.assertEqual(tid.get_cset(), h5py.h5t.CSET_ASCII)
         string_info = h5py.check_string_dtype(ds.dtype)
         self.assertEqual(string_info.encoding, 'ascii')
         self.assertEqual(string_info.length, 10)
 
+    def test_fixed_bytes_fillvalue(self):
+        """ Vlen bytes dataset handles fillvalue """
+        dt = h5py.string_dtype(encoding='ascii', length=10)
+        fill_value = b'bar'
+        ds = self.f.create_dataset('x', (100,), dtype=dt, fillvalue=fill_value)
+        self.assertEqual(self.f['x'][0], fill_value)
+        self.assertEqual(self.f['x'].asstr()[0], fill_value.decode())
+        self.assertEqual(self.f['x'].fillvalue, fill_value)
+
     def test_fixed_utf8(self):
         dt = h5py.string_dtype(encoding='utf-8', length=5)
         ds = self.f.create_dataset('x', (100,), dtype=dt)
         tid = ds.id.get_type()
         self.assertEqual(tid.get_cset(), h5py.h5t.CSET_UTF8)
         s = 'cù'
         ds[0] = s.encode('utf-8')
@@ -1153,14 +1188,23 @@
         ds[4:6] = np.array([s, s], dtype=object)
         ds[6:8] = np.array([s.encode('utf-8')] * 2, dtype=dt)
         with self.assertRaises(TypeError):
             ds[8:10] = np.array([s, s], dtype='U')
 
         np.testing.assert_array_equal(ds[:8], np.array([s.encode('utf-8')] * 8, dtype='S'))
 
+    def test_fixed_utf_8_fillvalue(self):
+        """ Vlen unicode dataset handles fillvalue """
+        dt = h5py.string_dtype(encoding='utf-8', length=10)
+        fill_value = 'bár'.encode("utf-8")
+        ds = self.f.create_dataset('x', (100,), dtype=dt, fillvalue=fill_value)
+        self.assertEqual(self.f['x'][0], fill_value)
+        self.assertEqual(self.f['x'].asstr()[0], fill_value.decode("utf-8"))
+        self.assertEqual(self.f['x'].fillvalue, fill_value)
+
     def test_fixed_unicode(self):
         """ Fixed-length unicode datasets are unsupported (raise TypeError) """
         dt = np.dtype("|U10")
         with self.assertRaises(TypeError):
             ds = self.f.create_dataset('x', (100,), dtype=dt)
 
     def test_roundtrip_vlen_bytes(self):
@@ -1332,14 +1376,24 @@
         np.testing.assert_array_equal(
             self.f['test'].fields(['x', 'y'])[:], testdata[['x', 'y']]
         )
         # Extract single field
         np.testing.assert_array_equal(
             self.f['test'].fields('x')[:], testdata['x']
         )
+        # Check __array__() method of fields wrapper
+        np.testing.assert_array_equal(
+            np.asarray(self.f['test'].fields(['x', 'y'])), testdata[['x', 'y']]
+        )
+        # Check type conversion of __array__() method
+        dt_int = np.dtype([('x', np.int32)])
+        np.testing.assert_array_equal(
+            np.asarray(self.f['test'].fields(['x']), dtype=dt_int),
+            testdata[['x']].astype(dt_int)
+        )
 
         # Check len() on fields wrapper
         assert len(self.f['test'].fields('x')) == 16
 
 
 class TestSubarray(BaseDataset):
     def test_write_list(self):
@@ -1736,14 +1790,46 @@
         si = ds.get_chunk_info_by_coord((0, 0))
         assert si.chunk_offset == (0, 0)
         assert si.filter_mask == 0
         assert si.byte_offset is not None
         assert si.size > 0
 
 
+@ut.skipUnless(h5py.version.hdf5_version_tuple >= (1, 12, 3) or
+               (h5py.version.hdf5_version_tuple >= (1, 10, 10) and h5py.version.hdf5_version_tuple < (1, 10, 99)),
+               "chunk iteration requires  HDF5 1.10.10 and later 1.10, or 1.12.3 and later")
+def test_chunk_iter():
+    """H5Dchunk_iter() for chunk information"""
+    from io import BytesIO
+    buf = BytesIO()
+    with h5py.File(buf, 'w') as f:
+        f.create_dataset('test', shape=(100, 100), chunks=(10, 10), dtype='i4')
+        f['test'][:] = 1
+
+    buf.seek(0)
+    with h5py.File(buf, 'r') as f:
+        dsid = f['test'].id
+
+        num_chunks = dsid.get_num_chunks()
+        assert num_chunks == 100
+        ci = {}
+        for j in range(num_chunks):
+            si = dsid.get_chunk_info(j)
+            ci[si.chunk_offset] = si
+
+        def callback(chunk_info):
+            known = ci[chunk_info.chunk_offset]
+            assert chunk_info.chunk_offset == known.chunk_offset
+            assert chunk_info.filter_mask == known.filter_mask
+            assert chunk_info.byte_offset == known.byte_offset
+            assert chunk_info.size == known.size
+
+        dsid.chunk_iter(callback)
+
+
 def test_empty_shape(writable_file):
     ds = writable_file.create_dataset('empty', dtype='int32')
     assert ds.shape is None
     assert ds.maxshape is None
 
 
 def test_zero_storage_size():
@@ -1801,14 +1887,36 @@
     ds = writable_file.create_dataset(
         'data', shape=(10, 10), dtype=np.uint8, compression=fake_filter_id,
         allow_unknown_filter=True
     )
     assert str(fake_filter_id) in ds._filters
 
 
+def test_dset_chunk_cache():
+    """Chunk cache configuration for individual datasets."""
+    from io import BytesIO
+    buf = BytesIO()
+    with h5py.File(buf, 'w') as fout:
+        ds = fout.create_dataset(
+            'x', shape=(10, 20), chunks=(5, 4), dtype='i4',
+            rdcc_nbytes=2 * 1024 * 1024, rdcc_w0=0.2, rdcc_nslots=997)
+        ds_chunk_cache = ds.id.get_access_plist().get_chunk_cache()
+        assert fout.id.get_access_plist().get_cache()[1:] != ds_chunk_cache
+        assert ds_chunk_cache == (997, 2 * 1024 * 1024, 0.2)
+
+    buf.seek(0)
+    with h5py.File(buf, 'r') as fin:
+        ds = fin.require_dataset(
+            'x', shape=(10, 20), dtype='i4',
+            rdcc_nbytes=3 * 1024 * 1024, rdcc_w0=0.67, rdcc_nslots=709)
+        ds_chunk_cache = ds.id.get_access_plist().get_chunk_cache()
+        assert fin.id.get_access_plist().get_cache()[1:] != ds_chunk_cache
+        assert ds_chunk_cache == (709, 3 * 1024 * 1024, 0.67)
+
+
 class TestCommutative(BaseDataset):
     """
     Test the symmetry of operators, at least with the numpy types.
     Issue: https://github.com/h5py/h5py/issues/1947
     """
     def test_numpy_commutative(self,):
         """
```

### Comparing `h5py-3.7.0/h5py/tests/test_dataset_getitem.py` & `h5py-3.8.0/h5py/tests/test_dataset_getitem.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_dataset_swmr.py` & `h5py-3.8.0/h5py/tests/test_dataset_swmr.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_datatype.py` & `h5py-3.8.0/h5py/tests/test_datatype.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_dimension_scales.py` & `h5py-3.8.0/h5py/tests/test_dimension_scales.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,7 +207,16 @@
 
     def test_attributes(self):
         self.f["data2"].attrs["DIMENSION_LIST"] = self.f["data"].attrs[
             "DIMENSION_LIST"]
         self.assertEqual(len(self.f['data2'].dims[0]), 0)
         self.assertEqual(len(self.f['data2'].dims[1]), 1)
         self.assertEqual(len(self.f['data2'].dims[2]), 2)
+
+    def test_is_scale(self):
+        """Test Dataset.is_scale property"""
+        self.assertTrue(self.f['x1'].is_scale)
+        self.assertTrue(self.f['x2'].is_scale)
+        self.assertTrue(self.f['y1'].is_scale)
+        self.assertFalse(self.f['z1'].is_scale)
+        self.assertFalse(self.f['data'].is_scale)
+        self.assertFalse(self.f['data2'].is_scale)
```

### Comparing `h5py-3.7.0/h5py/tests/test_dims_dimensionproxy.py` & `h5py-3.8.0/h5py/tests/test_dims_dimensionproxy.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_dtype.py` & `h5py-3.8.0/h5py/tests/test_dtype.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_errors.py` & `h5py-3.8.0/h5py/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_file.py` & `h5py-3.8.0/h5py/tests/test_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1005,30 +1005,14 @@
             f["data"] = 1
 
         with h5py.File(fname, mode="r", locking=False) as f:
             # Opening in write mode with locking is expected to work
             assert open_in_subprocess(fname, mode="w", locking=True)
 
 
-# unittest doesn't work with pytest fixtures (and possibly other features),
-# hence no subclassing TestCase
-class TestROS3:
-    @pytest.mark.skipif(h5py.version.hdf5_version_tuple < (1, 10, 6)
-                        or not h5.get_config().ros3,
-                        reason="ros3 file operations were added in HDF5 1.10.6+")
-    def test_ros3(self):
-        """ ROS3 driver and options """
-
-        with File("https://dandiarchive.s3.amazonaws.com/ros3test.hdf5", 'r',
-                  driver='ros3') as f:
-            assert f
-            assert 'mydataset' in f.keys()
-            assert f["mydataset"].shape == (100,)
-
-
 def test_close_gc(writable_file):
     # https://github.com/h5py/h5py/issues/1852
     for i in range(100):
         writable_file[str(i)] = []
 
     filename = writable_file.filename
     writable_file.close()
```

### Comparing `h5py-3.7.0/h5py/tests/test_file2.py` & `h5py-3.8.0/h5py/tests/test_file2.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 
 """
     Tests the h5py.File object.
 """
 
 import h5py
 from h5py._hl.files import _drivers
+from h5py import File
 
 from .common import ut, TestCase
 
+import pytest
 import io
 import tempfile
 import os
 
 
 def nfiles():
     return h5py.h5f.get_obj_count(h5py.h5f.OBJ_ALL, h5py.h5f.OBJ_FILE)
@@ -269,7 +271,45 @@
 
     def test_no_track_order(self):
         fname = self.mktemp()
         f = h5py.File(fname, 'w', track_order=False)  # name alphanumeric
         self.populate(f)
         self.assertEqual(list(f),
                          sorted([str(i) for i in range(100)]))
+
+
+class TestFileMetaBlockSize(TestCase):
+
+    """
+        Feature: The meta block size can be manipulated, changing how metadata
+        is aggregated and the offset of the first dataset.
+    """
+
+    def test_file_create_with_meta_block_size_4096(self):
+        # Test a large meta block size of 4 kibibytes
+        meta_block_size = 4096
+        with File(
+            self.mktemp(), 'w',
+            meta_block_size=meta_block_size,
+            libver="latest"
+        ) as f:
+            f["test"] = 5
+            self.assertEqual(f.meta_block_size, meta_block_size)
+            # Equality is expected for HDF5 1.10
+            self.assertGreaterEqual(f["test"].id.get_offset(), meta_block_size)
+
+    def test_file_create_with_meta_block_size_512(self):
+        # Test a small meta block size of 512 bytes
+        # The smallest verifiable meta_block_size is 463
+        meta_block_size = 512
+        libver = "latest"
+        with File(
+            self.mktemp(), 'w',
+            meta_block_size=meta_block_size,
+            libver=libver
+        ) as f:
+            f["test"] = 3
+            self.assertEqual(f.meta_block_size, meta_block_size)
+            # Equality is expected for HDF5 1.10
+            self.assertGreaterEqual(f["test"].id.get_offset(), meta_block_size)
+            # Default meta_block_size is 2048. This should fail if meta_block_size is not set.
+            self.assertLess(f["test"].id.get_offset(), meta_block_size*2)
```

### Comparing `h5py-3.7.0/h5py/tests/test_file_alignment.py` & `h5py-3.8.0/h5py/tests/test_file_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 # Create up to 1000 datasets
                 # They are all expected to be aligned
                 for i in range(1000):
                     dataset = h5file.create_dataset(
                         dataset_name(i), shape, dtype='uint8')
                     # Assign data so that the dataset is instantiated in
                     # the file
-                    dataset[...] = i
+                    dataset[...] = (i % 256)  # Truncate to uint8
                     assert is_aligned(dataset, offset=alignment_interval)
 
     def test_alignment_set_below_threshold(self):
         # 2022/01/19 hmaarrfk
         # UnitTest (TestCase) doesn't play well with pytest parametrization.
         alignment_threshold = 1000
         alignment_interval = 1024
```

### Comparing `h5py-3.7.0/h5py/tests/test_file_image.py` & `h5py-3.8.0/h5py/tests/test_file_image.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_filters.py` & `h5py-3.8.0/h5py/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_group.py` & `h5py-3.8.0/h5py/tests/test_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,29 @@
         group = self.f.get('foo')
         assert isinstance(group, Group)
         group = self.f.get('foo/bar')
         assert isinstance(group, Group)
         group = self.f.get('foo/bar/baz')
         assert isinstance(group, Group)
 
+    def test_require_shape(self):
+        ds = self.f.require_dataset("foo/resizable", shape=(0, 3), maxshape=(None, 3), dtype=int)
+        ds.resize(20, axis=0)
+        self.f.require_dataset("foo/resizable", shape=(0, 3), maxshape=(None, 3), dtype=int)
+        self.f.require_dataset("foo/resizable", shape=(20, 3), dtype=int)
+        with self.assertRaises(TypeError):
+            self.f.require_dataset("foo/resizable", shape=(0, 0), maxshape=(3, None), dtype=int)
+        with self.assertRaises(TypeError):
+            self.f.require_dataset("foo/resizable", shape=(0, 0), maxshape=(None, 5), dtype=int)
+        with self.assertRaises(TypeError):
+            self.f.require_dataset("foo/resizable", shape=(0, 0), maxshape=(None, 5, 2), dtype=int)
+        with self.assertRaises(TypeError):
+            self.f.require_dataset("foo/resizable", shape=(10, 3), dtype=int)
+
+
 class TestDelete(BaseGroup):
 
     """
         Feature: Objects can be unlinked via "del" operator
     """
 
     def test_delete(self):
```

### Comparing `h5py-3.7.0/h5py/tests/test_h5.py` & `h5py-3.8.0/h5py/tests/test_h5.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_h5d_direct_chunk.py` & `h5py-3.8.0/h5py/tests/test_h5d_direct_chunk.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_h5f.py` & `h5py-3.8.0/h5py/tests/test_h5f.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_h5p.py` & `h5py-3.8.0/h5py/tests/test_h5p.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_h5pl.py` & `h5py-3.8.0/h5py/tests/test_h5pl.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_h5t.py` & `h5py-3.8.0/h5py/tests/test_h5t.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_objects.py` & `h5py-3.8.0/h5py/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_selections.py` & `h5py-3.8.0/h5py/tests/test_selections.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,22 +101,30 @@
         dset = self.f.create_dataset('dset', (100,100))
         regref = dset.regionref[0:100, 0:100]
 
         # args is list, return a FancySelection
         st = sel.select((10,), list([1,2,3]), dset)
         self.assertIsInstance(st, sel.FancySelection)
 
+        # args[0] is tuple, return a FancySelection
+        st = sel.select((10,), ((1, 2, 3),), dset)
+        self.assertIsInstance(st, sel.FancySelection)
+
         # args is a Boolean mask, return a PointSelection
         st1 = sel.select((5,), np.array([True,False,False,False,True]), dset)
         self.assertIsInstance(st1, sel.PointSelection)
 
         # args is int, return a SimpleSelection
         st2 = sel.select((10,), 1, dset)
         self.assertIsInstance(st2, sel.SimpleSelection)
 
+        # args is str, should be rejected
+        with self.assertRaises(TypeError):
+            sel.select((100,), "foo", dset)
+
         # args is RegionReference, return a Selection instance
         st3 = sel.select((100,100), regref, dset)
         self.assertIsInstance(st3, sel.Selection)
 
         # args is RegionReference, but dataset is None
         with self.assertRaises(TypeError):
             sel.select((100,), regref, None)
```

### Comparing `h5py-3.7.0/h5py/tests/test_slicing.py` & `h5py-3.8.0/h5py/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_vds/test_highlevel_vds.py` & `h5py-3.8.0/h5py/tests/test_vds/test_highlevel_vds.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_vds/test_lowlevel_vds.py` & `h5py-3.8.0/h5py/tests/test_vds/test_lowlevel_vds.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/tests/test_vds/test_virtual_source.py` & `h5py-3.8.0/h5py/tests/test_vds/test_virtual_source.py`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/utils.pxd` & `h5py-3.8.0/h5py/utils.pxd`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/utils.pyx` & `h5py-3.8.0/h5py/utils.pyx`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/h5py/version.py` & `h5py-3.8.0/h5py/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # All should be integers, except pre, as validating versions is more than is
 # needed for our use case
 _H5PY_VERSION_CLS = namedtuple("_H5PY_VERSION_CLS",
                                "major minor bugfix pre post dev")
 
 hdf5_built_version_tuple = _h5.HDF5_VERSION_COMPILED_AGAINST
 
-version_tuple = _H5PY_VERSION_CLS(3, 7, 0, None, None, None)
+version_tuple = _H5PY_VERSION_CLS(3, 8, 0, None, None, None)
 
 version = "{0.major:d}.{0.minor:d}.{0.bugfix:d}".format(version_tuple)
 if version_tuple.pre is not None:
     version += version_tuple.pre
 if version_tuple.post is not None:
     version += ".post{0.post:d}".format(version_tuple)
 if version_tuple.dev is not None:
```

### Comparing `h5py-3.7.0/h5py.egg-info/PKG-INFO` & `h5py-3.8.0/h5py.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 Metadata-Version: 2.1
 Name: h5py
-Version: 3.7.0
+Version: 3.8.0
 Summary: Read and write HDF5 files from Python
-Home-page: http://www.h5py.org
-Author: Andrew Collette
-Author-email: andrew.collette@gmail.com
-Maintainer: Andrew Collette
-Maintainer-email: andrew.collette@gmail.com
-License: BSD
-Download-URL: https://pypi.python.org/pypi/h5py
+Author-email: Andrew Collette <andrew.collette@gmail.com>
+Maintainer-email: Thomas Kluyver <thomas@kluyver.me.uk>, Thomas A Caswell <tcaswell@bnl.gov>
+License: BSD-3-Clause
+Project-URL: Homepage, https://www.h5py.org/
 Project-URL: Source, https://github.com/h5py/h5py
-Platform: UNKNOWN
+Project-URL: Documentation, https://docs.h5py.org/en/stable/
+Project-URL: Release notes, https://docs.h5py.org/en/stable/whatsnew/index.html
+Project-URL: Discussion forum, https://forum.hdfgroup.org/c/hdf-tools/h5py
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-
 The h5py package provides both a high- and low-level interface to the HDF5
 library from Python. The low-level interface is intended to be a complete
 wrapping of the HDF5 API, while the high-level component supports  access to
 HDF5 files, datasets and groups using established Python and NumPy concepts.
 
 A strong emphasis on automatic conversion between Python (Numpy) datatypes and
 data structures and their HDF5 equivalents vastly simplifies the process of
 reading and writing data from Python.
 
-Supports HDF5 versions 1.8.4 and higher.  On Windows, HDF5 is included with
-the installer.
-
+Wheels are provided for several popular platforms, with an included copy of
+the HDF5 library (usually the latest version when h5py is released).
 
+You can also `build h5py from source
+<https://docs.h5py.org/en/stable/build.html#source-installation>`_
+with any HDF5 stable release from version 1.8.4 onwards, although naturally new
+HDF5 versions released after this version of h5py may not work.
+Odd-numbered minor versions of HDF5 (e.g. 1.13) are experimental, and may not
+be supported.
```

### Comparing `h5py-3.7.0/h5py.egg-info/SOURCES.txt` & `h5py-3.8.0/h5py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 docs/contributing.rst
 docs/faq.rst
 docs/index.rst
 docs/licenses.rst
 docs/mpi.rst
 docs/quick.rst
 docs/refs.rst
+docs/related_projects.rst
 docs/release_guide.rst
 docs/requirements-rtd.txt
 docs/special.rst
 docs/strings.rst
 docs/swmr.rst
 docs/vds.rst
 docs/high/attr.rst
@@ -54,14 +55,15 @@
 docs/whatsnew/3.1.rst
 docs/whatsnew/3.2.rst
 docs/whatsnew/3.3.rst
 docs/whatsnew/3.4.rst
 docs/whatsnew/3.5.rst
 docs/whatsnew/3.6.rst
 docs/whatsnew/3.7.rst
+docs/whatsnew/3.8.rst
 docs/whatsnew/index.rst
 docs_api/Makefile
 docs_api/automod.py
 docs_api/conf.py
 docs_api/h5.rst
 docs_api/h5a.rst
 docs_api/h5ac.rst
@@ -197,14 +199,15 @@
 h5py/tests/test_h5d_direct_chunk.py
 h5py/tests/test_h5f.py
 h5py/tests/test_h5o.py
 h5py/tests/test_h5p.py
 h5py/tests/test_h5pl.py
 h5py/tests/test_h5t.py
 h5py/tests/test_objects.py
+h5py/tests/test_ros3.py
 h5py/tests/test_selections.py
 h5py/tests/test_slicing.py
 h5py/tests/data_files/__init__.py
 h5py/tests/data_files/vlen_string_dset.h5
 h5py/tests/data_files/vlen_string_dset_utc.h5
 h5py/tests/data_files/vlen_string_s390x.h5
 h5py/tests/test_vds/__init__.py
```

### Comparing `h5py-3.7.0/licenses/hdf5.txt` & `h5py-3.8.0/licenses/hdf5.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/licenses/license.txt` & `h5py-3.8.0/licenses/license.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/licenses/pytables.txt` & `h5py-3.8.0/licenses/pytables.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/licenses/python.txt` & `h5py-3.8.0/licenses/python.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/licenses/stdint.txt` & `h5py-3.8.0/licenses/stdint.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/lzf/LICENSE.txt` & `h5py-3.8.0/lzf/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/lzf/README.txt` & `h5py-3.8.0/lzf/README.txt`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 * Downloads:  https://pypi.org/project/h5py/
 
 * Issue tracker:  https://github.com/h5py/h5py
 
 * Main web site and documentation:  http://h5py.org
 
-* mailing list:  https://groups.google.com/forum/#!forum/h5py
+* Discussion forum: https://forum.hdfgroup.org/c/hdf-tools/h5py
 
 
 History of changes
 ------------------
 
 Revision 3 (6/25/09)
     Fix issue with changed filter struct definition under HDF5 1.8.3.
```

### Comparing `h5py-3.7.0/lzf/example.c` & `h5py-3.8.0/lzf/example.c`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/lzf/lzf/lzf.h` & `h5py-3.8.0/lzf/lzf/lzf.h`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/lzf/lzf/lzfP.h` & `h5py-3.8.0/lzf/lzf/lzfP.h`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/lzf/lzf/lzf_c.c` & `h5py-3.8.0/lzf/lzf/lzf_c.c`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/lzf/lzf/lzf_d.c` & `h5py-3.8.0/lzf/lzf/lzf_d.c`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/lzf/lzf_filter.c` & `h5py-3.8.0/lzf/lzf_filter.c`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/lzf/lzf_filter.h` & `h5py-3.8.0/lzf/lzf_filter.h`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/pylintrc` & `h5py-3.8.0/pylintrc`

 * *Files identical despite different names*

### Comparing `h5py-3.7.0/setup_build.py` & `h5py-3.8.0/setup_build.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,19 @@
 
         settings = COMPILER_SETTINGS.copy()
 
         settings['include_dirs'][:0] = config.hdf5_includedirs
         settings['library_dirs'][:0] = config.hdf5_libdirs
         settings['define_macros'].extend(config.hdf5_define_macros)
 
+        if config.msmpi:
+            settings['include_dirs'].extend(config.msmpi_inc_dirs)
+            settings['library_dirs'].extend(config.msmpi_lib_dirs)
+            settings['libraries'].append('msmpi')
+
         try:
             numpy_includes = numpy.get_include()
         except AttributeError:
             # if numpy is not installed get the headers from the .egg directory
             import numpy.core
             numpy_includes = os.path.join(os.path.dirname(numpy.core.__file__), 'include')
```

### Comparing `h5py-3.7.0/setup_configure.py` & `h5py-3.8.0/setup_configure.py`

 * *Files 8% similar despite different names*

```diff
@@ -60,14 +60,29 @@
         self.hdf5_libdirs = hdf5_libdirs
         self.hdf5_define_macros = hdf5_define_macros
         self.hdf5_version = hdf5_version
         self.mpi = mpi
         self.ros3 = ros3
         self.direct_vfd = direct_vfd
 
+        if self.mpi and os.environ.get('H5PY_MSMPI') == 'ON':
+            self.msmpi = True
+            self.msmpi_inc_dirs = os.environ.get('MSMPI_INC').split(';')
+            import platform
+            bitness, _ = platform.architecture()
+            if bitness == '64bit':
+                mpi_lib_envvar = 'MSMPI_LIB64'
+            else:
+                mpi_lib_envvar = 'MSMPI_LIB32'
+            self.msmpi_lib_dirs = os.environ.get(mpi_lib_envvar).split(';')
+        else:
+            self.msmpi = False
+            self.msmpi_inc_dirs = []
+            self.msmpi_lib_dirs = []
+
     @classmethod
     def from_env(cls):
         mpi = mpi_enabled()
         h5_inc, h5_lib, h5_macros = cls._find_hdf5_compiler_settings(mpi)
 
         h5_version_s = os.environ.get('HDF5_VERSION')
         h5py_ros3 = os.environ.get('H5PY_ROS3')
@@ -171,14 +186,17 @@
             'hdf5_includedirs': self.hdf5_includedirs,
             'hdf5_libdirs': self.hdf5_libdirs,
             'hdf5_define_macros': self.hdf5_define_macros,
             'hdf5_version': list(self.hdf5_version),  # list() to match the JSON
             'mpi': self.mpi,
             'ros3': self.ros3,
             'direct_vfd': self.direct_vfd,
+            'msmpi': self.msmpi,
+            'msmpi_inc_dirs': self.msmpi_inc_dirs,
+            'msmpi_lib_dirs': self.msmpi_lib_dirs,
         }
 
     def changed(self):
         """Has the config changed since the last build?"""
         return self.as_dict() != load_stashed_config()
 
     def record_built(self):
@@ -188,21 +206,24 @@
     def summarise(self):
         def fmt_dirs(l):
             return '\n'.join((['['] + [f'  {d!r}' for d in l] + [']'])) if l else '[]'
 
         print('*' * 80)
         print(' ' * 23 + "Summary of the h5py configuration")
         print('')
-        print("HDF5 include dirs:", fmt_dirs(self.hdf5_includedirs))
-        print("HDF5 library dirs:", fmt_dirs(self.hdf5_libdirs))
-        print("     HDF5 Version:", repr(self.hdf5_version))
-        print("      MPI Enabled:", self.mpi)
-        print(" ROS3 VFD Enabled:", self.ros3)
-        print("DIRECT VFD Enabled:", self.direct_vfd)
-        print(" Rebuild Required:", self.changed())
+        print("  HDF5 include dirs:", fmt_dirs(self.hdf5_includedirs))
+        print("  HDF5 library dirs:", fmt_dirs(self.hdf5_libdirs))
+        print("       HDF5 Version:", repr(self.hdf5_version))
+        print("        MPI Enabled:", self.mpi)
+        print("   ROS3 VFD Enabled:", self.ros3)
+        print(" DIRECT VFD Enabled:", self.direct_vfd)
+        print("   Rebuild Required:", self.changed())
+        print("     MS-MPI Enabled:", self.msmpi)
+        print("MS-MPI include dirs:", self.msmpi_inc_dirs)
+        print("MS-MPI library dirs:", self.msmpi_lib_dirs)
         print('')
         print('*' * 80)
 
 
 class HDF5LibWrapper:
 
     def __init__(self, libdirs):
@@ -220,16 +241,20 @@
 
         # extra keyword args to pass to LoadLibrary
         load_kw = {}
         if sys.platform.startswith('darwin'):
             default_path = 'libhdf5.dylib'
             regexp = re.compile(r'^libhdf5.dylib')
         elif sys.platform.startswith('win'):
-            default_path = 'hdf5.dll'
-            regexp = re.compile(r'^hdf5.dll')
+            if 'MSC' in sys.version:
+                default_path = 'hdf5.dll'
+                regexp = re.compile(r'^hdf5.dll')
+            else:
+                default_path = 'libhdf5-0.dll'
+                regexp = re.compile(r'^libhdf5-[0-9].dll')
             if sys.version_info >= (3, 8):
                 # To overcome "difficulty" loading the library on windows
                 # https://bugs.python.org/issue42114
                 load_kw['winmode'] = 0
         elif sys.platform.startswith('cygwin'):
             default_path = 'cyghdf5-200.dll'
             regexp = re.compile(r'^cyghdf5-\d+.dll$')
```

### Comparing `h5py-3.7.0/tox.ini` & `h5py-3.8.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tox]
 # We want an envlist like
 # envlist = {py36,py37,pypy3}-{test}-{deps,mindeps}-{,mpi4py}-{,pre},nightly,docs,checkreadme,pre-commit
 # but we want to skip mpi and pre by default, so this envlist is below
-envlist = {py37,py38,py39,py310,pypy3}-{test}-{deps,mindeps},nightly,docs,apidocs,checkreadme,pre-commit,rever
+envlist = {py37,py38,py39,py310,py311,pypy3}-{test}-{deps,mindeps},nightly,docs,apidocs,checkreadme,pre-commit,rever
 isolated_build = True
 
 [testenv]
 deps =
     test: pytest
     test: pytest-cov
     test: pytest-mpi>=0.2
 
     py37-deps: numpy>=1.14.5
     py38-deps: numpy>=1.17.5
     py39-deps: numpy>=1.19.3
     py310-deps: numpy>=1.21.3
+    py311-deps: numpy>=1.23.2
 
     mindeps: oldest-supported-numpy
 
     mpi4py: mpi4py>=3.0.2
 
     tables-deps: tables>=3.4.4
     tables-mindeps: tables==3.4.4
@@ -41,29 +42,31 @@
     HDF5_LIBDIR
     HDF5_PKGCONFIG_NAME
     HDF5_MPI
     MPI_N_PROCS
     OMPI_* # used to configure OpenMPI
     CC
     ZLIB_ROOT
-whitelist_externals =
+allowlist_externals =
     mpirun
 setenv =
     COVERAGE_FILE={toxinidir}/.coverage_dir/coverage-{envname}
 # needed otherwise coverage cannot find the file when reporting
 
 pip_pre =
     pre: True
 
 [testenv:nightly]
 pip_pre = True
 basepython = python3.8
 
 [testenv:docs]
 skip_install=True
+# Work around https://github.com/tox-dev/tox/issues/2442
+package_env = DUMMY NON-EXISTENT ENV NAME
 changedir=docs
 deps=
     sphinx
 commands=
     sphinx-build -W -b html -d {envtmpdir}/doctrees .  {envtmpdir}/html
 
 [testenv:apidocs]
@@ -71,28 +74,38 @@
 deps=
     sphinx
 commands=
     sphinx-build -W -b html -d {envtmpdir}/doctrees .  _build/html
 
 [testenv:checkreadme]
 skip_install=True
-deps=twine
+# Work around https://github.com/tox-dev/tox/issues/2442
+package_env = DUMMY NON-EXISTENT ENV NAME
+deps=
+    build
+    twine
 commands=
-    python setup.py sdist
-    twine check dist/*
+    python -m build --sdist
+    twine check --strict dist/*
 
 [testenv:pre-commit]
 skip_install=True
+# Work around https://github.com/tox-dev/tox/issues/2442
+package_env = DUMMY NON-EXISTENT ENV NAME
 deps=pre-commit
-passenv = HOMEPATH SSH_AUTH_SOCK
+passenv =
+    HOMEPATH
+    SSH_AUTH_SOCK
 commands=
     pre-commit run --all-files
 
 [testenv:rever]
 skip_install=True
+# Work around https://github.com/tox-dev/tox/issues/2442
+package_env = DUMMY NON-EXISTENT ENV NAME
 deps=
     re-ver
     xonsh
     lazyasd
     ruamel.yaml
 commands=
     rever check --activities version_bump,changelog
```

