# Comparing `tmp/q2_itsxpress-1.8.0.tar.gz` & `tmp/q2_itsxpress-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/q2_itsxpress-1.8.0.tar", last modified: Tue Dec 10 18:38:12 2019, max compression
+gzip compressed data, was "q2_itsxpress-1.8.1.tar", last modified: Tue Jun 20 14:50:11 2023, max compression
```

## Comparing `q2_itsxpress-1.8.0.tar` & `q2_itsxpress-1.8.1.tar`

### file list

```diff
@@ -1,138 +1,137 @@
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/
--rw-r--r--   0 rivers     (501) staff       (20)    15889 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/PKG-INFO
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/q2_itsxpress/
--rw-r--r--   0 rivers     (501) staff       (20)     9903 2019-12-10 18:29:46.000000 q2_itsxpress-1.8.0/q2_itsxpress/plugin_setup.py
--rw-r--r--   0 rivers     (501) staff       (20)       63 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/q2_itsxpress/__init__.py
--rw-r--r--   0 rivers     (501) staff       (20)      360 2018-09-19 17:12:15.000000 q2_itsxpress-1.8.0/q2_itsxpress/citations.bib
--rw-r--r--   0 rivers     (501) staff       (20)    10512 2019-07-31 15:06:09.000000 q2_itsxpress-1.8.0/q2_itsxpress/_itsxpress.py
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/
--rw-r--r--   0 rivers     (501) staff       (20)      130 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/metadata.yaml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/
--rw-r--r--   0 rivers     (501) staff       (20)      136 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/action/
--rw-r--r--   0 rivers     (501) staff       (20)     4176 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)      130 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/action/
--rw-r--r--   0 rivers     (501) staff       (20)     4621 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/VERSION
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/
--rw-r--r--   0 rivers     (501) staff       (20)       88 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/MANIFEST
--rw-r--r--   0 rivers     (501) staff       (20)    14241 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)       19 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/metadata.yml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/out/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/
--rw-r--r--   0 rivers     (501) staff       (20)      130 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/metadata.yaml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/action/
--rw-r--r--   0 rivers     (501) staff       (20)     3968 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)      130 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/action/
--rw-r--r--   0 rivers     (501) staff       (20)     4618 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/VERSION
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/
--rw-r--r--   0 rivers     (501) staff       (20)    29923 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)      147 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/MANIFEST
--rw-r--r--   0 rivers     (501) staff       (20)    21109 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)       19 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/metadata.yml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/metadata.yaml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/
--rw-r--r--   0 rivers     (501) staff       (20)     3968 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/VERSION
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/
--rw-r--r--   0 rivers     (501) staff       (20)    29923 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)      105 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/MANIFEST
--rw-r--r--   0 rivers     (501) staff       (20)    21109 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)       19 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/metadata.yml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/metadata.yaml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/
--rw-r--r--   0 rivers     (501) staff       (20)     4013 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/VERSION
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/
--rw-r--r--   0 rivers     (501) staff       (20)      147 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/MANIFEST
--rw-r--r--   0 rivers     (501) staff       (20)       19 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/metadata.yml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/
--rw-r--r--   0 rivers     (501) staff       (20)      130 2018-07-26 13:40:30.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/metadata.yaml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/
--rw-r--r--   0 rivers     (501) staff       (20)      136 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/action/
--rw-r--r--   0 rivers     (501) staff       (20)     4176 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/VERSION
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/
--rw-r--r--   0 rivers     (501) staff       (20)       88 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/MANIFEST
--rw-r--r--   0 rivers     (501) staff       (20)    54523 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)       19 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/metadata.yml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/metadata.yaml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/
--rw-r--r--   0 rivers     (501) staff       (20)     4013 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/VERSION
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/
--rw-r--r--   0 rivers     (501) staff       (20)       19 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/metadata.yml
--rw-r--r--   0 rivers     (501) staff       (20)    55572 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired.qza
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/paired/
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/metadata.yaml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/
--rw-r--r--   0 rivers     (501) staff       (20)      139 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/metadata.yaml
--rw-r--r--   0 rivers     (501) staff       (20)      856 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/citations.bib
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/
--rw-r--r--   0 rivers     (501) staff       (20)     3968 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/action.yaml
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/VERSION
--rw-r--r--   0 rivers     (501) staff       (20)       39 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/VERSION
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/
--rw-r--r--   0 rivers     (501) staff       (20)    29923 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)      147 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/MANIFEST
--rw-r--r--   0 rivers     (501) staff       (20)    21109 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
--rw-r--r--   0 rivers     (501) staff       (20)       19 2018-07-03 20:26:25.000000 q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/metadata.yml
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/tests/__pycache__/
--rw-r--r--   0 rivers     (501) staff       (20)     6872 2019-07-31 15:33:25.000000 q2_itsxpress-1.8.0/tests/__pycache__/test_main.cpython-36.pyc
--rw-r--r--   0 rivers     (501) staff       (20)     7474 2019-06-14 19:59:07.000000 q2_itsxpress-1.8.0/tests/__pycache__/test_main.cpython-35.pyc
--rw-r--r--   0 rivers     (501) staff       (20)     9802 2019-07-31 15:31:47.000000 q2_itsxpress-1.8.0/tests/test_main.py
-drwxr-xr-x   0 rivers     (501) staff       (20)        0 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/q2_itsxpress.egg-info/
--rw-r--r--   0 rivers     (501) staff       (20)    15889 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/q2_itsxpress.egg-info/PKG-INFO
--rw-r--r--   0 rivers     (501) staff       (20)        1 2018-07-06 19:38:21.000000 q2_itsxpress-1.8.0/q2_itsxpress.egg-info/not-zip-safe
--rw-r--r--   0 rivers     (501) staff       (20)     7129 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/q2_itsxpress.egg-info/SOURCES.txt
--rw-r--r--   0 rivers     (501) staff       (20)       66 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/q2_itsxpress.egg-info/entry_points.txt
--rw-r--r--   0 rivers     (501) staff       (20)       31 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/q2_itsxpress.egg-info/requires.txt
--rw-r--r--   0 rivers     (501) staff       (20)       13 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/q2_itsxpress.egg-info/top_level.txt
--rw-r--r--   0 rivers     (501) staff       (20)        1 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/q2_itsxpress.egg-info/dependency_links.txt
--rw-r--r--   0 rivers     (501) staff       (20)       61 2018-09-21 11:34:41.000000 q2_itsxpress-1.8.0/MANIFEST.in
--rw-r--r--   0 rivers     (501) staff       (20)     1078 2019-12-10 18:29:42.000000 q2_itsxpress-1.8.0/setup.py
--rw-r--r--   0 rivers     (501) staff       (20)       38 2019-12-10 18:38:12.000000 q2_itsxpress-1.8.0/setup.cfg
--rw-r--r--   0 rivers     (501) staff       (20)    13247 2019-12-10 18:22:02.000000 q2_itsxpress-1.8.0/README.rst
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.429465 q2_itsxpress-1.8.1/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     6909 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/LICENSE.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       61 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/MANIFEST.in
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    22796 2023-06-20 14:50:11.429465 q2_itsxpress-1.8.1/PKG-INFO
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    14366 2023-06-20 14:49:34.000000 q2_itsxpress-1.8.1/README.rst
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     1148 2023-06-03 01:42:26.000000 q2_itsxpress-1.8.1/pyproject.toml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/q2_itsxpress/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       63 2023-02-25 15:30:11.000000 q2_itsxpress-1.8.1/q2_itsxpress/__init__.py
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    10322 2023-05-26 18:43:23.000000 q2_itsxpress-1.8.1/q2_itsxpress/_itsxpress.py
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      360 2023-02-25 15:30:09.000000 q2_itsxpress-1.8.1/q2_itsxpress/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    10048 2023-02-25 15:30:08.000000 q2_itsxpress-1.8.1/q2_itsxpress/plugin_setup.py
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/q2_itsxpress.egg-info/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    22796 2023-06-20 14:50:11.000000 q2_itsxpress-1.8.1/q2_itsxpress.egg-info/PKG-INFO
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     7082 2023-06-20 14:50:11.000000 q2_itsxpress-1.8.1/q2_itsxpress.egg-info/SOURCES.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)        1 2023-06-20 14:50:11.000000 q2_itsxpress-1.8.1/q2_itsxpress.egg-info/dependency_links.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       65 2023-06-20 14:50:11.000000 q2_itsxpress-1.8.1/q2_itsxpress.egg-info/entry_points.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       47 2023-06-20 14:50:11.000000 q2_itsxpress-1.8.1/q2_itsxpress.egg-info/requires.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       13 2023-06-20 14:50:11.000000 q2_itsxpress-1.8.1/q2_itsxpress.egg-info/top_level.txt
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       38 2023-06-20 14:50:11.429465 q2_itsxpress-1.8.1/setup.cfg
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/__pycache__/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     6581 2023-05-26 18:44:29.000000 q2_itsxpress-1.8.1/tests/__pycache__/test_main.cpython-38-pytest-7.1.3.pyc
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/test_data/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/out/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    21109 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    29923 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      147 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/MANIFEST
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       19 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/metadata.yml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      130 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     4618 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/action/action.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.413465 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     3968 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/action/action.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/metadata.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      130 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/paired/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.417465 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.417465 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    21109 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    29923 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      147 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/MANIFEST
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       19 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/metadata.yml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.417465 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.417465 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     3968 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/action.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/metadata.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    55572 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/paired.qza
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.417465 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.417465 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    21109 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    29923 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      105 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/MANIFEST
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       19 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/metadata.yml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     3968 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/action.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       19 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/metadata.yml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     4013 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/action.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      147 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/MANIFEST
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       19 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/data/metadata.yml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.421465 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     4013 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/action.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      139 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/singleIn/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.425465 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.425465 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    54523 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       88 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/MANIFEST
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       19 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/metadata.yml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      130 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.425465 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.425465 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     4176 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/action/action.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      136 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/singleOut/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.425465 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.425465 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)    14241 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       88 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/MANIFEST
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       19 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/metadata.yml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      130 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/metadata.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.429465 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.429465 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     4621 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/action/action.yaml
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.409464 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.429465 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)       39 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/VERSION
+drwxrwxr-x   0 sveinn    (1000) sveinn    (1000)        0 2023-06-20 14:50:11.429465 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/action/
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     4176 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/action/action.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      136 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/metadata.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      856 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/citations.bib
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)      130 2023-01-04 19:17:50.000000 q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/metadata.yaml
+-rw-rw-r--   0 sveinn    (1000) sveinn    (1000)     9806 2023-05-26 18:44:19.000000 q2_itsxpress-1.8.1/tests/test_main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `q2_itsxpress-1.8.0/PKG-INFO` & `q2_itsxpress-1.8.1/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,265 +1,275 @@
-Metadata-Version: 1.2
-Name: q2_itsxpress
-Version: 1.8.0
-Summary: A QIIME2 plugin to trim ITS regions using ITSxpress
-Home-page: https://github.com/usda-ars-gbru/q2_itsxpress
-Author: Adam R. Rivers, Kyle C. Weber
-Author-email: adam.rivers@ars.usda.gov, kweber1@ufl.edu
-License: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Description: Q2_ITSxpress: A Qiime2 plugin to rapidly trim the Internally transcribed spacer (ITS) region of FASTQ files
-        ===========================================================================================================
-        .. image:: https://travis-ci.org/USDA-ARS-GBRU/q2_itsxpress.svg?branch=master
-          :target: https://travis-ci.org/USDA-ARS-GBRU/q2_itsxpress
-        
-        .. image:: https://codecov.io/gh/USDA-ARS-GBRU/q2_itsxpress/branch/master/graph/badge.svg
-          :target: https://codecov.io/gh/USDA-ARS-GBRU/q2_itsxpress
-        
-        .. image:: https://api.codacy.com/project/badge/Grade/4d00341b4abc4e04a77cf5ca6674cd3c
-          :target: https://www.codacy.com/app/USDA-ARS-GBRU/q2_itsxpress?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=USDA-ARS-GBRU/q2_itsxpress&amp;utm_campaign=Badge_Grade
-        
-        .. image:: https://zenodo.org/badge/138209572.svg
-           :target: https://zenodo.org/badge/latestdoi/138209572
-        
-        
-        Authors
-        -------
-        * Adam R. Rivers, US Department of Agriculture, Agricultural Research Service
-        * Kyle C. Weber, US Department of Agriculture, Agricultural Research Service
-        
-        Citation
-        --------
-        Rivers AR, Weber KC, Gardner TG et al. ITSxpress: Software to rapidly trim
-        internally transcribed spacer sequences with quality scores for marker gene
-        analysis. F1000Research 2018, 7:1418. doi: `10.12688/f1000research.15704.1`_
-        
-        .. _`10.12688/f1000research.15704.1`: https://doi.org/10.12688/f1000research.15704.1
-        
-        Introduction
-        ------------
-        
-        The internally transcribed spacer (ITS) is a region between the small subunit
-        and large subunit rRNA genes. In is a commonly used phylogenetic marker for
-        Fungi and other Eukaryotes. The ITS contains the 5.8s gene and two variable
-        length spacer regions. In amplicon sequencing studies it is common practice to
-        trim off the conserved (SSU, 5,8S or LSU) regions. Bengtsson-Palme et al. (2013)
-        published a software package ITSx_ to do this.
-        
-        Q2_ITSxpress extends this work by rapidly trimming FASTQ sequences within
-        Qiime2.  Q2_ITSxpress is the Qiime2 plugin version of the stand alone command
-        line utility ITSxpress_. Q2_ITSxpress is designed to support the calling of
-        exact sequence variants rather than OTUs. This newer method of sequence
-        error-correction requires quality score data from each sequence, so each input
-        sequence must be trimmed. ITSxpress makes this possible by taking FASTQ data,
-        de-replicating the sequences then identifying the start and stop sites using
-        HMMSearch. Results are parsed and the trimmed files are returned. The ITS1,
-        ITS2 or the entire ITS region including the 5.8s rRNA gene can be selected.
-        ITSxpress uses the hmm models from ITSx so results are nearly identical.
-        
-        
-        Requirements/Dependencies
-        -------------------------
-        
-        * Qiime2 is required to run Q2-itsxpress (for stand alone software see ITSxpress_)
-        * To install Qiime2 follow these instructions: https://docs.qiime2.org/2019.10/install/
-        
-        Q2_itsxpress Installation
-        -------------------------
-        
-        1. Activate the Qiime2 conda environment
-        
-        .. code-block:: bash
-        
-          source activate qiime2-2019.10
-        
-        2. Install Q2_itsxpress using BioConda_. Be sure to install Q2_itsxpres in the Qiime2 environment.
-        
-        .. code-block:: bash
-        
-          conda install -c bioconda itsxpress
-          pip install q2-itsxpress
-        
-        3. In your Qiime2 environment, refresh the plugins.
-        
-        .. code-block:: bash
-        
-          qiime dev refresh-cache
-        
-        4. Check to see if the ITSxpress plugin is installed. You should see an output similar to the image below.
-        
-        .. code-block:: bash
-        
-          qiime itsxpress
-        
-        .. image:: ../../screenshot.png
-        
-        Usage
-        -----
-        
-        Within Qiime2 you can trim paired-end or single-end reads using these commands
-        
-        .. code-block:: bash
-        
-          qiime itsxpress trim-pair
-        
-          qiime itsxpress trim-pair-output-unmerged
-        
-          qiime itsxpress trim-single
-        
-        1. qiime itsxpress trim-single
-        
-          This command takes single-end data and returns trimmed reads. The sequence may
-          have been merged previously or have been generated from a long read technology
-          like PacBio. Merged and long reads trimmed by this function can be used by
-          Deblur but only long reads (not merged reads) trimmed by this function should
-          be passed to Dada2. Its statistical model for estimating error rates was not
-          designed for pre-merged reads.
-        
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |    Command-requirement           | Description                                                                           |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |   --i-per-sample-sequences       | - The artifact that contains the sequence file(s).                                    |
-        + 			           + - Either Joined Paired or just a single fastq.                                        +
-        |                                  | - One file sequence in the qza data folder.                                           |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --p-region                 | - The regions ITS2, ITS1, and ALL.                                                    |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |				   | -	Select the taxonomic group sequenced: A, B, C, D, E, F, G, H, I, L, M, O, P,	   |
-        +	--p-taxa		   +	Q, R, S, T, U, V, ALL.								   +
-        | 				   |											   |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --p-threads 	           | - The amount of threads to use.                                                       |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --o-trimmed                | - The resulting trimmed sequences from ITSxpress in a qza format.                     |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |      --cluster-id                | - The percent identity for clustering reads, set to 1 for exact dereplication.        |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        
-        
-        2. qiime itsxpress trim-pair
-        
-          This command takes paired-end data and returns merged, trimmed reads. The
-          merged reads trimmed by this function can be used by Deblur but not
-          Dada2. Its statistical model for estimating error rates was not
-          designed for pre-merged reads, instead use `qiime itsxpress trim-pair-output-unmerged`.
-        
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |    Command-requirement           | Description                                                                           |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |   --i-per-sample-sequences       | - The artifact that contains the sequence file(s).                                    |
-        + 			           + - Either Joined Paired or just a single fastq.                                        +
-        |                                  | - One file sequence in the qza data folder.                                           |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --p-region                 | - The regions ITS2, ITS1, and ALL.                                                    |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |				   | -	Select the taxonomic group sequenced: A, B, C, D, E, F, G, H, I, L, M, O, P,	   |
-        +	--p-taxa		   +	Q, R, S, T, U, V, ALL.								   +
-        | 				   |											   |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --p-threads 	           | - The amount of threads to use.                                                       |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --o-trimmed                | - The resulting trimmed sequences from ITSxpress in a qza format.                     |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |      --cluster-id                | - The percent identity for clustering reads, set to 1 for exact dereplication.        |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        
-        3. qiime itsxpress trim-pair-output-unmerged
-        
-          This command takes paired-end data and returns unmerged, trimmed reads. The
-          merged reads trimmed by this function can be used by Dada2 but not Deblur.
-          For Deblur use `qiime itsxpress trim-pair`.
-        
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |    Command-requirement           | Description                                                                           |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |   --i-per-sample-sequences       | - The artifact that contains the sequence file.                                       |
-        + 			           + - Only paired will work.                                                              +
-        |                                  | - Two file sequences in the qza data folder.                                          |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --p-region                 | - The regions ITS2, ITS1, and ALL.                                                    |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |				   | -	Select the taxonomic group sequenced: A, B, C, D, E, F, G, H, I, L, M, O, P,	   |
-        +	--p-taxa		   +	Q, R, S, T, U, V, ALL.								   +
-        | 				   |											   |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --p-threads 	           | - The amount of threads to use.                                                       |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |       --o-trimmed                | - The resulting trimmed sequences from ITSxpress in a qza format.                     |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        |      --cluster-id                | - The percent identity for clustering reads, set to 1 for exact dereplication.        |
-        +----------------------------------+---------------------------------------------------------------------------------------+
-        
-        Taxa Key
-        --------
-        
-        +-+-------------------------------------+
-        |A| Alveolata				|
-        +-+-------------------------------------+
-        |B| Bryophyta				|
-        +-+-------------------------------------+
-        |C| Bacillariophyta			|
-        +-+-------------------------------------+
-        |D| Amoebozoa				|
-        +-+-------------------------------------+
-        |E| Euglenozoa				|
-        +-+-------------------------------------+
-        |F| Fungi				|
-        +-+-------------------------------------+
-        |G| Chlorophyta (green algae)		|
-        +-+-------------------------------------+
-        |H| Rhodophyta (red algae)		|
-        +-+-------------------------------------+
-        |I| Phaeophyceae (brown algae)		|
-        +-+-------------------------------------+
-        |L| Marchantiophyta (liverworts)	|
-        +-+-------------------------------------+
-        |M| Metazoa				|
-        +-+-------------------------------------+
-        |O| Oomycota				|
-        +-+-------------------------------------+
-        |P| Haptophyceae (prymnesiophytes)	|
-        +-+-------------------------------------+
-        |Q| Raphidophyceae			|
-        +-+-------------------------------------+
-        |R| Rhizaria				|
-        +-+-------------------------------------+
-        |S| Synurophyceae			|
-        +-+-------------------------------------+
-        |T| Tracheophyta (higher plants)	|
-        +-+-------------------------------------+
-        |U| Eustigmatophyceae			|
-        +-+-+-----------------------------------+
-        |ALL| All				|
-        +---+-----------------------------------+
-        
-        
-        
-        Example
-        -------
-        
-        Use case: Trimming the ITS2 region from a fungal amplicon
-        sequencing dataset with a PairedSequencesWithQuailty qza using two cpu threads.
-        The example file used is in the Tests folder under paired.qza.
-        
-        .. code:: bash
-        
-          qiime itsxpress trim-pair --i-per-sample-sequences ~/parired.qza --p-region ITS2 \
-          --p-taxa F --p-threads 2 --o-trimmed ~/Desktop/out.qza
-        
-        License information
-        -------------------
-        
-        This software is a work of the United States Department of Agriculture,
-        Agricultural Research Service and is released under a Creative Commons CC0
-        public domain attribution.
-        
-        .. _ITSxpress: https://github.com/USDA-ARS-GBRU/itsxpress
-        .. _ITSx: http://microbiology.se/software/itsx/
-        .. _BioConda: https://bioconda.github.io/
-        
-Keywords: Amplicon sequencing fungal ITS QIIME2
-Platform: UNKNOWN
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Development Status :: 3 - Alpha
-Requires-Python: >3.5
+Q2_ITSxpress: A Qiime2 plugin to rapidly trim the Internally transcribed spacer (ITS) region of FASTQ files
+===========================================================================================================
+
+.. image:: https://github.com/USDA-ARS-GBRU/q2_itsxpress/actions/workflows/python-package.yml/badge.svg
+   :target: https://github.com/USDA-ARS-GBRU/q2_itsxpress/actions/workflows/python-package.yml
+   :alt: Build Status
+   
+.. image:: https://img.shields.io/github/v/release/USDA-ARS-GBRU/q2_itsxpress?style=social
+   :target: https://github.com/USDA-ARS-GBRU/q2_itsxpress/releases/latest
+   :alt: GitHub release (latest by date)
+   
+.. image:: https://zenodo.org/badge/138209572.svg
+   :target: https://zenodo.org/badge/latestdoi/138209572
+
+
+
+#####
+
+This is the end of life version 1 of q2_itsxpress and the command line version of ITSxpress. See 
+1.8.1-EOL branch of ITSxpress. The new version 2 of ITSxpress, has the Qiime2 plugin built in with command line version of ITSxpress.
+
+#####
+
+See ITSxpress 1.8.1-EOL branch here: ITSxpress-1.8.1-EOL_
+
+.. _`ITSxpress-1.8.1-EOL`: https://github.com/USDA-ARS-GBRU/itsxpress/tree/1.8.1-EOL
+
+
+Authors
+-------
+* Adam R. Rivers, US Department of Agriculture, Agricultural Research Service
+* Kyle C. Weber, US Department of Agriculture, Agricultural Research Service
+* Sveinn V. Einarsson, US Department of Agriculture, Agricultural Research Service
+
+Citation
+--------
+Rivers AR, Weber KC, Gardner TG et al. ITSxpress: Software to rapidly trim
+internally transcribed spacer sequences with quality scores for marker gene
+analysis. F1000Research 2018, 7:1418. doi: `10.12688/f1000research.15704.1`_
+
+.. _`10.12688/f1000research.15704.1`: https://doi.org/10.12688/f1000research.15704.1
+
+Introduction
+------------
+
+The internally transcribed spacer (ITS) is a region between the small subunit
+and large subunit rRNA genes. In is a commonly used phylogenetic marker for
+Fungi and other Eukaryotes. The ITS contains the 5.8s gene and two variable
+length spacer regions. In amplicon sequencing studies it is common practice to
+trim off the conserved (SSU, 5,8S or LSU) regions. Bengtsson-Palme et al. (2013)
+published a software package ITSx_ to do this.
+
+Q2-ITSxpress extends this work by rapidly trimming FASTQ sequences within
+Qiime2.  Q2-ITSxpress is the Qiime2 plugin version of the stand alone command
+line utility ITSxpress_. Q2_ITSxpress is designed to support the calling of
+exact sequence variants rather than OTUs. This newer method of sequence
+error-correction requires quality score data from each sequence, so each input
+sequence must be trimmed. ITSxpress makes this possible by taking FASTQ data,
+de-replicating the sequences then identifying the start and stop sites using
+HMMSearch. Results are parsed and the trimmed files are returned. The ITS1,
+ITS2 or the entire ITS region including the 5.8s rRNA gene can be selected.
+ITSxpress uses the hmm models from ITSx so results are nearly identical.
+
+
+Requirements/Dependencies
+-------------------------
+
+* Qiime2 is required to run Q2-itsxpress (for stand alone software see ITSxpress_)
+* To install Qiime2 follow these instructions: https://docs.qiime2.org/2022.8/install/
+* This end of life version 1 of q2-itsxpress and ITSxpress is **ONLY** compatible with Qiime2 version 2022.8. So make sure to follow the link above.
+
+* We are using mamba because it resolves packages better and faster, but conda can be substituted.
+	- Information on installing mamba or micromamba (either highly recommended) can be found here: `mamba installation guide`_
+
+.. _`mamba installation guide`: https://mamba.readthedocs.io/en/latest/installation.html
+
+Q2-itsxpress plugin installation
+--------------------------------
+1. Example on how to install and create new Qiime2-2022.8 environment.
+
+.. code-block:: bash
+
+  wget https://data.qiime2.org/distro/core/qiime2-2022.8-py38-osx-conda.yml
+  mamba env create -n qiime2-2022.8 --file qiime2-2022.8-py38-osx-conda.yml
+
+2. Activate the Qiime2 conda environment
+
+.. code-block:: bash
+
+  mamba activate qiime2-2022.8
+
+3. Install Q2_itsxpress using BioConda_. Be sure to install itsxpress and q2_itsxpress in the Qiime2 environment using the following commands.
+
+.. code-block:: bash
+
+  mamba install -c bioconda itsxpress==1.8.1
+  pip install q2-itsxpress
+
+4. In your Qiime2 environment, refresh the plugins.
+
+.. code-block:: bash
+
+  qiime dev refresh-cache
+
+5. Check to see if the ITSxpress plugin is installed. You should see an output similar to the image below.
+
+.. code-block:: bash
+
+  qiime itsxpress
+
+.. image:: ./screenshot.png
+
+Usage
+-----
+
+Within Qiime2 you can trim paired-end or single-end reads using these commands
+
+.. code-block:: bash
+
+  qiime itsxpress trim-pair
+
+  qiime itsxpress trim-pair-output-unmerged
+
+  qiime itsxpress trim-single
+
+1. qiime itsxpress trim-single
+
+  This command takes single-end data and returns trimmed reads. The sequence may
+  have been merged previously or have been generated from a long read technology
+  like PacBio. Merged and long reads trimmed by this function can be used by
+  Deblur but only long reads (not merged reads) trimmed by this function should
+  be passed to Dada2. Its statistical model for estimating error rates was not
+  designed for pre-merged reads.
+
++----------------------------------+---------------------------------------------------------------------------------------+
+|    Command-requirement           | Description                                                                           |
++----------------------------------+---------------------------------------------------------------------------------------+
+|   --i-per-sample-sequences       | - The artifact that contains the sequence file(s).                                    |
++ 			           + - Either Joined Paired or just a single fastq.                                        +
+|                                  | - One file sequence in the qza data folder.                                           |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --p-region                 | - The regions ITS2, ITS1, and ALL.                                                    |
++----------------------------------+---------------------------------------------------------------------------------------+
+|				   | -	Select the taxonomic group sequenced: A, B, C, D, E, F, G, H, I, L, M, O, P,	   |
++	--p-taxa		   +	Q, R, S, T, U, V, ALL.								   +
+| 				   |											   |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --p-threads 	           | - The amount of threads to use.                                                       |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --o-trimmed                | - The resulting trimmed sequences from ITSxpress in a qza format.                     |
++----------------------------------+---------------------------------------------------------------------------------------+
+|      --cluster-id                | - The percent identity for clustering reads, set to 1 for exact dereplication.        |
++----------------------------------+---------------------------------------------------------------------------------------+
+
+
+2. qiime itsxpress trim-pair
+
+  This command takes paired-end data and returns merged, trimmed reads. The
+  merged reads trimmed by this function can be used by Deblur but not
+  Dada2. Its statistical model for estimating error rates was not
+  designed for pre-merged reads, instead use `qiime itsxpress trim-pair-output-unmerged`.
+
++----------------------------------+---------------------------------------------------------------------------------------+
+|    Command-requirement           | Description                                                                           |
++----------------------------------+---------------------------------------------------------------------------------------+
+|   --i-per-sample-sequences       | - The artifact that contains the sequence file(s).                                    |
++ 			           + - Either Joined Paired or just a single fastq.                                        +
+|                                  | - One file sequence in the qza data folder.                                           |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --p-region                 | - The regions ITS2, ITS1, and ALL.                                                    |
++----------------------------------+---------------------------------------------------------------------------------------+
+|				   | -	Select the taxonomic group sequenced: A, B, C, D, E, F, G, H, I, L, M, O, P,	   |
++	--p-taxa		   +	Q, R, S, T, U, V, ALL.								   +
+| 				   |											   |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --p-threads 	           | - The amount of threads to use.                                                       |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --o-trimmed                | - The resulting trimmed sequences from ITSxpress in a qza format.                     |
++----------------------------------+---------------------------------------------------------------------------------------+
+|      --cluster-id                | - The percent identity for clustering reads, set to 1 for exact dereplication.        |
++----------------------------------+---------------------------------------------------------------------------------------+
+
+3. qiime itsxpress trim-pair-output-unmerged
+
+  This command takes paired-end data and returns unmerged, trimmed reads. The
+  merged reads trimmed by this function can be used by Dada2 but not Deblur.
+  For Deblur use `qiime itsxpress trim-pair`.
+
++----------------------------------+---------------------------------------------------------------------------------------+
+|    Command-requirement           | Description                                                                           |
++----------------------------------+---------------------------------------------------------------------------------------+
+|   --i-per-sample-sequences       | - The artifact that contains the sequence file.                                       |
++ 			           + - Only paired will work.                                                              +
+|                                  | - Two file sequences in the qza data folder.                                          |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --p-region                 | - The regions ITS2, ITS1, and ALL.                                                    |
++----------------------------------+---------------------------------------------------------------------------------------+
+|				   | -	Select the taxonomic group sequenced: A, B, C, D, E, F, G, H, I, L, M, O, P,	   |
++	--p-taxa		   +	Q, R, S, T, U, V, ALL.								   +
+| 				   |											   |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --p-threads 	           | - The amount of threads to use.                                                       |
++----------------------------------+---------------------------------------------------------------------------------------+
+|       --o-trimmed                | - The resulting trimmed sequences from ITSxpress in a qza format.                     |
++----------------------------------+---------------------------------------------------------------------------------------+
+|      --cluster-id                | - The percent identity for clustering reads, set to 1 for exact dereplication.        |
++----------------------------------+---------------------------------------------------------------------------------------+
+
+Taxa Key
+--------
+
++-+-------------------------------------+
+|A| Alveolata				|
++-+-------------------------------------+
+|B| Bryophyta				|
++-+-------------------------------------+
+|C| Bacillariophyta			|
++-+-------------------------------------+
+|D| Amoebozoa				|
++-+-------------------------------------+
+|E| Euglenozoa				|
++-+-------------------------------------+
+|F| Fungi				|
++-+-------------------------------------+
+|G| Chlorophyta (green algae)		|
++-+-------------------------------------+
+|H| Rhodophyta (red algae)		|
++-+-------------------------------------+
+|I| Phaeophyceae (brown algae)		|
++-+-------------------------------------+
+|L| Marchantiophyta (liverworts)	|
++-+-------------------------------------+
+|M| Metazoa				|
++-+-------------------------------------+
+|O| Oomycota				|
++-+-------------------------------------+
+|P| Haptophyceae (prymnesiophytes)	|
++-+-------------------------------------+
+|Q| Raphidophyceae			|
++-+-------------------------------------+
+|R| Rhizaria				|
++-+-------------------------------------+
+|S| Synurophyceae			|
++-+-------------------------------------+
+|T| Tracheophyta (higher plants)	|
++-+-------------------------------------+
+|U| Eustigmatophyceae			|
++-+-+-----------------------------------+
+|ALL| All				|
++---+-----------------------------------+
+
+
+
+Example
+-------
+
+Use case: Trimming the ITS2 region from a fungal amplicon
+sequencing dataset with a PairedSequencesWithQuailty qza using two cpu threads.
+The example file used is in the Tests folder under paired.qza.
+
+.. code:: bash
+
+  qiime itsxpress trim-pair --i-per-sample-sequences ~/parired.qza --p-region ITS2 \
+  --p-taxa F --p-threads 2 --o-trimmed ~/Desktop/out.qza
+
+License information
+-------------------
+
+This software is a work of the United States Department of Agriculture,
+Agricultural Research Service and is released under a Creative Commons CC0
+public domain attribution.
+
+.. _ITSxpress: https://github.com/USDA-ARS-GBRU/itsxpress
+.. _ITSx: http://microbiology.se/software/itsx/
+.. _BioConda: https://bioconda.github.io/
```

### Comparing `q2_itsxpress-1.8.0/q2_itsxpress/plugin_setup.py` & `q2_itsxpress-1.8.1/q2_itsxpress/plugin_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,22 @@
 
 from q2_itsxpress._itsxpress import (trim_single,
                                      trim_pair,
                                      trim_pair_output_unmerged,
                                      default_cluster_id)
 
 plugin = Plugin(
-    name='itsxpress',
-    version='1.8.0',
+    name='q2_itsxpress',
+    version='1.8.1',
     package='q2_itsxpress',
     website='https://github.com/USDA-ARS-GBRU/q2_itsxpress             '
             'ITSxpress: https://github.com/USDA-ARS-GBRU/itsxpress',
-    description='ITSxpress trims amplicon reads down to their ITS region. '
+    description='#####This is the end of life version 1 of ITSxpress. Please check Github for version 2'
+                'of ITSxpress.#####'
+                'ITSxpress trims amplicon reads down to their ITS region. '
                 'ITSxpress is designed to support the calling of exact sequence variants '
                 'rather than OTUs. This newer method of sequence error-correction requires '
                 'quality score data from each sequence, so each input sequence must be trimmed. '
                 'ITSxpress makes this possible by taking FASTQ data, de-replicating the '
                 'sequences then identifying the start and stop sites using HMMSearch. '
                 'Results are parsed and the trimmed files are returned. '
                 'The ITS 1, ITS2 or the entire ITS region including the 5.8s rRNA'
```

### Comparing `q2_itsxpress-1.8.0/q2_itsxpress/_itsxpress.py` & `q2_itsxpress-1.8.1/q2_itsxpress/_itsxpress.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python
 """A python module to integrate ITSxpress into QIIME for the trimming of amplicon sequences.
 
-Authors: Adam Rivers and Kyle Weber, USDA Agricultural Research Service
+Authors: Adam Rivers, Kyle Weber, Sveinn V. Einarsson USDA Agricultural Research Service
+
+#####This is the end of life version 1 of the qiime2 plugin for ITSxpress. Please check Github page below to access version 2 of ITSxpress#####
 
 The internally transcribed spacer region is a region between the highly conserved small
 subunit (SSU) of rRNA and the large subunit (LSU) of the rRNA. The eukaryotic ITS contains
 the 5.8s gene and two variable length spacer regions. In amplicon sequencing studies it is
 common practice to trim off the conserved (SSU, 5,8S or LSU) regions. Bengtsson-Palme
 et al. (2013) published software the software package ITSx to do this.
 
@@ -36,15 +38,15 @@
 
 def _set_fastqs_and_check(fastq: str,
                           fastq2: str,
                           sample_id: str,
                           single_end: bool,
                           reversed_primers: bool,
                           threads: int) -> object:
-    """Checks and writes the fastqs as well as if they are paired end, interleaved and single end.
+    """Checks and writes the fastqs as well as if they are paired end and single end.
 
         Args:
             fastq (str): The path to the forward reads file.
             fastq2 (str): The path to the reverse reads file.
             sample_id (str): The Sample ID.
             single_end (bool): If the sequences are singled ended or not
             threads (int): The amount of threads to use
@@ -64,30 +66,25 @@
                                                        fastq2=fastq2,
                                                        single_end=single_end)
     except (NotADirectoryError,
             FileNotFoundError):
 
         raise ValueError("There is a problem with the fastq file(s) you selected")
         # Create SeqSample objects and merge if needed.
-    if paired_end and interleaved:
-        sobj = itsxpress.SeqSamplePairedInterleaved(fastq=fastq,
-                                                    tempdir=None,
-                                                    reversed_primers=reversed_primers)
-        sobj._merge_reads(threads=threads)
-        return sobj
 
-    elif paired_end and not interleaved:
+
+    if paired_end:
         sobj = itsxpress.SeqSamplePairedNotInterleaved(fastq=fastq,
                                                        fastq2=fastq2,
                                                        tempdir=None,
                                                        reversed_primers=reversed_primers)
         sobj._merge_reads(threads=threads)
         return sobj
 
-    elif not paired_end and not interleaved:
+    elif not paired_end:
         sobj = itsxpress.SeqSampleNotPaired(fastq=fastq,
                                             tempdir=None)
         return sobj
 
 
 def _taxa_prefix_to_taxa(taxa_prefix: str) -> str:
     """Turns the taxa prefix letter into the taxa
@@ -194,15 +191,15 @@
     # Running the for loop for each sample
     for sample in samples.itertuples():
         # writing fastqs and their attributes and checking the files
         sobj = _set_fastqs_and_check(
             fastq=sample.forward,
             fastq2=sample.reverse if paired_in else None,
             sample_id=sample.Index,
-            single_end=paired_out,
+            single_end=False if paired_in else True,
             reversed_primers=reversed_primers,
             threads=threads)
         # Deduplicate
         if math.isclose(cluster_id, 1,rel_tol=1e-05):
             sobj.deduplicate(threads=threads)
         else:
             sobj.cluster(threads=threads, cluster_id=cluster_id)
```

### Comparing `q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz` & `q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/artifacts/445cf54a-bf06-4852-8010-13a60fa1598c/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/provenance/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz` & `q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz` & `q2_itsxpress-1.8.1/tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz` & `q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz` & `q2_itsxpress-1.8.1/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/provenance/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/artifacts/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz` & `q2_itsxpress-1.8.1/tests/test_data/singleIn/cfd0e65b-05fb-4329-9618-15ecd0aec9b3/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/singleOut/75aea4f5-f10e-421e-91d2-feda9fe7b2e1/provenance/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/pairedBrokenMissingData/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/pairedBrokenWithMANIFEST/50d5f31a-a761-4c04-990c-e7668fe6bf00/provenance/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/paired.qza` & `q2_itsxpress-1.8.1/tests/test_data/paired.qza`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/citations.bib` & `q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/citations.bib`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/action.yaml` & `q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/provenance/action/action.yaml`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz` & `q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/test_data/paired/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz` & `q2_itsxpress-1.8.1/tests/test_data/pairedAllForward/445cf54a-bf06-4852-8010-13a60fa1598c/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz`

 * *Files identical despite different names*

### Comparing `q2_itsxpress-1.8.0/tests/__pycache__/test_main.cpython-36.pyc` & `q2_itsxpress-1.8.1/tests/__pycache__/test_main.cpython-38-pytest-7.1.3.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,430 +1,412 @@
-00000000: 330d 0d0a 63b4 415d 4a26 0000 e300 0000  3...c.A]J&......
-00000010: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
-00000020: 0073 7601 0000 6400 6401 6c00 5a00 6400  .sv...d.d.l.Z.d.
-00000030: 6401 6c01 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
-00000040: 0100 6400 6403 6c04 6d05 5a05 6d06 5a06  ..d.d.l.m.Z.m.Z.
-00000050: 0100 6400 6404 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
-00000060: 6d0a 5a0a 0100 6400 6401 6c0b 6a0c 5a0c  m.Z...d.d.l.j.Z.
-00000070: 6400 6401 6c0d 5a0d 6400 6405 6c0e 6d0f  d.d.l.Z.d.d.l.m.
-00000080: 5a0f 0100 6400 6401 6c10 5a11 6500 6a12  Z...d.d.l.Z.e.j.
-00000090: 6a13 6500 6a12 6a14 6515 8301 8301 5a16  j.e.j.j.e.....Z.
-000000a0: 6500 6a12 6a17 6516 6406 6407 6408 6409  e.j.j.e.d.d.d.d.
-000000b0: 8305 5a18 6509 6518 640a 8302 5a19 6500  ..Z.e.e.d...Z.e.
-000000c0: 6a12 6a17 6516 6406 640b 640c 6409 8305  j.j.e.d.d.d.d...
-000000d0: 5a1a 6509 651a 640a 8302 5a1b 6500 6a12  Z.e.e.d...Z.e.j.
-000000e0: 6a17 6516 6406 640d 6408 6409 8305 5a1c  j.e.d.d.d.d...Z.
-000000f0: 6509 651c 640a 8302 5a1d 6500 6a12 6a17  e.e.d...Z.e.j.j.
-00000100: 6516 6406 640e 640f 6409 8305 5a1e 6509  e.d.d.d.d...Z.e.
-00000110: 651e 640a 8302 5a1f 6500 6a12 6a17 6516  e.d...Z.e.j.j.e.
-00000120: 6406 6410 6411 6409 8305 5a20 6509 6520  d.d.d.d...Z e.e 
-00000130: 640a 8302 5a21 6500 6a12 6a17 6516 6406  d...Z!e.j.j.e.d.
-00000140: 6412 6413 6409 8305 5a22 6508 6522 640a  d.d.d...Z"e.e"d.
-00000150: 8302 5a23 6414 5a24 6415 5a25 6416 6417  ..Z#d.Z$d.Z%d.d.
-00000160: 8400 5a26 4700 6418 6419 8400 6419 6501  ..Z&G.d.d...d.e.
-00000170: 6a27 8303 5a28 641a 641b 8400 5a29 641c  j'..Z(d.d...Z)d.
-00000180: 641d 8400 5a2a 4700 641e 641f 8400 641f  d...Z*G.d.d...d.
-00000190: 6501 6a27 8303 5a2b 6401 5300 2920 e900  e.j'..Z+d.S.) ..
-000001a0: 0000 004e 2901 da09 6765 7473 697a 656f  ...N)...getsizeo
-000001b0: 6629 02da 0365 715f da06 7261 6973 6573  f)...eq_..raises
-000001c0: 2903 da27 5369 6e67 6c65 4c61 6e65 5065  )..'SingleLanePe
-000001d0: 7253 616d 706c 6553 696e 676c 6545 6e64  rSampleSingleEnd
-000001e0: 4661 7374 7144 6972 466d 74da 2753 696e  FastqDirFmt.'Sin
-000001f0: 676c 654c 616e 6550 6572 5361 6d70 6c65  gleLanePerSample
-00000200: 5061 6972 6564 456e 6446 6173 7471 4469  PairedEndFastqDi
-00000210: 7246 6d74 da13 4661 7374 714d 616e 6966  rFmt..FastqManif
-00000220: 6573 7446 6f72 6d61 7429 01da 1072 6564  estFormat)...red
-00000230: 6972 6563 7465 645f 7374 6469 6fda 0974  irected_stdio..t
-00000240: 6573 745f 6461 7461 5a06 7061 6972 6564  est_dataZ.paired
-00000250: 7a24 3434 3563 6635 3461 2d62 6630 362d  z$445cf54a-bf06-
-00000260: 3438 3532 2d38 3031 302d 3133 6136 3066  4852-8010-13a60f
-00000270: 6131 3539 3863 da04 6461 7461 da01 725a  a1598c..data..rZ
-00000280: 1770 6169 7265 6442 726f 6b65 6e4d 6973  .pairedBrokenMis
-00000290: 7369 6e67 4461 7461 7a24 3530 6435 6633  singDataz$50d5f3
-000002a0: 3161 2d61 3736 312d 3463 3034 2d39 3930  1a-a761-4c04-990
-000002b0: 632d 6537 3636 3866 6536 6266 3030 5a10  c-e7668fe6bf00Z.
-000002c0: 7061 6972 6564 416c 6c46 6f72 7761 7264  pairedAllForward
-000002d0: da03 6f75 747a 2464 3939 3535 3734 392d  ..outz$d9955749-
-000002e0: 3030 6435 2d34 3461 652d 6136 3238 2d34  00d5-44ae-a628-4
-000002f0: 6232 6461 3433 3030 3065 315a 0973 696e  b2da43000e1Z.sin
-00000300: 676c 654f 7574 7a24 3735 6165 6134 6635  gleOutz$75aea4f5
-00000310: 2d66 3130 652d 3432 3165 2d39 3164 322d  -f10e-421e-91d2-
-00000320: 6665 6461 3966 6537 6232 6531 5a08 7369  feda9fe7b2e1Z.si
-00000330: 6e67 6c65 496e 7a24 6366 6430 6536 3562  ngleInz$cfd0e65b
-00000340: 2d30 3566 622d 3433 3239 2d39 3631 382d  -05fb-4329-9618-
-00000350: 3135 6563 6430 6165 6339 6233 7a29 5361  15ecd0aec9b3z)Sa
-00000360: 6d70 6c65 4461 7461 5b50 6169 7265 6445  mpleData[PairedE
-00000370: 6e64 5365 7175 656e 6365 7357 6974 6851  ndSequencesWithQ
-00000380: 7561 6c69 7479 5d7a 2053 616d 706c 6544  uality]z SampleD
-00000390: 6174 615b 5365 7175 656e 6365 7357 6974  ata[SequencesWit
-000003a0: 6851 7561 6c69 7479 5d63 0000 0000 0000  hQuality]c......
-000003b0: 0000 0100 0000 0300 0000 4300 0000 731a  ..........C...s.
-000003c0: 0000 0074 006a 0164 0164 028d 017d 0074  ...t.j.d.d...}.t
-000003d0: 027c 0064 0383 0201 0064 0053 0029 044e  .|.d.....d.S.).N
-000003e0: da01 4129 01da 0b74 6178 615f 7072 6566  ..A)...taxa_pref
-000003f0: 6978 da09 416c 7665 6f6c 6174 6129 03da  ix..Alveolata)..
-00000400: 0a5f 6974 7378 7072 6573 73da 145f 7461  ._itsxpress.._ta
-00000410: 7861 5f70 7265 6669 785f 746f 5f74 6178  xa_prefix_to_tax
-00000420: 6172 0300 0000 2901 da04 6578 7031 a900  ar....)...exp1..
-00000430: 7213 0000 00fa 372f 5573 6572 732f 7269  r.....7/Users/ri
-00000440: 7665 7273 2f44 6f63 756d 656e 7473 2f71  vers/Documents/q
-00000450: 325f 6974 7378 7072 6573 732f 7465 7374  2_itsxpress/test
-00000460: 732f 7465 7374 5f6d 6169 6e2e 7079 da18  s/test_main.py..
-00000470: 7465 7374 5f74 6178 615f 7072 6566 6978  test_taxa_prefix
-00000480: 5f74 6f5f 7461 7861 4400 0000 7304 0000  _to_taxaD...s...
-00000490: 0000 010c 0172 1500 0000 6300 0000 0000  .....r....c.....
-000004a0: 0000 0000 0000 0002 0000 0040 0000 0073  ...........@...s
-000004b0: 2c00 0000 6500 5a01 6400 5a02 6401 6402  ,...e.Z.d.Z.d.d.
-000004c0: 8400 5a03 6403 6404 8400 5a04 6405 6406  ..Z.d.d...Z.d.d.
-000004d0: 8400 5a05 6407 6408 8400 5a06 6409 5300  ..Z.d.d...Z.d.S.
-000004e0: 290a da16 5365 7446 6173 7471 7341 6e64  )...SetFastqsAnd
-000004f0: 4368 6563 6b54 6573 7473 6301 0000 0000  CheckTestsc.....
-00000500: 0000 0004 0000 0009 0000 0043 0000 0073  ...........C...s
-00000510: 4e00 0000 7400 6a01 6a02 7403 6a04 8301  N...t.j.j.t.j...
-00000520: 7d01 783a 7c01 6a05 8300 4400 5d2e 7d02  }.x:|.j...D.].}.
-00000530: 7406 6a07 7c02 6a08 6400 7c02 6a09 6401  t.j.|.j.d.|.j.d.
-00000540: 6402 6403 6404 8d06 7d03 7c00 6a0a 6405  d.d.d...}.|.j.d.
-00000550: 7c03 6a0b 6b06 8301 0100 7118 5700 6400  |.j.k.....q.W.d.
-00000560: 5300 2906 4e54 46e9 0100 0000 2906 da05  S.).NTF.....)...
-00000570: 6661 7374 71da 0666 6173 7471 32da 0973  fastq..fastq2..s
-00000580: 616d 706c 655f 6964 da0a 7369 6e67 6c65  ample_id..single
-00000590: 5f65 6e64 da10 7265 7665 7273 6564 5f70  _end..reversed_p
-000005a0: 7269 6d65 7273 da07 7468 7265 6164 737a  rimers..threadsz
-000005b0: 0d34 3737 342d 312d 4d53 4954 5333 290c  .4774-1-MSITS3).
-000005c0: da12 5445 5354 5f44 4154 415f 5349 4e47  ..TEST_DATA_SING
-000005d0: 4c45 494e da08 6d61 6e69 6665 7374 da04  LEIN..manifest..
-000005e0: 7669 6577 da02 7064 da09 4461 7461 4672  view..pd..DataFr
-000005f0: 616d 65da 0a69 7465 7274 7570 6c65 7372  ame..itertuplesr
-00000600: 1000 0000 da15 5f73 6574 5f66 6173 7471  ......_set_fastq
-00000610: 735f 616e 645f 6368 6563 6bda 0766 6f72  s_and_check..for
-00000620: 7761 7264 da05 496e 6465 78da 0a61 7373  ward..Index..ass
-00000630: 6572 7454 7275 6572 1800 0000 2904 da04  ertTruer....)...
-00000640: 7365 6c66 da07 7361 6d70 6c65 73da 0673  self..samples..s
-00000650: 616d 706c 65da 036f 6273 7213 0000 0072  ample..obsr....r
-00000660: 1300 0000 7214 0000 00da 0b74 6573 745f  ....r......test_
-00000670: 7369 6e67 6c65 4a00 0000 7312 0000 0000  singleJ...s.....
-00000680: 010e 010e 0108 0102 0104 0102 0102 0108  ................
-00000690: 017a 2253 6574 4661 7374 7173 416e 6443  .z"SetFastqsAndC
-000006a0: 6865 636b 5465 7374 732e 7465 7374 5f73  heckTests.test_s
-000006b0: 696e 676c 6563 0100 0000 0000 0000 0400  inglec..........
-000006c0: 0000 0900 0000 4300 0000 7350 0000 0074  ......C...sP...t
-000006d0: 006a 016a 0274 036a 0483 017d 0178 3c7c  .j.j.t.j...}.x<|
-000006e0: 016a 0583 0044 005d 307d 0274 066a 077c  .j...D.]0}.t.j.|
-000006f0: 026a 087c 026a 097c 026a 0a64 0164 0264  .j.|.j.|.j.d.d.d
-00000700: 0364 048d 067d 037c 006a 0b64 057c 036a  .d...}.|.j.d.|.j
-00000710: 0c6b 0683 0101 0071 1857 0064 0053 0029  .k.....q.W.d.S.)
-00000720: 064e 5446 7217 0000 0029 0672 1800 0000  .NTFr....).r....
-00000730: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-00000740: 1c00 0000 721d 0000 007a 0d34 3737 342d  ....r....z.4774-
-00000750: 312d 4d53 4954 5333 290d da09 5445 5354  1-MSITS3)...TEST
-00000760: 5f44 4154 4172 1f00 0000 7220 0000 0072  _DATAr....r ...r
-00000770: 2100 0000 7222 0000 0072 2300 0000 7210  !...r"...r#...r.
-00000780: 0000 0072 2400 0000 7225 0000 00da 0772  ...r$...r%.....r
-00000790: 6576 6572 7365 7226 0000 0072 2700 0000  everser&...r'...
-000007a0: 7218 0000 0029 0472 2800 0000 7229 0000  r....).r(...r)..
-000007b0: 0072 2a00 0000 722b 0000 0072 1300 0000  .r*...r+...r....
-000007c0: 7213 0000 0072 1400 0000 da0b 7465 7374  r....r......test
-000007d0: 5f70 6169 7265 6455 0000 0073 1200 0000  _pairedU...s....
-000007e0: 0001 0e01 0e01 0801 0401 0401 0201 0201  ................
-000007f0: 0801 7a22 5365 7446 6173 7471 7341 6e64  ..z"SetFastqsAnd
-00000800: 4368 6563 6b54 6573 7473 2e74 6573 745f  CheckTests.test_
-00000810: 7061 6972 6564 6301 0000 0000 0000 0004  pairedc.........
-00000820: 0000 0009 0000 0043 0000 0073 6000 0000  .......C...s`...
-00000830: 7400 6a01 6a02 7403 6a04 8301 7d01 784c  t.j.j.t.j...}.xL
-00000840: 7c01 6a05 8300 4400 5d40 7d02 7406 6a07  |.j...D.]@}.t.j.
-00000850: 7c02 6a08 7c02 6a09 7c02 6a0a 6401 6401  |.j.|.j.|.j.d.d.
-00000860: 6402 6403 8d06 7d03 7c00 6a0b 6404 7c03  d.d...}.|.j.d.|.
-00000870: 6a0c 6b06 8301 0100 7c00 6a0b 6404 7c03  j.k.....|.j.d.|.
-00000880: 6a0d 6b06 8301 0100 7118 5700 6400 5300  j.k.....q.W.d.S.
-00000890: 2905 4e46 7217 0000 0029 0672 1800 0000  ).NFr....).r....
-000008a0: 7219 0000 0072 1a00 0000 721b 0000 0072  r....r....r....r
-000008b0: 1c00 0000 721d 0000 007a 0d34 3737 342d  ....r....z.4774-
-000008c0: 312d 4d53 4954 5333 290e 722d 0000 0072  1-MSITS3).r-...r
-000008d0: 1f00 0000 7220 0000 0072 2100 0000 7222  ....r ...r!...r"
-000008e0: 0000 0072 2300 0000 7210 0000 0072 2400  ...r#...r....r$.
-000008f0: 0000 7225 0000 0072 2e00 0000 7226 0000  ..r%...r....r&..
-00000900: 0072 2700 0000 7218 0000 0072 1900 0000  .r'...r....r....
-00000910: 2904 7228 0000 0072 2900 0000 722a 0000  ).r(...r)...r*..
-00000920: 0072 2b00 0000 7213 0000 0072 1300 0000  .r+...r....r....
-00000930: 7214 0000 00da 1474 6573 745f 7061 6972  r......test_pair
-00000940: 6564 5f75 6e6d 6572 6765 6460 0000 0073  ed_unmerged`...s
-00000950: 1400 0000 0001 0e01 0e01 0801 0401 0401  ................
-00000960: 0201 0201 0801 1001 7a2b 5365 7446 6173  ........z+SetFas
-00000970: 7471 7341 6e64 4368 6563 6b54 6573 7473  tqsAndCheckTests
-00000980: 2e74 6573 745f 7061 6972 6564 5f75 6e6d  .test_paired_unm
-00000990: 6572 6765 6463 0100 0000 0000 0000 0200  ergedc..........
-000009a0: 0000 0600 0000 0300 0000 7344 0000 0074  ..........sD...t
-000009b0: 006a 016a 0274 036a 0483 017d 0178 307c  .j.j.t.j...}.x0|
-000009c0: 0144 005d 2889 0074 0574 0687 0066 0164  .D.](..t.t...f.d
-000009d0: 0164 0284 0883 0201 0074 0574 0687 0066  .d.......t.t...f
-000009e0: 0164 0364 0284 0883 0201 0071 1457 0064  .d.d.......q.W.d
-000009f0: 0053 0029 044e 6300 0000 0000 0000 0000  .S.).Nc.........
-00000a00: 0000 0008 0000 0013 0000 0073 1c00 0000  ...........s....
-00000a10: 7400 6a01 8800 6a02 8800 6a03 8800 6a04  t.j...j...j...j.
-00000a20: 6401 6401 6402 6403 8d06 5300 2904 4e46  d.d.d.d...S.).NF
-00000a30: 7217 0000 0029 0672 1800 0000 7219 0000  r....).r....r...
-00000a40: 0072 1a00 0000 721b 0000 0072 1c00 0000  .r....r....r....
-00000a50: 721d 0000 0029 0572 1000 0000 7224 0000  r....).r....r$..
-00000a60: 0072 2500 0000 722e 0000 0072 2600 0000  .r%...r....r&...
-00000a70: 7213 0000 0029 0172 2a00 0000 7213 0000  r....).r*...r...
-00000a80: 0072 1400 0000 da08 3c6c 616d 6264 613e  .r......<lambda>
-00000a90: 6f00 0000 730a 0000 0008 0104 0104 0102  o...s...........
-00000aa0: 0102 017a 3d53 6574 4661 7374 7173 416e  ...z=SetFastqsAn
-00000ab0: 6443 6865 636b 5465 7374 732e 7465 7374  dCheckTests.test
-00000ac0: 5f74 7269 6d5f 7061 6972 5f6e 6f5f 6262  _trim_pair_no_bb
-00000ad0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00000ae0: 613e 6300 0000 0000 0000 0000 0000 0008  a>c.............
-00000af0: 0000 0013 0000 0073 1c00 0000 7400 6a01  .......s....t.j.
-00000b00: 8800 6a02 8800 6a03 8800 6a04 6401 6402  ..j...j...j.d.d.
-00000b10: 6403 6404 8d06 5300 2905 4e54 4672 1700  d.d...S.).NTFr..
-00000b20: 0000 2906 7218 0000 0072 1900 0000 721a  ..).r....r....r.
-00000b30: 0000 0072 1b00 0000 721c 0000 0072 1d00  ...r....r....r..
-00000b40: 0000 2905 7210 0000 0072 2400 0000 7225  ..).r....r$...r%
-00000b50: 0000 0072 2e00 0000 7226 0000 0072 1300  ...r....r&...r..
-00000b60: 0000 2901 722a 0000 0072 1300 0000 7214  ..).r*...r....r.
-00000b70: 0000 0072 3100 0000 7500 0000 730a 0000  ...r1...u...s...
-00000b80: 0008 0104 0104 0102 0102 0129 0772 2d00  ...........).r-.
-00000b90: 0000 721f 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
-00000ba0: 0072 2200 0000 7204 0000 00da 0a56 616c  .r"...r......Val
-00000bb0: 7565 4572 726f 7229 0272 2800 0000 7229  ueError).r(...r)
-00000bc0: 0000 0072 1300 0000 2901 722a 0000 0072  ...r....).r*...r
-00000bd0: 1400 0000 da14 7465 7374 5f74 7269 6d5f  ......test_trim_
-00000be0: 7061 6972 5f6e 6f5f 6262 6c00 0000 7308  pair_no_bbl...s.
-00000bf0: 0000 0000 010e 010a 0112 067a 2b53 6574  ...........z+Set
-00000c00: 4661 7374 7173 416e 6443 6865 636b 5465  FastqsAndCheckTe
-00000c10: 7374 732e 7465 7374 5f74 7269 6d5f 7061  sts.test_trim_pa
-00000c20: 6972 5f6e 6f5f 6262 4e29 07da 085f 5f6e  ir_no_bbN)...__n
-00000c30: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000c40: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000c50: 2c00 0000 722f 0000 0072 3000 0000 7233  ,...r/...r0...r3
-00000c60: 0000 0072 1300 0000 7213 0000 0072 1300  ...r....r....r..
-00000c70: 0000 7214 0000 0072 1600 0000 4900 0000  ..r....r....I...
-00000c80: 7308 0000 0008 0108 0b08 0b08 0c72 1600  s............r..
-00000c90: 0000 6300 0000 0000 0000 0007 0000 0007  ..c.............
-00000ca0: 0000 0043 0000 0073 4200 0000 6401 7d00  ...C...sB...d.}.
-00000cb0: 6402 7d01 6403 7d02 6401 7d03 7400 6a01  d.}.d.}.d.}.t.j.
-00000cc0: 7402 7c00 7c01 7c02 7c03 6404 8d05 7d04  t.|.|.|.|.d...}.
-00000cd0: 7403 7c04 8301 7d05 7403 7404 8301 7d06  t.|...}.t.t...}.
-00000ce0: 7405 7c05 7c06 8302 0100 6400 5300 2905  t.|.|.....d.S.).
-00000cf0: 4e72 1700 0000 da01 46da 0449 5453 3229  Nr......F..ITS2)
-00000d00: 05da 1470 6572 5f73 616d 706c 655f 7365  ...per_sample_se
-00000d10: 7175 656e 6365 7372 1d00 0000 da04 7461  quencesr......ta
-00000d20: 7861 da06 7265 6769 6f6e da0a 636c 7573  xa..region..clus
-00000d30: 7465 725f 6964 2906 7210 0000 00da 0b74  ter_id).r......t
-00000d40: 7269 6d5f 7369 6e67 6c65 721e 0000 0072  rim_singler....r
-00000d50: 0200 0000 da13 5445 5354 5f44 4154 415f  ......TEST_DATA_
-00000d60: 5349 4e47 4c45 4f55 5472 0300 0000 2907  SINGLEOUTr....).
-00000d70: 721d 0000 0072 3a00 0000 723b 0000 0072  r....r:...r;...r
-00000d80: 3c00 0000 7212 0000 00da 0465 7870 325a  <...r......exp2Z
-00000d90: 0465 7870 3372 1300 0000 7213 0000 0072  .exp3r....r....r
-00000da0: 1400 0000 da1b 7465 7374 5f74 7269 6d5f  ......test_trim_
-00000db0: 7369 6e67 6c65 5f6e 6f5f 636c 7573 7465  single_no_cluste
-00000dc0: 727d 0000 0073 1800 0000 0001 0401 0401  r}...s..........
-00000dd0: 0401 0402 0601 0201 0201 0201 0801 0801  ................
-00000de0: 0801 7240 0000 0063 0000 0000 0000 0000  ..r@...c........
-00000df0: 0000 0000 0500 0000 0300 0000 7326 0000  ............s&..
-00000e00: 0064 0189 0264 0289 0164 0389 0074 0074  .d...d...d...t.t
-00000e10: 0187 0087 0187 0266 0364 0464 0584 0883  .......f.d.d....
-00000e20: 0201 0064 0053 0029 064e 7217 0000 0072  ...d.S.).Nr....r
-00000e30: 3700 0000 7238 0000 0063 0000 0000 0000  7...r8...c......
-00000e40: 0000 0000 0000 0600 0000 1300 0000 7312  ..............s.
-00000e50: 0000 0074 006a 0174 0288 0288 0188 0064  ...t.j.t.......d
-00000e60: 018d 0453 0029 024e 2904 7239 0000 0072  ...S.).N).r9...r
-00000e70: 1d00 0000 723a 0000 0072 3b00 0000 2903  ....r:...r;...).
-00000e80: 7210 0000 00da 0974 7269 6d5f 7061 6972  r......trim_pair
-00000e90: 722d 0000 0072 1300 0000 2903 723b 0000  r-...r....).r;..
-00000ea0: 0072 3a00 0000 721d 0000 0072 1300 0000  .r:...r....r....
-00000eb0: 7214 0000 0072 3100 0000 9100 0000 7306  r....r1.......s.
-00000ec0: 0000 0006 0102 0102 017a 2974 6573 745f  .........z)test_
-00000ed0: 7472 696d 5f70 6169 725f 6e6f 5f68 6d6d  trim_pair_no_hmm
-00000ee0: 6572 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  er.<locals>.<lam
-00000ef0: 6264 613e 2902 7204 0000 0072 3200 0000  bda>).r....r2...
-00000f00: 7213 0000 0072 1300 0000 2903 723b 0000  r....r....).r;..
-00000f10: 0072 3a00 0000 721d 0000 0072 1400 0000  .r:...r....r....
-00000f20: da17 7465 7374 5f74 7269 6d5f 7061 6972  ..test_trim_pair
-00000f30: 5f6e 6f5f 686d 6d65 728c 0000 0073 0800  _no_hmmer....s..
-00000f40: 0000 0001 0401 0401 0402 7242 0000 0063  ..........rB...c
-00000f50: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-00000f60: 4000 0000 732c 0000 0065 005a 0164 005a  @...s,...e.Z.d.Z
-00000f70: 0264 0164 0284 005a 0364 0364 0484 005a  .d.d...Z.d.d...Z
-00000f80: 0464 0564 0684 005a 0564 0764 0884 005a  .d.d...Z.d.d...Z
-00000f90: 0664 0953 0029 0ada 0954 7269 6d54 6573  .d.S.)...TrimTes
-00000fa0: 7473 6301 0000 0000 0000 0001 0000 0004  tsc.............
-00000fb0: 0000 0043 0000 0073 6400 0000 7400 6a01  ...C...sd...t.j.
-00000fc0: 6a02 8300 6a03 6401 1900 7c00 5f04 7c00  j...j.d...|._.|.
-00000fd0: 6a04 6a05 6402 1900 7c00 5f06 7c00 6a04  j.j.d...|._.|.j.
-00000fe0: 6a05 6403 1900 7c00 5f07 7c00 6a04 6a05  j.d...|._.|.j.j.
-00000ff0: 6404 1900 7c00 5f08 7400 6a09 6a0a 6405  d...|._.t.j.j.d.
-00001000: 740b 6406 8303 7c00 5f0c 7400 6a09 6a0a  t.d...|._.t.j.j.
-00001010: 6407 740d 6408 8303 7c00 5f0e 6400 5300  d.t.d...|._.d.S.
-00001020: 2909 4eda 0969 7473 7870 7265 7373 723d  ).N..itsxpressr=
-00001030: 0000 0072 4100 0000 da19 7472 696d 5f70  ...rA.....trim_p
-00001040: 6169 725f 6f75 7470 7574 5f75 6e6d 6572  air_output_unmer
-00001050: 6765 647a 2053 616d 706c 6544 6174 615b  gedz SampleData[
-00001060: 5365 7175 656e 6365 7357 6974 6851 7561  SequencesWithQua
-00001070: 6c69 7479 5d72 0500 0000 7a29 5361 6d70  lity]r....z)Samp
-00001080: 6c65 4461 7461 5b50 6169 7265 6445 6e64  leData[PairedEnd
-00001090: 5365 7175 656e 6365 7357 6974 6851 7561  SequencesWithQua
-000010a0: 6c69 7479 5d72 0600 0000 290f da06 7169  lity]r....)...qi
-000010b0: 696d 6532 da03 7364 6bda 0d50 6c75 6769  ime2..sdk..Plugi
-000010c0: 6e4d 616e 6167 6572 da07 706c 7567 696e  nManager..plugin
-000010d0: 73da 0670 6c75 6769 6eda 076d 6574 686f  s..plugin..metho
-000010e0: 6473 da0e 7472 696d 5f73 696e 676c 655f  ds..trim_single_
-000010f0: 666e da0e 7472 696d 5f70 6169 7265 645f  fn..trim_paired_
-00001100: 666e da17 7472 696d 5f70 6169 7265 645f  fn..trim_paired_
-00001110: 756e 6d65 7267 6564 5f66 6eda 0841 7274  unmerged_fn..Art
-00001120: 6966 6163 74da 0b69 6d70 6f72 745f 6461  ifact..import_da
-00001130: 7461 da12 5445 5354 5f46 494c 455f 5349  ta..TEST_FILE_SI
-00001140: 4e47 4c45 494e da07 7365 5f73 6571 73da  NGLEIN..se_seqs.
-00001150: 0954 4553 545f 4649 4c45 da07 7065 5f73  .TEST_FILE..pe_s
-00001160: 6571 7329 0172 2800 0000 7213 0000 0072  eqs).r(...r....r
-00001170: 1300 0000 7214 0000 00da 0573 6574 5570  ....r......setUp
-00001180: 9700 0000 7318 0000 0000 0112 010e 010e  ....s...........
-00001190: 020e 0206 0102 0102 0108 0106 0102 0102  ................
-000011a0: 017a 0f54 7269 6d54 6573 7473 2e73 6574  .z.TrimTests.set
-000011b0: 5570 6301 0000 0000 0000 0006 0000 000b  Upc.............
-000011c0: 0000 0043 0000 0073 8e00 0000 7400 7401  ...C...s....t.t.
-000011d0: 6a02 6401 8d01 8f16 0100 7c00 6a03 7c00  j.d.......|.j.|.
-000011e0: 6a04 6402 8302 5c01 7d01 5700 6400 5100  j.d...\.}.W.d.Q.
-000011f0: 5200 5800 7c00 6a05 7406 7c01 6a07 8301  R.X.|.j.t.|.j...
-00001200: 6403 8302 0100 7c01 6a08 7409 8301 7d02  d.....|.j.t...}.
-00001210: 7c00 6a05 740a 7c02 8301 740a 740b 8301  |.j.t.|...t.t...
-00001220: 8302 0100 7c01 6a08 7409 8301 7d03 740c  ....|.j.t...}.t.
-00001230: 7c03 6a0d 6a08 740e 8301 6a0f 8300 8301  |.j.j.t...j.....
-00001240: 7d04 6404 6405 6702 7d05 7c00 6a05 7c04  }.d.d.g.}.|.j.|.
-00001250: 7c05 8302 0100 6400 5300 2906 4e29 01da  |.....d.S.).N)..
-00001260: 0673 7464 6572 7272 3800 0000 7a20 5361  .stderrr8...z Sa
-00001270: 6d70 6c65 4461 7461 5b53 6571 7565 6e63  mpleData[Sequenc
-00001280: 6573 5769 7468 5175 616c 6974 795d 7a1d  esWithQuality]z.
-00001290: 7361 6d70 6c65 2d69 642c 6669 6c65 6e61  sample-id,filena
-000012a0: 6d65 2c64 6972 6563 7469 6f6e 0a7a 3b34  me,direction.z;4
-000012b0: 3737 342d 312d 4d53 4954 5333 2c34 3737  774-1-MSITS3,477
-000012c0: 342d 312d 4d53 4954 5333 5f30 5f4c 3030  4-1-MSITS3_0_L00
-000012d0: 315f 5231 5f30 3031 2e66 6173 7471 2e67  1_R1_001.fastq.g
-000012e0: 7a2c 666f 7277 6172 640a 2910 7208 0000  z,forward.).r...
-000012f0: 00da 026f 73da 0764 6576 6e75 6c6c 724c  ...os..devnullrL
-00001300: 0000 0072 5200 0000 da0b 6173 7365 7274  ...rR.....assert
-00001310: 4571 7561 6cda 0373 7472 da04 7479 7065  Equal..str..type
-00001320: 7220 0000 0072 0500 0000 7202 0000 0072  r ...r....r....r
-00001330: 3e00 0000 da04 6c69 7374 721f 0000 0072  >.....listr....r
-00001340: 0700 0000 da04 6f70 656e 2906 7228 0000  ......open).r(..
-00001350: 00da 0c6f 6273 5f61 7274 6966 6163 74da  ...obs_artifact.
-00001360: 076f 6273 5f64 6972 722b 0000 00da 0c6f  .obs_dirr+.....o
-00001370: 6273 5f6d 616e 6966 6573 74da 0c65 7870  bs_manifest..exp
-00001380: 5f6d 616e 6966 6573 7472 1300 0000 7213  _manifestr....r.
-00001390: 0000 0072 1400 0000 da18 7465 7374 5f74  ...r......test_t
-000013a0: 7269 6d5f 7369 6e67 6c65 5f73 7563 6365  rim_single_succe
-000013b0: 7373 a700 0000 7316 0000 0000 010e 011a  ss....s.........
-000013c0: 010c 0106 020a 0114 020a 0114 0202 0106  ................
-000013d0: 017a 2254 7269 6d54 6573 7473 2e74 6573  .z"TrimTests.tes
-000013e0: 745f 7472 696d 5f73 696e 676c 655f 7375  t_trim_single_su
-000013f0: 6363 6573 7363 0100 0000 0000 0000 0600  ccessc..........
-00001400: 0000 0b00 0000 4300 0000 738e 0000 0074  ......C...s....t
-00001410: 0074 016a 0264 018d 018f 1601 007c 006a  .t.j.d.......|.j
-00001420: 037c 006a 0464 0283 025c 017d 0157 0064  .|.j.d...\.}.W.d
-00001430: 0051 0052 0058 007c 006a 0574 067c 016a  .Q.R.X.|.j.t.|.j
-00001440: 0783 0164 0383 0201 007c 016a 0874 0983  ...d.....|.j.t..
-00001450: 017d 027c 006a 0574 0a7c 0283 0174 0a74  .}.|.j.t.|...t.t
-00001460: 0b83 0183 0201 007c 016a 0874 0983 017d  .......|.j.t...}
-00001470: 0374 0c7c 036a 0d6a 0874 0e83 016a 0f83  .t.|.j.j.t...j..
-00001480: 0083 017d 0464 0464 0567 027d 057c 006a  ...}.d.d.g.}.|.j
-00001490: 057c 047c 0583 0201 0064 0053 0029 064e  .|.|.....d.S.).N
-000014a0: 2901 7256 0000 0072 3800 0000 7a26 5361  ).rV...r8...z&Sa
-000014b0: 6d70 6c65 4461 7461 5b4a 6f69 6e65 6453  mpleData[JoinedS
-000014c0: 6571 7565 6e63 6573 5769 7468 5175 616c  equencesWithQual
-000014d0: 6974 795d 7a1d 7361 6d70 6c65 2d69 642c  ity]z.sample-id,
-000014e0: 6669 6c65 6e61 6d65 2c64 6972 6563 7469  filename,directi
-000014f0: 6f6e 0a7a 3b34 3737 342d 312d 4d53 4954  on.z;4774-1-MSIT
-00001500: 5333 2c34 3737 342d 312d 4d53 4954 5333  S3,4774-1-MSITS3
-00001510: 5f30 5f4c 3030 315f 5231 5f30 3031 2e66  _0_L001_R1_001.f
-00001520: 6173 7471 2e67 7a2c 666f 7277 6172 640a  astq.gz,forward.
-00001530: 2910 7208 0000 0072 5700 0000 7258 0000  ).r....rW...rX..
-00001540: 0072 4d00 0000 7254 0000 0072 5900 0000  .rM...rT...rY...
-00001550: 725a 0000 0072 5b00 0000 7220 0000 0072  rZ...r[...r ...r
-00001560: 0500 0000 7202 0000 00da 0d54 4553 545f  ....r......TEST_
-00001570: 4441 5441 5f4f 5554 725c 0000 0072 1f00  DATA_OUTr\...r..
-00001580: 0000 7207 0000 0072 5d00 0000 2906 7228  ..r....r]...).r(
-00001590: 0000 0072 5e00 0000 725f 0000 0072 2b00  ...r^...r_...r+.
-000015a0: 0000 7260 0000 0072 6100 0000 7213 0000  ..r`...ra...r...
-000015b0: 0072 1300 0000 7214 0000 00da 1674 6573  .r....r......tes
-000015c0: 745f 7472 696d 5f70 6169 725f 7375 6363  t_trim_pair_succ
-000015d0: 6573 73b7 0000 0073 1600 0000 0001 0e01  ess....s........
-000015e0: 1a01 0c01 0602 0a01 1402 0a01 1402 0201  ................
-000015f0: 0601 7a20 5472 696d 5465 7374 732e 7465  ..z TrimTests.te
-00001600: 7374 5f74 7269 6d5f 7061 6972 5f73 7563  st_trim_pair_suc
-00001610: 6365 7373 6301 0000 0000 0000 0005 0000  cessc...........
-00001620: 000a 0000 0043 0000 0073 7200 0000 7400  .....C...sr...t.
-00001630: 7401 6a02 6401 8d01 8f16 0100 7c00 6a03  t.j.d.......|.j.
-00001640: 7c00 6a04 6402 8302 5c01 7d01 5700 6400  |.j.d...\.}.W.d.
-00001650: 5100 5200 5800 7c00 6a05 7406 7c01 6a07  Q.R.X.|.j.t.|.j.
-00001660: 8301 6403 8302 0100 7c01 6a08 7409 8301  ..d.....|.j.t...
-00001670: 7d02 740a 7c02 6a0b 6a08 740c 8301 6a0d  }.t.|.j.j.t...j.
-00001680: 8300 8301 7d03 6404 6405 6406 6703 7d04  ....}.d.d.d.g.}.
-00001690: 7c00 6a05 7c03 7c04 8302 0100 6400 5300  |.j.|.|.....d.S.
-000016a0: 2907 4e29 0172 5600 0000 7238 0000 007a  ).N).rV...r8...z
-000016b0: 2953 616d 706c 6544 6174 615b 5061 6972  )SampleData[Pair
-000016c0: 6564 456e 6453 6571 7565 6e63 6573 5769  edEndSequencesWi
-000016d0: 7468 5175 616c 6974 795d 7a1d 7361 6d70  thQuality]z.samp
-000016e0: 6c65 2d69 642c 6669 6c65 6e61 6d65 2c64  le-id,filename,d
-000016f0: 6972 6563 7469 6f6e 0a7a 3b34 3737 342d  irection.z;4774-
-00001700: 312d 4d53 4954 5333 2c34 3737 342d 312d  1-MSITS3,4774-1-
-00001710: 4d53 4954 5333 5f30 5f4c 3030 315f 5231  MSITS3_0_L001_R1
-00001720: 5f30 3031 2e66 6173 7471 2e67 7a2c 666f  _001.fastq.gz,fo
-00001730: 7277 6172 640a 7a3b 3437 3734 2d31 2d4d  rward.z;4774-1-M
-00001740: 5349 5453 332c 3437 3734 2d31 2d4d 5349  SITS3,4774-1-MSI
-00001750: 5453 335f 315f 4c30 3031 5f52 325f 3030  TS3_1_L001_R2_00
-00001760: 312e 6661 7374 712e 677a 2c72 6576 6572  1.fastq.gz,rever
-00001770: 7365 0a29 0e72 0800 0000 7257 0000 0072  se.).r....rW...r
-00001780: 5800 0000 724e 0000 0072 5400 0000 7259  X...rN...rT...rY
-00001790: 0000 0072 5a00 0000 725b 0000 0072 2000  ...rZ...r[...r .
-000017a0: 0000 7206 0000 0072 5c00 0000 721f 0000  ..r....r\...r...
-000017b0: 0072 0700 0000 725d 0000 0029 0572 2800  .r....r]...).r(.
-000017c0: 0000 725e 0000 0072 2b00 0000 7260 0000  ..r^...r+...r`..
-000017d0: 0072 6100 0000 7213 0000 0072 1300 0000  .ra...r....r....
-000017e0: 7214 0000 00da 2674 6573 745f 7472 696d  r.....&test_trim
-000017f0: 5f70 6169 725f 6f75 7470 7574 5f75 6e6d  _pair_output_unm
-00001800: 6572 6765 645f 7375 6363 6573 73c7 0000  erged_success...
-00001810: 0073 1400 0000 0001 0e01 1a01 0c01 0601  .s..............
-00001820: 0a01 1402 0201 0201 0601 7a30 5472 696d  ..........z0Trim
-00001830: 5465 7374 732e 7465 7374 5f74 7269 6d5f  Tests.test_trim_
-00001840: 7061 6972 5f6f 7574 7075 745f 756e 6d65  pair_output_unme
-00001850: 7267 6564 5f73 7563 6365 7373 4e29 0772  rged_successN).r
-00001860: 3400 0000 7235 0000 0072 3600 0000 7255  4...r5...r6...rU
-00001870: 0000 0072 6200 0000 7264 0000 0072 6500  ...rb...rd...re.
-00001880: 0000 7213 0000 0072 1300 0000 7213 0000  ..r....r....r...
-00001890: 0072 1400 0000 7243 0000 0096 0000 0073  .r....rC.......s
-000018a0: 0800 0000 0801 0810 0810 0810 7243 0000  ............rC..
-000018b0: 0029 2c72 5700 0000 da08 756e 6974 7465  .),rW.....unitte
-000018c0: 7374 da03 7379 7372 0200 0000 da0a 6e6f  st..sysr......no
-000018d0: 7365 2e74 6f6f 6c73 7203 0000 0072 0400  se.toolsr....r..
-000018e0: 0000 da1d 7132 5f74 7970 6573 2e70 6572  ....q2_types.per
-000018f0: 5f73 616d 706c 655f 7365 7175 656e 6365  _sample_sequence
-00001900: 7372 0500 0000 7206 0000 0072 0700 0000  sr....r....r....
-00001910: da17 7132 5f69 7473 7870 7265 7373 2e5f  ..q2_itsxpress._
-00001920: 6974 7378 7072 6573 7372 1000 0000 7246  itsxpressr....rF
-00001930: 0000 00da 0b71 6969 6d65 322e 7574 696c  .....qiime2.util
-00001940: 7208 0000 00da 0670 616e 6461 7372 2100  r......pandasr!.
-00001950: 0000 da04 7061 7468 da07 6469 726e 616d  ....path..dirnam
-00001960: 65da 0761 6273 7061 7468 da08 5f5f 6669  e..abspath..__fi
-00001970: 6c65 5f5f 5a08 5445 5354 5f44 4952 da04  le__Z.TEST_DIR..
-00001980: 6a6f 696e 7253 0000 0072 2d00 0000 5a0e  joinrS...r-...Z.
-00001990: 5445 5354 5f46 494c 455f 5042 4d44 5a0e  TEST_FILE_PBMDZ.
-000019a0: 5445 5354 5f44 4154 415f 5042 4d44 5a0d  TEST_DATA_PBMDZ.
-000019b0: 5445 5354 5f46 494c 455f 5041 465a 0d54  TEST_FILE_PAFZ.T
-000019c0: 4553 545f 4441 5441 5f50 4146 5a0d 5445  EST_DATA_PAFZ.TE
-000019d0: 5354 5f46 494c 455f 4f55 5472 6300 0000  ST_FILE_OUTrc...
-000019e0: 5a13 5445 5354 5f46 494c 455f 5349 4e47  Z.TEST_FILE_SING
-000019f0: 4c45 4f55 5472 3e00 0000 7251 0000 0072  LEOUTr>...rQ...r
-00001a00: 1e00 0000 5a0f 4152 5449 4641 4354 5f54  ....Z.ARTIFACT_T
-00001a10: 5950 455f 505a 0f41 5254 4946 4143 545f  YPE_PZ.ARTIFACT_
-00001a20: 5459 5045 5f53 7215 0000 00da 0854 6573  TYPE_Sr......Tes
-00001a30: 7443 6173 6572 1600 0000 7240 0000 0072  tCaser....r@...r
-00001a40: 4200 0000 7243 0000 0072 1300 0000 7213  B...rC...r....r.
-00001a50: 0000 0072 1300 0000 7214 0000 00da 083c  ...r....r......<
-00001a60: 6d6f 6475 6c65 3e01 0000 0073 6800 0000  module>....sh...
-00001a70: 0801 0801 0c02 1001 1404 0a02 0801 0c01  ................
-00001a80: 0803 1402 0801 0201 0201 0201 0602 0a02  ................
-00001a90: 0801 0201 0201 0201 0602 0a02 0801 0201  ................
-00001aa0: 0201 0201 0601 0a02 0801 0201 0201 0201  ................
-00001ab0: 0601 0a02 0801 0201 0201 0201 0601 0a02  ................
-00001ac0: 0801 0201 0201 0201 0601 0a02 0402 0403  ................
-00001ad0: 0805 1234 080f 080a                      ...4....
+00000000: 550d 0d0a 0000 0000 03fe 7064 4e26 0000  U.........pdN&..
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0007 0000 0040 0000 0073 9201 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a01 6400 6401 6c02 6d03 0200  d.l.Z.d.d.l.m...
+00000040: 0100 6d04 5a05 0100 6400 6401 6c06 5a06  ..m.Z...d.d.l.Z.
+00000050: 6400 6401 6c07 5a07 6400 6402 6c08 6d09  d.d.l.Z.d.d.l.m.
+00000060: 5a09 0100 6400 6403 6c0a 6d0b 5a0b 6d0c  Z...d.d.l.m.Z.m.
+00000070: 5a0c 0100 6400 6404 6c0d 6d0e 5a0e 6d0f  Z...d.d.l.m.Z.m.
+00000080: 5a0f 6d10 5a10 0100 6400 6401 6c11 6d12  Z.m.Z...d.d.l.m.
+00000090: 5a12 0100 6400 6401 6c13 5a13 6400 6405  Z...d.d.l.Z.d.d.
+000000a0: 6c14 6d15 5a15 0100 6400 6401 6c16 5a17  l.m.Z...d.d.l.Z.
+000000b0: 6506 6a18 a019 6506 6a18 a01a 651b a101  e.j...e.j...e...
+000000c0: a101 5a1c 6506 6a18 a01d 651c 6406 6407  ..Z.e.j...e.d.d.
+000000d0: 6408 6409 a105 5a1e 650f 651e 640a 8302  d.d...Z.e.e.d...
+000000e0: 5a1f 6506 6a18 a01d 651c 6406 640b 640c  Z.e.j...e.d.d.d.
+000000f0: 6409 a105 5a20 650f 6520 640a 8302 5a21  d...Z e.e d...Z!
+00000100: 6506 6a18 a01d 651c 6406 640d 6408 6409  e.j...e.d.d.d.d.
+00000110: a105 5a22 650f 6522 640a 8302 5a23 6506  ..Z"e.e"d...Z#e.
+00000120: 6a18 a01d 651c 6406 640e 640f 6409 a105  j...e.d.d.d.d...
+00000130: 5a24 650f 6524 640a 8302 5a25 6506 6a18  Z$e.e$d...Z%e.j.
+00000140: a01d 651c 6406 6410 6411 6409 a105 5a26  ..e.d.d.d.d...Z&
+00000150: 650f 6526 640a 8302 5a27 6506 6a18 a01d  e.e&d...Z'e.j...
+00000160: 651c 6406 6412 6413 6409 a105 5a28 650e  e.d.d.d.d...Z(e.
+00000170: 6528 640a 8302 5a29 6414 5a2a 6415 5a2b  e(d...Z)d.Z*d.Z+
+00000180: 6416 6417 8400 5a2c 4700 6418 6419 8400  d.d...Z,G.d.d...
+00000190: 6419 6507 6a2d 8303 5a2e 641a 641b 8400  d.e.j-..Z.d.d...
+000001a0: 5a2f 641c 641d 8400 5a30 4700 641e 641f  Z/d.d...Z0G.d.d.
+000001b0: 8400 641f 6507 6a2d 8303 5a31 6401 5300  ..d.e.j-..Z1d.S.
+000001c0: 2920 e900 0000 004e 2901 da09 6765 7473  ) .....N)...gets
+000001d0: 697a 656f 6629 02da 0365 715f da06 7261  izeof)...eq_..ra
+000001e0: 6973 6573 2903 da27 5369 6e67 6c65 4c61  ises)..'SingleLa
+000001f0: 6e65 5065 7253 616d 706c 6553 696e 676c  nePerSampleSingl
+00000200: 6545 6e64 4661 7374 7144 6972 466d 74da  eEndFastqDirFmt.
+00000210: 2753 696e 676c 654c 616e 6550 6572 5361  'SingleLanePerSa
+00000220: 6d70 6c65 5061 6972 6564 456e 6446 6173  mplePairedEndFas
+00000230: 7471 4469 7246 6d74 da13 4661 7374 714d  tqDirFmt..FastqM
+00000240: 616e 6966 6573 7446 6f72 6d61 7429 01da  anifestFormat)..
+00000250: 1072 6564 6972 6563 7465 645f 7374 6469  .redirected_stdi
+00000260: 6fda 0974 6573 745f 6461 7461 da06 7061  o..test_data..pa
+00000270: 6972 6564 7a24 3434 3563 6635 3461 2d62  iredz$445cf54a-b
+00000280: 6630 362d 3438 3532 2d38 3031 302d 3133  f06-4852-8010-13
+00000290: 6136 3066 6131 3539 3863 da04 6461 7461  a60fa1598c..data
+000002a0: da01 72da 1770 6169 7265 6442 726f 6b65  ..r..pairedBroke
+000002b0: 6e4d 6973 7369 6e67 4461 7461 7a24 3530  nMissingDataz$50
+000002c0: 6435 6633 3161 2d61 3736 312d 3463 3034  d5f31a-a761-4c04
+000002d0: 2d39 3930 632d 6537 3636 3866 6536 6266  -990c-e7668fe6bf
+000002e0: 3030 da10 7061 6972 6564 416c 6c46 6f72  00..pairedAllFor
+000002f0: 7761 7264 da03 6f75 747a 2464 3939 3535  ward..outz$d9955
+00000300: 3734 392d 3030 6435 2d34 3461 652d 6136  749-00d5-44ae-a6
+00000310: 3238 2d34 6232 6461 3433 3030 3065 31da  28-4b2da43000e1.
+00000320: 0973 696e 676c 654f 7574 7a24 3735 6165  .singleOutz$75ae
+00000330: 6134 6635 2d66 3130 652d 3432 3165 2d39  a4f5-f10e-421e-9
+00000340: 3164 322d 6665 6461 3966 6537 6232 6531  1d2-feda9fe7b2e1
+00000350: da08 7369 6e67 6c65 496e 7a24 6366 6430  ..singleInz$cfd0
+00000360: 6536 3562 2d30 3566 622d 3433 3239 2d39  e65b-05fb-4329-9
+00000370: 3631 382d 3135 6563 6430 6165 6339 6233  618-15ecd0aec9b3
+00000380: fa29 5361 6d70 6c65 4461 7461 5b50 6169  .)SampleData[Pai
+00000390: 7265 6445 6e64 5365 7175 656e 6365 7357  redEndSequencesW
+000003a0: 6974 6851 7561 6c69 7479 5dfa 2053 616d  ithQuality]. Sam
+000003b0: 706c 6544 6174 615b 5365 7175 656e 6365  pleData[Sequence
+000003c0: 7357 6974 6851 7561 6c69 7479 5d63 0000  sWithQuality]c..
+000003d0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+000003e0: 0000 4300 0000 731a 0000 0074 006a 0164  ..C...s....t.j.d
+000003f0: 0164 028d 017d 0074 027c 0064 0383 0201  .d...}.t.|.d....
+00000400: 0064 0053 0029 044e da01 4129 015a 0b74  .d.S.).N..A).Z.t
+00000410: 6178 615f 7072 6566 6978 5a09 416c 7665  axa_prefixZ.Alve
+00000420: 6f6c 6174 6129 03da 0a5f 6974 7378 7072  olata)..._itsxpr
+00000430: 6573 735a 145f 7461 7861 5f70 7265 6669  essZ._taxa_prefi
+00000440: 785f 746f 5f74 6178 6172 0300 0000 2901  x_to_taxar....).
+00000450: da04 6578 7031 a900 7217 0000 00fa 5a2f  ..exp1..r.....Z/
+00000460: 686f 6d65 2f73 7665 696e 6e2f 4472 6f70  home/sveinn/Drop
+00000470: 626f 782f 5546 4c5f 5553 4441 5f69 7473  box/UFL_USDA_its
+00000480: 7870 7265 7373 2f56 5363 6f64 655f 6974  xpress/VScode_it
+00000490: 7378 7072 6573 7356 322f 7132 5f69 7473  sxpressV2/q2_its
+000004a0: 7870 7265 7373 2f74 6573 7473 2f74 6573  xpress/tests/tes
+000004b0: 745f 6d61 696e 2e70 79da 1874 6573 745f  t_main.py..test_
+000004c0: 7461 7861 5f70 7265 6669 785f 746f 5f74  taxa_prefix_to_t
+000004d0: 6178 6144 0000 0073 0400 0000 0001 0c01  axaD...s........
+000004e0: 7219 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000004f0: 0000 0000 0000 0200 0000 4000 0000 732c  ..........@...s,
+00000500: 0000 0065 005a 0164 005a 0264 0164 0284  ...e.Z.d.Z.d.d..
+00000510: 005a 0364 0364 0484 005a 0464 0564 0684  .Z.d.d...Z.d.d..
+00000520: 005a 0564 0764 0884 005a 0664 0953 0029  .Z.d.d...Z.d.S.)
+00000530: 0ada 1653 6574 4661 7374 7173 416e 6443  ...SetFastqsAndC
+00000540: 6865 636b 5465 7374 7363 0100 0000 0000  heckTestsc......
+00000550: 0000 0000 0000 0400 0000 0900 0000 4300  ..............C.
+00000560: 0000 734a 0000 0074 006a 01a0 0274 036a  ..sJ...t.j...t.j
+00000570: 04a1 017d 017c 01a0 05a1 0044 005d 2e7d  ...}.|.....D.].}
+00000580: 0274 066a 077c 026a 0864 007c 026a 0964  .t.j.|.j.d.|.j.d
+00000590: 0164 0264 0364 048d 067d 037c 00a0 0a64  .d.d.d...}.|...d
+000005a0: 057c 036a 0b6b 06a1 0101 0071 1664 0053  .|.j.k.....q.d.S
+000005b0: 00a9 064e 5446 e901 0000 00a9 06da 0566  ...NTF.........f
+000005c0: 6173 7471 da06 6661 7374 7132 5a09 7361  astq..fastq2Z.sa
+000005d0: 6d70 6c65 5f69 645a 0a73 696e 676c 655f  mple_idZ.single_
+000005e0: 656e 645a 1072 6576 6572 7365 645f 7072  endZ.reversed_pr
+000005f0: 696d 6572 73da 0774 6872 6561 6473 fa0d  imers..threads..
+00000600: 3437 3734 2d31 2d4d 5349 5453 3329 0cda  4774-1-MSITS3)..
+00000610: 1254 4553 545f 4441 5441 5f53 494e 474c  .TEST_DATA_SINGL
+00000620: 4549 4eda 086d 616e 6966 6573 74da 0476  EIN..manifest..v
+00000630: 6965 77da 0270 64da 0944 6174 6146 7261  iew..pd..DataFra
+00000640: 6d65 da0a 6974 6572 7475 706c 6573 7215  me..itertuplesr.
+00000650: 0000 00da 155f 7365 745f 6661 7374 7173  ....._set_fastqs
+00000660: 5f61 6e64 5f63 6865 636b da07 666f 7277  _and_check..forw
+00000670: 6172 64da 0549 6e64 6578 da0a 6173 7365  ard..Index..asse
+00000680: 7274 5472 7565 721e 0000 00a9 04da 0473  rtTruer........s
+00000690: 656c 66da 0773 616d 706c 6573 da06 7361  elf..samples..sa
+000006a0: 6d70 6c65 da03 6f62 7372 1700 0000 7217  mple..obsr....r.
+000006b0: 0000 0072 1800 0000 da0b 7465 7374 5f73  ...r......test_s
+000006c0: 696e 676c 654a 0000 0073 1400 0000 0001  ingleJ...s......
+000006d0: 0e01 0c01 0801 0201 0401 0201 0201 02fb  ................
+000006e0: 0606 7a22 5365 7446 6173 7471 7341 6e64  ..z"SetFastqsAnd
+000006f0: 4368 6563 6b54 6573 7473 2e74 6573 745f  CheckTests.test_
+00000700: 7369 6e67 6c65 6301 0000 0000 0000 0000  singlec.........
+00000710: 0000 0004 0000 0009 0000 0043 0000 0073  ...........C...s
+00000720: 4c00 0000 7400 6a01 a002 7403 6a04 a101  L...t.j...t.j...
+00000730: 7d01 7c01 a005 a100 4400 5d30 7d02 7406  }.|.....D.]0}.t.
+00000740: 6a07 7c02 6a08 7c02 6a09 7c02 6a0a 6401  j.|.j.|.j.|.j.d.
+00000750: 6402 6403 6404 8d06 7d03 7c00 a00b 6405  d.d.d...}.|...d.
+00000760: 7c03 6a0c 6b06 a101 0100 7116 6400 5300  |.j.k.....q.d.S.
+00000770: 721b 0000 0029 0dda 0954 4553 545f 4441  r....)...TEST_DA
+00000780: 5441 7223 0000 0072 2400 0000 7225 0000  TAr#...r$...r%..
+00000790: 0072 2600 0000 7227 0000 0072 1500 0000  .r&...r'...r....
+000007a0: 7228 0000 0072 2900 0000 da07 7265 7665  r(...r).....reve
+000007b0: 7273 6572 2a00 0000 722b 0000 0072 1e00  rser*...r+...r..
+000007c0: 0000 722c 0000 0072 1700 0000 7217 0000  ..r,...r....r...
+000007d0: 0072 1800 0000 da0b 7465 7374 5f70 6169  .r......test_pai
+000007e0: 7265 6455 0000 0073 1400 0000 0001 0e01  redU...s........
+000007f0: 0c01 0801 0401 0401 0201 0201 02fb 0606  ................
+00000800: 7a22 5365 7446 6173 7471 7341 6e64 4368  z"SetFastqsAndCh
+00000810: 6563 6b54 6573 7473 2e74 6573 745f 7061  eckTests.test_pa
+00000820: 6972 6564 6301 0000 0000 0000 0000 0000  iredc...........
+00000830: 0004 0000 0009 0000 0043 0000 0073 5c00  .........C...s\.
+00000840: 0000 7400 6a01 a002 7403 6a04 a101 7d01  ..t.j...t.j...}.
+00000850: 7c01 a005 a100 4400 5d40 7d02 7406 6a07  |.....D.]@}.t.j.
+00000860: 7c02 6a08 7c02 6a09 7c02 6a0a 6401 6401  |.j.|.j.|.j.d.d.
+00000870: 6402 6403 8d06 7d03 7c00 a00b 6404 7c03  d.d...}.|...d.|.
+00000880: 6a0c 6b06 a101 0100 7c00 a00b 6404 7c03  j.k.....|...d.|.
+00000890: 6a0d 6b06 a101 0100 7116 6400 5300 2905  j.k.....q.d.S.).
+000008a0: 4e46 721c 0000 0072 1d00 0000 7221 0000  NFr....r....r!..
+000008b0: 0029 0e72 3200 0000 7223 0000 0072 2400  .).r2...r#...r$.
+000008c0: 0000 7225 0000 0072 2600 0000 7227 0000  ..r%...r&...r'..
+000008d0: 0072 1500 0000 7228 0000 0072 2900 0000  .r....r(...r)...
+000008e0: 7233 0000 0072 2a00 0000 722b 0000 0072  r3...r*...r+...r
+000008f0: 1e00 0000 721f 0000 0072 2c00 0000 7217  ....r....r,...r.
+00000900: 0000 0072 1700 0000 7218 0000 00da 1474  ...r....r......t
+00000910: 6573 745f 7061 6972 6564 5f75 6e6d 6572  est_paired_unmer
+00000920: 6765 6460 0000 0073 1600 0000 0001 0e01  ged`...s........
+00000930: 0c01 0801 0401 0401 0201 0201 02fb 0606  ................
+00000940: 1001 7a2b 5365 7446 6173 7471 7341 6e64  ..z+SetFastqsAnd
+00000950: 4368 6563 6b54 6573 7473 2e74 6573 745f  CheckTests.test_
+00000960: 7061 6972 6564 5f75 6e6d 6572 6765 6463  paired_unmergedc
+00000970: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000980: 0600 0000 0300 0000 7340 0000 0074 006a  ........s@...t.j
+00000990: 01a0 0274 036a 04a1 017d 017c 0144 005d  ...t.j...}.|.D.]
+000009a0: 2889 0074 0574 0687 0066 0164 0164 0284  (..t.t...f.d.d..
+000009b0: 0883 0201 0074 0574 0687 0066 0164 0364  .....t.t...f.d.d
+000009c0: 0284 0883 0201 0071 1264 0053 0029 044e  .......q.d.S.).N
+000009d0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+000009e0: 0008 0000 0013 0000 0073 1c00 0000 7400  .........s....t.
+000009f0: 6a01 8800 6a02 8800 6a03 8800 6a04 6401  j...j...j...j.d.
+00000a00: 6401 6402 6403 8d06 5300 2904 4e46 721c  d.d.d...S.).NFr.
+00000a10: 0000 0072 1d00 0000 a905 7215 0000 0072  ...r......r....r
+00000a20: 2800 0000 7229 0000 0072 3300 0000 722a  (...r)...r3...r*
+00000a30: 0000 0072 1700 0000 a901 722f 0000 0072  ...r......r/...r
+00000a40: 1700 0000 7218 0000 00da 083c 6c61 6d62  ....r......<lamb
+00000a50: 6461 3e6f 0000 0073 0c00 0000 0801 0401  da>o...s........
+00000a60: 0401 0201 0201 02fb 7a3d 5365 7446 6173  ........z=SetFas
+00000a70: 7471 7341 6e64 4368 6563 6b54 6573 7473  tqsAndCheckTests
+00000a80: 2e74 6573 745f 7472 696d 5f70 6169 725f  .test_trim_pair_
+00000a90: 6e6f 5f62 622e 3c6c 6f63 616c 733e 2e3c  no_bb.<locals>.<
+00000aa0: 6c61 6d62 6461 3e63 0000 0000 0000 0000  lambda>c........
+00000ab0: 0000 0000 0000 0000 0800 0000 1300 0000  ................
+00000ac0: 731c 0000 0074 006a 0188 006a 0288 006a  s....t.j...j...j
+00000ad0: 0388 006a 0464 0164 0264 0364 048d 0653  ...j.d.d.d.d...S
+00000ae0: 0029 054e 5446 721c 0000 0072 1d00 0000  .).NTFr....r....
+00000af0: 7236 0000 0072 1700 0000 7237 0000 0072  r6...r....r7...r
+00000b00: 1700 0000 7218 0000 0072 3800 0000 7500  ....r....r8...u.
+00000b10: 0000 730c 0000 0008 0104 0104 0102 0102  ..s.............
+00000b20: 0102 fb29 0772 3200 0000 7223 0000 0072  ...).r2...r#...r
+00000b30: 2400 0000 7225 0000 0072 2600 0000 7204  $...r%...r&...r.
+00000b40: 0000 00da 0a56 616c 7565 4572 726f 7229  .....ValueError)
+00000b50: 0272 2d00 0000 722e 0000 0072 1700 0000  .r-...r....r....
+00000b60: 7237 0000 0072 1800 0000 da14 7465 7374  r7...r......test
+00000b70: 5f74 7269 6d5f 7061 6972 5f6e 6f5f 6262  _trim_pair_no_bb
+00000b80: 6c00 0000 7308 0000 0000 010e 0108 0112  l...s...........
+00000b90: 067a 2b53 6574 4661 7374 7173 416e 6443  .z+SetFastqsAndC
+00000ba0: 6865 636b 5465 7374 732e 7465 7374 5f74  heckTests.test_t
+00000bb0: 7269 6d5f 7061 6972 5f6e 6f5f 6262 4e29  rim_pair_no_bbN)
+00000bc0: 07da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000bd0: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000be0: 616d 655f 5f72 3100 0000 7234 0000 0072  ame__r1...r4...r
+00000bf0: 3500 0000 723a 0000 0072 1700 0000 7217  5...r:...r....r.
+00000c00: 0000 0072 1700 0000 7218 0000 0072 1a00  ...r....r....r..
+00000c10: 0000 4900 0000 7308 0000 0008 0108 0b08  ..I...s.........
+00000c20: 0b08 0c72 1a00 0000 6300 0000 0000 0000  ...r....c.......
+00000c30: 0000 0000 0007 0000 0007 0000 0043 0000  .............C..
+00000c40: 0073 4200 0000 6401 7d00 6402 7d01 6403  .sB...d.}.d.}.d.
+00000c50: 7d02 6401 7d03 7400 6a01 7402 7c00 7c01  }.d.}.t.j.t.|.|.
+00000c60: 7c02 7c03 6404 8d05 7d04 7403 7c04 8301  |.|.d...}.t.|...
+00000c70: 7d05 7403 7404 8301 7d06 7405 7c05 7c06  }.t.t...}.t.|.|.
+00000c80: 8302 0100 6400 5300 2905 4e72 1c00 0000  ....d.S.).Nr....
+00000c90: da01 46da 0449 5453 3229 05da 1470 6572  ..F..ITS2)...per
+00000ca0: 5f73 616d 706c 655f 7365 7175 656e 6365  _sample_sequence
+00000cb0: 7372 2000 0000 da04 7461 7861 da06 7265  sr .....taxa..re
+00000cc0: 6769 6f6e da0a 636c 7573 7465 725f 6964  gion..cluster_id
+00000cd0: 2906 7215 0000 00da 0b74 7269 6d5f 7369  ).r......trim_si
+00000ce0: 6e67 6c65 7222 0000 0072 0200 0000 da13  ngler"...r......
+00000cf0: 5445 5354 5f44 4154 415f 5349 4e47 4c45  TEST_DATA_SINGLE
+00000d00: 4f55 5472 0300 0000 2907 7220 0000 0072  OUTr....).r ...r
+00000d10: 4100 0000 7242 0000 0072 4300 0000 7216  A...rB...rC...r.
+00000d20: 0000 005a 0465 7870 325a 0465 7870 3372  ...Z.exp2Z.exp3r
+00000d30: 1700 0000 7217 0000 0072 1800 0000 da1b  ....r....r......
+00000d40: 7465 7374 5f74 7269 6d5f 7369 6e67 6c65  test_trim_single
+00000d50: 5f6e 6f5f 636c 7573 7465 727d 0000 0073  _no_cluster}...s
+00000d60: 1a00 0000 0001 0401 0401 0401 0402 0601  ................
+00000d70: 0201 0201 0201 02fc 0605 0801 0801 7246  ..............rF
+00000d80: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000d90: 0000 0000 0500 0000 0300 0000 7326 0000  ............s&..
+00000da0: 0064 0189 0264 0289 0164 0389 0074 0074  .d...d...d...t.t
+00000db0: 0187 0087 0187 0266 0364 0464 0584 0883  .......f.d.d....
+00000dc0: 0201 0064 0053 0029 064e 721c 0000 0072  ...d.S.).Nr....r
+00000dd0: 3e00 0000 723f 0000 0063 0000 0000 0000  >...r?...c......
+00000de0: 0000 0000 0000 0000 0000 0600 0000 1300  ................
+00000df0: 0000 7312 0000 0074 006a 0174 0288 0288  ..s....t.j.t....
+00000e00: 0188 0064 018d 0453 0029 024e 2904 7240  ...d...S.).N).r@
+00000e10: 0000 0072 2000 0000 7241 0000 0072 4200  ...r ...rA...rB.
+00000e20: 0000 2903 7215 0000 00da 0974 7269 6d5f  ..).r......trim_
+00000e30: 7061 6972 7232 0000 0072 1700 0000 a903  pairr2...r......
+00000e40: 7242 0000 0072 4100 0000 7220 0000 0072  rB...rA...r ...r
+00000e50: 1700 0000 7218 0000 0072 3800 0000 9200  ....r....r8.....
+00000e60: 0000 7308 0000 0006 0102 0102 0102 fd7a  ..s............z
+00000e70: 2974 6573 745f 7472 696d 5f70 6169 725f  )test_trim_pair_
+00000e80: 6e6f 5f68 6d6d 6572 2e3c 6c6f 6361 6c73  no_hmmer.<locals
+00000e90: 3e2e 3c6c 616d 6264 613e 2902 7204 0000  >.<lambda>).r...
+00000ea0: 0072 3900 0000 7217 0000 0072 1700 0000  .r9...r....r....
+00000eb0: 7248 0000 0072 1800 0000 da17 7465 7374  rH...r......test
+00000ec0: 5f74 7269 6d5f 7061 6972 5f6e 6f5f 686d  _trim_pair_no_hm
+00000ed0: 6d65 728d 0000 0073 0800 0000 0001 0401  mer....s........
+00000ee0: 0401 0402 7249 0000 0063 0000 0000 0000  ....rI...c......
+00000ef0: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00000f00: 0000 732c 0000 0065 005a 0164 005a 0264  ..s,...e.Z.d.Z.d
+00000f10: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
+00000f20: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
+00000f30: 0953 0029 0ada 0954 7269 6d54 6573 7473  .S.)...TrimTests
+00000f40: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000f50: 0005 0000 0043 0000 0073 6400 0000 7400  .....C...sd...t.
+00000f60: 6a01 a002 a100 6a03 6401 1900 7c00 5f04  j.....j.d...|._.
+00000f70: 7c00 6a04 6a05 6402 1900 7c00 5f06 7c00  |.j.j.d...|._.|.
+00000f80: 6a04 6a05 6403 1900 7c00 5f07 7c00 6a04  j.j.d...|._.|.j.
+00000f90: 6a05 6404 1900 7c00 5f08 7400 6a09 a00a  j.d...|._.t.j...
+00000fa0: 6405 740b 6406 a103 7c00 5f0c 7400 6a09  d.t.d...|._.t.j.
+00000fb0: a00a 6407 740d 6408 a103 7c00 5f0e 6400  ..d.t.d...|._.d.
+00000fc0: 5300 2909 4eda 0c71 325f 6974 7378 7072  S.).N..q2_itsxpr
+00000fd0: 6573 7372 4400 0000 7247 0000 005a 1974  essrD...rG...Z.t
+00000fe0: 7269 6d5f 7061 6972 5f6f 7574 7075 745f  rim_pair_output_
+00000ff0: 756e 6d65 7267 6564 7213 0000 0072 0500  unmergedr....r..
+00001000: 0000 7212 0000 0072 0600 0000 290f da06  ..r....r....)...
+00001010: 7169 696d 6532 5a03 7364 6bda 0d50 6c75  qiime2Z.sdk..Plu
+00001020: 6769 6e4d 616e 6167 6572 da07 706c 7567  ginManager..plug
+00001030: 696e 73da 0670 6c75 6769 6eda 076d 6574  ins..plugin..met
+00001040: 686f 6473 da0e 7472 696d 5f73 696e 676c  hods..trim_singl
+00001050: 655f 666e da0e 7472 696d 5f70 6169 7265  e_fn..trim_paire
+00001060: 645f 666e da17 7472 696d 5f70 6169 7265  d_fn..trim_paire
+00001070: 645f 756e 6d65 7267 6564 5f66 6e5a 0841  d_unmerged_fnZ.A
+00001080: 7274 6966 6163 745a 0b69 6d70 6f72 745f  rtifactZ.import_
+00001090: 6461 7461 da12 5445 5354 5f46 494c 455f  data..TEST_FILE_
+000010a0: 5349 4e47 4c45 494e da07 7365 5f73 6571  SINGLEIN..se_seq
+000010b0: 73da 0954 4553 545f 4649 4c45 da07 7065  s..TEST_FILE..pe
+000010c0: 5f73 6571 7329 0172 2d00 0000 7217 0000  _seqs).r-...r...
+000010d0: 0072 1700 0000 7218 0000 00da 0573 6574  .r....r......set
+000010e0: 5570 9800 0000 731e 0000 0000 0112 010e  Up....s.........
+000010f0: 010e 020a ff04 0306 0102 0102 0102 fd06  ................
+00001100: 0406 0102 0102 0102 fd7a 0f54 7269 6d54  .........z.TrimT
+00001110: 6573 7473 2e73 6574 5570 6301 0000 0000  ests.setUpc.....
+00001120: 0000 0000 0000 0006 0000 0009 0000 0043  ...............C
+00001130: 0000 0073 8e00 0000 7400 7401 6a02 6401  ...s....t.t.j.d.
+00001140: 8d01 8f16 0100 7c00 a003 7c00 6a04 6402  ......|...|.j.d.
+00001150: a102 5c01 7d01 5700 3500 5100 5200 5800  ..\.}.W.5.Q.R.X.
+00001160: 7c00 a005 7406 7c01 6a07 8301 6403 a102  |...t.|.j...d...
+00001170: 0100 7c01 a008 7409 a101 7d02 7c00 a005  ..|...t...}.|...
+00001180: 740a 7c02 8301 740a 740b 8301 a102 0100  t.|...t.t.......
+00001190: 7c01 a008 7409 a101 7d03 740c 7c03 6a0d  |...t...}.t.|.j.
+000011a0: a008 740e a101 a00f a100 8301 7d04 6404  ..t.........}.d.
+000011b0: 6405 6702 7d05 7c00 a005 7c04 7c05 a102  d.g.}.|...|.|...
+000011c0: 0100 6400 5300 2906 4ea9 01da 0673 7464  ..d.S.).N....std
+000011d0: 6572 7272 3f00 0000 7213 0000 00fa 1d73  errr?...r......s
+000011e0: 616d 706c 652d 6964 2c66 696c 656e 616d  ample-id,filenam
+000011f0: 652c 6469 7265 6374 696f 6e0a fa3b 3437  e,direction..;47
+00001200: 3734 2d31 2d4d 5349 5453 332c 3437 3734  74-1-MSITS3,4774
+00001210: 2d31 2d4d 5349 5453 335f 305f 4c30 3031  -1-MSITS3_0_L001
+00001220: 5f52 315f 3030 312e 6661 7374 712e 677a  _R1_001.fastq.gz
+00001230: 2c66 6f72 7761 7264 0a29 1072 0800 0000  ,forward.).r....
+00001240: da02 6f73 da07 6465 766e 756c 6c72 5100  ..os..devnullrQ.
+00001250: 0000 7255 0000 00da 0b61 7373 6572 7445  ..rU.....assertE
+00001260: 7175 616c da03 7374 72da 0474 7970 6572  qual..str..typer
+00001270: 2400 0000 7205 0000 0072 0200 0000 7245  $...r....r....rE
+00001280: 0000 00da 046c 6973 7472 2300 0000 7207  .....listr#...r.
+00001290: 0000 00da 046f 7065 6ea9 0672 2d00 0000  .....open..r-...
+000012a0: da0c 6f62 735f 6172 7469 6661 6374 5a07  ..obs_artifactZ.
+000012b0: 6f62 735f 6469 7272 3000 0000 da0c 6f62  obs_dirr0.....ob
+000012c0: 735f 6d61 6e69 6665 7374 da0c 6578 705f  s_manifest..exp_
+000012d0: 6d61 6e69 6665 7374 7217 0000 0072 1700  manifestr....r..
+000012e0: 0000 7218 0000 00da 1874 6573 745f 7472  ..r......test_tr
+000012f0: 696d 5f73 696e 676c 655f 7375 6363 6573  im_single_succes
+00001300: 73a8 0000 0073 1a00 0000 0001 0e01 1a01  s....s..........
+00001310: 0c01 02ff 0403 0a01 1402 0a01 1402 0201  ................
+00001320: 02fe 0403 7a22 5472 696d 5465 7374 732e  ....z"TrimTests.
+00001330: 7465 7374 5f74 7269 6d5f 7369 6e67 6c65  test_trim_single
+00001340: 5f73 7563 6365 7373 6301 0000 0000 0000  _successc.......
+00001350: 0000 0000 0006 0000 0009 0000 0043 0000  .............C..
+00001360: 0073 8e00 0000 7400 7401 6a02 6401 8d01  .s....t.t.j.d...
+00001370: 8f16 0100 7c00 a003 7c00 6a04 6402 a102  ....|...|.j.d...
+00001380: 5c01 7d01 5700 3500 5100 5200 5800 7c00  \.}.W.5.Q.R.X.|.
+00001390: a005 7406 7c01 6a07 8301 6403 a102 0100  ..t.|.j...d.....
+000013a0: 7c01 a008 7409 a101 7d02 7c00 a005 740a  |...t...}.|...t.
+000013b0: 7c02 8301 740a 740b 8301 a102 0100 7c01  |...t.t.......|.
+000013c0: a008 7409 a101 7d03 740c 7c03 6a0d a008  ..t...}.t.|.j...
+000013d0: 740e a101 a00f a100 8301 7d04 6404 6405  t.........}.d.d.
+000013e0: 6702 7d05 7c00 a005 7c04 7c05 a102 0100  g.}.|...|.|.....
+000013f0: 6400 5300 2906 4e72 5900 0000 723f 0000  d.S.).NrY...r?..
+00001400: 007a 2653 616d 706c 6544 6174 615b 4a6f  .z&SampleData[Jo
+00001410: 696e 6564 5365 7175 656e 6365 7357 6974  inedSequencesWit
+00001420: 6851 7561 6c69 7479 5d72 5b00 0000 725c  hQuality]r[...r\
+00001430: 0000 0029 1072 0800 0000 725d 0000 0072  ...).r....r]...r
+00001440: 5e00 0000 7252 0000 0072 5700 0000 725f  ^...rR...rW...r_
+00001450: 0000 0072 6000 0000 7261 0000 0072 2400  ...r`...ra...r$.
+00001460: 0000 7205 0000 0072 0200 0000 da0d 5445  ..r....r......TE
+00001470: 5354 5f44 4154 415f 4f55 5472 6200 0000  ST_DATA_OUTrb...
+00001480: 7223 0000 0072 0700 0000 7263 0000 0072  r#...r....rc...r
+00001490: 6400 0000 7217 0000 0072 1700 0000 7218  d...r....r....r.
+000014a0: 0000 00da 1674 6573 745f 7472 696d 5f70  .....test_trim_p
+000014b0: 6169 725f 7375 6363 6573 73b8 0000 0073  air_success....s
+000014c0: 1a00 0000 0001 0e01 1a01 0c01 02ff 0403  ................
+000014d0: 0a01 1402 0a01 1402 0201 02fe 0403 7a20  ..............z 
+000014e0: 5472 696d 5465 7374 732e 7465 7374 5f74  TrimTests.test_t
+000014f0: 7269 6d5f 7061 6972 5f73 7563 6365 7373  rim_pair_success
+00001500: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
+00001510: 0009 0000 0043 0000 0073 7200 0000 7400  .....C...sr...t.
+00001520: 7401 6a02 6401 8d01 8f16 0100 7c00 a003  t.j.d.......|...
+00001530: 7c00 6a04 6402 a102 5c01 7d01 5700 3500  |.j.d...\.}.W.5.
+00001540: 5100 5200 5800 7c00 a005 7406 7c01 6a07  Q.R.X.|...t.|.j.
+00001550: 8301 6403 a102 0100 7c01 a008 7409 a101  ..d.....|...t...
+00001560: 7d02 740a 7c02 6a0b a008 740c a101 a00d  }.t.|.j...t.....
+00001570: a100 8301 7d03 6404 6405 6406 6703 7d04  ....}.d.d.d.g.}.
+00001580: 7c00 a005 7c03 7c04 a102 0100 6400 5300  |...|.|.....d.S.
+00001590: 2907 4e72 5900 0000 723f 0000 0072 1200  ).NrY...r?...r..
+000015a0: 0000 725b 0000 0072 5c00 0000 7a3b 3437  ..r[...r\...z;47
+000015b0: 3734 2d31 2d4d 5349 5453 332c 3437 3734  74-1-MSITS3,4774
+000015c0: 2d31 2d4d 5349 5453 335f 315f 4c30 3031  -1-MSITS3_1_L001
+000015d0: 5f52 325f 3030 312e 6661 7374 712e 677a  _R2_001.fastq.gz
+000015e0: 2c72 6576 6572 7365 0a29 0e72 0800 0000  ,reverse.).r....
+000015f0: 725d 0000 0072 5e00 0000 7253 0000 0072  r]...r^...rS...r
+00001600: 5700 0000 725f 0000 0072 6000 0000 7261  W...r_...r`...ra
+00001610: 0000 0072 2400 0000 7206 0000 0072 6200  ...r$...r....rb.
+00001620: 0000 7223 0000 0072 0700 0000 7263 0000  ..r#...r....rc..
+00001630: 0029 0572 2d00 0000 7265 0000 0072 3000  .).r-...re...r0.
+00001640: 0000 7266 0000 0072 6700 0000 7217 0000  ..rf...rg...r...
+00001650: 0072 1700 0000 7218 0000 00da 2674 6573  .r....r.....&tes
+00001660: 745f 7472 696d 5f70 6169 725f 6f75 7470  t_trim_pair_outp
+00001670: 7574 5f75 6e6d 6572 6765 645f 7375 6363  ut_unmerged_succ
+00001680: 6573 73c8 0000 0073 1800 0000 0001 0e01  ess....s........
+00001690: 1a01 0c01 02ff 0402 0a01 1402 0201 0201  ................
+000016a0: 02fd 0404 7a30 5472 696d 5465 7374 732e  ....z0TrimTests.
+000016b0: 7465 7374 5f74 7269 6d5f 7061 6972 5f6f  test_trim_pair_o
+000016c0: 7574 7075 745f 756e 6d65 7267 6564 5f73  utput_unmerged_s
+000016d0: 7563 6365 7373 4e29 0772 3b00 0000 723c  uccessN).r;...r<
+000016e0: 0000 0072 3d00 0000 7258 0000 0072 6800  ...r=...rX...rh.
+000016f0: 0000 726a 0000 0072 6b00 0000 7217 0000  ..rj...rk...r...
+00001700: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00001710: 724a 0000 0097 0000 0073 0800 0000 0801  rJ.......s......
+00001720: 0810 0810 0810 724a 0000 0029 32da 0862  ......rJ...)2..b
+00001730: 7569 6c74 696e 73da 0c40 7079 5f62 7569  uiltins..@py_bui
+00001740: 6c74 696e 73da 195f 7079 7465 7374 2e61  ltins.._pytest.a
+00001750: 7373 6572 7469 6f6e 2e72 6577 7269 7465  ssertion.rewrite
+00001760: da09 6173 7365 7274 696f 6eda 0772 6577  ..assertion..rew
+00001770: 7269 7465 da0a 4070 7974 6573 745f 6172  rite..@pytest_ar
+00001780: 725d 0000 00da 0875 6e69 7474 6573 74da  r].....unittest.
+00001790: 0373 7973 7202 0000 005a 0a6e 6f73 652e  .sysr....Z.nose.
+000017a0: 746f 6f6c 7372 0300 0000 7204 0000 005a  toolsr....r....Z
+000017b0: 1d71 325f 7479 7065 732e 7065 725f 7361  .q2_types.per_sa
+000017c0: 6d70 6c65 5f73 6571 7565 6e63 6573 7205  mple_sequencesr.
+000017d0: 0000 0072 0600 0000 7207 0000 005a 1771  ...r....r....Z.q
+000017e0: 325f 6974 7378 7072 6573 732e 5f69 7473  2_itsxpress._its
+000017f0: 7870 7265 7373 7215 0000 0072 4c00 0000  xpressr....rL...
+00001800: 5a0b 7169 696d 6532 2e75 7469 6c72 0800  Z.qiime2.utilr..
+00001810: 0000 5a06 7061 6e64 6173 7225 0000 00da  ..Z.pandasr%....
+00001820: 0470 6174 68da 0764 6972 6e61 6d65 da07  .path..dirname..
+00001830: 6162 7370 6174 68da 085f 5f66 696c 655f  abspath..__file_
+00001840: 5f5a 0854 4553 545f 4449 52da 046a 6f69  _Z.TEST_DIR..joi
+00001850: 6e72 5600 0000 7232 0000 005a 0e54 4553  nrV...r2...Z.TES
+00001860: 545f 4649 4c45 5f50 424d 445a 0e54 4553  T_FILE_PBMDZ.TES
+00001870: 545f 4441 5441 5f50 424d 445a 0d54 4553  T_DATA_PBMDZ.TES
+00001880: 545f 4649 4c45 5f50 4146 5a0d 5445 5354  T_FILE_PAFZ.TEST
+00001890: 5f44 4154 415f 5041 465a 0d54 4553 545f  _DATA_PAFZ.TEST_
+000018a0: 4649 4c45 5f4f 5554 7269 0000 005a 1354  FILE_OUTri...Z.T
+000018b0: 4553 545f 4649 4c45 5f53 494e 474c 454f  EST_FILE_SINGLEO
+000018c0: 5554 7245 0000 0072 5400 0000 7222 0000  UTrE...rT...r"..
+000018d0: 005a 0f41 5254 4946 4143 545f 5459 5045  .Z.ARTIFACT_TYPE
+000018e0: 5f50 5a0f 4152 5449 4641 4354 5f54 5950  _PZ.ARTIFACT_TYP
+000018f0: 455f 5372 1900 0000 da08 5465 7374 4361  E_Sr......TestCa
+00001900: 7365 721a 0000 0072 4600 0000 7249 0000  ser....rF...rI..
+00001910: 0072 4a00 0000 7217 0000 0072 1700 0000  .rJ...r....r....
+00001920: 7217 0000 0072 1800 0000 da08 3c6d 6f64  r....r......<mod
+00001930: 756c 653e 0100 0000 7378 0000 0008 0012  ule>....sx......
+00001940: 0008 0108 010c 0210 0114 040c 0208 010c  ................
+00001950: 0108 0314 0208 0102 0102 0102 0102 fc04  ................
+00001960: 060a 0208 0102 0102 0102 0102 fc04 060a  ................
+00001970: 0208 0102 0102 0102 0102 fc04 050a 0208  ................
+00001980: 0102 0102 0102 0102 fc04 050a 0208 0102  ................
+00001990: 0102 0102 0102 fc04 050a 0208 0102 0102  ................
+000019a0: 0102 0102 fc04 050a 0204 0204 0308 0512  ................
+000019b0: 3408 1008 0a                             4....
```

### Comparing `q2_itsxpress-1.8.0/tests/test_main.py` & `q2_itsxpress-1.8.1/tests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,27 +133,28 @@
                                 taxa=taxa,
                                 region=region,
                                 cluster_id=cluster_id)
     exp2 = getsizeof(exp1)
     exp3 = getsizeof(TEST_DATA_SINGLEOUT)
     eq_(exp2, exp3)
 
+
 def test_trim_pair_no_hmmer():
     threads = 1
     taxa = "F"
     region = "ITS2"
 
     raises(ValueError, lambda: _itsxpress.trim_pair(per_sample_sequences=TEST_DATA,
                                                     threads=threads,
                                                     taxa=taxa,
                                                     region=region))
 
 class TrimTests(unittest.TestCase):
     def setUp(self):
-        self.plugin = qiime2.sdk.PluginManager().plugins['itsxpress']
+        self.plugin = qiime2.sdk.PluginManager().plugins['q2_itsxpress']
         self.trim_single_fn = self.plugin.methods['trim_single']
         self.trim_paired_fn = self.plugin.methods['trim_pair']
         self.trim_paired_unmerged_fn = \
             self.plugin.methods['trim_pair_output_unmerged']
 
         self.se_seqs = qiime2.Artifact.import_data(
             'SampleData[SequencesWithQuality]',
```

### Comparing `q2_itsxpress-1.8.0/q2_itsxpress.egg-info/SOURCES.txt` & `q2_itsxpress-1.8.1/q2_itsxpress.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+LICENSE.txt
 MANIFEST.in
 README.rst
-setup.py
+pyproject.toml
 q2_itsxpress/__init__.py
 q2_itsxpress/_itsxpress.py
 q2_itsxpress/citations.bib
 q2_itsxpress/plugin_setup.py
 q2_itsxpress.egg-info/PKG-INFO
 q2_itsxpress.egg-info/SOURCES.txt
 q2_itsxpress.egg-info/dependency_links.txt
 q2_itsxpress.egg-info/entry_points.txt
-q2_itsxpress.egg-info/not-zip-safe
 q2_itsxpress.egg-info/requires.txt
 q2_itsxpress.egg-info/top_level.txt
 tests/test_main.py
-tests/__pycache__/test_main.cpython-35.pyc
-tests/__pycache__/test_main.cpython-36.pyc
+tests/__pycache__/test_main.cpython-38-pytest-7.1.3.pyc
 tests/test_data/paired.qza
 tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/VERSION
 tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/metadata.yaml
 tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_0_L001_R1_001.fastq.gz
 tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/4774-1-MSITS3_1_L001_R2_001.fastq.gz
 tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/MANIFEST
 tests/test_data/out/d9955749-00d5-44ae-a628-4b2da43000e1/data/metadata.yml
```

