# Comparing `tmp/tmkit-0.0.0.1.tar.gz` & `tmp/tmkit-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmkit-0.0.0.1.tar", last modified: Mon Jun 19 23:14:32 2023, max compression
+gzip compressed data, was "tmkit-0.0.0.2.tar", last modified: Mon Jun 19 23:19:13 2023, max compression
```

## Comparing `tmkit-0.0.0.1.tar` & `tmkit-0.0.0.2.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.619811 tmkit-0.0.0.1/
--rw-rw-rw-   0        0        0    35823 2022-10-06 19:26:08.000000 tmkit-0.0.0.1/LICENSE
--rw-rw-rw-   0        0        0      302 2023-06-19 23:14:32.617812 tmkit-0.0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1506 2023-03-29 23:16:56.000000 tmkit-0.0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 23:14:32.619811 tmkit-0.0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      715 2023-06-19 23:14:27.000000 tmkit-0.0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.239815 tmkit-0.0.0.1/tmkit/
--rw-rw-rw-   0        0        0      458 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/Path.py
--rw-rw-rw-   0        0        0     4375 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/SeqNetRR.py
--rw-rw-rw-   0        0        0      237 2022-10-06 14:33:16.000000 tmkit-0.0.0.1/tmkit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.268812 tmkit-0.0.0.1/tmkit/base/
--rw-rw-rw-   0        0        0     2936 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/base/PDB.py
--rw-rw-rw-   0        0        0     1004 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/base/Position.py
--rw-rw-rw-   0        0        0       76 2019-09-15 16:59:06.000000 tmkit-0.0.0.1/tmkit/base/__init__.py
--rw-rw-rw-   0        0        0     2114 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/cath.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.282816 tmkit-0.0.0.1/tmkit/chain/
--rw-rw-rw-   0        0        0     5301 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/chain/Collate.py
--rw-rw-rw-   0        0        0     8052 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/chain/CollateBatch.py
--rw-rw-rw-   0        0        0      599 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/chain/PDB.py
--rw-rw-rw-   0        0        0        0 2022-08-06 11:29:10.000000 tmkit-0.0.0.1/tmkit/chain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.288812 tmkit-0.0.0.1/tmkit/channel/
--rw-rw-rw-   0        0        0     7568 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/channel/Workbench.py
--rw-rw-rw-   0        0        0        0 2019-08-11 19:08:40.000000 tmkit-0.0.0.1/tmkit/channel/__init__.py
--rw-rw-rw-   0        0        0     3047 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/collate.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.297811 tmkit-0.0.0.1/tmkit/contact/
--rw-rw-rw-   0        0        0     7971 2023-06-19 13:33:30.000000 tmkit-0.0.0.1/tmkit/contact/Evaluator.py
--rw-rw-rw-   0        0        0    24790 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/contact/Reader.py
--rw-rw-rw-   0        0        0        0 2019-08-11 18:38:08.000000 tmkit-0.0.0.1/tmkit/contact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.306813 tmkit-0.0.0.1/tmkit/db/
--rw-rw-rw-   0        0        0     7934 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/db/Connectivity.py
--rw-rw-rw-   0        0        0     3676 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/db/Reader.py
--rw-rw-rw-   0        0        0        0 2019-05-10 13:10:28.000000 tmkit-0.0.0.1/tmkit/db/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.311811 tmkit-0.0.0.1/tmkit/db/biogrid/
--rw-rw-rw-   0        0        0     1710 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/db/biogrid/Reader.py
--rw-rw-rw-   0        0        0        0 2020-07-08 14:38:06.000000 tmkit-0.0.0.1/tmkit/db/biogrid/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.316811 tmkit-0.0.0.1/tmkit/db/cath/
--rw-rw-rw-   0        0        0     5065 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/db/cath/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-11 11:28:12.000000 tmkit-0.0.0.1/tmkit/db/cath/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.320811 tmkit-0.0.0.1/tmkit/db/construct/
--rw-rw-rw-   0        0        0     3320 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/db/construct/Network.py
--rw-rw-rw-   0        0        0        0 2020-08-28 22:57:35.000000 tmkit-0.0.0.1/tmkit/db/construct/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.325811 tmkit-0.0.0.1/tmkit/db/intact/
--rw-rw-rw-   0        0        0     2075 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/db/intact/Reader.py
--rw-rw-rw-   0        0        0        0 2020-07-11 22:05:59.000000 tmkit-0.0.0.1/tmkit/db/intact/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.330812 tmkit-0.0.0.1/tmkit/db/muthtp/
--rw-rw-rw-   0        0        0     3703 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/db/muthtp/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-07 05:11:20.000000 tmkit-0.0.0.1/tmkit/db/muthtp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.336812 tmkit-0.0.0.1/tmkit/db/predmuthtp/
--rw-rw-rw-   0        0        0     2939 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/db/predmuthtp/Reader.py
--rw-rw-rw-   0        0        0        0 2022-08-07 05:11:42.000000 tmkit-0.0.0.1/tmkit/db/predmuthtp/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/edge.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.341815 tmkit-0.0.0.1/tmkit/feature/
--rw-rw-rw-   0        0        0     8018 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/feature/HelixSurface.py
--rw-rw-rw-   0        0        0        0 2022-07-15 21:53:29.000000 tmkit-0.0.0.1/tmkit/feature/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.344812 tmkit-0.0.0.1/tmkit/feature/lips/
--rw-rw-rw-   0        0        0        0 2019-08-01 10:52:35.000000 tmkit-0.0.0.1/tmkit/feature/lips/__init__.py
--rw-rw-rw-   0        0        0     9415 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/feature.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.357814 tmkit-0.0.0.1/tmkit/id/
--rw-rw-rw-   0        0        0      568 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/id/Fasta.py
--rw-rw-rw-   0        0        0     2717 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/id/Mapping.py
--rw-rw-rw-   0        0        0     1035 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/id/PDB.py
--rw-rw-rw-   0        0        0        0 2020-04-26 23:07:36.000000 tmkit-0.0.0.1/tmkit/id/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.367811 tmkit-0.0.0.1/tmkit/interface/
--rw-rw-rw-   0        0        0      387 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/interface/Tool.py
--rw-rw-rw-   0        0        0      398 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/interface/Topology.py
--rw-rw-rw-   0        0        0        0 2020-07-09 17:22:43.000000 tmkit-0.0.0.1/tmkit/interface/__init__.py
--rw-rw-rw-   0        0        0      811 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/mapping.py
--rw-rw-rw-   0        0        0     6409 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/msa.py
--rw-rw-rw-   0        0        0     1928 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/mut.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.372813 tmkit-0.0.0.1/tmkit/name/
--rw-rw-rw-   0        0        0     4437 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/name/Mapping.py
--rw-rw-rw-   0        0        0        0 2022-08-06 12:13:25.000000 tmkit-0.0.0.1/tmkit/name/__init__.py
--rw-rw-rw-   0        0        0        0 2022-07-16 21:39:03.000000 tmkit-0.0.0.1/tmkit/pl.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.375811 tmkit-0.0.0.1/tmkit/position/
--rw-rw-rw-   0        0        0       16 2019-09-15 17:43:20.000000 tmkit-0.0.0.1/tmkit/position/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.384813 tmkit-0.0.0.1/tmkit/position/scenario/
--rw-rw-rw-   0        0        0     1724 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/position/scenario/Segment.py
--rw-rw-rw-   0        0        0     2421 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/position/scenario/Separation.py
--rw-rw-rw-   0        0        0        0 2019-09-21 21:40:26.000000 tmkit-0.0.0.1/tmkit/position/scenario/__init__.py
--rw-rw-rw-   0        0        0     4938 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/ppi.py
--rw-rw-rw-   0        0        0     2260 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/qc.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.394815 tmkit-0.0.0.1/tmkit/retrieve/
--rw-rw-rw-   0        0        0    15864 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/retrieve/MSA.py
--rw-rw-rw-   0        0        0     3976 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/retrieve/PDB.py
--rw-rw-rw-   0        0        0     2142 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/retrieve/XML.py
--rw-rw-rw-   0        0        0        0 2019-05-10 15:10:49.000000 tmkit-0.0.0.1/tmkit/retrieve/__init__.py
--rw-rw-rw-   0        0        0     5100 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/rrc.py
--rw-rw-rw-   0        0        0     4126 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/seq.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.410812 tmkit-0.0.0.1/tmkit/seqnetrr/
--rw-rw-rw-   0        0        0     9679 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/Compare.py
--rw-rw-rw-   0        0        0    13327 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/Controller.py
--rw-rw-rw-   0        0        0      491 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/Path.py
--rw-rw-rw-   0        0        0    34474 2022-10-06 14:12:35.000000 tmkit-0.0.0.1/tmkit/seqnetrr/Plot.py
--rw-rw-rw-   0        0        0        0 2022-05-17 20:55:49.000000 tmkit-0.0.0.1/tmkit/seqnetrr/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.426811 tmkit-0.0.0.1/tmkit/seqnetrr/combo/
--rw-rw-rw-   0        0        0     2183 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/combo/Length.py
--rw-rw-rw-   0        0        0      470 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/combo/Param.py
--rw-rw-rw-   0        0        0     1676 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/combo/Position.py
--rw-rw-rw-   0        0        0     2494 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/combo/Separation.py
--rw-rw-rw-   0        0        0        0 2019-08-11 16:35:38.000000 tmkit-0.0.0.1/tmkit/seqnetrr/combo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.436811 tmkit-0.0.0.1/tmkit/seqnetrr/graph/
--rw-rw-rw-   0        0        0    19034 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/seqnetrr/graph/Bipartite.py
--rw-rw-rw-   0        0        0     4855 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/seqnetrr/graph/Cumulative.py
--rw-rw-rw-   0        0        0    21160 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/graph/Unipartite.py
--rw-rw-rw-   0        0        0        0 2022-05-18 21:29:35.000000 tmkit-0.0.0.1/tmkit/seqnetrr/graph/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.441811 tmkit-0.0.0.1/tmkit/seqnetrr/net/
--rw-rw-rw-   0        0        0    25261 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/net/Reader.py
--rw-rw-rw-   0        0        0        0 2022-06-12 23:19:50.000000 tmkit-0.0.0.1/tmkit/seqnetrr/net/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.445811 tmkit-0.0.0.1/tmkit/seqnetrr/sequence/
--rw-rw-rw-   0        0        0     1965 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/seqnetrr/sequence/Fasta.py
--rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.0.1/tmkit/seqnetrr/sequence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.459812 tmkit-0.0.0.1/tmkit/seqnetrr/util/
--rw-rw-rw-   0        0        0     5609 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/util/ComputLib.py
--rw-rw-rw-   0        0        0      838 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/util/Console.py
--rw-rw-rw-   0        0        0     2866 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/seqnetrr/util/Reader.py
--rw-rw-rw-   0        0        0     2201 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/util/Writer.py
--rw-rw-rw-   0        0        0        0 2022-05-18 16:43:31.000000 tmkit-0.0.0.1/tmkit/seqnetrr/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.467811 tmkit-0.0.0.1/tmkit/seqnetrr/window/
--rw-rw-rw-   0        0        0     5855 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/seqnetrr/window/Pair.py
--rw-rw-rw-   0        0        0     5780 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/seqnetrr/window/Single.py
--rw-rw-rw-   0        0        0        0 2019-09-18 20:19:22.000000 tmkit-0.0.0.1/tmkit/seqnetrr/window/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.475814 tmkit-0.0.0.1/tmkit/seqnetrr/window/base/
--rw-rw-rw-   0        0        0     1316 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/window/base/Pair.py
--rw-rw-rw-   0        0        0     1318 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/seqnetrr/window/base/Single.py
--rw-rw-rw-   0        0        0        0 2019-09-19 13:22:58.000000 tmkit-0.0.0.1/tmkit/seqnetrr/window/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.492811 tmkit-0.0.0.1/tmkit/sequence/
--rw-rw-rw-   0        0        0      590 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/sequence/Fasta.py
--rw-rw-rw-   0        0        0      454 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/sequence/Index.py
--rw-rw-rw-   0        0        0     2052 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/sequence/PDB.py
--rw-rw-rw-   0        0        0     1685 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/sequence/XML.py
--rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.0.1/tmkit/sequence/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.498813 tmkit-0.0.0.1/tmkit/structure/
--rw-rw-rw-   0        0        0      578 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/structure/PDB.py
--rw-rw-rw-   0        0        0        0 2019-08-02 11:11:48.000000 tmkit-0.0.0.1/tmkit/structure/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.503811 tmkit-0.0.0.1/tmkit/structure/ppi/
--rw-rw-rw-   0        0        0     1451 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/structure/ppi/Label.py
--rw-rw-rw-   0        0        0        0 2019-09-15 17:30:37.000000 tmkit-0.0.0.1/tmkit/structure/ppi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.509814 tmkit-0.0.0.1/tmkit/structure/rrc/
--rw-rw-rw-   0        0        0     1811 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/structure/rrc/Label.py
--rw-rw-rw-   0        0        0        0 2019-09-15 17:30:31.000000 tmkit-0.0.0.1/tmkit/structure/rrc/__init__.py
--rw-rw-rw-   0        0        0     5542 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/topo.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.517811 tmkit-0.0.0.1/tmkit/topology/
--rw-rw-rw-   0        0        0     4387 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/topology/Phobius.py
--rw-rw-rw-   0        0        0     7728 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/topology/TMHMM.py
--rw-rw-rw-   0        0        0        0 2019-05-10 13:11:26.000000 tmkit-0.0.0.1/tmkit/topology/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.522811 tmkit-0.0.0.1/tmkit/topology/lib/
--rw-rw-rw-   0        0        0    25043 2022-07-15 23:01:47.000000 tmkit-0.0.0.1/tmkit/topology/lib/Phobius.py
--rw-rw-rw-   0        0        0        0 2022-07-16 23:17:45.000000 tmkit-0.0.0.1/tmkit/topology/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.538811 tmkit-0.0.0.1/tmkit/topology/pdbtm/
--rw-rw-rw-   0        0        0     4886 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/topology/pdbtm/Component.py
--rw-rw-rw-   0        0        0     3293 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/topology/pdbtm/Determine.py
--rw-rw-rw-   0        0        0     3737 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/topology/pdbtm/Segment.py
--rw-rw-rw-   0        0        0     1683 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/topology/pdbtm/TMH.py
--rw-rw-rw-   0        0        0     2224 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/topology/pdbtm/ToFastaId.py
--rw-rw-rw-   0        0        0        0 2019-11-07 10:51:46.000000 tmkit-0.0.0.1/tmkit/topology/pdbtm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.550811 tmkit-0.0.0.1/tmkit/util/
--rw-rw-rw-   0        0        0      890 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/util/Console.py
--rw-rw-rw-   0        0        0     4073 2023-06-19 11:34:17.000000 tmkit-0.0.0.1/tmkit/util/Kit.py
--rw-rw-rw-   0        0        0     2948 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/util/Reader.py
--rw-rw-rw-   0        0        0     1272 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/util/Writer.py
--rw-rw-rw-   0        0        0        0 2022-07-15 19:58:41.000000 tmkit-0.0.0.1/tmkit/util/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.552812 tmkit-0.0.0.1/tmkit/visualize/
--rw-rw-rw-   0        0        0        0 2022-08-07 22:43:33.000000 tmkit-0.0.0.1/tmkit/visualize/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.557811 tmkit-0.0.0.1/tmkit/visualize/func/
--rw-rw-rw-   0        0        0     2028 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/visualize/func/Coloring.py
--rw-rw-rw-   0        0        0        0 2022-08-11 11:29:35.000000 tmkit-0.0.0.1/tmkit/visualize/func/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.564814 tmkit-0.0.0.1/tmkit/visualize/isite/
--rw-rw-rw-   0        0        0     5480 2023-06-19 11:53:42.000000 tmkit-0.0.0.1/tmkit/visualize/isite/Labelling.py
--rw-rw-rw-   0        0        0     3958 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/visualize/isite/ProtocolDeepTMInter.py
--rw-rw-rw-   0        0        0        0 2020-12-31 08:21:51.000000 tmkit-0.0.0.1/tmkit/visualize/isite/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.584811 tmkit-0.0.0.1/tmkit/visualize/lib/
--rw-rw-rw-   0        0        0      394 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/visualize/lib/Color.py
--rw-rw-rw-   0        0        0     3872 2021-01-03 13:07:00.000000 tmkit-0.0.0.1/tmkit/visualize/lib/InterfaceResidues.py
--rw-rw-rw-   0        0        0      418 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/visualize/lib/Select.py
--rw-rw-rw-   0        0        0        0 2022-07-20 21:45:22.000000 tmkit-0.0.0.1/tmkit/visualize/lib/__init__.py
--rw-rw-rw-   0        0        0     2955 2022-07-21 00:23:12.000000 tmkit-0.0.0.1/tmkit/visualize/lib/focal_blur.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.591811 tmkit-0.0.0.1/tmkit/visualize/lib/palette/
--rw-rw-rw-   0        0        0        0 2022-08-11 11:29:11.000000 tmkit-0.0.0.1/tmkit/visualize/lib/palette/__init__.py
--rw-rw-rw-   0        0        0     8267 2021-02-09 21:44:23.000000 tmkit-0.0.0.1/tmkit/visualize/lib/palette/data2bfactor.py
--rw-rw-rw-   0        0        0     3582 2021-02-09 22:35:52.000000 tmkit-0.0.0.1/tmkit/visualize/lib/palette/spectrumany.py
--rw-rw-rw-   0        0        0    14191 2022-07-15 18:10:13.000000 tmkit-0.0.0.1/tmkit/visualize/lib/show_contacts.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.615811 tmkit-0.0.0.1/tmkit/visualize/small/
--rw-rw-rw-   0        0        0      697 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/visualize/small/Label.py
--rw-rw-rw-   0        0        0     2579 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/visualize/small/Local.py
--rw-rw-rw-   0        0        0      471 2023-06-19 10:50:53.000000 tmkit-0.0.0.1/tmkit/visualize/small/Palette.py
--rw-rw-rw-   0        0        0      678 2023-06-19 10:50:52.000000 tmkit-0.0.0.1/tmkit/visualize/small/Select.py
--rw-rw-rw-   0        0        0      217 2022-08-07 23:17:31.000000 tmkit-0.0.0.1/tmkit/visualize/small/Style.py
--rw-rw-rw-   0        0        0        0 2021-01-01 12:44:05.000000 tmkit-0.0.0.1/tmkit/visualize/small/__init__.py
--rw-rw-rw-   0        0        0     5489 2023-06-19 13:41:00.000000 tmkit-0.0.0.1/tmkit/vs.py
-drwxrwxrwx   0        0        0        0 2023-06-19 23:14:32.258811 tmkit-0.0.0.1/tmkit.egg-info/
--rw-rw-rw-   0        0        0      302 2023-06-19 23:14:32.000000 tmkit-0.0.0.1/tmkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3999 2023-06-19 23:14:32.000000 tmkit-0.0.0.1/tmkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 23:14:32.000000 tmkit-0.0.0.1/tmkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-06-19 23:14:32.000000 tmkit-0.0.0.1/tmkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-19 23:14:32.000000 tmkit-0.0.0.1/tmkit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.635598 tmkit-0.0.0.2/
+-rw-rw-rw-   0        0        0    35823 2022-10-06 19:26:08.000000 tmkit-0.0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-06-19 23:19:13.633599 tmkit-0.0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1506 2023-03-29 23:16:56.000000 tmkit-0.0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 23:19:13.636599 tmkit-0.0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      715 2023-06-19 23:18:35.000000 tmkit-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.258597 tmkit-0.0.0.2/tmkit/
+-rw-rw-rw-   0        0        0      458 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/Path.py
+-rw-rw-rw-   0        0        0     4375 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/SeqNetRR.py
+-rw-rw-rw-   0        0        0      261 2023-06-19 23:18:35.000000 tmkit-0.0.0.2/tmkit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.287598 tmkit-0.0.0.2/tmkit/base/
+-rw-rw-rw-   0        0        0     2936 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/base/PDB.py
+-rw-rw-rw-   0        0        0     1004 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/base/Position.py
+-rw-rw-rw-   0        0        0       76 2019-09-15 16:59:06.000000 tmkit-0.0.0.2/tmkit/base/__init__.py
+-rw-rw-rw-   0        0        0     2114 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/cath.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.302625 tmkit-0.0.0.2/tmkit/chain/
+-rw-rw-rw-   0        0        0     5301 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/chain/Collate.py
+-rw-rw-rw-   0        0        0     8052 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/chain/CollateBatch.py
+-rw-rw-rw-   0        0        0      599 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/chain/PDB.py
+-rw-rw-rw-   0        0        0        0 2022-08-06 11:29:10.000000 tmkit-0.0.0.2/tmkit/chain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.307627 tmkit-0.0.0.2/tmkit/channel/
+-rw-rw-rw-   0        0        0     7568 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/channel/Workbench.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 19:08:40.000000 tmkit-0.0.0.2/tmkit/channel/__init__.py
+-rw-rw-rw-   0        0        0     3047 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/collate.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.316600 tmkit-0.0.0.2/tmkit/contact/
+-rw-rw-rw-   0        0        0     7971 2023-06-19 13:33:30.000000 tmkit-0.0.0.2/tmkit/contact/Evaluator.py
+-rw-rw-rw-   0        0        0    24790 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/contact/Reader.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 18:38:08.000000 tmkit-0.0.0.2/tmkit/contact/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.324598 tmkit-0.0.0.2/tmkit/db/
+-rw-rw-rw-   0        0        0     7934 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/db/Connectivity.py
+-rw-rw-rw-   0        0        0     3676 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/db/Reader.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 13:10:28.000000 tmkit-0.0.0.2/tmkit/db/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.329597 tmkit-0.0.0.2/tmkit/db/biogrid/
+-rw-rw-rw-   0        0        0     1710 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/biogrid/Reader.py
+-rw-rw-rw-   0        0        0        0 2020-07-08 14:38:06.000000 tmkit-0.0.0.2/tmkit/db/biogrid/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.334596 tmkit-0.0.0.2/tmkit/db/cath/
+-rw-rw-rw-   0        0        0     5065 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/cath/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-11 11:28:12.000000 tmkit-0.0.0.2/tmkit/db/cath/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.339598 tmkit-0.0.0.2/tmkit/db/construct/
+-rw-rw-rw-   0        0        0     3320 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/construct/Network.py
+-rw-rw-rw-   0        0        0        0 2020-08-28 22:57:35.000000 tmkit-0.0.0.2/tmkit/db/construct/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.344596 tmkit-0.0.0.2/tmkit/db/intact/
+-rw-rw-rw-   0        0        0     2075 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/intact/Reader.py
+-rw-rw-rw-   0        0        0        0 2020-07-11 22:05:59.000000 tmkit-0.0.0.2/tmkit/db/intact/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.350596 tmkit-0.0.0.2/tmkit/db/muthtp/
+-rw-rw-rw-   0        0        0     3703 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/muthtp/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-07 05:11:20.000000 tmkit-0.0.0.2/tmkit/db/muthtp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.355597 tmkit-0.0.0.2/tmkit/db/predmuthtp/
+-rw-rw-rw-   0        0        0     2939 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/db/predmuthtp/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-08-07 05:11:42.000000 tmkit-0.0.0.2/tmkit/db/predmuthtp/__init__.py
+-rw-rw-rw-   0        0        0     1690 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/edge.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.361599 tmkit-0.0.0.2/tmkit/feature/
+-rw-rw-rw-   0        0        0     8018 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/feature/HelixSurface.py
+-rw-rw-rw-   0        0        0        0 2022-07-15 21:53:29.000000 tmkit-0.0.0.2/tmkit/feature/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.363597 tmkit-0.0.0.2/tmkit/feature/lips/
+-rw-rw-rw-   0        0        0        0 2019-08-01 10:52:35.000000 tmkit-0.0.0.2/tmkit/feature/lips/__init__.py
+-rw-rw-rw-   0        0        0     9415 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/feature.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.375596 tmkit-0.0.0.2/tmkit/id/
+-rw-rw-rw-   0        0        0      568 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/id/Fasta.py
+-rw-rw-rw-   0        0        0     2717 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/id/Mapping.py
+-rw-rw-rw-   0        0        0     1035 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/id/PDB.py
+-rw-rw-rw-   0        0        0        0 2020-04-26 23:07:36.000000 tmkit-0.0.0.2/tmkit/id/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.385598 tmkit-0.0.0.2/tmkit/interface/
+-rw-rw-rw-   0        0        0      387 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/interface/Tool.py
+-rw-rw-rw-   0        0        0      398 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/interface/Topology.py
+-rw-rw-rw-   0        0        0        0 2020-07-09 17:22:43.000000 tmkit-0.0.0.2/tmkit/interface/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/mapping.py
+-rw-rw-rw-   0        0        0     6409 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/msa.py
+-rw-rw-rw-   0        0        0     1928 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/mut.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.390596 tmkit-0.0.0.2/tmkit/name/
+-rw-rw-rw-   0        0        0     4437 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/name/Mapping.py
+-rw-rw-rw-   0        0        0        0 2022-08-06 12:13:25.000000 tmkit-0.0.0.2/tmkit/name/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-07-16 21:39:03.000000 tmkit-0.0.0.2/tmkit/pl.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.392596 tmkit-0.0.0.2/tmkit/position/
+-rw-rw-rw-   0        0        0       16 2019-09-15 17:43:20.000000 tmkit-0.0.0.2/tmkit/position/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.401596 tmkit-0.0.0.2/tmkit/position/scenario/
+-rw-rw-rw-   0        0        0     1724 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/position/scenario/Segment.py
+-rw-rw-rw-   0        0        0     2421 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/position/scenario/Separation.py
+-rw-rw-rw-   0        0        0        0 2019-09-21 21:40:26.000000 tmkit-0.0.0.2/tmkit/position/scenario/__init__.py
+-rw-rw-rw-   0        0        0     4938 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/ppi.py
+-rw-rw-rw-   0        0        0     2260 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/qc.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.412598 tmkit-0.0.0.2/tmkit/retrieve/
+-rw-rw-rw-   0        0        0    15864 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/retrieve/MSA.py
+-rw-rw-rw-   0        0        0     3976 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/retrieve/PDB.py
+-rw-rw-rw-   0        0        0     2142 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/retrieve/XML.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 15:10:49.000000 tmkit-0.0.0.2/tmkit/retrieve/__init__.py
+-rw-rw-rw-   0        0        0     5100 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/rrc.py
+-rw-rw-rw-   0        0        0     4126 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seq.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.427598 tmkit-0.0.0.2/tmkit/seqnetrr/
+-rw-rw-rw-   0        0        0     9679 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/Compare.py
+-rw-rw-rw-   0        0        0    13327 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/Controller.py
+-rw-rw-rw-   0        0        0      491 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/Path.py
+-rw-rw-rw-   0        0        0    34474 2022-10-06 14:12:35.000000 tmkit-0.0.0.2/tmkit/seqnetrr/Plot.py
+-rw-rw-rw-   0        0        0        0 2022-05-17 20:55:49.000000 tmkit-0.0.0.2/tmkit/seqnetrr/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.442597 tmkit-0.0.0.2/tmkit/seqnetrr/combo/
+-rw-rw-rw-   0        0        0     2183 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/Length.py
+-rw-rw-rw-   0        0        0      470 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/Param.py
+-rw-rw-rw-   0        0        0     1676 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/Position.py
+-rw-rw-rw-   0        0        0     2494 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/Separation.py
+-rw-rw-rw-   0        0        0        0 2019-08-11 16:35:38.000000 tmkit-0.0.0.2/tmkit/seqnetrr/combo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.452597 tmkit-0.0.0.2/tmkit/seqnetrr/graph/
+-rw-rw-rw-   0        0        0    19034 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/graph/Bipartite.py
+-rw-rw-rw-   0        0        0     4855 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/graph/Cumulative.py
+-rw-rw-rw-   0        0        0    21160 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/graph/Unipartite.py
+-rw-rw-rw-   0        0        0        0 2022-05-18 21:29:35.000000 tmkit-0.0.0.2/tmkit/seqnetrr/graph/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.458632 tmkit-0.0.0.2/tmkit/seqnetrr/net/
+-rw-rw-rw-   0        0        0    25261 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/net/Reader.py
+-rw-rw-rw-   0        0        0        0 2022-06-12 23:19:50.000000 tmkit-0.0.0.2/tmkit/seqnetrr/net/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.462630 tmkit-0.0.0.2/tmkit/seqnetrr/sequence/
+-rw-rw-rw-   0        0        0     1965 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/sequence/Fasta.py
+-rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.0.2/tmkit/seqnetrr/sequence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.476624 tmkit-0.0.0.2/tmkit/seqnetrr/util/
+-rw-rw-rw-   0        0        0     5609 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/ComputLib.py
+-rw-rw-rw-   0        0        0      838 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/Console.py
+-rw-rw-rw-   0        0        0     2866 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/Reader.py
+-rw-rw-rw-   0        0        0     2201 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/Writer.py
+-rw-rw-rw-   0        0        0        0 2022-05-18 16:43:31.000000 tmkit-0.0.0.2/tmkit/seqnetrr/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.484597 tmkit-0.0.0.2/tmkit/seqnetrr/window/
+-rw-rw-rw-   0        0        0     5855 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/Pair.py
+-rw-rw-rw-   0        0        0     5780 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/Single.py
+-rw-rw-rw-   0        0        0        0 2019-09-18 20:19:22.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.492598 tmkit-0.0.0.2/tmkit/seqnetrr/window/base/
+-rw-rw-rw-   0        0        0     1316 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/base/Pair.py
+-rw-rw-rw-   0        0        0     1318 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/base/Single.py
+-rw-rw-rw-   0        0        0        0 2019-09-19 13:22:58.000000 tmkit-0.0.0.2/tmkit/seqnetrr/window/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.508597 tmkit-0.0.0.2/tmkit/sequence/
+-rw-rw-rw-   0        0        0      590 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/sequence/Fasta.py
+-rw-rw-rw-   0        0        0      454 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/sequence/Index.py
+-rw-rw-rw-   0        0        0     2052 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/sequence/PDB.py
+-rw-rw-rw-   0        0        0     1685 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/sequence/XML.py
+-rw-rw-rw-   0        0        0        0 2019-08-02 11:12:19.000000 tmkit-0.0.0.2/tmkit/sequence/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.514597 tmkit-0.0.0.2/tmkit/structure/
+-rw-rw-rw-   0        0        0      578 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/structure/PDB.py
+-rw-rw-rw-   0        0        0        0 2019-08-02 11:11:48.000000 tmkit-0.0.0.2/tmkit/structure/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.521603 tmkit-0.0.0.2/tmkit/structure/ppi/
+-rw-rw-rw-   0        0        0     1451 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/structure/ppi/Label.py
+-rw-rw-rw-   0        0        0        0 2019-09-15 17:30:37.000000 tmkit-0.0.0.2/tmkit/structure/ppi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.526598 tmkit-0.0.0.2/tmkit/structure/rrc/
+-rw-rw-rw-   0        0        0     1811 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/structure/rrc/Label.py
+-rw-rw-rw-   0        0        0        0 2019-09-15 17:30:31.000000 tmkit-0.0.0.2/tmkit/structure/rrc/__init__.py
+-rw-rw-rw-   0        0        0     5542 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topo.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.533629 tmkit-0.0.0.2/tmkit/topology/
+-rw-rw-rw-   0        0        0     4387 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/Phobius.py
+-rw-rw-rw-   0        0        0     7728 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/TMHMM.py
+-rw-rw-rw-   0        0        0        0 2019-05-10 13:11:26.000000 tmkit-0.0.0.2/tmkit/topology/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.537612 tmkit-0.0.0.2/tmkit/topology/lib/
+-rw-rw-rw-   0        0        0    25043 2022-07-15 23:01:47.000000 tmkit-0.0.0.2/tmkit/topology/lib/Phobius.py
+-rw-rw-rw-   0        0        0        0 2022-07-16 23:17:45.000000 tmkit-0.0.0.2/tmkit/topology/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.553631 tmkit-0.0.0.2/tmkit/topology/pdbtm/
+-rw-rw-rw-   0        0        0     4886 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/Component.py
+-rw-rw-rw-   0        0        0     3293 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/Determine.py
+-rw-rw-rw-   0        0        0     3737 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/Segment.py
+-rw-rw-rw-   0        0        0     1683 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/TMH.py
+-rw-rw-rw-   0        0        0     2224 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/ToFastaId.py
+-rw-rw-rw-   0        0        0        0 2019-11-07 10:51:46.000000 tmkit-0.0.0.2/tmkit/topology/pdbtm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.565627 tmkit-0.0.0.2/tmkit/util/
+-rw-rw-rw-   0        0        0      890 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/util/Console.py
+-rw-rw-rw-   0        0        0     4073 2023-06-19 11:34:17.000000 tmkit-0.0.0.2/tmkit/util/Kit.py
+-rw-rw-rw-   0        0        0     2948 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/util/Reader.py
+-rw-rw-rw-   0        0        0     1272 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/util/Writer.py
+-rw-rw-rw-   0        0        0        0 2022-07-15 19:58:41.000000 tmkit-0.0.0.2/tmkit/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.567629 tmkit-0.0.0.2/tmkit/visualize/
+-rw-rw-rw-   0        0        0        0 2022-08-07 22:43:33.000000 tmkit-0.0.0.2/tmkit/visualize/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.572597 tmkit-0.0.0.2/tmkit/visualize/func/
+-rw-rw-rw-   0        0        0     2028 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/func/Coloring.py
+-rw-rw-rw-   0        0        0        0 2022-08-11 11:29:35.000000 tmkit-0.0.0.2/tmkit/visualize/func/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.581602 tmkit-0.0.0.2/tmkit/visualize/isite/
+-rw-rw-rw-   0        0        0     5480 2023-06-19 11:53:42.000000 tmkit-0.0.0.2/tmkit/visualize/isite/Labelling.py
+-rw-rw-rw-   0        0        0     3958 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/visualize/isite/ProtocolDeepTMInter.py
+-rw-rw-rw-   0        0        0        0 2020-12-31 08:21:51.000000 tmkit-0.0.0.2/tmkit/visualize/isite/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.600603 tmkit-0.0.0.2/tmkit/visualize/lib/
+-rw-rw-rw-   0        0        0      394 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/lib/Color.py
+-rw-rw-rw-   0        0        0     3872 2021-01-03 13:07:00.000000 tmkit-0.0.0.2/tmkit/visualize/lib/InterfaceResidues.py
+-rw-rw-rw-   0        0        0      418 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/lib/Select.py
+-rw-rw-rw-   0        0        0        0 2022-07-20 21:45:22.000000 tmkit-0.0.0.2/tmkit/visualize/lib/__init__.py
+-rw-rw-rw-   0        0        0     2955 2022-07-21 00:23:12.000000 tmkit-0.0.0.2/tmkit/visualize/lib/focal_blur.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.608598 tmkit-0.0.0.2/tmkit/visualize/lib/palette/
+-rw-rw-rw-   0        0        0        0 2022-08-11 11:29:11.000000 tmkit-0.0.0.2/tmkit/visualize/lib/palette/__init__.py
+-rw-rw-rw-   0        0        0     8267 2021-02-09 21:44:23.000000 tmkit-0.0.0.2/tmkit/visualize/lib/palette/data2bfactor.py
+-rw-rw-rw-   0        0        0     3582 2021-02-09 22:35:52.000000 tmkit-0.0.0.2/tmkit/visualize/lib/palette/spectrumany.py
+-rw-rw-rw-   0        0        0    14191 2022-07-15 18:10:13.000000 tmkit-0.0.0.2/tmkit/visualize/lib/show_contacts.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.631598 tmkit-0.0.0.2/tmkit/visualize/small/
+-rw-rw-rw-   0        0        0      697 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/visualize/small/Label.py
+-rw-rw-rw-   0        0        0     2579 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/small/Local.py
+-rw-rw-rw-   0        0        0      471 2023-06-19 10:50:53.000000 tmkit-0.0.0.2/tmkit/visualize/small/Palette.py
+-rw-rw-rw-   0        0        0      678 2023-06-19 10:50:52.000000 tmkit-0.0.0.2/tmkit/visualize/small/Select.py
+-rw-rw-rw-   0        0        0      217 2022-08-07 23:17:31.000000 tmkit-0.0.0.2/tmkit/visualize/small/Style.py
+-rw-rw-rw-   0        0        0        0 2021-01-01 12:44:05.000000 tmkit-0.0.0.2/tmkit/visualize/small/__init__.py
+-rw-rw-rw-   0        0        0     5489 2023-06-19 13:41:00.000000 tmkit-0.0.0.2/tmkit/vs.py
+drwxrwxrwx   0        0        0        0 2023-06-19 23:19:13.277627 tmkit-0.0.0.2/tmkit.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3999 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       89 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 23:19:13.000000 tmkit-0.0.0.2/tmkit.egg-info/top_level.txt
```

### Comparing `tmkit-0.0.0.1/LICENSE` & `tmkit-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/README.md` & `tmkit-0.0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/setup.py` & `tmkit-0.0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tmkit",
     # name="tmkitx",
-    version="0.0.0.1",
+    version="0.0.0.2",
     keywords=("pip", "tmkit"),
     description="TMKit",
     long_description="TMKit",
     license="GNU GENERAL V3.0",
 
     url="https://github.com/2003100127/tmkit",
     author="Jianfeng Sun",
```

### Comparing `tmkit-0.0.0.1/tmkit/SeqNetRR.py` & `tmkit-0.0.0.2/tmkit/SeqNetRR.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/base/PDB.py` & `tmkit-0.0.0.2/tmkit/base/PDB.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/base/Position.py` & `tmkit-0.0.0.2/tmkit/base/Position.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/cath.py` & `tmkit-0.0.0.2/tmkit/cath.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/chain/Collate.py` & `tmkit-0.0.0.2/tmkit/chain/Collate.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/chain/CollateBatch.py` & `tmkit-0.0.0.2/tmkit/chain/CollateBatch.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/chain/PDB.py` & `tmkit-0.0.0.2/tmkit/chain/PDB.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/channel/Workbench.py` & `tmkit-0.0.0.2/tmkit/channel/Workbench.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/collate.py` & `tmkit-0.0.0.2/tmkit/collate.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/contact/Evaluator.py` & `tmkit-0.0.0.2/tmkit/contact/Evaluator.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/contact/Reader.py` & `tmkit-0.0.0.2/tmkit/contact/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/db/Connectivity.py` & `tmkit-0.0.0.2/tmkit/db/Connectivity.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/db/Reader.py` & `tmkit-0.0.0.2/tmkit/db/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/db/biogrid/Reader.py` & `tmkit-0.0.0.2/tmkit/db/biogrid/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/db/cath/Reader.py` & `tmkit-0.0.0.2/tmkit/db/cath/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/db/construct/Network.py` & `tmkit-0.0.0.2/tmkit/db/construct/Network.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/db/intact/Reader.py` & `tmkit-0.0.0.2/tmkit/db/intact/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/db/muthtp/Reader.py` & `tmkit-0.0.0.2/tmkit/db/muthtp/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/db/predmuthtp/Reader.py` & `tmkit-0.0.0.2/tmkit/db/predmuthtp/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/edge.py` & `tmkit-0.0.0.2/tmkit/edge.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/feature/HelixSurface.py` & `tmkit-0.0.0.2/tmkit/feature/HelixSurface.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/feature.py` & `tmkit-0.0.0.2/tmkit/feature.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/id/Fasta.py` & `tmkit-0.0.0.2/tmkit/id/Fasta.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/id/Mapping.py` & `tmkit-0.0.0.2/tmkit/id/Mapping.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/id/PDB.py` & `tmkit-0.0.0.2/tmkit/id/PDB.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/mapping.py` & `tmkit-0.0.0.2/tmkit/mapping.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/msa.py` & `tmkit-0.0.0.2/tmkit/msa.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/mut.py` & `tmkit-0.0.0.2/tmkit/mut.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/name/Mapping.py` & `tmkit-0.0.0.2/tmkit/name/Mapping.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/position/scenario/Segment.py` & `tmkit-0.0.0.2/tmkit/position/scenario/Segment.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/position/scenario/Separation.py` & `tmkit-0.0.0.2/tmkit/position/scenario/Separation.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/ppi.py` & `tmkit-0.0.0.2/tmkit/ppi.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/qc.py` & `tmkit-0.0.0.2/tmkit/qc.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/retrieve/MSA.py` & `tmkit-0.0.0.2/tmkit/retrieve/MSA.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/retrieve/PDB.py` & `tmkit-0.0.0.2/tmkit/retrieve/PDB.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/retrieve/XML.py` & `tmkit-0.0.0.2/tmkit/retrieve/XML.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/rrc.py` & `tmkit-0.0.0.2/tmkit/rrc.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seq.py` & `tmkit-0.0.0.2/tmkit/seq.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/Compare.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/Compare.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/Controller.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/Controller.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/Plot.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/Plot.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/combo/Length.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/combo/Length.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/combo/Position.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/combo/Position.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/combo/Separation.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/combo/Separation.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/graph/Bipartite.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/graph/Bipartite.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/graph/Cumulative.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/graph/Cumulative.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/graph/Unipartite.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/graph/Unipartite.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/net/Reader.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/net/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/sequence/Fasta.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/util/ComputLib.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/util/ComputLib.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/util/Console.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/util/Console.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/util/Reader.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/util/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/util/Writer.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/util/Writer.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/window/Pair.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/window/Pair.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/window/Single.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/window/Single.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/window/base/Pair.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/window/base/Pair.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/seqnetrr/window/base/Single.py` & `tmkit-0.0.0.2/tmkit/seqnetrr/window/base/Single.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/sequence/Fasta.py` & `tmkit-0.0.0.2/tmkit/sequence/Fasta.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/sequence/PDB.py` & `tmkit-0.0.0.2/tmkit/sequence/PDB.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/sequence/XML.py` & `tmkit-0.0.0.2/tmkit/sequence/XML.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/structure/PDB.py` & `tmkit-0.0.0.2/tmkit/structure/PDB.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/structure/ppi/Label.py` & `tmkit-0.0.0.2/tmkit/structure/ppi/Label.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/structure/rrc/Label.py` & `tmkit-0.0.0.2/tmkit/structure/rrc/Label.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topo.py` & `tmkit-0.0.0.2/tmkit/topo.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topology/Phobius.py` & `tmkit-0.0.0.2/tmkit/topology/Phobius.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topology/TMHMM.py` & `tmkit-0.0.0.2/tmkit/topology/TMHMM.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topology/lib/Phobius.py` & `tmkit-0.0.0.2/tmkit/topology/lib/Phobius.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topology/pdbtm/Component.py` & `tmkit-0.0.0.2/tmkit/topology/pdbtm/Component.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topology/pdbtm/Determine.py` & `tmkit-0.0.0.2/tmkit/topology/pdbtm/Determine.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topology/pdbtm/Segment.py` & `tmkit-0.0.0.2/tmkit/topology/pdbtm/Segment.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topology/pdbtm/TMH.py` & `tmkit-0.0.0.2/tmkit/topology/pdbtm/TMH.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/topology/pdbtm/ToFastaId.py` & `tmkit-0.0.0.2/tmkit/topology/pdbtm/ToFastaId.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/util/Console.py` & `tmkit-0.0.0.2/tmkit/util/Console.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/util/Kit.py` & `tmkit-0.0.0.2/tmkit/util/Kit.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/util/Reader.py` & `tmkit-0.0.0.2/tmkit/util/Reader.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/util/Writer.py` & `tmkit-0.0.0.2/tmkit/util/Writer.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/func/Coloring.py` & `tmkit-0.0.0.2/tmkit/visualize/func/Coloring.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/isite/Labelling.py` & `tmkit-0.0.0.2/tmkit/visualize/isite/Labelling.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/isite/ProtocolDeepTMInter.py` & `tmkit-0.0.0.2/tmkit/visualize/isite/ProtocolDeepTMInter.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/lib/InterfaceResidues.py` & `tmkit-0.0.0.2/tmkit/visualize/lib/InterfaceResidues.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/lib/focal_blur.py` & `tmkit-0.0.0.2/tmkit/visualize/lib/focal_blur.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/lib/palette/data2bfactor.py` & `tmkit-0.0.0.2/tmkit/visualize/lib/palette/data2bfactor.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/lib/palette/spectrumany.py` & `tmkit-0.0.0.2/tmkit/visualize/lib/palette/spectrumany.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/lib/show_contacts.py` & `tmkit-0.0.0.2/tmkit/visualize/lib/show_contacts.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/small/Label.py` & `tmkit-0.0.0.2/tmkit/visualize/small/Label.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/small/Local.py` & `tmkit-0.0.0.2/tmkit/visualize/small/Local.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/visualize/small/Select.py` & `tmkit-0.0.0.2/tmkit/visualize/small/Select.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit/vs.py` & `tmkit-0.0.0.2/tmkit/vs.py`

 * *Files identical despite different names*

### Comparing `tmkit-0.0.0.1/tmkit.egg-info/SOURCES.txt` & `tmkit-0.0.0.2/tmkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

