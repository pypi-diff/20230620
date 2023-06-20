# Comparing `tmp/shorttext-1.5.8.tar.gz` & `tmp/shorttext-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/shorttext-1.5.8.tar", last modified: Fri Sep 23 04:19:46 2022, max compression
+gzip compressed data, was "dist/shorttext-1.5.9.tar", last modified: Tue Jun 20 03:26:59 2023, max compression
```

## Comparing `shorttext-1.5.8.tar` & `shorttext-1.5.9.tar`

### file list

```diff
@@ -1,118 +1,117 @@
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.670027 shorttext-1.5.8/
--rw-r--r--   0 stephenhky   (501) staff       (20)     1055 2020-08-16 04:30:18.000000 shorttext-1.5.8/LICENSE
--rw-r--r--   0 stephenhky   (501) staff       (20)      429 2022-09-23 04:19:36.000000 shorttext-1.5.8/MANIFEST.in
--rw-r--r--   0 stephenhky   (501) staff       (20)    10149 2022-09-23 04:19:46.670298 shorttext-1.5.8/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)     8958 2022-09-23 04:19:36.000000 shorttext-1.5.8/README.md
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.581105 shorttext-1.5.8/bin/
--rw-r--r--   0 stephenhky   (501) staff       (20)     4151 2021-12-30 18:22:16.000000 shorttext-1.5.8/bin/ShortTextCategorizerConsole
--rw-r--r--   0 stephenhky   (501) staff       (20)     2021 2021-12-30 18:22:16.000000 shorttext-1.5.8/bin/ShortTextWordEmbedSimilarity
--rw-r--r--   0 stephenhky   (501) staff       (20)     3331 2020-08-16 04:30:18.000000 shorttext-1.5.8/bin/WordEmbedAPI
--rw-r--r--   0 stephenhky   (501) staff       (20)       83 2022-09-22 14:30:44.000000 shorttext-1.5.8/pyproject.toml
--rw-r--r--   0 stephenhky   (501) staff       (20)      245 2022-09-22 14:30:44.000000 shorttext-1.5.8/requirements.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)      157 2022-09-23 04:19:46.671352 shorttext-1.5.8/setup.cfg
--rw-r--r--   0 stephenhky   (501) staff       (20)     3594 2022-09-23 04:19:36.000000 shorttext-1.5.8/setup.py
--rw-r--r--   0 stephenhky   (501) staff       (20)       42 2022-09-22 14:30:44.000000 shorttext-1.5.8/setup_requirements.txt
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.582795 shorttext-1.5.8/shorttext/
--rw-r--r--   0 stephenhky   (501) staff       (20)      200 2022-09-22 14:30:44.000000 shorttext-1.5.8/shorttext/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.587477 shorttext-1.5.8/shorttext/classifiers/
--rw-r--r--   0 stephenhky   (501) staff       (20)     1061 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.588324 shorttext-1.5.8/shorttext/classifiers/bow/
--rw-r--r--   0 stephenhky   (501) staff       (20)       40 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/bow/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.590202 shorttext-1.5.8/shorttext/classifiers/bow/maxent/
--rw-r--r--   0 stephenhky   (501) staff       (20)     9969 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/classifiers/bow/maxent/MaxEntClassification.py
--rw-r--r--   0 stephenhky   (501) staff       (20)       34 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/bow/maxent/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.593083 shorttext-1.5.8/shorttext/classifiers/bow/topic/
--rw-r--r--   0 stephenhky   (501) staff       (20)    17751 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/bow/topic/SkLearnClassification.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     9086 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/bow/topic/TopicVectorDistanceClassification.py
--rw-r--r--   0 stephenhky   (501) staff       (20)       84 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/bow/topic/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.593920 shorttext-1.5.8/shorttext/classifiers/embed/
--rw-r--r--   0 stephenhky   (501) staff       (20)      572 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/embed/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.596752 shorttext-1.5.8/shorttext/classifiers/embed/nnlib/
--rw-r--r--   0 stephenhky   (501) staff       (20)    11720 2022-08-30 03:03:26.000000 shorttext-1.5.8/shorttext/classifiers/embed/nnlib/VarNNEmbedVecClassification.py
--rw-r--r--   0 stephenhky   (501) staff       (20)       66 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/embed/nnlib/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     9667 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/classifiers/embed/nnlib/frameworks.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.602821 shorttext-1.5.8/shorttext/classifiers/embed/sumvec/
--rw-r--r--   0 stephenhky   (501) staff       (20)     6626 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/classifiers/embed/sumvec/SumEmbedVecClassification.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     9553 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/embed/sumvec/VarNNSumEmbedVecClassification.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      109 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/embed/sumvec/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2372 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/classifiers/embed/sumvec/frameworks.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.605383 shorttext-1.5.8/shorttext/data/
--rw-r--r--   0 stephenhky   (501) staff       (20)      155 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/data/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     8304 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/data/data_retrieval.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1184 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/data/shorttext_exampledata.csv
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.606095 shorttext-1.5.8/shorttext/generators/
--rw-r--r--   0 stephenhky   (501) staff       (20)      556 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/generators/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.609815 shorttext-1.5.8/shorttext/generators/bow/
--rw-r--r--   0 stephenhky   (501) staff       (20)     9515 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/generators/bow/AutoEncodingTopicModeling.py
--rw-r--r--   0 stephenhky   (501) staff       (20)    13618 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/generators/bow/GensimTopicModeling.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     5182 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/generators/bow/LatentTopicModeling.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      109 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/generators/bow/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.612271 shorttext-1.5.8/shorttext/generators/charbase/
--rw-r--r--   0 stephenhky   (501) staff       (20)       25 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/generators/charbase/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     4191 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/generators/charbase/char2vec.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.614782 shorttext-1.5.8/shorttext/generators/seq2seq/
--rw-r--r--   0 stephenhky   (501) staff       (20)       50 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/generators/seq2seq/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     8153 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/generators/seq2seq/charbaseS2S.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     8182 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/generators/seq2seq/s2skeras.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.615654 shorttext-1.5.8/shorttext/metrics/
--rw-r--r--   0 stephenhky   (501) staff       (20)      101 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/metrics/__init__.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.627513 shorttext-1.5.8/shorttext/metrics/dynprog/
--rw-r--r--   0 stephenhky   (501) staff       (20)      182 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/metrics/dynprog/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)   872412 2022-09-22 14:30:44.000000 shorttext-1.5.8/shorttext/metrics/dynprog/dldist.c
--rw-r--r--   0 stephenhky   (501) staff       (20)      955 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/metrics/dynprog/dldist.pyx
--rw-r--r--   0 stephenhky   (501) staff       (20)     3026 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/metrics/dynprog/jaccard.py
--rw-r--r--   0 stephenhky   (501) staff       (20)   225352 2022-09-22 14:30:44.000000 shorttext-1.5.8/shorttext/metrics/dynprog/lcp.c
--rw-r--r--   0 stephenhky   (501) staff       (20)      330 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/metrics/dynprog/lcp.pyx
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.629168 shorttext-1.5.8/shorttext/metrics/embedfuzzy/
--rw-r--r--   0 stephenhky   (501) staff       (20)       40 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/metrics/embedfuzzy/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1636 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/metrics/embedfuzzy/jaccard.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.631689 shorttext-1.5.8/shorttext/metrics/transformers/
--rw-r--r--   0 stephenhky   (501) staff       (20)       35 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/metrics/transformers/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     4690 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/metrics/transformers/bertscore.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.634257 shorttext-1.5.8/shorttext/metrics/wasserstein/
--rwxr-xr-x   0 stephenhky   (501) staff       (20)       76 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/metrics/wasserstein/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     4327 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/metrics/wasserstein/wordmoverdist.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3191 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/smartload.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.641160 shorttext-1.5.8/shorttext/spell/
--rw-r--r--   0 stephenhky   (501) staff       (20)      159 2022-09-22 03:31:05.000000 shorttext-1.5.8/shorttext/spell/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      752 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/spell/basespellcorrector.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     8334 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/spell/binarize.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      648 2022-09-22 14:30:44.000000 shorttext-1.5.8/shorttext/spell/editor.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     2030 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/spell/norvig.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     8630 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/spell/sakaguchi.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.643713 shorttext-1.5.8/shorttext/stack/
--rw-r--r--   0 stephenhky   (501) staff       (20)       74 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/stack/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)    11750 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/stack/stacking.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.660193 shorttext-1.5.8/shorttext/utils/
--rw-r--r--   0 stephenhky   (501) staff       (20)      694 2022-08-26 21:53:09.000000 shorttext-1.5.8/shorttext/utils/__init__.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1051 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/utils/classification_exceptions.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     8905 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/utils/compactmodel_io.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      526 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/utils/deprecation.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     8040 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/utils/dtm.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     3506 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/utils/gensim_corpora.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1086 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/utils/kerasmodel_io.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1165 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/utils/misc.py
--rw-r--r--   0 stephenhky   (501) staff       (20)    18405 2022-08-26 21:53:09.000000 shorttext-1.5.8/shorttext/utils/nonneg_stopwords.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)    18416 2020-08-16 04:30:18.000000 shorttext-1.5.8/shorttext/utils/stopwords.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)     4201 2022-08-26 21:53:09.000000 shorttext-1.5.8/shorttext/utils/textpreprocessing.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     6012 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/utils/transformers.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     6906 2021-12-30 18:22:16.000000 shorttext-1.5.8/shorttext/utils/wordembed.py
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.587045 shorttext-1.5.8/shorttext.egg-info/
--rw-r--r--   0 stephenhky   (501) staff       (20)    10149 2022-09-23 04:19:46.000000 shorttext-1.5.8/shorttext.egg-info/PKG-INFO
--rw-r--r--   0 stephenhky   (501) staff       (20)     3165 2022-09-23 04:19:46.000000 shorttext-1.5.8/shorttext.egg-info/SOURCES.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2022-09-23 04:19:46.000000 shorttext-1.5.8/shorttext.egg-info/dependency_links.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-09-02 22:21:18.000000 shorttext-1.5.8/shorttext.egg-info/not-zip-safe
--rw-r--r--   0 stephenhky   (501) staff       (20)      245 2022-09-23 04:19:46.000000 shorttext-1.5.8/shorttext.egg-info/requires.txt
--rw-r--r--   0 stephenhky   (501) staff       (20)       10 2022-09-23 04:19:46.000000 shorttext-1.5.8/shorttext.egg-info/top_level.txt
-drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2022-09-23 04:19:46.669275 shorttext-1.5.8/test/
--rw-r--r--   0 stephenhky   (501) staff       (20)     1705 2021-12-30 18:22:16.000000 shorttext-1.5.8/test/test_bertrepresentations.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      599 2021-12-30 18:22:16.000000 shorttext-1.5.8/test/test_charonehot.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1620 2020-08-16 04:30:18.000000 shorttext-1.5.8/test/test_dtm.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1679 2020-08-16 04:30:18.000000 shorttext-1.5.8/test/test_fuzzylogic.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      577 2020-08-16 04:30:18.000000 shorttext-1.5.8/test/test_norvigspell.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1478 2021-04-09 15:34:12.000000 shorttext-1.5.8/test/test_sakaguchispell.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     5822 2020-08-16 04:30:18.000000 shorttext-1.5.8/test/test_stacking.py
--rw-r--r--   0 stephenhky   (501) staff       (20)      965 2022-08-26 21:53:09.000000 shorttext-1.5.8/test/test_textpreprocessing.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     4578 2021-12-30 18:31:29.000000 shorttext-1.5.8/test/test_var_nn_embedded_vec_classifier.py
--rw-r--r--   0 stephenhky   (501) staff       (20)     1401 2021-12-30 18:22:16.000000 shorttext-1.5.8/test/test_wmd.py
--rw-r--r--   0 stephenhky   (501) staff       (20)       29 2021-12-30 18:22:16.000000 shorttext-1.5.8/test_requirements.txt
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.708875 shorttext-1.5.9/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1055 2020-08-16 04:30:18.000000 shorttext-1.5.9/LICENSE
+-rw-r--r--   0 stephenhky   (501) staff       (20)      429 2022-10-29 20:54:47.000000 shorttext-1.5.9/MANIFEST.in
+-rw-r--r--   0 stephenhky   (501) staff       (20)    10199 2023-06-20 03:26:59.709273 shorttext-1.5.9/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)     9000 2023-06-20 03:25:26.000000 shorttext-1.5.9/README.md
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.631157 shorttext-1.5.9/bin/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4151 2023-02-25 20:12:30.000000 shorttext-1.5.9/bin/ShortTextCategorizerConsole
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2021 2023-02-25 20:12:30.000000 shorttext-1.5.9/bin/ShortTextWordEmbedSimilarity
+-rw-r--r--   0 stephenhky   (501) staff       (20)       83 2022-10-29 20:54:47.000000 shorttext-1.5.9/pyproject.toml
+-rw-r--r--   0 stephenhky   (501) staff       (20)      245 2023-06-20 03:24:43.000000 shorttext-1.5.9/requirements.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)      157 2023-06-20 03:26:59.710482 shorttext-1.5.9/setup.cfg
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3559 2023-06-20 03:26:57.000000 shorttext-1.5.9/setup.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)       42 2022-10-29 20:54:47.000000 shorttext-1.5.9/setup_requirements.txt
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.632466 shorttext-1.5.9/shorttext/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      200 2022-10-29 20:54:47.000000 shorttext-1.5.9/shorttext/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.639935 shorttext-1.5.9/shorttext/classifiers/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1061 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.640682 shorttext-1.5.9/shorttext/classifiers/bow/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       40 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/bow/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.641935 shorttext-1.5.9/shorttext/classifiers/bow/maxent/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     9969 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/classifiers/bow/maxent/MaxEntClassification.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)       34 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/bow/maxent/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.643579 shorttext-1.5.9/shorttext/classifiers/bow/topic/
+-rw-r--r--   0 stephenhky   (501) staff       (20)    17751 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/bow/topic/SkLearnClassification.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     9086 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/bow/topic/TopicVectorDistanceClassification.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)       84 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/bow/topic/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.644071 shorttext-1.5.9/shorttext/classifiers/embed/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      572 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/embed/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.646924 shorttext-1.5.9/shorttext/classifiers/embed/nnlib/
+-rw-r--r--   0 stephenhky   (501) staff       (20)    11720 2022-10-29 20:54:47.000000 shorttext-1.5.9/shorttext/classifiers/embed/nnlib/VarNNEmbedVecClassification.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)       66 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/embed/nnlib/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     9667 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/classifiers/embed/nnlib/frameworks.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.650741 shorttext-1.5.9/shorttext/classifiers/embed/sumvec/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     6626 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/classifiers/embed/sumvec/SumEmbedVecClassification.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     9553 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/embed/sumvec/VarNNSumEmbedVecClassification.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      109 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/embed/sumvec/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2372 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/classifiers/embed/sumvec/frameworks.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.655775 shorttext-1.5.9/shorttext/data/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      155 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/data/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8304 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/data/data_retrieval.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1184 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/data/shorttext_exampledata.csv
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.657176 shorttext-1.5.9/shorttext/generators/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      556 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/generators/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.660971 shorttext-1.5.9/shorttext/generators/bow/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     9515 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/generators/bow/AutoEncodingTopicModeling.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)    13618 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/generators/bow/GensimTopicModeling.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     5182 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/generators/bow/LatentTopicModeling.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      109 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/generators/bow/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.662349 shorttext-1.5.9/shorttext/generators/charbase/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       25 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/generators/charbase/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4191 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/generators/charbase/char2vec.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.664587 shorttext-1.5.9/shorttext/generators/seq2seq/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       50 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/generators/seq2seq/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8153 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/generators/seq2seq/charbaseS2S.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8182 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/generators/seq2seq/s2skeras.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.665345 shorttext-1.5.9/shorttext/metrics/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      101 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/metrics/__init__.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.672667 shorttext-1.5.9/shorttext/metrics/dynprog/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      182 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/metrics/dynprog/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)   854046 2023-06-20 03:26:44.000000 shorttext-1.5.9/shorttext/metrics/dynprog/dldist.c
+-rw-r--r--   0 stephenhky   (501) staff       (20)      955 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/metrics/dynprog/dldist.pyx
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3026 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/metrics/dynprog/jaccard.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)   210722 2023-06-20 03:26:44.000000 shorttext-1.5.9/shorttext/metrics/dynprog/lcp.c
+-rw-r--r--   0 stephenhky   (501) staff       (20)      330 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/metrics/dynprog/lcp.pyx
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.674598 shorttext-1.5.9/shorttext/metrics/embedfuzzy/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       40 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/metrics/embedfuzzy/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1636 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/metrics/embedfuzzy/jaccard.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.676458 shorttext-1.5.9/shorttext/metrics/transformers/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       35 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/metrics/transformers/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4690 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/metrics/transformers/bertscore.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.677925 shorttext-1.5.9/shorttext/metrics/wasserstein/
+-rwxr-xr-x   0 stephenhky   (501) staff       (20)       76 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/metrics/wasserstein/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4327 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/metrics/wasserstein/wordmoverdist.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3191 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/smartload.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.682072 shorttext-1.5.9/shorttext/spell/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      159 2022-09-22 03:31:05.000000 shorttext-1.5.9/shorttext/spell/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      752 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/spell/basespellcorrector.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8334 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/spell/binarize.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      648 2022-10-29 20:54:47.000000 shorttext-1.5.9/shorttext/spell/editor.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     2030 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/spell/norvig.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8630 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/spell/sakaguchi.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.683393 shorttext-1.5.9/shorttext/stack/
+-rw-r--r--   0 stephenhky   (501) staff       (20)       74 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/stack/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)    11750 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/stack/stacking.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.697210 shorttext-1.5.9/shorttext/utils/
+-rw-r--r--   0 stephenhky   (501) staff       (20)      694 2022-08-26 21:53:09.000000 shorttext-1.5.9/shorttext/utils/__init__.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1051 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/utils/classification_exceptions.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8905 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/utils/compactmodel_io.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      526 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/utils/deprecation.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     8040 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/utils/dtm.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3506 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/utils/gensim_corpora.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1086 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/utils/kerasmodel_io.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1165 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/utils/misc.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)    18405 2022-08-26 21:53:09.000000 shorttext-1.5.9/shorttext/utils/nonneg_stopwords.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)    18416 2020-08-16 04:30:18.000000 shorttext-1.5.9/shorttext/utils/stopwords.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4201 2022-08-26 21:53:09.000000 shorttext-1.5.9/shorttext/utils/textpreprocessing.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     6012 2021-12-30 18:22:16.000000 shorttext-1.5.9/shorttext/utils/transformers.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     6906 2023-02-25 20:12:30.000000 shorttext-1.5.9/shorttext/utils/wordembed.py
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.639014 shorttext-1.5.9/shorttext.egg-info/
+-rw-r--r--   0 stephenhky   (501) staff       (20)    10199 2023-06-20 03:26:59.000000 shorttext-1.5.9/shorttext.egg-info/PKG-INFO
+-rw-r--r--   0 stephenhky   (501) staff       (20)     3148 2023-06-20 03:26:59.000000 shorttext-1.5.9/shorttext.egg-info/SOURCES.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2023-06-20 03:26:59.000000 shorttext-1.5.9/shorttext.egg-info/dependency_links.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)        1 2020-09-02 22:21:18.000000 shorttext-1.5.9/shorttext.egg-info/not-zip-safe
+-rw-r--r--   0 stephenhky   (501) staff       (20)      245 2023-06-20 03:26:59.000000 shorttext-1.5.9/shorttext.egg-info/requires.txt
+-rw-r--r--   0 stephenhky   (501) staff       (20)       10 2023-06-20 03:26:59.000000 shorttext-1.5.9/shorttext.egg-info/top_level.txt
+drwxr-xr-x   0 stephenhky   (501) staff       (20)        0 2023-06-20 03:26:59.708057 shorttext-1.5.9/test/
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1705 2021-12-30 18:22:16.000000 shorttext-1.5.9/test/test_bertrepresentations.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      599 2021-12-30 18:22:16.000000 shorttext-1.5.9/test/test_charonehot.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1620 2020-08-16 04:30:18.000000 shorttext-1.5.9/test/test_dtm.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1679 2020-08-16 04:30:18.000000 shorttext-1.5.9/test/test_fuzzylogic.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      577 2020-08-16 04:30:18.000000 shorttext-1.5.9/test/test_norvigspell.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1478 2021-04-09 15:34:12.000000 shorttext-1.5.9/test/test_sakaguchispell.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     5822 2020-08-16 04:30:18.000000 shorttext-1.5.9/test/test_stacking.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)      965 2022-08-26 21:53:09.000000 shorttext-1.5.9/test/test_textpreprocessing.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     4578 2022-10-29 21:03:20.000000 shorttext-1.5.9/test/test_var_nn_embedded_vec_classifier.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)     1401 2022-10-29 21:03:20.000000 shorttext-1.5.9/test/test_wmd.py
+-rw-r--r--   0 stephenhky   (501) staff       (20)       29 2021-12-30 18:22:16.000000 shorttext-1.5.9/test_requirements.txt
```

### Comparing `shorttext-1.5.8/LICENSE` & `shorttext-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/PKG-INFO` & `shorttext-1.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shorttext
-Version: 1.5.8
+Version: 1.5.9
 Summary: Short Text Mining
 Home-page: https://github.com/stephenhky/PyShortTextCategorization
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Description: ## Introduction
         
@@ -85,14 +85,15 @@
         * "Python Package for Short Text Mining", [WordPress](https://datawarrior.wordpress.com/2016/12/22/python-package-for-short-text-mining/)
         * "Document-Term Matrix: Text Mining in R and Python," [WordPress](https://datawarrior.wordpress.com/2018/01/22/document-term-matrix-text-mining-in-r-and-python/)
         * An [earlier version](https://github.com/stephenhky/PyShortTextCategorization/tree/b298d3ce7d06a9b4e0f7d32f27bab66064ba7afa) of this repository is a demonstration of the following blog post: [Short Text Categorization using Deep Neural Networks and Word-Embedding Models](https://datawarrior.wordpress.com/2016/10/12/short-text-categorization-using-deep-neural-networks-and-word-embedding-models/)
         
         
         ## News
         
+        * 06/19/2023: `shorttext` 1.5.9 released.
         * 09/23/2022: `shorttext` 1.5.8 released.
         * 09/22/2022: `shorttext` 1.5.7 released.
         * 08/29/2022: `shorttext` 1.5.6 released.
         * 05/28/2022: `shorttext` 1.5.5 released.
         * 12/15/2021: `shorttext` 1.5.4 released.
         * 07/11/2021: `shorttext` 1.5.3 released.
         * 07/06/2021: `shorttext` 1.5.2 released.
```

### Comparing `shorttext-1.5.8/README.md` & `shorttext-1.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
 * "Python Package for Short Text Mining", [WordPress](https://datawarrior.wordpress.com/2016/12/22/python-package-for-short-text-mining/)
 * "Document-Term Matrix: Text Mining in R and Python," [WordPress](https://datawarrior.wordpress.com/2018/01/22/document-term-matrix-text-mining-in-r-and-python/)
 * An [earlier version](https://github.com/stephenhky/PyShortTextCategorization/tree/b298d3ce7d06a9b4e0f7d32f27bab66064ba7afa) of this repository is a demonstration of the following blog post: [Short Text Categorization using Deep Neural Networks and Word-Embedding Models](https://datawarrior.wordpress.com/2016/10/12/short-text-categorization-using-deep-neural-networks-and-word-embedding-models/)
 
 
 ## News
 
+* 06/19/2023: `shorttext` 1.5.9 released.
 * 09/23/2022: `shorttext` 1.5.8 released.
 * 09/22/2022: `shorttext` 1.5.7 released.
 * 08/29/2022: `shorttext` 1.5.6 released.
 * 05/28/2022: `shorttext` 1.5.5 released.
 * 12/15/2021: `shorttext` 1.5.4 released.
 * 07/11/2021: `shorttext` 1.5.3 released.
 * 07/06/2021: `shorttext` 1.5.2 released.
```

### Comparing `shorttext-1.5.8/bin/ShortTextCategorizerConsole` & `shorttext-1.5.9/bin/ShortTextCategorizerConsole`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/bin/ShortTextWordEmbedSimilarity` & `shorttext-1.5.9/bin/ShortTextWordEmbedSimilarity`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/setup.py` & `shorttext-1.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 def test_requirements():
     return [package_string.strip() for package_string in open('test_requirements.txt', 'r')]
 
 
 
 setup(name='shorttext',
-      version='1.5.8',
+      version='1.5.9',
       description="Short Text Mining",
       long_description=package_description(),
       long_description_content_type='text/markdown',
       classifiers=[
           "Topic :: Scientific/Engineering :: Artificial Intelligence",
           "Topic :: Scientific/Engineering :: Mathematics",
           "Topic :: Text Processing :: Linguistic",
@@ -82,12 +82,11 @@
                                   'metrics/dynprog/*.pyx', 'metrics/dynprog/*.c',
                                   'spell/*.pyx', 'spell/*.c']},
       include_dirs=[np.get_include()],
       python_requires='>=3.7',
       setup_requires=setup_requirements(),
       install_requires=install_requirements(),
       scripts=['bin/ShortTextCategorizerConsole',
-               'bin/ShortTextWordEmbedSimilarity',
-               'bin/WordEmbedAPI'],
+               'bin/ShortTextWordEmbedSimilarity'],
       test_suite="test",
       tests_requires=test_requirements(),
       zip_safe=False)
```

### Comparing `shorttext-1.5.8/shorttext/classifiers/__init__.py` & `shorttext-1.5.9/shorttext/classifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/bow/maxent/MaxEntClassification.py` & `shorttext-1.5.9/shorttext/classifiers/bow/maxent/MaxEntClassification.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/bow/topic/SkLearnClassification.py` & `shorttext-1.5.9/shorttext/classifiers/bow/topic/SkLearnClassification.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/bow/topic/TopicVectorDistanceClassification.py` & `shorttext-1.5.9/shorttext/classifiers/bow/topic/TopicVectorDistanceClassification.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/embed/__init__.py` & `shorttext-1.5.9/shorttext/classifiers/embed/__init__.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/embed/nnlib/VarNNEmbedVecClassification.py` & `shorttext-1.5.9/shorttext/classifiers/embed/nnlib/VarNNEmbedVecClassification.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/embed/nnlib/frameworks.py` & `shorttext-1.5.9/shorttext/classifiers/embed/nnlib/frameworks.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/embed/sumvec/SumEmbedVecClassification.py` & `shorttext-1.5.9/shorttext/classifiers/embed/sumvec/SumEmbedVecClassification.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/embed/sumvec/VarNNSumEmbedVecClassification.py` & `shorttext-1.5.9/shorttext/classifiers/embed/sumvec/VarNNSumEmbedVecClassification.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/classifiers/embed/sumvec/frameworks.py` & `shorttext-1.5.9/shorttext/classifiers/embed/sumvec/frameworks.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/data/data_retrieval.py` & `shorttext-1.5.9/shorttext/data/data_retrieval.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/data/shorttext_exampledata.csv` & `shorttext-1.5.9/shorttext/data/shorttext_exampledata.csv`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/generators/__init__.py` & `shorttext-1.5.9/shorttext/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/generators/bow/AutoEncodingTopicModeling.py` & `shorttext-1.5.9/shorttext/generators/bow/AutoEncodingTopicModeling.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/generators/bow/GensimTopicModeling.py` & `shorttext-1.5.9/shorttext/generators/bow/GensimTopicModeling.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/generators/bow/LatentTopicModeling.py` & `shorttext-1.5.9/shorttext/generators/bow/LatentTopicModeling.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/generators/charbase/char2vec.py` & `shorttext-1.5.9/shorttext/generators/charbase/char2vec.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/generators/seq2seq/charbaseS2S.py` & `shorttext-1.5.9/shorttext/generators/seq2seq/charbaseS2S.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/generators/seq2seq/s2skeras.py` & `shorttext-1.5.9/shorttext/generators/seq2seq/s2skeras.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/metrics/dynprog/dldist.c` & `shorttext-1.5.9/shorttext/metrics/dynprog/dldist.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.22 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "shorttext.metrics.dynprog.dldist",
         "sources": [
             "shorttext/metrics/dynprog/dldist.pyx"
         ]
     },
     "module_name": "shorttext.metrics.dynprog.dldist"
 }
 END: Cython Metadata */
 
-#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
-#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_22"
+#define CYTHON_HEX_VERSION 0x001D16F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -58,15 +56,14 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -95,22 +92,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -140,67 +133,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
-  #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -220,64 +164,53 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
+  #if PY_VERSION_HEX < 0x030300F0
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+  #ifndef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #if PY_MAJOR_VERSION < 3
-    #include "longintrepr.h"
-  #endif
+  #include "longintrepr.h"
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -386,76 +319,17 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-  #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
-                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
-                                                    PyObject *fv, PyObject *cell, PyObject* fn,
-                                                    PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
-        PyObject *type, *value, *traceback;
-        PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(call_result);
-        Py_XDECREF(empty);
-        if (type) {
-            PyErr_Restore(type, value, traceback);
-        }
-        return co;
-    }
+#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -561,33 +435,25 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
-  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
   #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
   #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
@@ -685,18 +551,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -713,18 +579,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -859,15 +723,14 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -1015,47 +878,51 @@
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* Atomics.proto */
 #include <pythread.h>
 #ifndef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 1
 #endif
-#define __PYX_CYTHON_ATOMICS_ENABLED() CYTHON_ATOMICS
 #define __pyx_atomic_int_type int
-#if CYTHON_ATOMICS && (__GNUC__ >= 5 || (__GNUC__ == 4 &&\
-                    (__GNUC_MINOR__ > 1 ||\
-                    (__GNUC_MINOR__ == 1 && __GNUC_PATCHLEVEL__ >= 2))))
-    #define __pyx_atomic_incr_aligned(value) __sync_fetch_and_add(value, 1)
-    #define __pyx_atomic_decr_aligned(value) __sync_fetch_and_sub(value, 1)
+#if CYTHON_ATOMICS && __GNUC__ >= 4 && (__GNUC_MINOR__ > 1 ||\
+                    (__GNUC_MINOR__ == 1 && __GNUC_PATCHLEVEL >= 2)) &&\
+                    !defined(__i386__)
+    #define __pyx_atomic_incr_aligned(value, lock) __sync_fetch_and_add(value, 1)
+    #define __pyx_atomic_decr_aligned(value, lock) __sync_fetch_and_sub(value, 1)
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Using GNU atomics"
     #endif
-#elif CYTHON_ATOMICS && defined(_MSC_VER) && CYTHON_COMPILING_IN_NOGIL
-    #include <intrin.h>
+#elif CYTHON_ATOMICS && defined(_MSC_VER) && 0
+    #include <Windows.h>
     #undef __pyx_atomic_int_type
-    #define __pyx_atomic_int_type long
-    #pragma intrinsic (_InterlockedExchangeAdd)
-    #define __pyx_atomic_incr_aligned(value) _InterlockedExchangeAdd(value, 1)
-    #define __pyx_atomic_decr_aligned(value) _InterlockedExchangeAdd(value, -1)
+    #define __pyx_atomic_int_type LONG
+    #define __pyx_atomic_incr_aligned(value, lock) InterlockedIncrement(value)
+    #define __pyx_atomic_decr_aligned(value, lock) InterlockedDecrement(value)
     #ifdef __PYX_DEBUG_ATOMICS
         #pragma message ("Using MSVC atomics")
     #endif
+#elif CYTHON_ATOMICS && (defined(__ICC) || defined(__INTEL_COMPILER)) && 0
+    #define __pyx_atomic_incr_aligned(value, lock) _InterlockedIncrement(value)
+    #define __pyx_atomic_decr_aligned(value, lock) _InterlockedDecrement(value)
+    #ifdef __PYX_DEBUG_ATOMICS
+        #warning "Using Intel atomics"
+    #endif
 #else
     #undef CYTHON_ATOMICS
     #define CYTHON_ATOMICS 0
     #ifdef __PYX_DEBUG_ATOMICS
         #warning "Not using atomics"
     #endif
 #endif
 typedef volatile __pyx_atomic_int_type __pyx_atomic_int;
 #if CYTHON_ATOMICS
     #define __pyx_add_acquisition_count(memview)\
-             __pyx_atomic_incr_aligned(__pyx_get_slice_count_pointer(memview))
+             __pyx_atomic_incr_aligned(__pyx_get_slice_count_pointer(memview), memview->lock)
     #define __pyx_sub_acquisition_count(memview)\
-            __pyx_atomic_decr_aligned(__pyx_get_slice_count_pointer(memview))
+            __pyx_atomic_decr_aligned(__pyx_get_slice_count_pointer(memview), memview->lock)
 #else
     #define __pyx_add_acquisition_count(memview)\
             __pyx_add_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
     #define __pyx_sub_acquisition_count(memview)\
             __pyx_sub_acquisition_count_locked(__pyx_get_slice_count_pointer(memview), memview->lock)
 #endif
 
@@ -1104,195 +971,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1323,51 +1190,51 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "View.MemoryView":106
+/* "View.MemoryView":105
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
 struct __pyx_array_obj {
@@ -1384,28 +1251,28 @@
   PyObject *_format;
   void (*callback_free_data)(void *);
   int free_data;
   int dtype_is_object;
 };
 
 
-/* "View.MemoryView":280
+/* "View.MemoryView":279
  * 
  * @cname('__pyx_MemviewEnum')
  * cdef class Enum(object):             # <<<<<<<<<<<<<<
  *     cdef object name
  *     def __init__(self, name):
  */
 struct __pyx_MemviewEnum_obj {
   PyObject_HEAD
   PyObject *name;
 };
 
 
-/* "View.MemoryView":331
+/* "View.MemoryView":330
  * 
  * @cname('__pyx_memoryview')
  * cdef class memoryview(object):             # <<<<<<<<<<<<<<
  * 
  *     cdef object obj
  */
 struct __pyx_memoryview_obj {
@@ -1420,15 +1287,15 @@
   Py_buffer view;
   int flags;
   int dtype_is_object;
   __Pyx_TypeInfo *typeinfo;
 };
 
 
-/* "View.MemoryView":967
+/* "View.MemoryView":965
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 struct __pyx_memoryviewslice_obj {
@@ -1437,29 +1304,29 @@
   PyObject *from_object;
   PyObject *(*to_object_func)(char *);
   int (*to_dtype_func)(char *, PyObject *);
 };
 
 
 
-/* "View.MemoryView":106
+/* "View.MemoryView":105
  * 
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
  */
 
 struct __pyx_vtabstruct_array {
   PyObject *(*get_memview)(struct __pyx_array_obj *);
 };
 static struct __pyx_vtabstruct_array *__pyx_vtabptr_array;
 
 
-/* "View.MemoryView":331
+/* "View.MemoryView":330
  * 
  * @cname('__pyx_memoryview')
  * cdef class memoryview(object):             # <<<<<<<<<<<<<<
  * 
  *     cdef object obj
  */
 
@@ -1471,15 +1338,15 @@
   PyObject *(*setitem_indexed)(struct __pyx_memoryview_obj *, PyObject *, PyObject *);
   PyObject *(*convert_item_to_object)(struct __pyx_memoryview_obj *, char *);
   PyObject *(*assign_item_from_object)(struct __pyx_memoryview_obj *, char *, PyObject *);
 };
 static struct __pyx_vtabstruct_memoryview *__pyx_vtabptr_memoryview;
 
 
-/* "View.MemoryView":967
+/* "View.MemoryView":965
  * 
  * @cname('__pyx_memoryviewslice')
  * cdef class _memoryviewslice(memoryview):             # <<<<<<<<<<<<<<
  *     "Internal class for passing memoryview slices to Python"
  * 
  */
 
@@ -1773,29 +1640,21 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyObjectCall2Args.proto */
 static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
@@ -1817,15 +1676,15 @@
 /* StrEquals.proto */
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
 #else
 #define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
 #endif
 
-/* DivInt[Py_ssize_t].proto */
+/* None.proto */
 static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t, Py_ssize_t);
 
 /* UnaryNegOverflows.proto */
 #define UNARY_NEG_WOULD_OVERFLOW(x)\
         (((x) < 0) & ((unsigned long)(x) == 0-(unsigned long)(x)))
 
 static CYTHON_UNUSED int __pyx_array_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
@@ -1954,23 +1813,17 @@
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
-/* DivInt[long].proto */
+/* None.proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
-/* PySequenceContains.proto */
-static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
-    int result = PySequence_Contains(seq, item);
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
-
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* PyObject_GenericGetAttrNoDict.proto */
@@ -2068,40 +1921,14 @@
 static CYTHON_INLINE PyObject *__pyx_capsule_create(void *p, const char *sig);
 
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
-/* IsLittleEndian.proto */
-static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
-
-/* BufferFormatCheck.proto */
-static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
-static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
-                              __Pyx_BufFmt_StackElem* stack,
-                              __Pyx_TypeInfo* type);
-
-/* TypeInfoCompare.proto */
-static int __pyx_typeinfo_cmp(__Pyx_TypeInfo *a, __Pyx_TypeInfo *b);
-
-/* MemviewSliceValidateAndInit.proto */
-static int __Pyx_ValidateAndInit_memviewslice(
-                int *axes_specs,
-                int c_or_f_flag,
-                int buf_flags,
-                int ndim,
-                __Pyx_TypeInfo *dtype,
-                __Pyx_BufFmt_StackElem stack[],
-                __Pyx_memviewslice *memviewslice,
-                PyObject *original_obj);
-
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_int(PyObject *, int writable_flag);
-
 /* RealImag.proto */
 #if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     #define __Pyx_CREAL(z) ((z).real())
     #define __Pyx_CIMAG(z) ((z).imag())
   #else
     #define __Pyx_CREAL(z) (__real__(z))
@@ -2214,14 +2041,40 @@
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
+/* IsLittleEndian.proto */
+static CYTHON_INLINE int __Pyx_Is_Little_Endian(void);
+
+/* BufferFormatCheck.proto */
+static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts);
+static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
+                              __Pyx_BufFmt_StackElem* stack,
+                              __Pyx_TypeInfo* type);
+
+/* TypeInfoCompare.proto */
+static int __pyx_typeinfo_cmp(__Pyx_TypeInfo *a, __Pyx_TypeInfo *b);
+
+/* MemviewSliceValidateAndInit.proto */
+static int __Pyx_ValidateAndInit_memviewslice(
+                int *axes_specs,
+                int c_or_f_flag,
+                int buf_flags,
+                int ndim,
+                __Pyx_TypeInfo *dtype,
+                __Pyx_BufFmt_StackElem stack[],
+                __Pyx_memviewslice *memviewslice,
+                PyObject *original_obj);
+
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_int(PyObject *, int writable_flag);
+
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
@@ -2425,15 +2278,15 @@
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
-static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))";
+static const char __pyx_k_Incompatible_checksums_s_vs_0xb0[] = "Incompatible checksums (%s vs 0xb068931 = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
@@ -2445,15 +2298,15 @@
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_n_s_ImportError;
-static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xb0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
@@ -2594,16 +2447,14 @@
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
-static PyObject *__pyx_int_112105877;
-static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
@@ -2619,23 +2470,22 @@
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
-static PyObject *__pyx_tuple__22;
+static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__29;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__30;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__29;
 /* Late includes */
 
 /* "shorttext/metrics/dynprog/dldist.pyx":5
  * cimport numpy as np
  * 
  * def damerau_levenshtein(str word1, str word2):             # <<<<<<<<<<<<<<
  *     cdef int len1 = len(word1)
@@ -3229,15 +3079,15 @@
   __pyx_L0:;
   __PYX_XDEC_MEMVIEW(&__pyx_v_matrix, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3246,29 +3096,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3279,15 +3129,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3296,29 +3146,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3329,15 +3179,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3346,29 +3196,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3379,15 +3229,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3396,29 +3246,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3429,15 +3279,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3446,29 +3296,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3479,212 +3329,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3700,15 +3550,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3716,84 +3566,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3808,15 +3658,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3832,15 +3682,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3848,84 +3698,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3940,15 +3790,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3964,15 +3814,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3980,84 +3830,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4072,189 +3922,189 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":123
+/* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -4298,21 +4148,21 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_shape)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_itemsize)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(2, 123, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 1); __PYX_ERR(2, 122, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_format)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(2, 123, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, 2); __PYX_ERR(2, 122, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_mode);
           if (value) { values[3] = value; kw_args--; }
         }
@@ -4320,15 +4170,15 @@
         case  4:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_allocate_buffer);
           if (value) { values[4] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 123, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 122, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
         CYTHON_FALLTHROUGH;
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
@@ -4336,46 +4186,46 @@
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_shape = ((PyObject*)values[0]);
-    __pyx_v_itemsize = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_itemsize == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 123, __pyx_L3_error)
+    __pyx_v_itemsize = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_itemsize == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 122, __pyx_L3_error)
     __pyx_v_format = values[2];
     __pyx_v_mode = values[3];
     if (values[4]) {
-      __pyx_v_allocate_buffer = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_allocate_buffer == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 124, __pyx_L3_error)
+      __pyx_v_allocate_buffer = __Pyx_PyObject_IsTrue(values[4]); if (unlikely((__pyx_v_allocate_buffer == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 123, __pyx_L3_error)
     } else {
 
-      /* "View.MemoryView":124
+      /* "View.MemoryView":123
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,
  *                   mode="c", bint allocate_buffer=True):             # <<<<<<<<<<<<<<
  * 
  *         cdef int idx
  */
       __pyx_v_allocate_buffer = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 123, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 3, 5, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 122, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.array.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(2, 123, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_shape), (&PyTuple_Type), 1, "shape", 1))) __PYX_ERR(2, 122, __pyx_L1_error)
   if (unlikely(((PyObject *)__pyx_v_format) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(2, 123, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "format"); __PYX_ERR(2, 122, __pyx_L1_error)
   }
   __pyx_r = __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(((struct __pyx_array_obj *)__pyx_v_self), __pyx_v_shape, __pyx_v_itemsize, __pyx_v_format, __pyx_v_mode, __pyx_v_allocate_buffer);
 
-  /* "View.MemoryView":123
+  /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -4409,579 +4259,579 @@
   Py_ssize_t __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
   __Pyx_INCREF(__pyx_v_format);
 
-  /* "View.MemoryView":130
+  /* "View.MemoryView":129
  *         cdef PyObject **p
  * 
  *         self.ndim = <int> len(shape)             # <<<<<<<<<<<<<<
  *         self.itemsize = itemsize
  * 
  */
   if (unlikely(__pyx_v_shape == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(2, 130, __pyx_L1_error)
+    __PYX_ERR(2, 129, __pyx_L1_error)
   }
-  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(2, 130, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_GET_SIZE(__pyx_v_shape); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(2, 129, __pyx_L1_error)
   __pyx_v_self->ndim = ((int)__pyx_t_1);
 
-  /* "View.MemoryView":131
+  /* "View.MemoryView":130
  * 
  *         self.ndim = <int> len(shape)
  *         self.itemsize = itemsize             # <<<<<<<<<<<<<<
  * 
  *         if not self.ndim:
  */
   __pyx_v_self->itemsize = __pyx_v_itemsize;
 
-  /* "View.MemoryView":133
+  /* "View.MemoryView":132
  *         self.itemsize = itemsize
  * 
  *         if not self.ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_self->ndim != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":134
+    /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 133, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 134, __pyx_L1_error)
+    __PYX_ERR(2, 133, __pyx_L1_error)
 
-    /* "View.MemoryView":133
+    /* "View.MemoryView":132
  *         self.itemsize = itemsize
  * 
  *         if not self.ndim:             # <<<<<<<<<<<<<<
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  */
   }
 
-  /* "View.MemoryView":136
+  /* "View.MemoryView":135
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  *         if itemsize <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  */
   __pyx_t_2 = ((__pyx_v_itemsize <= 0) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":137
+    /* "View.MemoryView":136
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 136, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 137, __pyx_L1_error)
+    __PYX_ERR(2, 136, __pyx_L1_error)
 
-    /* "View.MemoryView":136
+    /* "View.MemoryView":135
  *             raise ValueError("Empty shape tuple for cython.array")
  * 
  *         if itemsize <= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  */
   }
 
-  /* "View.MemoryView":139
+  /* "View.MemoryView":138
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  *         if not isinstance(format, bytes):             # <<<<<<<<<<<<<<
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  */
   __pyx_t_2 = PyBytes_Check(__pyx_v_format); 
   __pyx_t_4 = ((!(__pyx_t_2 != 0)) != 0);
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":140
+    /* "View.MemoryView":139
  * 
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')             # <<<<<<<<<<<<<<
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format
  */
-    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 140, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_format, __pyx_n_s_encode); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_6 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
       __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
       if (likely(__pyx_t_6)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
         __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_5, function);
       }
     }
     __pyx_t_3 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_6, __pyx_n_s_ASCII) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_n_s_ASCII);
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 140, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 139, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF_SET(__pyx_v_format, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":139
+    /* "View.MemoryView":138
  *             raise ValueError("itemsize <= 0 for cython.array")
  * 
  *         if not isinstance(format, bytes):             # <<<<<<<<<<<<<<
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  */
   }
 
-  /* "View.MemoryView":141
+  /* "View.MemoryView":140
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 140, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":142
+  /* "View.MemoryView":141
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string
  *         self.format = self._format             # <<<<<<<<<<<<<<
  * 
  * 
  */
   if (unlikely(__pyx_v_self->_format == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(2, 142, __pyx_L1_error)
+    __PYX_ERR(2, 141, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_self->_format); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(2, 142, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_self->_format); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(2, 141, __pyx_L1_error)
   __pyx_v_self->format = __pyx_t_7;
 
-  /* "View.MemoryView":145
+  /* "View.MemoryView":144
  * 
  * 
  *         self._shape = <Py_ssize_t *> PyObject_Malloc(sizeof(Py_ssize_t)*self.ndim*2)             # <<<<<<<<<<<<<<
  *         self._strides = self._shape + self.ndim
  * 
  */
   __pyx_v_self->_shape = ((Py_ssize_t *)PyObject_Malloc((((sizeof(Py_ssize_t)) * __pyx_v_self->ndim) * 2)));
 
-  /* "View.MemoryView":146
+  /* "View.MemoryView":145
  * 
  *         self._shape = <Py_ssize_t *> PyObject_Malloc(sizeof(Py_ssize_t)*self.ndim*2)
  *         self._strides = self._shape + self.ndim             # <<<<<<<<<<<<<<
  * 
  *         if not self._shape:
  */
   __pyx_v_self->_strides = (__pyx_v_self->_shape + __pyx_v_self->ndim);
 
-  /* "View.MemoryView":148
+  /* "View.MemoryView":147
  *         self._strides = self._shape + self.ndim
  * 
  *         if not self._shape:             # <<<<<<<<<<<<<<
  *             raise MemoryError("unable to allocate shape and strides.")
  * 
  */
   __pyx_t_4 = ((!(__pyx_v_self->_shape != 0)) != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "View.MemoryView":149
+    /* "View.MemoryView":148
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 148, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 149, __pyx_L1_error)
+    __PYX_ERR(2, 148, __pyx_L1_error)
 
-    /* "View.MemoryView":148
+    /* "View.MemoryView":147
  *         self._strides = self._shape + self.ndim
  * 
  *         if not self._shape:             # <<<<<<<<<<<<<<
  *             raise MemoryError("unable to allocate shape and strides.")
  * 
  */
   }
 
-  /* "View.MemoryView":152
+  /* "View.MemoryView":151
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  */
   __pyx_t_8 = 0;
   __pyx_t_3 = __pyx_v_shape; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
   for (;;) {
     if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(2, 152, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(2, 151, __pyx_L1_error)
     #else
-    __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 152, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 151, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 152, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_5); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 151, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_9;
     __pyx_v_idx = __pyx_t_8;
     __pyx_t_8 = (__pyx_t_8 + 1);
 
-    /* "View.MemoryView":153
+    /* "View.MemoryView":152
  * 
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim
  */
     __pyx_t_4 = ((__pyx_v_dim <= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":154
+      /* "View.MemoryView":153
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))             # <<<<<<<<<<<<<<
  *             self._shape[idx] = dim
  * 
  */
-      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 154, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 154, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 154, __pyx_L1_error)
+      __pyx_t_10 = PyTuple_New(2); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_GIVEREF(__pyx_t_5);
       PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_5);
       __Pyx_GIVEREF(__pyx_t_6);
       PyTuple_SET_ITEM(__pyx_t_10, 1, __pyx_t_6);
       __pyx_t_5 = 0;
       __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 154, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyString_Format(__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_t_10); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 154, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 153, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __PYX_ERR(2, 154, __pyx_L1_error)
+      __PYX_ERR(2, 153, __pyx_L1_error)
 
-      /* "View.MemoryView":153
+      /* "View.MemoryView":152
  * 
  *         for idx, dim in enumerate(shape):
  *             if dim <= 0:             # <<<<<<<<<<<<<<
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim
  */
     }
 
-    /* "View.MemoryView":155
+    /* "View.MemoryView":154
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  *             self._shape[idx] = dim             # <<<<<<<<<<<<<<
  * 
  *         cdef char order
  */
     (__pyx_v_self->_shape[__pyx_v_idx]) = __pyx_v_dim;
 
-    /* "View.MemoryView":152
+    /* "View.MemoryView":151
  * 
  * 
  *         for idx, dim in enumerate(shape):             # <<<<<<<<<<<<<<
  *             if dim <= 0:
  *                 raise ValueError("Invalid shape in axis %d: %d." % (idx, dim))
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":158
+  /* "View.MemoryView":157
  * 
  *         cdef char order
  *         if mode == 'fortran':             # <<<<<<<<<<<<<<
  *             order = b'F'
  *             self.mode = u'fortran'
  */
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_fortran, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 158, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_fortran, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 157, __pyx_L1_error)
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":159
+    /* "View.MemoryView":158
  *         cdef char order
  *         if mode == 'fortran':
  *             order = b'F'             # <<<<<<<<<<<<<<
  *             self.mode = u'fortran'
  *         elif mode == 'c':
  */
     __pyx_v_order = 'F';
 
-    /* "View.MemoryView":160
+    /* "View.MemoryView":159
  *         if mode == 'fortran':
  *             order = b'F'
  *             self.mode = u'fortran'             # <<<<<<<<<<<<<<
  *         elif mode == 'c':
  *             order = b'C'
  */
     __Pyx_INCREF(__pyx_n_u_fortran);
     __Pyx_GIVEREF(__pyx_n_u_fortran);
     __Pyx_GOTREF(__pyx_v_self->mode);
     __Pyx_DECREF(__pyx_v_self->mode);
     __pyx_v_self->mode = __pyx_n_u_fortran;
 
-    /* "View.MemoryView":158
+    /* "View.MemoryView":157
  * 
  *         cdef char order
  *         if mode == 'fortran':             # <<<<<<<<<<<<<<
  *             order = b'F'
  *             self.mode = u'fortran'
  */
     goto __pyx_L10;
   }
 
-  /* "View.MemoryView":161
+  /* "View.MemoryView":160
  *             order = b'F'
  *             self.mode = u'fortran'
  *         elif mode == 'c':             # <<<<<<<<<<<<<<
  *             order = b'C'
  *             self.mode = u'c'
  */
-  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_c, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 161, __pyx_L1_error)
+  __pyx_t_4 = (__Pyx_PyString_Equals(__pyx_v_mode, __pyx_n_s_c, Py_EQ)); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(2, 160, __pyx_L1_error)
   if (likely(__pyx_t_4)) {
 
-    /* "View.MemoryView":162
+    /* "View.MemoryView":161
  *             self.mode = u'fortran'
  *         elif mode == 'c':
  *             order = b'C'             # <<<<<<<<<<<<<<
  *             self.mode = u'c'
  *         else:
  */
     __pyx_v_order = 'C';
 
-    /* "View.MemoryView":163
+    /* "View.MemoryView":162
  *         elif mode == 'c':
  *             order = b'C'
  *             self.mode = u'c'             # <<<<<<<<<<<<<<
  *         else:
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)
  */
     __Pyx_INCREF(__pyx_n_u_c);
     __Pyx_GIVEREF(__pyx_n_u_c);
     __Pyx_GOTREF(__pyx_v_self->mode);
     __Pyx_DECREF(__pyx_v_self->mode);
     __pyx_v_self->mode = __pyx_n_u_c;
 
-    /* "View.MemoryView":161
+    /* "View.MemoryView":160
  *             order = b'F'
  *             self.mode = u'fortran'
  *         elif mode == 'c':             # <<<<<<<<<<<<<<
  *             order = b'C'
  *             self.mode = u'c'
  */
     goto __pyx_L10;
   }
 
-  /* "View.MemoryView":165
+  /* "View.MemoryView":164
  *             self.mode = u'c'
  *         else:
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)             # <<<<<<<<<<<<<<
  * 
  *         self.len = fill_contig_strides_array(self._shape, self._strides,
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 165, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_v_mode); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 165, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 164, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_10);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_10, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-    __PYX_ERR(2, 165, __pyx_L1_error)
+    __PYX_ERR(2, 164, __pyx_L1_error)
   }
   __pyx_L10:;
 
-  /* "View.MemoryView":167
+  /* "View.MemoryView":166
  *             raise ValueError("Invalid mode, expected 'c' or 'fortran', got %s" % mode)
  * 
  *         self.len = fill_contig_strides_array(self._shape, self._strides,             # <<<<<<<<<<<<<<
  *                                              itemsize, self.ndim, order)
  * 
  */
   __pyx_v_self->len = __pyx_fill_contig_strides_array(__pyx_v_self->_shape, __pyx_v_self->_strides, __pyx_v_itemsize, __pyx_v_self->ndim, __pyx_v_order);
 
-  /* "View.MemoryView":170
+  /* "View.MemoryView":169
  *                                              itemsize, self.ndim, order)
  * 
  *         self.free_data = allocate_buffer             # <<<<<<<<<<<<<<
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:
  */
   __pyx_v_self->free_data = __pyx_v_allocate_buffer;
 
-  /* "View.MemoryView":171
+  /* "View.MemoryView":170
  * 
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'             # <<<<<<<<<<<<<<
  *         if allocate_buffer:
  * 
  */
-  __pyx_t_10 = PyObject_RichCompare(__pyx_v_format, __pyx_n_b_O, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 171, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 171, __pyx_L1_error)
+  __pyx_t_10 = PyObject_RichCompare(__pyx_v_format, __pyx_n_b_O, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 170, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
   __pyx_v_self->dtype_is_object = __pyx_t_4;
 
-  /* "View.MemoryView":172
+  /* "View.MemoryView":171
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_4 = (__pyx_v_allocate_buffer != 0);
   if (__pyx_t_4) {
 
-    /* "View.MemoryView":175
+    /* "View.MemoryView":174
  * 
  * 
  *             self.data = <char *>malloc(self.len)             # <<<<<<<<<<<<<<
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")
  */
     __pyx_v_self->data = ((char *)malloc(__pyx_v_self->len));
 
-    /* "View.MemoryView":176
+    /* "View.MemoryView":175
  * 
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("unable to allocate array data.")
  * 
  */
     __pyx_t_4 = ((!(__pyx_v_self->data != 0)) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":177
+      /* "View.MemoryView":176
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__6, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(2, 176, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __PYX_ERR(2, 177, __pyx_L1_error)
+      __PYX_ERR(2, 176, __pyx_L1_error)
 
-      /* "View.MemoryView":176
+      /* "View.MemoryView":175
  * 
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:             # <<<<<<<<<<<<<<
  *                 raise MemoryError("unable to allocate array data.")
  * 
  */
     }
 
-    /* "View.MemoryView":179
+    /* "View.MemoryView":178
  *                 raise MemoryError("unable to allocate array data.")
  * 
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  */
     __pyx_t_4 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":180
+      /* "View.MemoryView":179
  * 
  *             if self.dtype_is_object:
  *                 p = <PyObject **> self.data             # <<<<<<<<<<<<<<
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None
  */
       __pyx_v_p = ((PyObject **)__pyx_v_self->data);
 
-      /* "View.MemoryView":181
+      /* "View.MemoryView":180
  *             if self.dtype_is_object:
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):             # <<<<<<<<<<<<<<
  *                     p[i] = Py_None
  *                     Py_INCREF(Py_None)
  */
       if (unlikely(__pyx_v_itemsize == 0)) {
         PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-        __PYX_ERR(2, 181, __pyx_L1_error)
+        __PYX_ERR(2, 180, __pyx_L1_error)
       }
       else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_self->len))) {
         PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-        __PYX_ERR(2, 181, __pyx_L1_error)
+        __PYX_ERR(2, 180, __pyx_L1_error)
       }
       __pyx_t_1 = __Pyx_div_Py_ssize_t(__pyx_v_self->len, __pyx_v_itemsize);
       __pyx_t_9 = __pyx_t_1;
       for (__pyx_t_11 = 0; __pyx_t_11 < __pyx_t_9; __pyx_t_11+=1) {
         __pyx_v_i = __pyx_t_11;
 
-        /* "View.MemoryView":182
+        /* "View.MemoryView":181
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None             # <<<<<<<<<<<<<<
  *                     Py_INCREF(Py_None)
  * 
  */
         (__pyx_v_p[__pyx_v_i]) = Py_None;
 
-        /* "View.MemoryView":183
+        /* "View.MemoryView":182
  *                 for i in range(self.len / itemsize):
  *                     p[i] = Py_None
  *                     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
         Py_INCREF(Py_None);
       }
 
-      /* "View.MemoryView":179
+      /* "View.MemoryView":178
  *                 raise MemoryError("unable to allocate array data.")
  * 
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 p = <PyObject **> self.data
  *                 for i in range(self.len / itemsize):
  */
     }
 
-    /* "View.MemoryView":172
+    /* "View.MemoryView":171
  *         self.free_data = allocate_buffer
  *         self.dtype_is_object = format == b'O'
  *         if allocate_buffer:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":123
+  /* "View.MemoryView":122
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
  * 
  */
 
@@ -4997,15 +4847,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_format);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":186
+/* "View.MemoryView":185
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  */
 
@@ -5040,249 +4890,249 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":187
+  /* "View.MemoryView":186
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1             # <<<<<<<<<<<<<<
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  */
   __pyx_v_bufmode = -1;
 
-  /* "View.MemoryView":188
+  /* "View.MemoryView":187
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  *         if self.mode == u"c":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_c, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 188, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_c, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 187, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":189
+    /* "View.MemoryView":188
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS             # <<<<<<<<<<<<<<
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  */
     __pyx_v_bufmode = (PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS);
 
-    /* "View.MemoryView":188
+    /* "View.MemoryView":187
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         cdef int bufmode = -1
  *         if self.mode == u"c":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":190
+  /* "View.MemoryView":189
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  */
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_fortran, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 190, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_v_self->mode, __pyx_n_u_fortran, Py_EQ)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 189, __pyx_L1_error)
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":191
+    /* "View.MemoryView":190
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS             # <<<<<<<<<<<<<<
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  */
     __pyx_v_bufmode = (PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS);
 
-    /* "View.MemoryView":190
+    /* "View.MemoryView":189
  *         if self.mode == u"c":
  *             bufmode = PyBUF_C_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         elif self.mode == u"fortran":             # <<<<<<<<<<<<<<
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":192
+  /* "View.MemoryView":191
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):             # <<<<<<<<<<<<<<
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  */
   __pyx_t_1 = ((!((__pyx_v_flags & __pyx_v_bufmode) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":193
+    /* "View.MemoryView":192
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 192, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 193, __pyx_L1_error)
+    __PYX_ERR(2, 192, __pyx_L1_error)
 
-    /* "View.MemoryView":192
+    /* "View.MemoryView":191
  *         elif self.mode == u"fortran":
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):             # <<<<<<<<<<<<<<
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  */
   }
 
-  /* "View.MemoryView":194
+  /* "View.MemoryView":193
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data             # <<<<<<<<<<<<<<
  *         info.len = self.len
  *         info.ndim = self.ndim
  */
   __pyx_t_4 = __pyx_v_self->data;
   __pyx_v_info->buf = __pyx_t_4;
 
-  /* "View.MemoryView":195
+  /* "View.MemoryView":194
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")
  *         info.buf = self.data
  *         info.len = self.len             # <<<<<<<<<<<<<<
  *         info.ndim = self.ndim
  *         info.shape = self._shape
  */
   __pyx_t_5 = __pyx_v_self->len;
   __pyx_v_info->len = __pyx_t_5;
 
-  /* "View.MemoryView":196
+  /* "View.MemoryView":195
  *         info.buf = self.data
  *         info.len = self.len
  *         info.ndim = self.ndim             # <<<<<<<<<<<<<<
  *         info.shape = self._shape
  *         info.strides = self._strides
  */
   __pyx_t_6 = __pyx_v_self->ndim;
   __pyx_v_info->ndim = __pyx_t_6;
 
-  /* "View.MemoryView":197
+  /* "View.MemoryView":196
  *         info.len = self.len
  *         info.ndim = self.ndim
  *         info.shape = self._shape             # <<<<<<<<<<<<<<
  *         info.strides = self._strides
  *         info.suboffsets = NULL
  */
   __pyx_t_7 = __pyx_v_self->_shape;
   __pyx_v_info->shape = __pyx_t_7;
 
-  /* "View.MemoryView":198
+  /* "View.MemoryView":197
  *         info.ndim = self.ndim
  *         info.shape = self._shape
  *         info.strides = self._strides             # <<<<<<<<<<<<<<
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize
  */
   __pyx_t_7 = __pyx_v_self->_strides;
   __pyx_v_info->strides = __pyx_t_7;
 
-  /* "View.MemoryView":199
+  /* "View.MemoryView":198
  *         info.shape = self._shape
  *         info.strides = self._strides
  *         info.suboffsets = NULL             # <<<<<<<<<<<<<<
  *         info.itemsize = self.itemsize
  *         info.readonly = 0
  */
   __pyx_v_info->suboffsets = NULL;
 
-  /* "View.MemoryView":200
+  /* "View.MemoryView":199
  *         info.strides = self._strides
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize             # <<<<<<<<<<<<<<
  *         info.readonly = 0
  * 
  */
   __pyx_t_5 = __pyx_v_self->itemsize;
   __pyx_v_info->itemsize = __pyx_t_5;
 
-  /* "View.MemoryView":201
+  /* "View.MemoryView":200
  *         info.suboffsets = NULL
  *         info.itemsize = self.itemsize
  *         info.readonly = 0             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   __pyx_v_info->readonly = 0;
 
-  /* "View.MemoryView":203
+  /* "View.MemoryView":202
  *         info.readonly = 0
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":204
+    /* "View.MemoryView":203
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_4 = __pyx_v_self->format;
     __pyx_v_info->format = __pyx_t_4;
 
-    /* "View.MemoryView":203
+    /* "View.MemoryView":202
  *         info.readonly = 0
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.format
  *         else:
  */
     goto __pyx_L5;
   }
 
-  /* "View.MemoryView":206
+  /* "View.MemoryView":205
  *             info.format = self.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.obj = self
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L5:;
 
-  /* "View.MemoryView":208
+  /* "View.MemoryView":207
  *             info.format = NULL
  * 
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":186
+  /* "View.MemoryView":185
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         cdef int bufmode = -1
  *         if self.mode == u"c":
  */
 
@@ -5304,15 +5154,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":212
+/* "View.MemoryView":211
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
@@ -5328,122 +5178,122 @@
 }
 
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":213
+  /* "View.MemoryView":212
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  */
   __pyx_t_1 = ((__pyx_v_self->callback_free_data != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":214
+    /* "View.MemoryView":213
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)             # <<<<<<<<<<<<<<
  *         elif self.free_data:
  *             if self.dtype_is_object:
  */
     __pyx_v_self->callback_free_data(__pyx_v_self->data);
 
-    /* "View.MemoryView":213
+    /* "View.MemoryView":212
  * 
  *     def __dealloc__(array self):
  *         if self.callback_free_data != NULL:             # <<<<<<<<<<<<<<
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":215
+  /* "View.MemoryView":214
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  *         elif self.free_data:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,
  */
   __pyx_t_1 = (__pyx_v_self->free_data != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":216
+    /* "View.MemoryView":215
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  */
     __pyx_t_1 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":217
+      /* "View.MemoryView":216
  *         elif self.free_data:
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,             # <<<<<<<<<<<<<<
  *                                           self._strides, self.ndim, False)
  *             free(self.data)
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_self->data, __pyx_v_self->_shape, __pyx_v_self->_strides, __pyx_v_self->ndim, 0);
 
-      /* "View.MemoryView":216
+      /* "View.MemoryView":215
  *             self.callback_free_data(self.data)
  *         elif self.free_data:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  */
     }
 
-    /* "View.MemoryView":219
+    /* "View.MemoryView":218
  *                 refcount_objects_in_slice(self.data, self._shape,
  *                                           self._strides, self.ndim, False)
  *             free(self.data)             # <<<<<<<<<<<<<<
  *         PyObject_Free(self._shape)
  * 
  */
     free(__pyx_v_self->data);
 
-    /* "View.MemoryView":215
+    /* "View.MemoryView":214
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  *         elif self.free_data:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 refcount_objects_in_slice(self.data, self._shape,
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":220
+  /* "View.MemoryView":219
  *                                           self._strides, self.ndim, False)
  *             free(self.data)
  *         PyObject_Free(self._shape)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   PyObject_Free(__pyx_v_self->_shape);
 
-  /* "View.MemoryView":212
+  /* "View.MemoryView":211
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")
  * 
  *     def __dealloc__(array self):             # <<<<<<<<<<<<<<
  *         if self.callback_free_data != NULL:
  *             self.callback_free_data(self.data)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":223
+/* "View.MemoryView":222
  * 
  *     @property
  *     def memview(self):             # <<<<<<<<<<<<<<
  *         return self.get_memview()
  * 
  */
 
@@ -5465,29 +5315,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":224
+  /* "View.MemoryView":223
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
  *     @cname('get_memview')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_array *)__pyx_v_self->__pyx_vtab)->get_memview(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 224, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_array *)__pyx_v_self->__pyx_vtab)->get_memview(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 223, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":223
+  /* "View.MemoryView":222
  * 
  *     @property
  *     def memview(self):             # <<<<<<<<<<<<<<
  *         return self.get_memview()
  * 
  */
 
@@ -5498,15 +5348,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":227
+/* "View.MemoryView":226
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
 
@@ -5518,54 +5368,54 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_memview", 0);
 
-  /* "View.MemoryView":228
+  /* "View.MemoryView":227
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  */
   __pyx_v_flags = ((PyBUF_ANY_CONTIGUOUS | PyBUF_FORMAT) | PyBUF_WRITABLE);
 
-  /* "View.MemoryView":229
+  /* "View.MemoryView":228
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 229, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":227
+  /* "View.MemoryView":226
  * 
  *     @cname('get_memview')
  *     cdef get_memview(self):             # <<<<<<<<<<<<<<
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE
  *         return  memoryview(self, flags, self.dtype_is_object)
  */
 
@@ -5578,15 +5428,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":231
+/* "View.MemoryView":230
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
@@ -5604,39 +5454,39 @@
 }
 
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":232
+  /* "View.MemoryView":231
  * 
  *     def __len__(self):
  *         return self._shape[0]             # <<<<<<<<<<<<<<
  * 
  *     def __getattr__(self, attr):
  */
   __pyx_r = (__pyx_v_self->_shape[0]);
   goto __pyx_L0;
 
-  /* "View.MemoryView":231
+  /* "View.MemoryView":230
  *         return  memoryview(self, flags, self.dtype_is_object)
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         return self._shape[0]
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":234
+/* "View.MemoryView":233
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
@@ -5659,32 +5509,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getattr__", 0);
 
-  /* "View.MemoryView":235
+  /* "View.MemoryView":234
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
  *     def __getitem__(self, item):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 235, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetAttr(__pyx_t_1, __pyx_v_attr); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 235, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetAttr(__pyx_t_1, __pyx_v_attr); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 234, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":234
+  /* "View.MemoryView":233
  *         return self._shape[0]
  * 
  *     def __getattr__(self, attr):             # <<<<<<<<<<<<<<
  *         return getattr(self.memview, attr)
  * 
  */
 
@@ -5696,15 +5546,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":237
+/* "View.MemoryView":236
  *         return getattr(self.memview, attr)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.memview[item]
  * 
  */
 
@@ -5727,32 +5577,32 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":238
+  /* "View.MemoryView":237
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(self, item, value):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 238, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetItem(__pyx_t_1, __pyx_v_item); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 237, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":237
+  /* "View.MemoryView":236
  *         return getattr(self.memview, attr)
  * 
  *     def __getitem__(self, item):             # <<<<<<<<<<<<<<
  *         return self.memview[item]
  * 
  */
 
@@ -5764,15 +5614,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":240
+/* "View.MemoryView":239
  *         return self.memview[item]
  * 
  *     def __setitem__(self, item, value):             # <<<<<<<<<<<<<<
  *         self.memview[item] = value
  * 
  */
 
@@ -5794,27 +5644,27 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
 
-  /* "View.MemoryView":241
+  /* "View.MemoryView":240
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 241, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_memview); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_item, __pyx_v_value) < 0)) __PYX_ERR(2, 241, __pyx_L1_error)
+  if (unlikely(PyObject_SetItem(__pyx_t_1, __pyx_v_item, __pyx_v_value) < 0)) __PYX_ERR(2, 240, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":240
+  /* "View.MemoryView":239
  *         return self.memview[item]
  * 
  *     def __setitem__(self, item, value):             # <<<<<<<<<<<<<<
  *         self.memview[item] = value
  * 
  */
 
@@ -5939,15 +5789,15 @@
   __Pyx_AddTraceback("View.MemoryView.array.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":245
+/* "View.MemoryView":244
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
 
@@ -5961,145 +5811,145 @@
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("array_cwrapper", 0);
 
-  /* "View.MemoryView":249
+  /* "View.MemoryView":248
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_buf == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":250
+    /* "View.MemoryView":249
  * 
  *     if buf == NULL:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))             # <<<<<<<<<<<<<<
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 250, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 250, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 250, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 250, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(4); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_v_shape);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 3, __pyx_t_4);
     __pyx_t_2 = 0;
     __pyx_t_3 = 0;
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 250, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_5, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 249, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":249
+    /* "View.MemoryView":248
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":252
+  /* "View.MemoryView":251
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),             # <<<<<<<<<<<<<<
  *                        allocate_buffer=False)
  *         result.data = buf
  */
   /*else*/ {
-    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 252, __pyx_L1_error)
+    __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_itemsize); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 252, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyBytes_FromString(__pyx_v_format); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 252, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_mode, 0, strlen(__pyx_v_mode), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 252, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(4); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_v_shape);
     __Pyx_GIVEREF(__pyx_v_shape);
     PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_shape);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_5);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_2, 3, __pyx_t_3);
     __pyx_t_4 = 0;
     __pyx_t_5 = 0;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":253
+    /* "View.MemoryView":252
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  *                        allocate_buffer=False)             # <<<<<<<<<<<<<<
  *         result.data = buf
  * 
  */
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 253, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 252, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(2, 253, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_allocate_buffer, Py_False) < 0) __PYX_ERR(2, 252, __pyx_L1_error)
 
-    /* "View.MemoryView":252
+    /* "View.MemoryView":251
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
  *     else:
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),             # <<<<<<<<<<<<<<
  *                        allocate_buffer=False)
  *         result.data = buf
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 252, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_array_type), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 251, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result = ((struct __pyx_array_obj *)__pyx_t_5);
     __pyx_t_5 = 0;
 
-    /* "View.MemoryView":254
+    /* "View.MemoryView":253
  *         result = array(shape, itemsize, format, mode.decode('ASCII'),
  *                        allocate_buffer=False)
  *         result.data = buf             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
     __pyx_v_result->data = __pyx_v_buf;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":256
+  /* "View.MemoryView":255
  *         result.data = buf
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(((PyObject *)__pyx_r));
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":245
+  /* "View.MemoryView":244
  * 
  * @cname("__pyx_array_new")
  * cdef array array_cwrapper(tuple shape, Py_ssize_t itemsize, char *format,             # <<<<<<<<<<<<<<
  *                           char *mode, char *buf):
  *     cdef array result
  */
 
@@ -6114,15 +5964,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":282
+/* "View.MemoryView":281
  * cdef class Enum(object):
  *     cdef object name
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *     def __repr__(self):
  */
 
@@ -6151,26 +6001,26 @@
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(2, 282, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(2, 281, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_name = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 282, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 281, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.Enum.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(((struct __pyx_MemviewEnum_obj *)__pyx_v_self), __pyx_v_name);
 
@@ -6180,42 +6030,42 @@
 }
 
 static int __pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum___init__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v_name) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "View.MemoryView":283
+  /* "View.MemoryView":282
  *     cdef object name
  *     def __init__(self, name):
  *         self.name = name             # <<<<<<<<<<<<<<
  *     def __repr__(self):
  *         return self.name
  */
   __Pyx_INCREF(__pyx_v_name);
   __Pyx_GIVEREF(__pyx_v_name);
   __Pyx_GOTREF(__pyx_v_self->name);
   __Pyx_DECREF(__pyx_v_self->name);
   __pyx_v_self->name = __pyx_v_name;
 
-  /* "View.MemoryView":282
+  /* "View.MemoryView":281
  * cdef class Enum(object):
  *     cdef object name
  *     def __init__(self, name):             # <<<<<<<<<<<<<<
  *         self.name = name
  *     def __repr__(self):
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":284
+/* "View.MemoryView":283
  *     def __init__(self, name):
  *         self.name = name
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -6233,27 +6083,27 @@
 }
 
 static PyObject *__pyx_MemviewEnum___pyx_pf_15View_dot_MemoryView_4Enum_2__repr__(struct __pyx_MemviewEnum_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":285
+  /* "View.MemoryView":284
  *         self.name = name
  *     def __repr__(self):
  *         return self.name             # <<<<<<<<<<<<<<
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->name);
   __pyx_r = __pyx_v_self->name;
   goto __pyx_L0;
 
-  /* "View.MemoryView":284
+  /* "View.MemoryView":283
  *     def __init__(self, name):
  *         self.name = name
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return self.name
  * 
  */
 
@@ -6553,98 +6403,98 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":299
+/* "View.MemoryView":298
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
 
 static void *__pyx_align_pointer(void *__pyx_v_memory, size_t __pyx_v_alignment) {
   Py_intptr_t __pyx_v_aligned_p;
   size_t __pyx_v_offset;
   void *__pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":301
+  /* "View.MemoryView":300
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory             # <<<<<<<<<<<<<<
  *     cdef size_t offset
  * 
  */
   __pyx_v_aligned_p = ((Py_intptr_t)__pyx_v_memory);
 
-  /* "View.MemoryView":305
+  /* "View.MemoryView":304
  * 
  *     with cython.cdivision(True):
  *         offset = aligned_p % alignment             # <<<<<<<<<<<<<<
  * 
  *     if offset > 0:
  */
   __pyx_v_offset = (__pyx_v_aligned_p % __pyx_v_alignment);
 
-  /* "View.MemoryView":307
+  /* "View.MemoryView":306
  *         offset = aligned_p % alignment
  * 
  *     if offset > 0:             # <<<<<<<<<<<<<<
  *         aligned_p += alignment - offset
  * 
  */
   __pyx_t_1 = ((__pyx_v_offset > 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":308
+    /* "View.MemoryView":307
  * 
  *     if offset > 0:
  *         aligned_p += alignment - offset             # <<<<<<<<<<<<<<
  * 
  *     return <void *> aligned_p
  */
     __pyx_v_aligned_p = (__pyx_v_aligned_p + (__pyx_v_alignment - __pyx_v_offset));
 
-    /* "View.MemoryView":307
+    /* "View.MemoryView":306
  *         offset = aligned_p % alignment
  * 
  *     if offset > 0:             # <<<<<<<<<<<<<<
  *         aligned_p += alignment - offset
  * 
  */
   }
 
-  /* "View.MemoryView":310
+  /* "View.MemoryView":309
  *         aligned_p += alignment - offset
  * 
  *     return <void *> aligned_p             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((void *)__pyx_v_aligned_p);
   goto __pyx_L0;
 
-  /* "View.MemoryView":299
+  /* "View.MemoryView":298
  * 
  * @cname('__pyx_align_pointer')
  * cdef void *align_pointer(void *memory, size_t alignment) nogil:             # <<<<<<<<<<<<<<
  *     "Align pointer memory on a given boundary"
  *     cdef Py_intptr_t aligned_p = <Py_intptr_t> memory
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":346
+/* "View.MemoryView":345
  *     cdef __Pyx_TypeInfo *typeinfo
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):             # <<<<<<<<<<<<<<
  *         self.obj = obj
  *         self.flags = flags
  */
 
@@ -6681,47 +6531,47 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_obj)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_flags)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(2, 346, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, 1); __PYX_ERR(2, 345, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_dtype_is_object);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 346, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(2, 345, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_obj = values[0];
-    __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 346, __pyx_L3_error)
+    __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 345, __pyx_L3_error)
     if (values[2]) {
-      __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 346, __pyx_L3_error)
+      __pyx_v_dtype_is_object = __Pyx_PyObject_IsTrue(values[2]); if (unlikely((__pyx_v_dtype_is_object == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 345, __pyx_L3_error)
     } else {
       __pyx_v_dtype_is_object = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 346, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(2, 345, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("View.MemoryView.memoryview.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview___cinit__(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_obj, __pyx_v_flags, __pyx_v_dtype_is_object);
 
@@ -6738,37 +6588,37 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "View.MemoryView":347
+  /* "View.MemoryView":346
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
  */
   __Pyx_INCREF(__pyx_v_obj);
   __Pyx_GIVEREF(__pyx_v_obj);
   __Pyx_GOTREF(__pyx_v_self->obj);
   __Pyx_DECREF(__pyx_v_self->obj);
   __pyx_v_self->obj = __pyx_v_obj;
 
-  /* "View.MemoryView":348
+  /* "View.MemoryView":347
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj
  *         self.flags = flags             # <<<<<<<<<<<<<<
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  */
   __pyx_v_self->flags = __pyx_v_flags;
 
-  /* "View.MemoryView":349
+  /* "View.MemoryView":348
  *         self.obj = obj
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  */
   __pyx_t_2 = (((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))) == ((PyObject *)__pyx_memoryview_type));
@@ -6780,250 +6630,231 @@
   }
   __pyx_t_3 = (__pyx_v_obj != Py_None);
   __pyx_t_2 = (__pyx_t_3 != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":350
+    /* "View.MemoryView":349
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)             # <<<<<<<<<<<<<<
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  */
-    __pyx_t_4 = __Pyx_GetBuffer(__pyx_v_obj, (&__pyx_v_self->view), __pyx_v_flags); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 350, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetBuffer(__pyx_v_obj, (&__pyx_v_self->view), __pyx_v_flags); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 349, __pyx_L1_error)
 
-    /* "View.MemoryView":351
+    /* "View.MemoryView":350
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:             # <<<<<<<<<<<<<<
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)
  */
     __pyx_t_1 = ((((PyObject *)__pyx_v_self->view.obj) == NULL) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":352
+      /* "View.MemoryView":351
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None             # <<<<<<<<<<<<<<
  *                 Py_INCREF(Py_None)
  * 
  */
       ((Py_buffer *)(&__pyx_v_self->view))->obj = Py_None;
 
-      /* "View.MemoryView":353
+      /* "View.MemoryView":352
  *             if <PyObject *> self.view.obj == NULL:
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
- *         if not __PYX_CYTHON_ATOMICS_ENABLED():
+ *         global __pyx_memoryview_thread_locks_used
  */
       Py_INCREF(Py_None);
 
-      /* "View.MemoryView":351
+      /* "View.MemoryView":350
  *         if type(self) is memoryview or obj is not None:
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:             # <<<<<<<<<<<<<<
  *                 (<__pyx_buffer *> &self.view).obj = Py_None
  *                 Py_INCREF(Py_None)
  */
     }
 
-    /* "View.MemoryView":349
+    /* "View.MemoryView":348
  *         self.obj = obj
  *         self.flags = flags
  *         if type(self) is memoryview or obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_GetBuffer(obj, &self.view, flags)
  *             if <PyObject *> self.view.obj == NULL:
  */
   }
 
   /* "View.MemoryView":355
- *                 Py_INCREF(Py_None)
  * 
- *         if not __PYX_CYTHON_ATOMICS_ENABLED():             # <<<<<<<<<<<<<<
- *             global __pyx_memoryview_thread_locks_used
- *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *         global __pyx_memoryview_thread_locks_used
+ *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
+ *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *             __pyx_memoryview_thread_locks_used += 1
  */
-  __pyx_t_1 = ((!(__PYX_CYTHON_ATOMICS_ENABLED() != 0)) != 0);
+  __pyx_t_1 = ((__pyx_memoryview_thread_locks_used < 8) != 0);
   if (__pyx_t_1) {
 
+    /* "View.MemoryView":356
+ *         global __pyx_memoryview_thread_locks_used
+ *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]             # <<<<<<<<<<<<<<
+ *             __pyx_memoryview_thread_locks_used += 1
+ *         if self.lock is NULL:
+ */
+    __pyx_v_self->lock = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
+
     /* "View.MemoryView":357
- *         if not __PYX_CYTHON_ATOMICS_ENABLED():
- *             global __pyx_memoryview_thread_locks_used
- *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
- *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *                 __pyx_memoryview_thread_locks_used += 1
+ *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+ *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *             __pyx_memoryview_thread_locks_used += 1             # <<<<<<<<<<<<<<
+ *         if self.lock is NULL:
+ *             self.lock = PyThread_allocate_lock()
  */
-    __pyx_t_1 = ((__pyx_memoryview_thread_locks_used < 8) != 0);
-    if (__pyx_t_1) {
+    __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used + 1);
 
-      /* "View.MemoryView":358
- *             global __pyx_memoryview_thread_locks_used
- *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
- *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]             # <<<<<<<<<<<<<<
- *                 __pyx_memoryview_thread_locks_used += 1
- *             if self.lock is NULL:
+    /* "View.MemoryView":355
+ * 
+ *         global __pyx_memoryview_thread_locks_used
+ *         if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
+ *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *             __pyx_memoryview_thread_locks_used += 1
  */
-      __pyx_v_self->lock = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
+  }
 
-      /* "View.MemoryView":359
- *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
- *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *                 __pyx_memoryview_thread_locks_used += 1             # <<<<<<<<<<<<<<
+  /* "View.MemoryView":358
+ *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *             __pyx_memoryview_thread_locks_used += 1
+ *         if self.lock is NULL:             # <<<<<<<<<<<<<<
+ *             self.lock = PyThread_allocate_lock()
  *             if self.lock is NULL:
- *                 self.lock = PyThread_allocate_lock()
  */
-      __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used + 1);
+  __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
+  if (__pyx_t_1) {
 
-      /* "View.MemoryView":357
- *         if not __PYX_CYTHON_ATOMICS_ENABLED():
- *             global __pyx_memoryview_thread_locks_used
- *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:             # <<<<<<<<<<<<<<
- *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *                 __pyx_memoryview_thread_locks_used += 1
+    /* "View.MemoryView":359
+ *             __pyx_memoryview_thread_locks_used += 1
+ *         if self.lock is NULL:
+ *             self.lock = PyThread_allocate_lock()             # <<<<<<<<<<<<<<
+ *             if self.lock is NULL:
+ *                 raise MemoryError
  */
-    }
+    __pyx_v_self->lock = PyThread_allocate_lock();
 
     /* "View.MemoryView":360
- *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *                 __pyx_memoryview_thread_locks_used += 1
+ *         if self.lock is NULL:
+ *             self.lock = PyThread_allocate_lock()
  *             if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                 self.lock = PyThread_allocate_lock()
- *                 if self.lock is NULL:
+ *                 raise MemoryError
+ * 
  */
     __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
-    if (__pyx_t_1) {
+    if (unlikely(__pyx_t_1)) {
 
       /* "View.MemoryView":361
- *                 __pyx_memoryview_thread_locks_used += 1
- *             if self.lock is NULL:
- *                 self.lock = PyThread_allocate_lock()             # <<<<<<<<<<<<<<
- *                 if self.lock is NULL:
- *                     raise MemoryError
- */
-      __pyx_v_self->lock = PyThread_allocate_lock();
-
-      /* "View.MemoryView":362
+ *             self.lock = PyThread_allocate_lock()
  *             if self.lock is NULL:
- *                 self.lock = PyThread_allocate_lock()
- *                 if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                     raise MemoryError
- * 
- */
-      __pyx_t_1 = ((__pyx_v_self->lock == NULL) != 0);
-      if (unlikely(__pyx_t_1)) {
-
-        /* "View.MemoryView":363
- *                 self.lock = PyThread_allocate_lock()
- *                 if self.lock is NULL:
- *                     raise MemoryError             # <<<<<<<<<<<<<<
+ *                 raise MemoryError             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
-        PyErr_NoMemory(); __PYX_ERR(2, 363, __pyx_L1_error)
-
-        /* "View.MemoryView":362
- *             if self.lock is NULL:
- *                 self.lock = PyThread_allocate_lock()
- *                 if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                     raise MemoryError
- * 
- */
-      }
+      PyErr_NoMemory(); __PYX_ERR(2, 361, __pyx_L1_error)
 
       /* "View.MemoryView":360
- *                 self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
- *                 __pyx_memoryview_thread_locks_used += 1
+ *         if self.lock is NULL:
+ *             self.lock = PyThread_allocate_lock()
  *             if self.lock is NULL:             # <<<<<<<<<<<<<<
- *                 self.lock = PyThread_allocate_lock()
- *                 if self.lock is NULL:
+ *                 raise MemoryError
+ * 
  */
     }
 
-    /* "View.MemoryView":355
- *                 Py_INCREF(Py_None)
- * 
- *         if not __PYX_CYTHON_ATOMICS_ENABLED():             # <<<<<<<<<<<<<<
- *             global __pyx_memoryview_thread_locks_used
- *             if __pyx_memoryview_thread_locks_used < THREAD_LOCKS_PREALLOCATED:
+    /* "View.MemoryView":358
+ *             self.lock = __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]
+ *             __pyx_memoryview_thread_locks_used += 1
+ *         if self.lock is NULL:             # <<<<<<<<<<<<<<
+ *             self.lock = PyThread_allocate_lock()
+ *             if self.lock is NULL:
  */
   }
 
-  /* "View.MemoryView":365
- *                     raise MemoryError
+  /* "View.MemoryView":363
+ *                 raise MemoryError
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":366
+    /* "View.MemoryView":364
  * 
  *         if flags & PyBUF_FORMAT:
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')             # <<<<<<<<<<<<<<
  *         else:
  *             self.dtype_is_object = dtype_is_object
  */
     __pyx_t_2 = (((__pyx_v_self->view.format[0]) == 'O') != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
-      goto __pyx_L12_bool_binop_done;
+      goto __pyx_L11_bool_binop_done;
     }
     __pyx_t_2 = (((__pyx_v_self->view.format[1]) == '\x00') != 0);
     __pyx_t_1 = __pyx_t_2;
-    __pyx_L12_bool_binop_done:;
+    __pyx_L11_bool_binop_done:;
     __pyx_v_self->dtype_is_object = __pyx_t_1;
 
-    /* "View.MemoryView":365
- *                     raise MemoryError
+    /* "View.MemoryView":363
+ *                 raise MemoryError
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  */
-    goto __pyx_L11;
+    goto __pyx_L10;
   }
 
-  /* "View.MemoryView":368
+  /* "View.MemoryView":366
  *             self.dtype_is_object = (self.view.format[0] == b'O' and self.view.format[1] == b'\0')
  *         else:
  *             self.dtype_is_object = dtype_is_object             # <<<<<<<<<<<<<<
  * 
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(
  */
   /*else*/ {
     __pyx_v_self->dtype_is_object = __pyx_v_dtype_is_object;
   }
-  __pyx_L11:;
+  __pyx_L10:;
 
-  /* "View.MemoryView":370
+  /* "View.MemoryView":368
  *             self.dtype_is_object = dtype_is_object
  * 
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(             # <<<<<<<<<<<<<<
  *                   <void *> &self.acquisition_count[0], sizeof(__pyx_atomic_int))
  *         self.typeinfo = NULL
  */
   __pyx_v_self->acquisition_count_aligned_p = ((__pyx_atomic_int *)__pyx_align_pointer(((void *)(&(__pyx_v_self->acquisition_count[0]))), (sizeof(__pyx_atomic_int))));
 
-  /* "View.MemoryView":372
+  /* "View.MemoryView":370
  *         self.acquisition_count_aligned_p = <__pyx_atomic_int *> align_pointer(
  *                   <void *> &self.acquisition_count[0], sizeof(__pyx_atomic_int))
  *         self.typeinfo = NULL             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(memoryview self):
  */
   __pyx_v_self->typeinfo = NULL;
 
-  /* "View.MemoryView":346
+  /* "View.MemoryView":345
  *     cdef __Pyx_TypeInfo *typeinfo
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):             # <<<<<<<<<<<<<<
  *         self.obj = obj
  *         self.flags = flags
  */
 
@@ -7034,15 +6865,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":374
+/* "View.MemoryView":372
  *         self.typeinfo = NULL
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
@@ -7065,215 +6896,215 @@
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   PyThread_type_lock __pyx_t_6;
   PyThread_type_lock __pyx_t_7;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":375
+  /* "View.MemoryView":373
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  */
   __pyx_t_1 = (__pyx_v_self->obj != Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":376
+    /* "View.MemoryView":374
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)             # <<<<<<<<<<<<<<
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
  */
     __Pyx_ReleaseBuffer((&__pyx_v_self->view));
 
-    /* "View.MemoryView":375
+    /* "View.MemoryView":373
  * 
  *     def __dealloc__(memoryview self):
  *         if self.obj is not None:             # <<<<<<<<<<<<<<
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":377
+  /* "View.MemoryView":375
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   __pyx_t_2 = ((((Py_buffer *)(&__pyx_v_self->view))->obj == Py_None) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":379
+    /* "View.MemoryView":377
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL             # <<<<<<<<<<<<<<
  *             Py_DECREF(Py_None)
  * 
  */
     ((Py_buffer *)(&__pyx_v_self->view))->obj = NULL;
 
-    /* "View.MemoryView":380
+    /* "View.MemoryView":378
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  *             Py_DECREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *         cdef int i
  */
     Py_DECREF(Py_None);
 
-    /* "View.MemoryView":377
+    /* "View.MemoryView":375
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  *         elif (<__pyx_buffer *> &self.view).obj == Py_None:             # <<<<<<<<<<<<<<
  * 
  *             (<__pyx_buffer *> &self.view).obj = NULL
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":384
+  /* "View.MemoryView":382
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   __pyx_t_2 = ((__pyx_v_self->lock != NULL) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":385
+    /* "View.MemoryView":383
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):             # <<<<<<<<<<<<<<
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  */
     __pyx_t_3 = __pyx_memoryview_thread_locks_used;
     __pyx_t_4 = __pyx_t_3;
     for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
       __pyx_v_i = __pyx_t_5;
 
-      /* "View.MemoryView":386
+      /* "View.MemoryView":384
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       __pyx_t_2 = (((__pyx_memoryview_thread_locks[__pyx_v_i]) == __pyx_v_self->lock) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":387
+        /* "View.MemoryView":385
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1             # <<<<<<<<<<<<<<
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  */
         __pyx_memoryview_thread_locks_used = (__pyx_memoryview_thread_locks_used - 1);
 
-        /* "View.MemoryView":388
+        /* "View.MemoryView":386
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         __pyx_t_2 = ((__pyx_v_i != __pyx_memoryview_thread_locks_used) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":390
+          /* "View.MemoryView":388
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])             # <<<<<<<<<<<<<<
  *                     break
  *             else:
  */
           __pyx_t_6 = (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]);
           __pyx_t_7 = (__pyx_memoryview_thread_locks[__pyx_v_i]);
 
-          /* "View.MemoryView":389
+          /* "View.MemoryView":387
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (             # <<<<<<<<<<<<<<
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break
  */
           (__pyx_memoryview_thread_locks[__pyx_v_i]) = __pyx_t_6;
           (__pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used]) = __pyx_t_7;
 
-          /* "View.MemoryView":388
+          /* "View.MemoryView":386
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:             # <<<<<<<<<<<<<<
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  */
         }
 
-        /* "View.MemoryView":391
+        /* "View.MemoryView":389
  *                         __pyx_memoryview_thread_locks[i], __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used] = (
  *                             __pyx_memoryview_thread_locks[__pyx_memoryview_thread_locks_used], __pyx_memoryview_thread_locks[i])
  *                     break             # <<<<<<<<<<<<<<
  *             else:
  *                 PyThread_free_lock(self.lock)
  */
         goto __pyx_L6_break;
 
-        /* "View.MemoryView":386
+        /* "View.MemoryView":384
  *         if self.lock != NULL:
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:             # <<<<<<<<<<<<<<
  *                     __pyx_memoryview_thread_locks_used -= 1
  *                     if i != __pyx_memoryview_thread_locks_used:
  */
       }
     }
     /*else*/ {
 
-      /* "View.MemoryView":393
+      /* "View.MemoryView":391
  *                     break
  *             else:
  *                 PyThread_free_lock(self.lock)             # <<<<<<<<<<<<<<
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  */
       PyThread_free_lock(__pyx_v_self->lock);
     }
     __pyx_L6_break:;
 
-    /* "View.MemoryView":384
+    /* "View.MemoryView":382
  *         cdef int i
  *         global __pyx_memoryview_thread_locks_used
  *         if self.lock != NULL:             # <<<<<<<<<<<<<<
  *             for i in range(__pyx_memoryview_thread_locks_used):
  *                 if __pyx_memoryview_thread_locks[i] is self.lock:
  */
   }
 
-  /* "View.MemoryView":374
+  /* "View.MemoryView":372
  *         self.typeinfo = NULL
  * 
  *     def __dealloc__(memoryview self):             # <<<<<<<<<<<<<<
  *         if self.obj is not None:
  *             __Pyx_ReleaseBuffer(&self.view)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":395
+/* "View.MemoryView":393
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -7291,107 +7122,107 @@
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_item_pointer", 0);
 
-  /* "View.MemoryView":397
+  /* "View.MemoryView":395
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
  *         for dim, idx in enumerate(index):
  */
   __pyx_v_itemp = ((char *)__pyx_v_self->view.buf);
 
-  /* "View.MemoryView":399
+  /* "View.MemoryView":397
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   __pyx_t_1 = 0;
   if (likely(PyList_CheckExact(__pyx_v_index)) || PyTuple_CheckExact(__pyx_v_index)) {
     __pyx_t_2 = __pyx_v_index; __Pyx_INCREF(__pyx_t_2); __pyx_t_3 = 0;
     __pyx_t_4 = NULL;
   } else {
-    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 399, __pyx_L1_error)
+    __pyx_t_3 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 397, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 399, __pyx_L1_error)
+    __pyx_t_4 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 397, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_4)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_3 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 399, __pyx_L1_error)
+        __pyx_t_5 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 397, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 399, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 397, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       } else {
         if (__pyx_t_3 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 399, __pyx_L1_error)
+        __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_3); __Pyx_INCREF(__pyx_t_5); __pyx_t_3++; if (unlikely(0 < 0)) __PYX_ERR(2, 397, __pyx_L1_error)
         #else
-        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 399, __pyx_L1_error)
+        __pyx_t_5 = PySequence_ITEM(__pyx_t_2, __pyx_t_3); __pyx_t_3++; if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 397, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         #endif
       }
     } else {
       __pyx_t_5 = __pyx_t_4(__pyx_t_2);
       if (unlikely(!__pyx_t_5)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 399, __pyx_L1_error)
+          else __PYX_ERR(2, 397, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_5);
     }
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_5);
     __pyx_t_5 = 0;
     __pyx_v_dim = __pyx_t_1;
     __pyx_t_1 = (__pyx_t_1 + 1);
 
-    /* "View.MemoryView":400
+    /* "View.MemoryView":398
  * 
  *         for dim, idx in enumerate(index):
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)             # <<<<<<<<<<<<<<
  * 
  *         return itemp
  */
-    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 400, __pyx_L1_error)
-    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(2, 400, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyIndex_AsSsize_t(__pyx_v_idx); if (unlikely((__pyx_t_6 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 398, __pyx_L1_error)
+    __pyx_t_7 = __pyx_pybuffer_index((&__pyx_v_self->view), __pyx_v_itemp, __pyx_t_6, __pyx_v_dim); if (unlikely(__pyx_t_7 == ((char *)NULL))) __PYX_ERR(2, 398, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_7;
 
-    /* "View.MemoryView":399
+    /* "View.MemoryView":397
  *         cdef char *itemp = <char *> self.view.buf
  * 
  *         for dim, idx in enumerate(index):             # <<<<<<<<<<<<<<
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":402
+  /* "View.MemoryView":400
  *             itemp = pybuffer_index(&self.view, itemp, idx, dim)
  * 
  *         return itemp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_itemp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":395
+  /* "View.MemoryView":393
  *                 PyThread_free_lock(self.lock)
  * 
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:             # <<<<<<<<<<<<<<
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf
  */
 
@@ -7403,15 +7234,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":405
+/* "View.MemoryView":403
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -7441,143 +7272,143 @@
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
-  /* "View.MemoryView":406
+  /* "View.MemoryView":404
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   __pyx_t_1 = (__pyx_v_index == __pyx_builtin_Ellipsis);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":407
+    /* "View.MemoryView":405
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:
  *             return self             # <<<<<<<<<<<<<<
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __pyx_r = ((PyObject *)__pyx_v_self);
     goto __pyx_L0;
 
-    /* "View.MemoryView":406
+    /* "View.MemoryView":404
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
  * 
  */
   }
 
-  /* "View.MemoryView":409
+  /* "View.MemoryView":407
  *             return self
  * 
  *         have_slices, indices = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         cdef char *itemp
  */
-  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 409, __pyx_L1_error)
+  __pyx_t_3 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (likely(__pyx_t_3 != Py_None)) {
     PyObject* sequence = __pyx_t_3;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(2, 409, __pyx_L1_error)
+      __PYX_ERR(2, 407, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_t_5);
     #else
-    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 409, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 409, __pyx_L1_error)
+    __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     #endif
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 409, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 407, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_v_indices = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "View.MemoryView":412
+  /* "View.MemoryView":410
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 412, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 410, __pyx_L1_error)
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":413
+    /* "View.MemoryView":411
  *         cdef char *itemp
  *         if have_slices:
  *             return memview_slice(self, indices)             # <<<<<<<<<<<<<<
  *         else:
  *             itemp = self.get_item_pointer(indices)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 413, __pyx_L1_error)
+    __pyx_t_3 = ((PyObject *)__pyx_memview_slice(__pyx_v_self, __pyx_v_indices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":412
+    /* "View.MemoryView":410
  * 
  *         cdef char *itemp
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             return memview_slice(self, indices)
  *         else:
  */
   }
 
-  /* "View.MemoryView":415
+  /* "View.MemoryView":413
  *             return memview_slice(self, indices)
  *         else:
  *             itemp = self.get_item_pointer(indices)             # <<<<<<<<<<<<<<
  *             return self.convert_item_to_object(itemp)
  * 
  */
   /*else*/ {
-    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(2, 415, __pyx_L1_error)
+    __pyx_t_6 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_indices); if (unlikely(__pyx_t_6 == ((char *)NULL))) __PYX_ERR(2, 413, __pyx_L1_error)
     __pyx_v_itemp = __pyx_t_6;
 
-    /* "View.MemoryView":416
+    /* "View.MemoryView":414
  *         else:
  *             itemp = self.get_item_pointer(indices)
  *             return self.convert_item_to_object(itemp)             # <<<<<<<<<<<<<<
  * 
  *     def __setitem__(memoryview self, object index, object value):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 416, __pyx_L1_error)
+    __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->convert_item_to_object(__pyx_v_self, __pyx_v_itemp); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":405
+  /* "View.MemoryView":403
  * 
  * 
  *     def __getitem__(memoryview self, object index):             # <<<<<<<<<<<<<<
  *         if index is Ellipsis:
  *             return self
  */
 
@@ -7592,15 +7423,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_indices);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":418
+/* "View.MemoryView":416
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -7628,182 +7459,182 @@
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
-  /* "View.MemoryView":419
+  /* "View.MemoryView":417
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   __pyx_t_1 = (__pyx_v_self->view.readonly != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":420
+    /* "View.MemoryView":418
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 420, __pyx_L1_error)
+    __PYX_ERR(2, 418, __pyx_L1_error)
 
-    /* "View.MemoryView":419
+    /* "View.MemoryView":417
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":422
+  /* "View.MemoryView":420
  *             raise TypeError("Cannot assign to read-only memoryview")
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *         if have_slices:
  */
-  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 422, __pyx_L1_error)
+  __pyx_t_2 = _unellipsify(__pyx_v_index, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 420, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(__pyx_t_2 != Py_None)) {
     PyObject* sequence = __pyx_t_2;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(2, 422, __pyx_L1_error)
+      __PYX_ERR(2, 420, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     __pyx_t_3 = PyTuple_GET_ITEM(sequence, 0); 
     __pyx_t_4 = PyTuple_GET_ITEM(sequence, 1); 
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 422, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 422, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else {
-    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 422, __pyx_L1_error)
+    __Pyx_RaiseNoneNotIterableError(); __PYX_ERR(2, 420, __pyx_L1_error)
   }
   __pyx_v_have_slices = __pyx_t_3;
   __pyx_t_3 = 0;
   __Pyx_DECREF_SET(__pyx_v_index, __pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "View.MemoryView":424
+  /* "View.MemoryView":422
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 424, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_have_slices); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 422, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":425
+    /* "View.MemoryView":423
  * 
  *         if have_slices:
  *             obj = self.is_slice(value)             # <<<<<<<<<<<<<<
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)
  */
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 425, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->is_slice(__pyx_v_self, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 423, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_v_obj = __pyx_t_2;
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":426
+    /* "View.MemoryView":424
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 426, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_obj); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 424, __pyx_L1_error)
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":427
+      /* "View.MemoryView":425
  *             obj = self.is_slice(value)
  *             if obj:
  *                 self.setitem_slice_assignment(self[index], obj)             # <<<<<<<<<<<<<<
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)
  */
-      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 427, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 425, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 427, __pyx_L1_error)
+      __pyx_t_4 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assignment(__pyx_v_self, __pyx_t_2, __pyx_v_obj); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 425, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-      /* "View.MemoryView":426
+      /* "View.MemoryView":424
  *         if have_slices:
  *             obj = self.is_slice(value)
  *             if obj:             # <<<<<<<<<<<<<<
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":429
+    /* "View.MemoryView":427
  *                 self.setitem_slice_assignment(self[index], obj)
  *             else:
  *                 self.setitem_slice_assign_scalar(self[index], value)             # <<<<<<<<<<<<<<
  *         else:
  *             self.setitem_indexed(index, value)
  */
     /*else*/ {
-      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 429, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_self), __pyx_v_index); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(2, 429, __pyx_L1_error)
-      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 429, __pyx_L1_error)
+      if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_memoryview_type))))) __PYX_ERR(2, 427, __pyx_L1_error)
+      __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_slice_assign_scalar(__pyx_v_self, ((struct __pyx_memoryview_obj *)__pyx_t_4), __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 427, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":424
+    /* "View.MemoryView":422
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  * 
  *         if have_slices:             # <<<<<<<<<<<<<<
  *             obj = self.is_slice(value)
  *             if obj:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":431
+  /* "View.MemoryView":429
  *                 self.setitem_slice_assign_scalar(self[index], value)
  *         else:
  *             self.setitem_indexed(index, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef is_slice(self, obj):
  */
   /*else*/ {
-    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 431, __pyx_L1_error)
+    __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->setitem_indexed(__pyx_v_self, __pyx_v_index, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 429, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":418
+  /* "View.MemoryView":416
  *             return self.convert_item_to_object(itemp)
  * 
  *     def __setitem__(memoryview self, object index, object value):             # <<<<<<<<<<<<<<
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")
  */
 
@@ -7820,15 +7651,15 @@
   __Pyx_XDECREF(__pyx_v_have_slices);
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":433
+/* "View.MemoryView":431
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -7846,26 +7677,26 @@
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_slice", 0);
   __Pyx_INCREF(__pyx_v_obj);
 
-  /* "View.MemoryView":434
+  /* "View.MemoryView":432
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_obj, __pyx_memoryview_type); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":435
+    /* "View.MemoryView":433
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
     {
@@ -7873,59 +7704,59 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_3);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       /*try:*/ {
 
-        /* "View.MemoryView":436
+        /* "View.MemoryView":434
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 436, __pyx_L4_error)
+        __pyx_t_6 = __Pyx_PyInt_From_int(((__pyx_v_self->flags & (~PyBUF_WRITABLE)) | PyBUF_ANY_CONTIGUOUS)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 434, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":437
+        /* "View.MemoryView":435
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)             # <<<<<<<<<<<<<<
  *             except TypeError:
  *                 return None
  */
-        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 437, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyBool_FromLong(__pyx_v_self->dtype_is_object); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 435, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
 
-        /* "View.MemoryView":436
+        /* "View.MemoryView":434
  *         if not isinstance(obj, memoryview):
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,             # <<<<<<<<<<<<<<
  *                                  self.dtype_is_object)
  *             except TypeError:
  */
-        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 436, __pyx_L4_error)
+        __pyx_t_8 = PyTuple_New(3); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 434, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_INCREF(__pyx_v_obj);
         __Pyx_GIVEREF(__pyx_v_obj);
         PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_obj);
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_6);
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_8, 2, __pyx_t_7);
         __pyx_t_6 = 0;
         __pyx_t_7 = 0;
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 436, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_8, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 434, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_DECREF_SET(__pyx_v_obj, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "View.MemoryView":435
+        /* "View.MemoryView":433
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       }
@@ -7934,30 +7765,30 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "View.MemoryView":438
+      /* "View.MemoryView":436
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  *             except TypeError:             # <<<<<<<<<<<<<<
  *                 return None
  * 
  */
       __pyx_t_9 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_9) {
         __Pyx_AddTraceback("View.MemoryView.memoryview.is_slice", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(2, 438, __pyx_L6_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_8, &__pyx_t_6) < 0) __PYX_ERR(2, 436, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GOTREF(__pyx_t_6);
 
-        /* "View.MemoryView":439
+        /* "View.MemoryView":437
  *                                  self.dtype_is_object)
  *             except TypeError:
  *                 return None             # <<<<<<<<<<<<<<
  * 
  *         return obj
  */
         __Pyx_XDECREF(__pyx_r);
@@ -7966,15 +7797,15 @@
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         goto __pyx_L7_except_return;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "View.MemoryView":435
+      /* "View.MemoryView":433
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):
  *             try:             # <<<<<<<<<<<<<<
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  *                                  self.dtype_is_object)
  */
       __Pyx_XGIVEREF(__pyx_t_3);
@@ -7987,36 +7818,36 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
       goto __pyx_L0;
       __pyx_L9_try_end:;
     }
 
-    /* "View.MemoryView":434
+    /* "View.MemoryView":432
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
  *             try:
  *                 obj = memoryview(obj, self.flags & ~PyBUF_WRITABLE | PyBUF_ANY_CONTIGUOUS,
  */
   }
 
-  /* "View.MemoryView":441
+  /* "View.MemoryView":439
  *                 return None
  * 
  *         return obj             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assignment(self, dst, src):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_obj);
   __pyx_r = __pyx_v_obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":433
+  /* "View.MemoryView":431
  *             self.setitem_indexed(index, value)
  * 
  *     cdef is_slice(self, obj):             # <<<<<<<<<<<<<<
  *         if not isinstance(obj, memoryview):
  *             try:
  */
 
@@ -8030,15 +7861,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_obj);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":443
+/* "View.MemoryView":441
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -8054,60 +7885,60 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
 
-  /* "View.MemoryView":447
+  /* "View.MemoryView":445
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(2, 447, __pyx_L1_error)
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 447, __pyx_L1_error)
+  if (!(likely(((__pyx_v_src) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_src, __pyx_memoryview_type))))) __PYX_ERR(2, 445, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_src), (&__pyx_v_src_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 445, __pyx_L1_error)
 
-  /* "View.MemoryView":448
+  /* "View.MemoryView":446
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],             # <<<<<<<<<<<<<<
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  */
-  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(2, 448, __pyx_L1_error)
-  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 448, __pyx_L1_error)
+  if (!(likely(((__pyx_v_dst) == Py_None) || likely(__Pyx_TypeTest(__pyx_v_dst, __pyx_memoryview_type))))) __PYX_ERR(2, 446, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_get_slice_from_memoryview(((struct __pyx_memoryview_obj *)__pyx_v_dst), (&__pyx_v_dst_slice)); if (unlikely(__pyx_t_2 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 446, __pyx_L1_error)
 
-  /* "View.MemoryView":449
+  /* "View.MemoryView":447
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 449, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_src, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 449, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_4 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 449, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_dst, __pyx_n_s_ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 447, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 449, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_As_int(__pyx_t_3); if (unlikely((__pyx_t_5 == (int)-1) && PyErr_Occurred())) __PYX_ERR(2, 447, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":447
+  /* "View.MemoryView":445
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  */
-  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 447, __pyx_L1_error)
+  __pyx_t_6 = __pyx_memoryview_copy_contents((__pyx_t_1[0]), (__pyx_t_2[0]), __pyx_t_4, __pyx_t_5, __pyx_v_self->dtype_is_object); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 445, __pyx_L1_error)
 
-  /* "View.MemoryView":443
+  /* "View.MemoryView":441
  *         return obj
  * 
  *     cdef setitem_slice_assignment(self, dst, src):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice dst_slice
  *         cdef __Pyx_memviewslice src_slice
  */
 
@@ -8120,15 +7951,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":451
+/* "View.MemoryView":449
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -8153,204 +7984,204 @@
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
 
-  /* "View.MemoryView":453
+  /* "View.MemoryView":451
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
  * 
  */
   __pyx_v_tmp = NULL;
 
-  /* "View.MemoryView":458
+  /* "View.MemoryView":456
  *         cdef __Pyx_memviewslice *dst_slice
  *         cdef __Pyx_memviewslice tmp_slice
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)             # <<<<<<<<<<<<<<
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 458, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_dst, (&__pyx_v_tmp_slice)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 456, __pyx_L1_error)
   __pyx_v_dst_slice = __pyx_t_1;
 
-  /* "View.MemoryView":460
+  /* "View.MemoryView":458
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
   __pyx_t_2 = ((((size_t)__pyx_v_self->view.itemsize) > (sizeof(__pyx_v_array))) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":461
+    /* "View.MemoryView":459
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)             # <<<<<<<<<<<<<<
  *             if tmp == NULL:
  *                 raise MemoryError
  */
     __pyx_v_tmp = PyMem_Malloc(__pyx_v_self->view.itemsize);
 
-    /* "View.MemoryView":462
+    /* "View.MemoryView":460
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     __pyx_t_2 = ((__pyx_v_tmp == NULL) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":463
+      /* "View.MemoryView":461
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  *                 raise MemoryError             # <<<<<<<<<<<<<<
  *             item = tmp
  *         else:
  */
-      PyErr_NoMemory(); __PYX_ERR(2, 463, __pyx_L1_error)
+      PyErr_NoMemory(); __PYX_ERR(2, 461, __pyx_L1_error)
 
-      /* "View.MemoryView":462
+      /* "View.MemoryView":460
  *         if <size_t>self.view.itemsize > sizeof(array):
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:             # <<<<<<<<<<<<<<
  *                 raise MemoryError
  *             item = tmp
  */
     }
 
-    /* "View.MemoryView":464
+    /* "View.MemoryView":462
  *             if tmp == NULL:
  *                 raise MemoryError
  *             item = tmp             # <<<<<<<<<<<<<<
  *         else:
  *             item = <void *> array
  */
     __pyx_v_item = __pyx_v_tmp;
 
-    /* "View.MemoryView":460
+    /* "View.MemoryView":458
  *         dst_slice = get_slice_from_memview(dst, &tmp_slice)
  * 
  *         if <size_t>self.view.itemsize > sizeof(array):             # <<<<<<<<<<<<<<
  *             tmp = PyMem_Malloc(self.view.itemsize)
  *             if tmp == NULL:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":466
+  /* "View.MemoryView":464
  *             item = tmp
  *         else:
  *             item = <void *> array             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
   /*else*/ {
     __pyx_v_item = ((void *)__pyx_v_array);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":468
+  /* "View.MemoryView":466
  *             item = <void *> array
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value
  */
   /*try:*/ {
 
-    /* "View.MemoryView":469
+    /* "View.MemoryView":467
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
     __pyx_t_2 = (__pyx_v_self->dtype_is_object != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":470
+      /* "View.MemoryView":468
  *         try:
  *             if self.dtype_is_object:
  *                 (<PyObject **> item)[0] = <PyObject *> value             # <<<<<<<<<<<<<<
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)
  */
       (((PyObject **)__pyx_v_item)[0]) = ((PyObject *)__pyx_v_value);
 
-      /* "View.MemoryView":469
+      /* "View.MemoryView":467
  * 
  *         try:
  *             if self.dtype_is_object:             # <<<<<<<<<<<<<<
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  */
       goto __pyx_L8;
     }
 
-    /* "View.MemoryView":472
+    /* "View.MemoryView":470
  *                 (<PyObject **> item)[0] = <PyObject *> value
  *             else:
  *                 self.assign_item_from_object(<char *> item, value)             # <<<<<<<<<<<<<<
  * 
  * 
  */
     /*else*/ {
-      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 472, __pyx_L6_error)
+      __pyx_t_3 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, ((char *)__pyx_v_item), __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 470, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __pyx_L8:;
 
-    /* "View.MemoryView":476
+    /* "View.MemoryView":474
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     __pyx_t_2 = ((__pyx_v_self->view.suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":477
+      /* "View.MemoryView":475
  * 
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)             # <<<<<<<<<<<<<<
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  *                                 item, self.dtype_is_object)
  */
-      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 477, __pyx_L6_error)
+      __pyx_t_3 = assert_direct_dimensions(__pyx_v_self->view.suboffsets, __pyx_v_self->view.ndim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 475, __pyx_L6_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-      /* "View.MemoryView":476
+      /* "View.MemoryView":474
  * 
  * 
  *             if self.view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,
  */
     }
 
-    /* "View.MemoryView":478
+    /* "View.MemoryView":476
  *             if self.view.suboffsets != NULL:
  *                 assert_direct_dimensions(self.view.suboffsets, self.view.ndim)
  *             slice_assign_scalar(dst_slice, dst.view.ndim, self.view.itemsize,             # <<<<<<<<<<<<<<
  *                                 item, self.dtype_is_object)
  *         finally:
  */
     __pyx_memoryview_slice_assign_scalar(__pyx_v_dst_slice, __pyx_v_dst->view.ndim, __pyx_v_self->view.itemsize, __pyx_v_item, __pyx_v_self->dtype_is_object);
   }
 
-  /* "View.MemoryView":481
+  /* "View.MemoryView":479
  *                                 item, self.dtype_is_object)
  *         finally:
  *             PyMem_Free(tmp)             # <<<<<<<<<<<<<<
  * 
  *     cdef setitem_indexed(self, index, value):
  */
   /*finally:*/ {
@@ -8389,15 +8220,15 @@
       __pyx_t_7 = 0; __pyx_t_8 = 0; __pyx_t_9 = 0; __pyx_t_10 = 0; __pyx_t_11 = 0; __pyx_t_12 = 0;
       __pyx_lineno = __pyx_t_4; __pyx_clineno = __pyx_t_5; __pyx_filename = __pyx_t_6;
       goto __pyx_L1_error;
     }
     __pyx_L7:;
   }
 
-  /* "View.MemoryView":451
+  /* "View.MemoryView":449
  *                                  src.ndim, dst.ndim, self.dtype_is_object)
  * 
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):             # <<<<<<<<<<<<<<
  *         cdef int array[128]
  *         cdef void *tmp = NULL
  */
 
@@ -8410,15 +8241,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":483
+/* "View.MemoryView":481
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -8429,36 +8260,36 @@
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_indexed", 0);
 
-  /* "View.MemoryView":484
+  /* "View.MemoryView":482
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
  * 
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(2, 484, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->get_item_pointer(__pyx_v_self, __pyx_v_index); if (unlikely(__pyx_t_1 == ((char *)NULL))) __PYX_ERR(2, 482, __pyx_L1_error)
   __pyx_v_itemp = __pyx_t_1;
 
-  /* "View.MemoryView":485
+  /* "View.MemoryView":483
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 485, __pyx_L1_error)
+  __pyx_t_2 = ((struct __pyx_vtabstruct_memoryview *)__pyx_v_self->__pyx_vtab)->assign_item_from_object(__pyx_v_self, __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 483, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":483
+  /* "View.MemoryView":481
  *             PyMem_Free(tmp)
  * 
  *     cdef setitem_indexed(self, index, value):             # <<<<<<<<<<<<<<
  *         cdef char *itemp = self.get_item_pointer(index)
  *         self.assign_item_from_object(itemp, value)
  */
 
@@ -8471,15 +8302,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":487
+/* "View.MemoryView":485
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -8501,39 +8332,39 @@
   size_t __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":490
+  /* "View.MemoryView":488
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 490, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 488, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":493
+  /* "View.MemoryView":491
  *         cdef bytes bytesitem
  * 
  *         bytesitem = itemp[:self.view.itemsize]             # <<<<<<<<<<<<<<
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromStringAndSize(__pyx_v_itemp + 0, __pyx_v_self->view.itemsize - 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_bytesitem = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":494
+  /* "View.MemoryView":492
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
   {
@@ -8541,24 +8372,24 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_2, &__pyx_t_3, &__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     /*try:*/ {
 
-      /* "View.MemoryView":495
+      /* "View.MemoryView":493
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)             # <<<<<<<<<<<<<<
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")
  */
-      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 495, __pyx_L3_error)
+      __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_unpack); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 493, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 495, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 493, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
         if (likely(__pyx_t_7)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -8567,94 +8398,94 @@
           __Pyx_DECREF_SET(__pyx_t_5, function);
           __pyx_t_8 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
         PyObject *__pyx_temp[3] = {__pyx_t_7, __pyx_t_6, __pyx_v_bytesitem};
-        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 2+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       } else
       #endif
       {
-        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 495, __pyx_L3_error)
+        __pyx_t_9 = PyTuple_New(2+__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 493, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_9);
         if (__pyx_t_7) {
           __Pyx_GIVEREF(__pyx_t_7); PyTuple_SET_ITEM(__pyx_t_9, 0, __pyx_t_7); __pyx_t_7 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_6);
         PyTuple_SET_ITEM(__pyx_t_9, 0+__pyx_t_8, __pyx_t_6);
         __Pyx_INCREF(__pyx_v_bytesitem);
         __Pyx_GIVEREF(__pyx_v_bytesitem);
         PyTuple_SET_ITEM(__pyx_t_9, 1+__pyx_t_8, __pyx_v_bytesitem);
         __pyx_t_6 = 0;
-        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 495, __pyx_L3_error)
+        __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_9, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 493, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __pyx_v_result = __pyx_t_1;
       __pyx_t_1 = 0;
 
-      /* "View.MemoryView":494
+      /* "View.MemoryView":492
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     }
 
-    /* "View.MemoryView":499
+    /* "View.MemoryView":497
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
     /*else:*/ {
       __pyx_t_10 = strlen(__pyx_v_self->view.format); 
       __pyx_t_11 = ((__pyx_t_10 == 1) != 0);
       if (__pyx_t_11) {
 
-        /* "View.MemoryView":500
+        /* "View.MemoryView":498
  *         else:
  *             if len(self.view.format) == 1:
  *                 return result[0]             # <<<<<<<<<<<<<<
  *             return result
  * 
  */
         __Pyx_XDECREF(__pyx_r);
-        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 500, __pyx_L5_except_error)
+        __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_result, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 498, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_1);
         __pyx_r = __pyx_t_1;
         __pyx_t_1 = 0;
         goto __pyx_L6_except_return;
 
-        /* "View.MemoryView":499
+        /* "View.MemoryView":497
  *             raise ValueError("Unable to convert item to object")
  *         else:
  *             if len(self.view.format) == 1:             # <<<<<<<<<<<<<<
  *                 return result[0]
  *             return result
  */
       }
 
-      /* "View.MemoryView":501
+      /* "View.MemoryView":499
  *             if len(self.view.format) == 1:
  *                 return result[0]
  *             return result             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
       __Pyx_XDECREF(__pyx_r);
@@ -8665,52 +8496,52 @@
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
 
-    /* "View.MemoryView":496
+    /* "View.MemoryView":494
  *         try:
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:             # <<<<<<<<<<<<<<
  *             raise ValueError("Unable to convert item to object")
  *         else:
  */
     __Pyx_ErrFetch(&__pyx_t_1, &__pyx_t_5, &__pyx_t_9);
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 496, __pyx_L5_except_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_error); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 494, __pyx_L5_except_error)
     __Pyx_GOTREF(__pyx_t_6);
     __pyx_t_8 = __Pyx_PyErr_GivenExceptionMatches(__pyx_t_1, __pyx_t_6);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_ErrRestore(__pyx_t_1, __pyx_t_5, __pyx_t_9);
     __pyx_t_1 = 0; __pyx_t_5 = 0; __pyx_t_9 = 0;
     if (__pyx_t_8) {
       __Pyx_AddTraceback("View.MemoryView.memoryview.convert_item_to_object", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(2, 496, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_9, &__pyx_t_5, &__pyx_t_1) < 0) __PYX_ERR(2, 494, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_1);
 
-      /* "View.MemoryView":497
+      /* "View.MemoryView":495
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 495, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(2, 497, __pyx_L5_except_error)
+      __PYX_ERR(2, 495, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "View.MemoryView":494
+    /* "View.MemoryView":492
  * 
  *         bytesitem = itemp[:self.view.itemsize]
  *         try:             # <<<<<<<<<<<<<<
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  */
     __Pyx_XGIVEREF(__pyx_t_2);
@@ -8722,15 +8553,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_ExceptionReset(__pyx_t_2, __pyx_t_3, __pyx_t_4);
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":487
+  /* "View.MemoryView":485
  *         self.assign_item_from_object(itemp, value)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -8748,15 +8579,15 @@
   __Pyx_XDECREF(__pyx_v_bytesitem);
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":503
+/* "View.MemoryView":501
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -8782,88 +8613,88 @@
   char *__pyx_t_13;
   char *__pyx_t_14;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":506
+  /* "View.MemoryView":504
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
  *         cdef bytes bytesvalue
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 506, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_struct, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_struct = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":511
+  /* "View.MemoryView":509
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
   __pyx_t_2 = PyTuple_Check(__pyx_v_value); 
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "View.MemoryView":512
+    /* "View.MemoryView":510
  * 
  *         if isinstance(value, tuple):
  *             bytesvalue = struct.pack(self.view.format, *value)             # <<<<<<<<<<<<<<
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)
  */
-    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_5 = PyTuple_New(1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_4);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PySequence_Tuple(__pyx_v_value); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_6 = PyNumber_Add(__pyx_t_5, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 510, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 510, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "View.MemoryView":511
+    /* "View.MemoryView":509
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":514
+  /* "View.MemoryView":512
  *             bytesvalue = struct.pack(self.view.format, *value)
  *         else:
  *             bytesvalue = struct.pack(self.view.format, value)             # <<<<<<<<<<<<<<
  * 
  *         for i, c in enumerate(bytesvalue):
  */
   /*else*/ {
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 514, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_struct, __pyx_n_s_pack); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 514, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromString(__pyx_v_self->view.format); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_5 = NULL;
     __pyx_t_7 = 0;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_6);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -8872,102 +8703,102 @@
         __Pyx_DECREF_SET(__pyx_t_6, function);
         __pyx_t_7 = 1;
       }
     }
     #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     #if CYTHON_FAST_PYCCALL
     if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
       PyObject *__pyx_temp[3] = {__pyx_t_5, __pyx_t_1, __pyx_v_value};
-      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_7, 2+__pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     } else
     #endif
     {
-      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 514, __pyx_L1_error)
+      __pyx_t_8 = PyTuple_New(2+__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 512, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       if (__pyx_t_5) {
         __Pyx_GIVEREF(__pyx_t_5); PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_t_5); __pyx_t_5 = NULL;
       }
       __Pyx_GIVEREF(__pyx_t_1);
       PyTuple_SET_ITEM(__pyx_t_8, 0+__pyx_t_7, __pyx_t_1);
       __Pyx_INCREF(__pyx_v_value);
       __Pyx_GIVEREF(__pyx_v_value);
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
-      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":516
+  /* "View.MemoryView":514
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
   __pyx_t_9 = 0;
   if (unlikely(__pyx_v_bytesvalue == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' is not iterable");
-    __PYX_ERR(2, 516, __pyx_L1_error)
+    __PYX_ERR(2, 514, __pyx_L1_error)
   }
   __Pyx_INCREF(__pyx_v_bytesvalue);
   __pyx_t_10 = __pyx_v_bytesvalue;
   __pyx_t_12 = PyBytes_AS_STRING(__pyx_t_10);
   __pyx_t_13 = (__pyx_t_12 + PyBytes_GET_SIZE(__pyx_t_10));
   for (__pyx_t_14 = __pyx_t_12; __pyx_t_14 < __pyx_t_13; __pyx_t_14++) {
     __pyx_t_11 = __pyx_t_14;
     __pyx_v_c = (__pyx_t_11[0]);
 
-    /* "View.MemoryView":517
+    /* "View.MemoryView":515
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     __pyx_v_i = __pyx_t_9;
 
-    /* "View.MemoryView":516
+    /* "View.MemoryView":514
  *             bytesvalue = struct.pack(self.view.format, value)
  * 
  *         for i, c in enumerate(bytesvalue):             # <<<<<<<<<<<<<<
  *             itemp[i] = c
  * 
  */
     __pyx_t_9 = (__pyx_t_9 + 1);
 
-    /* "View.MemoryView":517
+    /* "View.MemoryView":515
  * 
  *         for i, c in enumerate(bytesvalue):
  *             itemp[i] = c             # <<<<<<<<<<<<<<
  * 
  *     @cname('getbuffer')
  */
     (__pyx_v_itemp[__pyx_v_i]) = __pyx_v_c;
   }
   __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-  /* "View.MemoryView":503
+  /* "View.MemoryView":501
  *             return result
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  */
 
@@ -8987,15 +8818,15 @@
   __Pyx_XDECREF(__pyx_v_struct);
   __Pyx_XDECREF(__pyx_v_bytesvalue);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":520
+/* "View.MemoryView":518
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -9030,15 +8861,15 @@
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
 
-  /* "View.MemoryView":521
+  /* "View.MemoryView":519
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   __pyx_t_2 = ((__pyx_v_flags & PyBUF_WRITABLE) != 0);
@@ -9048,268 +8879,268 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (__pyx_v_self->view.readonly != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":522
+    /* "View.MemoryView":520
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 520, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 522, __pyx_L1_error)
+    __PYX_ERR(2, 520, __pyx_L1_error)
 
-    /* "View.MemoryView":521
+    /* "View.MemoryView":519
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:             # <<<<<<<<<<<<<<
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  */
   }
 
-  /* "View.MemoryView":524
+  /* "View.MemoryView":522
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_ND) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":525
+    /* "View.MemoryView":523
  * 
  *         if flags & PyBUF_ND:
  *             info.shape = self.view.shape             # <<<<<<<<<<<<<<
  *         else:
  *             info.shape = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.shape;
     __pyx_v_info->shape = __pyx_t_4;
 
-    /* "View.MemoryView":524
+    /* "View.MemoryView":522
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  * 
  *         if flags & PyBUF_ND:             # <<<<<<<<<<<<<<
  *             info.shape = self.view.shape
  *         else:
  */
     goto __pyx_L6;
   }
 
-  /* "View.MemoryView":527
+  /* "View.MemoryView":525
  *             info.shape = self.view.shape
  *         else:
  *             info.shape = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_STRIDES:
  */
   /*else*/ {
     __pyx_v_info->shape = NULL;
   }
   __pyx_L6:;
 
-  /* "View.MemoryView":529
+  /* "View.MemoryView":527
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_STRIDES) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":530
+    /* "View.MemoryView":528
  * 
  *         if flags & PyBUF_STRIDES:
  *             info.strides = self.view.strides             # <<<<<<<<<<<<<<
  *         else:
  *             info.strides = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.strides;
     __pyx_v_info->strides = __pyx_t_4;
 
-    /* "View.MemoryView":529
+    /* "View.MemoryView":527
  *             info.shape = NULL
  * 
  *         if flags & PyBUF_STRIDES:             # <<<<<<<<<<<<<<
  *             info.strides = self.view.strides
  *         else:
  */
     goto __pyx_L7;
   }
 
-  /* "View.MemoryView":532
+  /* "View.MemoryView":530
  *             info.strides = self.view.strides
  *         else:
  *             info.strides = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_INDIRECT:
  */
   /*else*/ {
     __pyx_v_info->strides = NULL;
   }
   __pyx_L7:;
 
-  /* "View.MemoryView":534
+  /* "View.MemoryView":532
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_INDIRECT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":535
+    /* "View.MemoryView":533
  * 
  *         if flags & PyBUF_INDIRECT:
  *             info.suboffsets = self.view.suboffsets             # <<<<<<<<<<<<<<
  *         else:
  *             info.suboffsets = NULL
  */
     __pyx_t_4 = __pyx_v_self->view.suboffsets;
     __pyx_v_info->suboffsets = __pyx_t_4;
 
-    /* "View.MemoryView":534
+    /* "View.MemoryView":532
  *             info.strides = NULL
  * 
  *         if flags & PyBUF_INDIRECT:             # <<<<<<<<<<<<<<
  *             info.suboffsets = self.view.suboffsets
  *         else:
  */
     goto __pyx_L8;
   }
 
-  /* "View.MemoryView":537
+  /* "View.MemoryView":535
  *             info.suboffsets = self.view.suboffsets
  *         else:
  *             info.suboffsets = NULL             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_FORMAT:
  */
   /*else*/ {
     __pyx_v_info->suboffsets = NULL;
   }
   __pyx_L8:;
 
-  /* "View.MemoryView":539
+  /* "View.MemoryView":537
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_flags & PyBUF_FORMAT) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":540
+    /* "View.MemoryView":538
  * 
  *         if flags & PyBUF_FORMAT:
  *             info.format = self.view.format             # <<<<<<<<<<<<<<
  *         else:
  *             info.format = NULL
  */
     __pyx_t_5 = __pyx_v_self->view.format;
     __pyx_v_info->format = __pyx_t_5;
 
-    /* "View.MemoryView":539
+    /* "View.MemoryView":537
  *             info.suboffsets = NULL
  * 
  *         if flags & PyBUF_FORMAT:             # <<<<<<<<<<<<<<
  *             info.format = self.view.format
  *         else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":542
+  /* "View.MemoryView":540
  *             info.format = self.view.format
  *         else:
  *             info.format = NULL             # <<<<<<<<<<<<<<
  * 
  *         info.buf = self.view.buf
  */
   /*else*/ {
     __pyx_v_info->format = NULL;
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":544
+  /* "View.MemoryView":542
  *             info.format = NULL
  * 
  *         info.buf = self.view.buf             # <<<<<<<<<<<<<<
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  */
   __pyx_t_6 = __pyx_v_self->view.buf;
   __pyx_v_info->buf = __pyx_t_6;
 
-  /* "View.MemoryView":545
+  /* "View.MemoryView":543
  * 
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim             # <<<<<<<<<<<<<<
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  */
   __pyx_t_7 = __pyx_v_self->view.ndim;
   __pyx_v_info->ndim = __pyx_t_7;
 
-  /* "View.MemoryView":546
+  /* "View.MemoryView":544
  *         info.buf = self.view.buf
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize             # <<<<<<<<<<<<<<
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  */
   __pyx_t_8 = __pyx_v_self->view.itemsize;
   __pyx_v_info->itemsize = __pyx_t_8;
 
-  /* "View.MemoryView":547
+  /* "View.MemoryView":545
  *         info.ndim = self.view.ndim
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len             # <<<<<<<<<<<<<<
  *         info.readonly = self.view.readonly
  *         info.obj = self
  */
   __pyx_t_8 = __pyx_v_self->view.len;
   __pyx_v_info->len = __pyx_t_8;
 
-  /* "View.MemoryView":548
+  /* "View.MemoryView":546
  *         info.itemsize = self.view.itemsize
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly             # <<<<<<<<<<<<<<
  *         info.obj = self
  * 
  */
   __pyx_t_1 = __pyx_v_self->view.readonly;
   __pyx_v_info->readonly = __pyx_t_1;
 
-  /* "View.MemoryView":549
+  /* "View.MemoryView":547
  *         info.len = self.view.len
  *         info.readonly = self.view.readonly
  *         info.obj = self             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
   __Pyx_GOTREF(__pyx_v_info->obj);
   __Pyx_DECREF(__pyx_v_info->obj);
   __pyx_v_info->obj = ((PyObject *)__pyx_v_self);
 
-  /* "View.MemoryView":520
+  /* "View.MemoryView":518
  * 
  *     @cname('getbuffer')
  *     def __getbuffer__(self, Py_buffer *info, int flags):             # <<<<<<<<<<<<<<
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")
  */
 
@@ -9331,15 +9162,15 @@
     __Pyx_DECREF(__pyx_v_info->obj); __pyx_v_info->obj = 0;
   }
   __pyx_L2:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":555
+/* "View.MemoryView":553
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -9363,49 +9194,49 @@
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":556
+  /* "View.MemoryView":554
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
  *         return result
  */
-  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 556, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object(__pyx_v_self); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 554, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(2, 556, __pyx_L1_error)
+  if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_memoryviewslice_type))))) __PYX_ERR(2, 554, __pyx_L1_error)
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":557
+  /* "View.MemoryView":555
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)             # <<<<<<<<<<<<<<
  *         return result
  * 
  */
-  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 557, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memslice_transpose((&__pyx_v_result->from_slice)); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 555, __pyx_L1_error)
 
-  /* "View.MemoryView":558
+  /* "View.MemoryView":556
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  *         return result             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":555
+  /* "View.MemoryView":553
  * 
  *     @property
  *     def T(self):             # <<<<<<<<<<<<<<
  *         cdef _memoryviewslice result = memoryview_copy(self)
  *         transpose_memslice(&result.from_slice)
  */
 
@@ -9417,15 +9248,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":561
+/* "View.MemoryView":559
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
@@ -9443,42 +9274,42 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4base___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":562
+  /* "View.MemoryView":560
  *     @property
  *     def base(self):
  *         return self.obj             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->obj);
   __pyx_r = __pyx_v_self->obj;
   goto __pyx_L0;
 
-  /* "View.MemoryView":561
+  /* "View.MemoryView":559
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.obj
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":565
+/* "View.MemoryView":563
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -9505,41 +9336,41 @@
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":566
+  /* "View.MemoryView":564
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 566, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_3 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
   for (__pyx_t_4 = __pyx_v_self->view.shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_length = (__pyx_t_2[0]);
-    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 566, __pyx_L1_error)
+    __pyx_t_5 = PyInt_FromSsize_t(__pyx_v_length); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 564, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(2, 566, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(2, 564, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
-  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 566, __pyx_L1_error)
+  __pyx_t_5 = PyList_AsTuple(((PyObject*)__pyx_t_1)); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 564, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":565
+  /* "View.MemoryView":563
  * 
  *     @property
  *     def shape(self):             # <<<<<<<<<<<<<<
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])
  * 
  */
 
@@ -9551,15 +9382,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":569
+/* "View.MemoryView":567
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -9587,73 +9418,73 @@
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":570
+  /* "View.MemoryView":568
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   __pyx_t_1 = ((__pyx_v_self->view.strides == NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":572
+    /* "View.MemoryView":570
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 570, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 572, __pyx_L1_error)
+    __PYX_ERR(2, 570, __pyx_L1_error)
 
-    /* "View.MemoryView":570
+    /* "View.MemoryView":568
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
  *             raise ValueError("Buffer view does not expose strides")
  */
   }
 
-  /* "View.MemoryView":574
+  /* "View.MemoryView":572
  *             raise ValueError("Buffer view does not expose strides")
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 574, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = (__pyx_v_self->view.strides + __pyx_v_self->view.ndim);
   for (__pyx_t_5 = __pyx_v_self->view.strides; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
     __pyx_t_3 = __pyx_t_5;
     __pyx_v_stride = (__pyx_t_3[0]);
-    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 574, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t(__pyx_v_stride); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(2, 574, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(2, 572, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   }
-  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 574, __pyx_L1_error)
+  __pyx_t_6 = PyList_AsTuple(((PyObject*)__pyx_t_2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 572, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_6;
   __pyx_t_6 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":569
+  /* "View.MemoryView":567
  * 
  *     @property
  *     def strides(self):             # <<<<<<<<<<<<<<
  *         if self.view.strides == NULL:
  * 
  */
 
@@ -9665,15 +9496,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":577
+/* "View.MemoryView":575
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -9701,77 +9532,77 @@
   Py_ssize_t *__pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":578
+  /* "View.MemoryView":576
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.suboffsets == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":579
+    /* "View.MemoryView":577
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__14, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 577, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":578
+    /* "View.MemoryView":576
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
  * 
  */
   }
 
-  /* "View.MemoryView":581
+  /* "View.MemoryView":579
  *             return (-1,) * self.view.ndim
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 581, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_5 = (__pyx_v_self->view.suboffsets + __pyx_v_self->view.ndim);
   for (__pyx_t_6 = __pyx_v_self->view.suboffsets; __pyx_t_6 < __pyx_t_5; __pyx_t_6++) {
     __pyx_t_4 = __pyx_t_6;
     __pyx_v_suboffset = (__pyx_t_4[0]);
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 581, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_suboffset); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(2, 581, __pyx_L1_error)
+    if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_2))) __PYX_ERR(2, 579, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
-  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 581, __pyx_L1_error)
+  __pyx_t_2 = PyList_AsTuple(((PyObject*)__pyx_t_3)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 579, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":577
+  /* "View.MemoryView":575
  * 
  *     @property
  *     def suboffsets(self):             # <<<<<<<<<<<<<<
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim
  */
 
@@ -9783,15 +9614,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":584
+/* "View.MemoryView":582
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -9813,29 +9644,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":585
+  /* "View.MemoryView":583
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 585, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 583, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":584
+  /* "View.MemoryView":582
  * 
  *     @property
  *     def ndim(self):             # <<<<<<<<<<<<<<
  *         return self.view.ndim
  * 
  */
 
@@ -9846,15 +9677,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":588
+/* "View.MemoryView":586
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -9876,29 +9707,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":589
+  /* "View.MemoryView":587
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 589, __pyx_L1_error)
+  __pyx_t_1 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 587, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":588
+  /* "View.MemoryView":586
  * 
  *     @property
  *     def itemsize(self):             # <<<<<<<<<<<<<<
  *         return self.view.itemsize
  * 
  */
 
@@ -9909,15 +9740,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":592
+/* "View.MemoryView":590
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -9941,35 +9772,35 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":593
+  /* "View.MemoryView":591
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 593, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 593, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_self->view.itemsize); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 593, __pyx_L1_error)
+  __pyx_t_3 = PyNumber_Multiply(__pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 591, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":592
+  /* "View.MemoryView":590
  * 
  *     @property
  *     def nbytes(self):             # <<<<<<<<<<<<<<
  *         return self.size * self.view.itemsize
  * 
  */
 
@@ -9982,15 +9813,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":596
+/* "View.MemoryView":594
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -10019,98 +9850,98 @@
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":597
+  /* "View.MemoryView":595
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   __pyx_t_1 = (__pyx_v_self->_size == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":598
+    /* "View.MemoryView":596
  *     def size(self):
  *         if self._size is None:
  *             result = 1             # <<<<<<<<<<<<<<
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  */
     __Pyx_INCREF(__pyx_int_1);
     __pyx_v_result = __pyx_int_1;
 
-    /* "View.MemoryView":600
+    /* "View.MemoryView":598
  *             result = 1
  * 
  *             for length in self.view.shape[:self.view.ndim]:             # <<<<<<<<<<<<<<
  *                 result *= length
  * 
  */
     __pyx_t_4 = (__pyx_v_self->view.shape + __pyx_v_self->view.ndim);
     for (__pyx_t_5 = __pyx_v_self->view.shape; __pyx_t_5 < __pyx_t_4; __pyx_t_5++) {
       __pyx_t_3 = __pyx_t_5;
-      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 600, __pyx_L1_error)
+      __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_3[0])); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 598, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_6);
       __pyx_t_6 = 0;
 
-      /* "View.MemoryView":601
+      /* "View.MemoryView":599
  * 
  *             for length in self.view.shape[:self.view.ndim]:
  *                 result *= length             # <<<<<<<<<<<<<<
  * 
  *             self._size = result
  */
-      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 601, __pyx_L1_error)
+      __pyx_t_6 = PyNumber_InPlaceMultiply(__pyx_v_result, __pyx_v_length); if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 599, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF_SET(__pyx_v_result, __pyx_t_6);
       __pyx_t_6 = 0;
     }
 
-    /* "View.MemoryView":603
+    /* "View.MemoryView":601
  *                 result *= length
  * 
  *             self._size = result             # <<<<<<<<<<<<<<
  * 
  *         return self._size
  */
     __Pyx_INCREF(__pyx_v_result);
     __Pyx_GIVEREF(__pyx_v_result);
     __Pyx_GOTREF(__pyx_v_self->_size);
     __Pyx_DECREF(__pyx_v_self->_size);
     __pyx_v_self->_size = __pyx_v_result;
 
-    /* "View.MemoryView":597
+    /* "View.MemoryView":595
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
  * 
  */
   }
 
-  /* "View.MemoryView":605
+  /* "View.MemoryView":603
  *             self._size = result
  * 
  *         return self._size             # <<<<<<<<<<<<<<
  * 
  *     def __len__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_size);
   __pyx_r = __pyx_v_self->_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":596
+  /* "View.MemoryView":594
  * 
  *     @property
  *     def size(self):             # <<<<<<<<<<<<<<
  *         if self._size is None:
  *             result = 1
  */
 
@@ -10123,15 +9954,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":607
+/* "View.MemoryView":605
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
@@ -10150,68 +9981,68 @@
 
 static Py_ssize_t __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_10__len__(struct __pyx_memoryview_obj *__pyx_v_self) {
   Py_ssize_t __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__len__", 0);
 
-  /* "View.MemoryView":608
+  /* "View.MemoryView":606
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   __pyx_t_1 = ((__pyx_v_self->view.ndim >= 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":609
+    /* "View.MemoryView":607
  *     def __len__(self):
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]             # <<<<<<<<<<<<<<
  * 
  *         return 0
  */
     __pyx_r = (__pyx_v_self->view.shape[0]);
     goto __pyx_L0;
 
-    /* "View.MemoryView":608
+    /* "View.MemoryView":606
  * 
  *     def __len__(self):
  *         if self.view.ndim >= 1:             # <<<<<<<<<<<<<<
  *             return self.view.shape[0]
  * 
  */
   }
 
-  /* "View.MemoryView":611
+  /* "View.MemoryView":609
  *             return self.view.shape[0]
  * 
  *         return 0             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":607
+  /* "View.MemoryView":605
  *         return self._size
  * 
  *     def __len__(self):             # <<<<<<<<<<<<<<
  *         if self.view.ndim >= 1:
  *             return self.view.shape[0]
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":613
+/* "View.MemoryView":611
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -10235,64 +10066,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "View.MemoryView":614
+  /* "View.MemoryView":612
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 614, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 614, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 614, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "View.MemoryView":615
+  /* "View.MemoryView":613
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))             # <<<<<<<<<<<<<<
  * 
  *     def __str__(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 615, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_id, ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 613, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "View.MemoryView":614
+  /* "View.MemoryView":612
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
  * 
  */
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 614, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 614, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":613
+  /* "View.MemoryView":611
  *         return 0
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,
  *                                                id(self))
  */
 
@@ -10305,15 +10136,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":617
+/* "View.MemoryView":615
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -10336,43 +10167,43 @@
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
-  /* "View.MemoryView":618
+  /* "View.MemoryView":616
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_base); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 618, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_class); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_name_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 618, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 618, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_MemoryView_of_r_object, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":617
+  /* "View.MemoryView":615
  *                                                id(self))
  * 
  *     def __str__(self):             # <<<<<<<<<<<<<<
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)
  * 
  */
 
@@ -10384,15 +10215,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":621
+/* "View.MemoryView":619
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -10417,39 +10248,39 @@
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_c_contig", 0);
 
-  /* "View.MemoryView":624
+  /* "View.MemoryView":622
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 624, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 622, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":625
+  /* "View.MemoryView":623
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def is_f_contig(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 625, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'C', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 623, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":621
+  /* "View.MemoryView":619
  * 
  * 
  *     def is_c_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -10460,15 +10291,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":627
+/* "View.MemoryView":625
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -10493,39 +10324,39 @@
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_f_contig", 0);
 
-  /* "View.MemoryView":630
+  /* "View.MemoryView":628
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  */
-  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 630, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_get_slice_from_memoryview(__pyx_v_self, (&__pyx_v_tmp)); if (unlikely(__pyx_t_1 == ((__Pyx_memviewslice *)NULL))) __PYX_ERR(2, 628, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":631
+  /* "View.MemoryView":629
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)             # <<<<<<<<<<<<<<
  * 
  *     def copy(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 631, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_memviewslice_is_contig((__pyx_v_mslice[0]), 'F', __pyx_v_self->view.ndim)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 629, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":627
+  /* "View.MemoryView":625
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
  * 
  *     def is_f_contig(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  */
 
@@ -10536,15 +10367,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":633
+/* "View.MemoryView":631
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -10569,57 +10400,57 @@
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
 
-  /* "View.MemoryView":635
+  /* "View.MemoryView":633
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &mslice)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_F_CONTIGUOUS));
 
-  /* "View.MemoryView":637
+  /* "View.MemoryView":635
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  * 
  *         slice_copy(self, &mslice)             # <<<<<<<<<<<<<<
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,
  *                                    self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_mslice));
 
-  /* "View.MemoryView":638
+  /* "View.MemoryView":636
  * 
  *         slice_copy(self, &mslice)
  *         mslice = slice_copy_contig(&mslice, "c", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                    self.view.itemsize,
  *                                    flags|PyBUF_C_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 638, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_mslice), ((char *)"c"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_C_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 636, __pyx_L1_error)
   __pyx_v_mslice = __pyx_t_1;
 
-  /* "View.MemoryView":643
+  /* "View.MemoryView":641
  *                                    self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &mslice)             # <<<<<<<<<<<<<<
  * 
  *     def copy_fortran(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 643, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_mslice)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 641, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":633
+  /* "View.MemoryView":631
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
  * 
  *     def copy(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS
  */
 
@@ -10630,15 +10461,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":645
+/* "View.MemoryView":643
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -10664,57 +10495,57 @@
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy_fortran", 0);
 
-  /* "View.MemoryView":647
+  /* "View.MemoryView":645
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
  *         slice_copy(self, &src)
  */
   __pyx_v_flags = (__pyx_v_self->flags & (~PyBUF_C_CONTIGUOUS));
 
-  /* "View.MemoryView":649
+  /* "View.MemoryView":647
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  * 
  *         slice_copy(self, &src)             # <<<<<<<<<<<<<<
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,
  *                                 self.view.itemsize,
  */
   __pyx_memoryview_slice_copy(__pyx_v_self, (&__pyx_v_src));
 
-  /* "View.MemoryView":650
+  /* "View.MemoryView":648
  * 
  *         slice_copy(self, &src)
  *         dst = slice_copy_contig(&src, "fortran", self.view.ndim,             # <<<<<<<<<<<<<<
  *                                 self.view.itemsize,
  *                                 flags|PyBUF_F_CONTIGUOUS,
  */
-  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 650, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_new_contig((&__pyx_v_src), ((char *)"fortran"), __pyx_v_self->view.ndim, __pyx_v_self->view.itemsize, (__pyx_v_flags | PyBUF_F_CONTIGUOUS), __pyx_v_self->dtype_is_object); if (unlikely(PyErr_Occurred())) __PYX_ERR(2, 648, __pyx_L1_error)
   __pyx_v_dst = __pyx_t_1;
 
-  /* "View.MemoryView":655
+  /* "View.MemoryView":653
  *                                 self.dtype_is_object)
  * 
  *         return memoryview_copy_from_slice(self, &dst)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 655, __pyx_L1_error)
+  __pyx_t_2 = __pyx_memoryview_copy_object_from_slice(__pyx_v_self, (&__pyx_v_dst)); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 653, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":645
+  /* "View.MemoryView":643
  *         return memoryview_copy_from_slice(self, &mslice)
  * 
  *     def copy_fortran(self):             # <<<<<<<<<<<<<<
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS
  */
 
@@ -10838,15 +10669,15 @@
   __Pyx_AddTraceback("View.MemoryView.memoryview.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":659
+/* "View.MemoryView":657
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -10858,64 +10689,64 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
 
-  /* "View.MemoryView":660
+  /* "View.MemoryView":658
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
  *     return result
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 660, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 658, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 660, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 658, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 660, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 658, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_v_o);
   __Pyx_GIVEREF(__pyx_v_o);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_o);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 660, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryview_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 658, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryview_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":661
+  /* "View.MemoryView":659
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo             # <<<<<<<<<<<<<<
  *     return result
  * 
  */
   __pyx_v_result->typeinfo = __pyx_v_typeinfo;
 
-  /* "View.MemoryView":662
+  /* "View.MemoryView":660
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_check')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":659
+  /* "View.MemoryView":657
  * 
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):             # <<<<<<<<<<<<<<
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)
  *     result.typeinfo = typeinfo
  */
 
@@ -10929,54 +10760,54 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":665
+/* "View.MemoryView":663
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *__pyx_v_o) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("memoryview_check", 0);
 
-  /* "View.MemoryView":666
+  /* "View.MemoryView":664
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):
  *     return isinstance(o, memoryview)             # <<<<<<<<<<<<<<
  * 
  * cdef tuple _unellipsify(object index, int ndim):
  */
   __pyx_t_1 = __Pyx_TypeCheck(__pyx_v_o, __pyx_memoryview_type); 
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":665
+  /* "View.MemoryView":663
  * 
  * @cname('__pyx_memoryview_check')
  * cdef inline bint memoryview_check(object o):             # <<<<<<<<<<<<<<
  *     return isinstance(o, memoryview)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":668
+/* "View.MemoryView":666
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -11002,243 +10833,243 @@
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unellipsify", 0);
 
-  /* "View.MemoryView":673
+  /* "View.MemoryView":671
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
   __pyx_t_1 = PyTuple_Check(__pyx_v_index); 
   __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":674
+    /* "View.MemoryView":672
  *     """
  *     if not isinstance(index, tuple):
  *         tup = (index,)             # <<<<<<<<<<<<<<
  *     else:
  *         tup = index
  */
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 674, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 672, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_index);
     __Pyx_GIVEREF(__pyx_v_index);
     PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_v_index);
     __pyx_v_tup = __pyx_t_3;
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":673
+    /* "View.MemoryView":671
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":676
+  /* "View.MemoryView":674
  *         tup = (index,)
  *     else:
  *         tup = index             # <<<<<<<<<<<<<<
  * 
  *     result = []
  */
   /*else*/ {
     __Pyx_INCREF(__pyx_v_index);
     __pyx_v_tup = __pyx_v_index;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":678
+  /* "View.MemoryView":676
  *         tup = index
  * 
  *     result = []             # <<<<<<<<<<<<<<
  *     have_slices = False
  *     seen_ellipsis = False
  */
-  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 678, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 676, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_result = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":679
+  /* "View.MemoryView":677
  * 
  *     result = []
  *     have_slices = False             # <<<<<<<<<<<<<<
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  */
   __pyx_v_have_slices = 0;
 
-  /* "View.MemoryView":680
+  /* "View.MemoryView":678
  *     result = []
  *     have_slices = False
  *     seen_ellipsis = False             # <<<<<<<<<<<<<<
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  */
   __pyx_v_seen_ellipsis = 0;
 
-  /* "View.MemoryView":681
+  /* "View.MemoryView":679
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   __Pyx_INCREF(__pyx_int_0);
   __pyx_t_3 = __pyx_int_0;
   if (likely(PyList_CheckExact(__pyx_v_tup)) || PyTuple_CheckExact(__pyx_v_tup)) {
     __pyx_t_4 = __pyx_v_tup; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 681, __pyx_L1_error)
+    __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_v_tup); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 679, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 681, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_4)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(2, 679, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_4))) {
         if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 681, __pyx_L1_error)
+        __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 679, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       } else {
         if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 681, __pyx_L1_error)
+        __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(2, 679, __pyx_L1_error)
         #else
-        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
+        __pyx_t_7 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         #endif
       }
     } else {
       __pyx_t_7 = __pyx_t_6(__pyx_t_4);
       if (unlikely(!__pyx_t_7)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 681, __pyx_L1_error)
+          else __PYX_ERR(2, 679, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_7);
     }
     __Pyx_XDECREF_SET(__pyx_v_item, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_XDECREF_SET(__pyx_v_idx, __pyx_t_3);
-    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 681, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_AddObjC(__pyx_t_3, __pyx_int_1, 1, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 679, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_3);
     __pyx_t_3 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "View.MemoryView":682
+    /* "View.MemoryView":680
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
     __pyx_t_2 = (__pyx_v_item == __pyx_builtin_Ellipsis);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":683
+      /* "View.MemoryView":681
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
       __pyx_t_1 = ((!(__pyx_v_seen_ellipsis != 0)) != 0);
       if (__pyx_t_1) {
 
-        /* "View.MemoryView":684
+        /* "View.MemoryView":682
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
-        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 684, __pyx_L1_error)
+        __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(2, 682, __pyx_L1_error)
+        __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 682, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
             __Pyx_INCREF(__pyx_slice__17);
             __Pyx_GIVEREF(__pyx_slice__17);
             PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__17);
           }
         }
-        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 684, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 682, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-        /* "View.MemoryView":685
+        /* "View.MemoryView":683
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True             # <<<<<<<<<<<<<<
  *             else:
  *                 result.append(slice(None))
  */
         __pyx_v_seen_ellipsis = 1;
 
-        /* "View.MemoryView":683
+        /* "View.MemoryView":681
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:
  *             if not seen_ellipsis:             # <<<<<<<<<<<<<<
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  *                 seen_ellipsis = True
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":687
+      /* "View.MemoryView":685
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__17); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 685, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":688
+      /* "View.MemoryView":686
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  */
       __pyx_v_have_slices = 1;
 
-      /* "View.MemoryView":682
+      /* "View.MemoryView":680
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):
  *         if item is Ellipsis:             # <<<<<<<<<<<<<<
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":690
+    /* "View.MemoryView":688
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
     /*else*/ {
@@ -11250,40 +11081,40 @@
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = ((!(PyIndex_Check(__pyx_v_item) != 0)) != 0);
       __pyx_t_1 = __pyx_t_10;
       __pyx_L9_bool_binop_done:;
       if (unlikely(__pyx_t_1)) {
 
-        /* "View.MemoryView":691
+        /* "View.MemoryView":689
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):
  *                 raise TypeError("Cannot index with type '%s'" % type(item))             # <<<<<<<<<<<<<<
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  */
-        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 691, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyString_FormatSafe(__pyx_kp_s_Cannot_index_with_type_s, ((PyObject *)Py_TYPE(__pyx_v_item))); if (unlikely(!__pyx_t_7)) __PYX_ERR(2, 689, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
-        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 691, __pyx_L1_error)
+        __pyx_t_11 = __Pyx_PyObject_CallOneArg(__pyx_builtin_TypeError, __pyx_t_7); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 689, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_11);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_Raise(__pyx_t_11, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        __PYX_ERR(2, 691, __pyx_L1_error)
+        __PYX_ERR(2, 689, __pyx_L1_error)
 
-        /* "View.MemoryView":690
+        /* "View.MemoryView":688
  *             have_slices = True
  *         else:
  *             if not isinstance(item, slice) and not PyIndex_Check(item):             # <<<<<<<<<<<<<<
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  */
       }
 
-      /* "View.MemoryView":693
+      /* "View.MemoryView":691
  *                 raise TypeError("Cannot index with type '%s'" % type(item))
  * 
  *             have_slices = have_slices or isinstance(item, slice)             # <<<<<<<<<<<<<<
  *             result.append(item)
  * 
  */
       __pyx_t_10 = (__pyx_v_have_slices != 0);
@@ -11294,120 +11125,120 @@
       }
       __pyx_t_10 = PySlice_Check(__pyx_v_item); 
       __pyx_t_2 = (__pyx_t_10 != 0);
       __pyx_t_1 = __pyx_t_2;
       __pyx_L11_bool_binop_done:;
       __pyx_v_have_slices = __pyx_t_1;
 
-      /* "View.MemoryView":694
+      /* "View.MemoryView":692
  * 
  *             have_slices = have_slices or isinstance(item, slice)
  *             result.append(item)             # <<<<<<<<<<<<<<
  * 
  *     nslices = ndim - len(result)
  */
-      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 694, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_v_item); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 692, __pyx_L1_error)
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":681
+    /* "View.MemoryView":679
  *     have_slices = False
  *     seen_ellipsis = False
  *     for idx, item in enumerate(tup):             # <<<<<<<<<<<<<<
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  */
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":696
+  /* "View.MemoryView":694
  *             result.append(item)
  * 
  *     nslices = ndim - len(result)             # <<<<<<<<<<<<<<
  *     if nslices:
  *         result.extend([slice(None)] * nslices)
  */
-  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(2, 696, __pyx_L1_error)
+  __pyx_t_5 = PyList_GET_SIZE(__pyx_v_result); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(2, 694, __pyx_L1_error)
   __pyx_v_nslices = (__pyx_v_ndim - __pyx_t_5);
 
-  /* "View.MemoryView":697
+  /* "View.MemoryView":695
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   __pyx_t_1 = (__pyx_v_nslices != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":698
+    /* "View.MemoryView":696
  *     nslices = ndim - len(result)
  *     if nslices:
  *         result.extend([slice(None)] * nslices)             # <<<<<<<<<<<<<<
  * 
  *     return have_slices or nslices, tuple(result)
  */
-    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 698, __pyx_L1_error)
+    __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 696, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
         __Pyx_INCREF(__pyx_slice__17);
         __Pyx_GIVEREF(__pyx_slice__17);
         PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__17);
       }
     }
-    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 698, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 696, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "View.MemoryView":697
+    /* "View.MemoryView":695
  * 
  *     nslices = ndim - len(result)
  *     if nslices:             # <<<<<<<<<<<<<<
  *         result.extend([slice(None)] * nslices)
  * 
  */
   }
 
-  /* "View.MemoryView":700
+  /* "View.MemoryView":698
  *         result.extend([slice(None)] * nslices)
  * 
  *     return have_slices or nslices, tuple(result)             # <<<<<<<<<<<<<<
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  */
   __Pyx_XDECREF(__pyx_r);
   if (!__pyx_v_have_slices) {
   } else {
-    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyBool_FromLong(__pyx_v_have_slices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L14_bool_binop_done;
   }
-  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t(__pyx_v_nslices); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = __pyx_t_4;
   __pyx_t_4 = 0;
   __pyx_L14_bool_binop_done:;
-  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 700, __pyx_L1_error)
+  __pyx_t_4 = PyList_AsTuple(__pyx_v_result); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 700, __pyx_L1_error)
+  __pyx_t_11 = PyTuple_New(2); if (unlikely(!__pyx_t_11)) __PYX_ERR(2, 698, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_11);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_11, 1, __pyx_t_4);
   __pyx_t_3 = 0;
   __pyx_t_4 = 0;
   __pyx_r = ((PyObject*)__pyx_t_11);
   __pyx_t_11 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":668
+  /* "View.MemoryView":666
  *     return isinstance(o, memoryview)
  * 
  * cdef tuple _unellipsify(object index, int ndim):             # <<<<<<<<<<<<<<
  *     """
  *     Replace all ellipses with full slices and fill incomplete indices with
  */
 
@@ -11425,15 +11256,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_item);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":702
+/* "View.MemoryView":700
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -11447,60 +11278,60 @@
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
-  /* "View.MemoryView":703
+  /* "View.MemoryView":701
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")
  */
   __pyx_t_2 = (__pyx_v_suboffsets + __pyx_v_ndim);
   for (__pyx_t_3 = __pyx_v_suboffsets; __pyx_t_3 < __pyx_t_2; __pyx_t_3++) {
     __pyx_t_1 = __pyx_t_3;
     __pyx_v_suboffset = (__pyx_t_1[0]);
 
-    /* "View.MemoryView":704
+    /* "View.MemoryView":702
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     __pyx_t_4 = ((__pyx_v_suboffset >= 0) != 0);
     if (unlikely(__pyx_t_4)) {
 
-      /* "View.MemoryView":705
+      /* "View.MemoryView":703
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 703, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(2, 705, __pyx_L1_error)
+      __PYX_ERR(2, 703, __pyx_L1_error)
 
-      /* "View.MemoryView":704
+      /* "View.MemoryView":702
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             raise ValueError("Indirect dimensions not supported")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":702
+  /* "View.MemoryView":700
  *     return have_slices or nslices, tuple(result)
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):             # <<<<<<<<<<<<<<
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
 
@@ -11513,15 +11344,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":712
+/* "View.MemoryView":710
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -11557,529 +11388,529 @@
   int __pyx_t_11;
   Py_ssize_t __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memview_slice", 0);
 
-  /* "View.MemoryView":713
+  /* "View.MemoryView":711
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
  *     cdef __Pyx_memviewslice src, dst
  */
   __pyx_v_new_ndim = 0;
   __pyx_v_suboffset_dim = -1;
 
-  /* "View.MemoryView":720
+  /* "View.MemoryView":718
  * 
  * 
  *     memset(&dst, 0, sizeof(dst))             # <<<<<<<<<<<<<<
  * 
  *     cdef _memoryviewslice memviewsliceobj
  */
   (void)(memset((&__pyx_v_dst), 0, (sizeof(__pyx_v_dst))));
 
-  /* "View.MemoryView":724
+  /* "View.MemoryView":722
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
   if (unlikely(!Py_OptimizeFlag)) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
-      __PYX_ERR(2, 724, __pyx_L1_error)
+      __PYX_ERR(2, 722, __pyx_L1_error)
     }
   }
   #endif
 
-  /* "View.MemoryView":726
+  /* "View.MemoryView":724
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":727
+    /* "View.MemoryView":725
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview             # <<<<<<<<<<<<<<
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 727, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 725, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_memviewsliceobj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":728
+    /* "View.MemoryView":726
  *     if isinstance(memview, _memoryviewslice):
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, &src)
  */
     __pyx_v_p_src = (&__pyx_v_memviewsliceobj->from_slice);
 
-    /* "View.MemoryView":726
+    /* "View.MemoryView":724
  *     assert memview.view.ndim > 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         memviewsliceobj = memview
  *         p_src = &memviewsliceobj.from_slice
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":730
+  /* "View.MemoryView":728
  *         p_src = &memviewsliceobj.from_slice
  *     else:
  *         slice_copy(memview, &src)             # <<<<<<<<<<<<<<
  *         p_src = &src
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_src));
 
-    /* "View.MemoryView":731
+    /* "View.MemoryView":729
  *     else:
  *         slice_copy(memview, &src)
  *         p_src = &src             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_p_src = (&__pyx_v_src);
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":737
+  /* "View.MemoryView":735
  * 
  * 
  *     dst.memview = p_src.memview             # <<<<<<<<<<<<<<
  *     dst.data = p_src.data
  * 
  */
   __pyx_t_4 = __pyx_v_p_src->memview;
   __pyx_v_dst.memview = __pyx_t_4;
 
-  /* "View.MemoryView":738
+  /* "View.MemoryView":736
  * 
  *     dst.memview = p_src.memview
  *     dst.data = p_src.data             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_5 = __pyx_v_p_src->data;
   __pyx_v_dst.data = __pyx_t_5;
 
-  /* "View.MemoryView":743
+  /* "View.MemoryView":741
  * 
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst             # <<<<<<<<<<<<<<
  *     cdef int *p_suboffset_dim = &suboffset_dim
  *     cdef Py_ssize_t start, stop, step
  */
   __pyx_v_p_dst = (&__pyx_v_dst);
 
-  /* "View.MemoryView":744
+  /* "View.MemoryView":742
  * 
  *     cdef __Pyx_memviewslice *p_dst = &dst
  *     cdef int *p_suboffset_dim = &suboffset_dim             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t start, stop, step
  *     cdef bint have_start, have_stop, have_step
  */
   __pyx_v_p_suboffset_dim = (&__pyx_v_suboffset_dim);
 
-  /* "View.MemoryView":748
+  /* "View.MemoryView":746
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   __pyx_t_6 = 0;
   if (likely(PyList_CheckExact(__pyx_v_indices)) || PyTuple_CheckExact(__pyx_v_indices)) {
     __pyx_t_3 = __pyx_v_indices; __Pyx_INCREF(__pyx_t_3); __pyx_t_7 = 0;
     __pyx_t_8 = NULL;
   } else {
-    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 748, __pyx_L1_error)
+    __pyx_t_7 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_indices); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 746, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 748, __pyx_L1_error)
+    __pyx_t_8 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 746, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_8)) {
       if (likely(PyList_CheckExact(__pyx_t_3))) {
         if (__pyx_t_7 >= PyList_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 748, __pyx_L1_error)
+        __pyx_t_9 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 746, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 748, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 746, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       } else {
         if (__pyx_t_7 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 748, __pyx_L1_error)
+        __pyx_t_9 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_7); __Pyx_INCREF(__pyx_t_9); __pyx_t_7++; if (unlikely(0 < 0)) __PYX_ERR(2, 746, __pyx_L1_error)
         #else
-        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 748, __pyx_L1_error)
+        __pyx_t_9 = PySequence_ITEM(__pyx_t_3, __pyx_t_7); __pyx_t_7++; if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 746, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
         #endif
       }
     } else {
       __pyx_t_9 = __pyx_t_8(__pyx_t_3);
       if (unlikely(!__pyx_t_9)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(2, 748, __pyx_L1_error)
+          else __PYX_ERR(2, 746, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_9);
     }
     __Pyx_XDECREF_SET(__pyx_v_index, __pyx_t_9);
     __pyx_t_9 = 0;
     __pyx_v_dim = __pyx_t_6;
     __pyx_t_6 = (__pyx_t_6 + 1);
 
-    /* "View.MemoryView":749
+    /* "View.MemoryView":747
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
     __pyx_t_2 = (PyIndex_Check(__pyx_v_index) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":753
+      /* "View.MemoryView":751
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  *                 index, 0, 0, # start, stop, step             # <<<<<<<<<<<<<<
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  */
-      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 753, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyIndex_AsSsize_t(__pyx_v_index); if (unlikely((__pyx_t_10 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 751, __pyx_L1_error)
 
-      /* "View.MemoryView":750
+      /* "View.MemoryView":748
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 750, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_t_10, 0, 0, 0, 0, 0, 0); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 748, __pyx_L1_error)
 
-      /* "View.MemoryView":749
+      /* "View.MemoryView":747
  * 
  *     for dim, index in enumerate(indices):
  *         if PyIndex_Check(index):             # <<<<<<<<<<<<<<
  *             slice_memviewslice(
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":756
+    /* "View.MemoryView":754
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
     __pyx_t_2 = (__pyx_v_index == Py_None);
     __pyx_t_1 = (__pyx_t_2 != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":757
+      /* "View.MemoryView":755
  *                 False)
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1             # <<<<<<<<<<<<<<
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  */
       (__pyx_v_p_dst->shape[__pyx_v_new_ndim]) = 1;
 
-      /* "View.MemoryView":758
+      /* "View.MemoryView":756
  *         elif index is None:
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0             # <<<<<<<<<<<<<<
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1
  */
       (__pyx_v_p_dst->strides[__pyx_v_new_ndim]) = 0;
 
-      /* "View.MemoryView":759
+      /* "View.MemoryView":757
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1             # <<<<<<<<<<<<<<
  *             new_ndim += 1
  *         else:
  */
       (__pyx_v_p_dst->suboffsets[__pyx_v_new_ndim]) = -1L;
 
-      /* "View.MemoryView":760
+      /* "View.MemoryView":758
  *             p_dst.strides[new_ndim] = 0
  *             p_dst.suboffsets[new_ndim] = -1
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  *         else:
  *             start = index.start or 0
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
 
-      /* "View.MemoryView":756
+      /* "View.MemoryView":754
  *                 0, 0, 0, # have_{start,stop,step}
  *                 False)
  *         elif index is None:             # <<<<<<<<<<<<<<
  *             p_dst.shape[new_ndim] = 1
  *             p_dst.strides[new_ndim] = 0
  */
       goto __pyx_L6;
     }
 
-    /* "View.MemoryView":762
+    /* "View.MemoryView":760
  *             new_ndim += 1
  *         else:
  *             start = index.start or 0             # <<<<<<<<<<<<<<
  *             stop = index.stop or 0
  *             step = index.step or 0
  */
     /*else*/ {
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 762, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 760, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 762, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 760, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 762, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 760, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L7_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L7_bool_binop_done:;
       __pyx_v_start = __pyx_t_10;
 
-      /* "View.MemoryView":763
+      /* "View.MemoryView":761
  *         else:
  *             start = index.start or 0
  *             stop = index.stop or 0             # <<<<<<<<<<<<<<
  *             step = index.step or 0
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 763, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 761, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 763, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 761, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 763, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 761, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L9_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L9_bool_binop_done:;
       __pyx_v_stop = __pyx_t_10;
 
-      /* "View.MemoryView":764
+      /* "View.MemoryView":762
  *             start = index.start or 0
  *             stop = index.stop or 0
  *             step = index.step or 0             # <<<<<<<<<<<<<<
  * 
  *             have_start = index.start is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 764, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 762, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 764, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_9); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(2, 762, __pyx_L1_error)
       if (!__pyx_t_1) {
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       } else {
-        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 764, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyIndex_AsSsize_t(__pyx_t_9); if (unlikely((__pyx_t_12 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 762, __pyx_L1_error)
         __pyx_t_10 = __pyx_t_12;
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L11_bool_binop_done;
       }
       __pyx_t_10 = 0;
       __pyx_L11_bool_binop_done:;
       __pyx_v_step = __pyx_t_10;
 
-      /* "View.MemoryView":766
+      /* "View.MemoryView":764
  *             step = index.step or 0
  * 
  *             have_start = index.start is not None             # <<<<<<<<<<<<<<
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 766, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_start); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 764, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_start = __pyx_t_1;
 
-      /* "View.MemoryView":767
+      /* "View.MemoryView":765
  * 
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None             # <<<<<<<<<<<<<<
  *             have_step = index.step is not None
  * 
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 767, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_stop); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 765, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_stop = __pyx_t_1;
 
-      /* "View.MemoryView":768
+      /* "View.MemoryView":766
  *             have_start = index.start is not None
  *             have_stop = index.stop is not None
  *             have_step = index.step is not None             # <<<<<<<<<<<<<<
  * 
  *             slice_memviewslice(
  */
-      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 768, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyObject_GetAttrStr(__pyx_v_index, __pyx_n_s_step); if (unlikely(!__pyx_t_9)) __PYX_ERR(2, 766, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
       __pyx_t_1 = (__pyx_t_9 != Py_None);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_v_have_step = __pyx_t_1;
 
-      /* "View.MemoryView":770
+      /* "View.MemoryView":768
  *             have_step = index.step is not None
  * 
  *             slice_memviewslice(             # <<<<<<<<<<<<<<
  *                 p_dst, p_src.shape[dim], p_src.strides[dim], p_src.suboffsets[dim],
  *                 dim, new_ndim, p_suboffset_dim,
  */
-      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 770, __pyx_L1_error)
+      __pyx_t_11 = __pyx_memoryview_slice_memviewslice(__pyx_v_p_dst, (__pyx_v_p_src->shape[__pyx_v_dim]), (__pyx_v_p_src->strides[__pyx_v_dim]), (__pyx_v_p_src->suboffsets[__pyx_v_dim]), __pyx_v_dim, __pyx_v_new_ndim, __pyx_v_p_suboffset_dim, __pyx_v_start, __pyx_v_stop, __pyx_v_step, __pyx_v_have_start, __pyx_v_have_stop, __pyx_v_have_step, 1); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(2, 768, __pyx_L1_error)
 
-      /* "View.MemoryView":776
+      /* "View.MemoryView":774
  *                 have_start, have_stop, have_step,
  *                 True)
  *             new_ndim += 1             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
       __pyx_v_new_ndim = (__pyx_v_new_ndim + 1);
     }
     __pyx_L6:;
 
-    /* "View.MemoryView":748
+    /* "View.MemoryView":746
  *     cdef bint have_start, have_stop, have_step
  * 
  *     for dim, index in enumerate(indices):             # <<<<<<<<<<<<<<
  *         if PyIndex_Check(index):
  *             slice_memviewslice(
  */
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "View.MemoryView":778
+  /* "View.MemoryView":776
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":779
+    /* "View.MemoryView":777
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":780
+    /* "View.MemoryView":778
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_dtype_func,
  *                                     memview.dtype_is_object)
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 780, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 778, __pyx_L1_error) }
 
-    /* "View.MemoryView":781
+    /* "View.MemoryView":779
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  *     else:
  */
-    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 781, __pyx_L1_error) }
+    if (unlikely(!__pyx_v_memviewsliceobj)) { __Pyx_RaiseUnboundLocalError("memviewsliceobj"); __PYX_ERR(2, 779, __pyx_L1_error) }
 
-    /* "View.MemoryView":779
+    /* "View.MemoryView":777
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         return memoryview_fromslice(dst, new_ndim,             # <<<<<<<<<<<<<<
  *                                     memviewsliceobj.to_object_func,
  *                                     memviewsliceobj.to_dtype_func,
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 779, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, __pyx_v_memviewsliceobj->to_object_func, __pyx_v_memviewsliceobj->to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 777, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 779, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 777, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":778
+    /* "View.MemoryView":776
  *             new_ndim += 1
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         return memoryview_fromslice(dst, new_ndim,
  *                                     memviewsliceobj.to_object_func,
  */
   }
 
-  /* "View.MemoryView":784
+  /* "View.MemoryView":782
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(((PyObject *)__pyx_r));
 
-    /* "View.MemoryView":785
+    /* "View.MemoryView":783
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,
  *                                     memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 784, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_fromslice(__pyx_v_dst, __pyx_v_new_ndim, NULL, NULL, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 782, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "View.MemoryView":784
+    /* "View.MemoryView":782
  *                                     memview.dtype_is_object)
  *     else:
  *         return memoryview_fromslice(dst, new_ndim, NULL, NULL,             # <<<<<<<<<<<<<<
  *                                     memview.dtype_is_object)
  * 
  */
-    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 784, __pyx_L1_error)
+    if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_memoryview_type))))) __PYX_ERR(2, 782, __pyx_L1_error)
     __pyx_r = ((struct __pyx_memoryview_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":712
+  /* "View.MemoryView":710
  * 
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):             # <<<<<<<<<<<<<<
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim
  *     cdef bint negative_step
  */
 
@@ -12093,15 +11924,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_memviewsliceobj);
   __Pyx_XDECREF(__pyx_v_index);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":809
+/* "View.MemoryView":807
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -12112,95 +11943,95 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":829
+  /* "View.MemoryView":827
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
   __pyx_t_1 = ((!(__pyx_v_is_slice != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":831
+    /* "View.MemoryView":829
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     __pyx_t_1 = ((__pyx_v_start < 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":832
+      /* "View.MemoryView":830
  * 
  *         if start < 0:
  *             start += shape             # <<<<<<<<<<<<<<
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  */
       __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-      /* "View.MemoryView":831
+      /* "View.MemoryView":829
  *     if not is_slice:
  * 
  *         if start < 0:             # <<<<<<<<<<<<<<
  *             start += shape
  *         if not 0 <= start < shape:
  */
     }
 
-    /* "View.MemoryView":833
+    /* "View.MemoryView":831
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     __pyx_t_1 = (0 <= __pyx_v_start);
     if (__pyx_t_1) {
       __pyx_t_1 = (__pyx_v_start < __pyx_v_shape);
     }
     __pyx_t_2 = ((!(__pyx_t_1 != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":834
+      /* "View.MemoryView":832
  *             start += shape
  *         if not 0 <= start < shape:
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)             # <<<<<<<<<<<<<<
  *     else:
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 834, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"Index out of bounds (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 832, __pyx_L1_error)
 
-      /* "View.MemoryView":833
+      /* "View.MemoryView":831
  *         if start < 0:
  *             start += shape
  *         if not 0 <= start < shape:             # <<<<<<<<<<<<<<
  *             _err_dim(IndexError, "Index out of bounds (axis %d)", dim)
  *     else:
  */
     }
 
-    /* "View.MemoryView":829
+    /* "View.MemoryView":827
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":837
+  /* "View.MemoryView":835
  *     else:
  * 
  *         negative_step = have_step != 0 and step < 0             # <<<<<<<<<<<<<<
  * 
  *         if have_step and step == 0:
  */
   /*else*/ {
@@ -12211,15 +12042,15 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step < 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L6_bool_binop_done:;
     __pyx_v_negative_step = __pyx_t_2;
 
-    /* "View.MemoryView":839
+    /* "View.MemoryView":837
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     __pyx_t_1 = (__pyx_v_have_step != 0);
@@ -12229,639 +12060,639 @@
       goto __pyx_L9_bool_binop_done;
     }
     __pyx_t_1 = ((__pyx_v_step == 0) != 0);
     __pyx_t_2 = __pyx_t_1;
     __pyx_L9_bool_binop_done:;
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":840
+      /* "View.MemoryView":838
  * 
  *         if have_step and step == 0:
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 840, __pyx_L1_error)
+      __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Step may not be zero (axis %d)"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 838, __pyx_L1_error)
 
-      /* "View.MemoryView":839
+      /* "View.MemoryView":837
  *         negative_step = have_step != 0 and step < 0
  * 
  *         if have_step and step == 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Step may not be zero (axis %d)", dim)
  * 
  */
     }
 
-    /* "View.MemoryView":843
+    /* "View.MemoryView":841
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
     __pyx_t_2 = (__pyx_v_have_start != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":844
+      /* "View.MemoryView":842
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
       __pyx_t_2 = ((__pyx_v_start < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":845
+        /* "View.MemoryView":843
  *         if have_start:
  *             if start < 0:
  *                 start += shape             # <<<<<<<<<<<<<<
  *                 if start < 0:
  *                     start = 0
  */
         __pyx_v_start = (__pyx_v_start + __pyx_v_shape);
 
-        /* "View.MemoryView":846
+        /* "View.MemoryView":844
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         __pyx_t_2 = ((__pyx_v_start < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":847
+          /* "View.MemoryView":845
  *                 start += shape
  *                 if start < 0:
  *                     start = 0             # <<<<<<<<<<<<<<
  *             elif start >= shape:
  *                 if negative_step:
  */
           __pyx_v_start = 0;
 
-          /* "View.MemoryView":846
+          /* "View.MemoryView":844
  *             if start < 0:
  *                 start += shape
  *                 if start < 0:             # <<<<<<<<<<<<<<
  *                     start = 0
  *             elif start >= shape:
  */
         }
 
-        /* "View.MemoryView":844
+        /* "View.MemoryView":842
  * 
  *         if have_start:
  *             if start < 0:             # <<<<<<<<<<<<<<
  *                 start += shape
  *                 if start < 0:
  */
         goto __pyx_L12;
       }
 
-      /* "View.MemoryView":848
+      /* "View.MemoryView":846
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       __pyx_t_2 = ((__pyx_v_start >= __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":849
+        /* "View.MemoryView":847
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
         __pyx_t_2 = (__pyx_v_negative_step != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":850
+          /* "View.MemoryView":848
  *             elif start >= shape:
  *                 if negative_step:
  *                     start = shape - 1             # <<<<<<<<<<<<<<
  *                 else:
  *                     start = shape
  */
           __pyx_v_start = (__pyx_v_shape - 1);
 
-          /* "View.MemoryView":849
+          /* "View.MemoryView":847
  *                     start = 0
  *             elif start >= shape:
  *                 if negative_step:             # <<<<<<<<<<<<<<
  *                     start = shape - 1
  *                 else:
  */
           goto __pyx_L14;
         }
 
-        /* "View.MemoryView":852
+        /* "View.MemoryView":850
  *                     start = shape - 1
  *                 else:
  *                     start = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         /*else*/ {
           __pyx_v_start = __pyx_v_shape;
         }
         __pyx_L14:;
 
-        /* "View.MemoryView":848
+        /* "View.MemoryView":846
  *                 if start < 0:
  *                     start = 0
  *             elif start >= shape:             # <<<<<<<<<<<<<<
  *                 if negative_step:
  *                     start = shape - 1
  */
       }
       __pyx_L12:;
 
-      /* "View.MemoryView":843
+      /* "View.MemoryView":841
  * 
  * 
  *         if have_start:             # <<<<<<<<<<<<<<
  *             if start < 0:
  *                 start += shape
  */
       goto __pyx_L11;
     }
 
-    /* "View.MemoryView":854
+    /* "View.MemoryView":852
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":855
+        /* "View.MemoryView":853
  *         else:
  *             if negative_step:
  *                 start = shape - 1             # <<<<<<<<<<<<<<
  *             else:
  *                 start = 0
  */
         __pyx_v_start = (__pyx_v_shape - 1);
 
-        /* "View.MemoryView":854
+        /* "View.MemoryView":852
  *                     start = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 start = shape - 1
  *             else:
  */
         goto __pyx_L15;
       }
 
-      /* "View.MemoryView":857
+      /* "View.MemoryView":855
  *                 start = shape - 1
  *             else:
  *                 start = 0             # <<<<<<<<<<<<<<
  * 
  *         if have_stop:
  */
       /*else*/ {
         __pyx_v_start = 0;
       }
       __pyx_L15:;
     }
     __pyx_L11:;
 
-    /* "View.MemoryView":859
+    /* "View.MemoryView":857
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
     __pyx_t_2 = (__pyx_v_have_stop != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":860
+      /* "View.MemoryView":858
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
       __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":861
+        /* "View.MemoryView":859
  *         if have_stop:
  *             if stop < 0:
  *                 stop += shape             # <<<<<<<<<<<<<<
  *                 if stop < 0:
  *                     stop = 0
  */
         __pyx_v_stop = (__pyx_v_stop + __pyx_v_shape);
 
-        /* "View.MemoryView":862
+        /* "View.MemoryView":860
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         __pyx_t_2 = ((__pyx_v_stop < 0) != 0);
         if (__pyx_t_2) {
 
-          /* "View.MemoryView":863
+          /* "View.MemoryView":861
  *                 stop += shape
  *                 if stop < 0:
  *                     stop = 0             # <<<<<<<<<<<<<<
  *             elif stop > shape:
  *                 stop = shape
  */
           __pyx_v_stop = 0;
 
-          /* "View.MemoryView":862
+          /* "View.MemoryView":860
  *             if stop < 0:
  *                 stop += shape
  *                 if stop < 0:             # <<<<<<<<<<<<<<
  *                     stop = 0
  *             elif stop > shape:
  */
         }
 
-        /* "View.MemoryView":860
+        /* "View.MemoryView":858
  * 
  *         if have_stop:
  *             if stop < 0:             # <<<<<<<<<<<<<<
  *                 stop += shape
  *                 if stop < 0:
  */
         goto __pyx_L17;
       }
 
-      /* "View.MemoryView":864
+      /* "View.MemoryView":862
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       __pyx_t_2 = ((__pyx_v_stop > __pyx_v_shape) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":865
+        /* "View.MemoryView":863
  *                     stop = 0
  *             elif stop > shape:
  *                 stop = shape             # <<<<<<<<<<<<<<
  *         else:
  *             if negative_step:
  */
         __pyx_v_stop = __pyx_v_shape;
 
-        /* "View.MemoryView":864
+        /* "View.MemoryView":862
  *                 if stop < 0:
  *                     stop = 0
  *             elif stop > shape:             # <<<<<<<<<<<<<<
  *                 stop = shape
  *         else:
  */
       }
       __pyx_L17:;
 
-      /* "View.MemoryView":859
+      /* "View.MemoryView":857
  *                 start = 0
  * 
  *         if have_stop:             # <<<<<<<<<<<<<<
  *             if stop < 0:
  *                 stop += shape
  */
       goto __pyx_L16;
     }
 
-    /* "View.MemoryView":867
+    /* "View.MemoryView":865
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_negative_step != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":868
+        /* "View.MemoryView":866
  *         else:
  *             if negative_step:
  *                 stop = -1             # <<<<<<<<<<<<<<
  *             else:
  *                 stop = shape
  */
         __pyx_v_stop = -1L;
 
-        /* "View.MemoryView":867
+        /* "View.MemoryView":865
  *                 stop = shape
  *         else:
  *             if negative_step:             # <<<<<<<<<<<<<<
  *                 stop = -1
  *             else:
  */
         goto __pyx_L19;
       }
 
-      /* "View.MemoryView":870
+      /* "View.MemoryView":868
  *                 stop = -1
  *             else:
  *                 stop = shape             # <<<<<<<<<<<<<<
  * 
  *         if not have_step:
  */
       /*else*/ {
         __pyx_v_stop = __pyx_v_shape;
       }
       __pyx_L19:;
     }
     __pyx_L16:;
 
-    /* "View.MemoryView":872
+    /* "View.MemoryView":870
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     __pyx_t_2 = ((!(__pyx_v_have_step != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":873
+      /* "View.MemoryView":871
  * 
  *         if not have_step:
  *             step = 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_step = 1;
 
-      /* "View.MemoryView":872
+      /* "View.MemoryView":870
  *                 stop = shape
  * 
  *         if not have_step:             # <<<<<<<<<<<<<<
  *             step = 1
  * 
  */
     }
 
-    /* "View.MemoryView":877
+    /* "View.MemoryView":875
  * 
  *         with cython.cdivision(True):
  *             new_shape = (stop - start) // step             # <<<<<<<<<<<<<<
  * 
  *             if (stop - start) - step * new_shape:
  */
     __pyx_v_new_shape = ((__pyx_v_stop - __pyx_v_start) / __pyx_v_step);
 
-    /* "View.MemoryView":879
+    /* "View.MemoryView":877
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     __pyx_t_2 = (((__pyx_v_stop - __pyx_v_start) - (__pyx_v_step * __pyx_v_new_shape)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":880
+      /* "View.MemoryView":878
  * 
  *             if (stop - start) - step * new_shape:
  *                 new_shape += 1             # <<<<<<<<<<<<<<
  * 
  *         if new_shape < 0:
  */
       __pyx_v_new_shape = (__pyx_v_new_shape + 1);
 
-      /* "View.MemoryView":879
+      /* "View.MemoryView":877
  *             new_shape = (stop - start) // step
  * 
  *             if (stop - start) - step * new_shape:             # <<<<<<<<<<<<<<
  *                 new_shape += 1
  * 
  */
     }
 
-    /* "View.MemoryView":882
+    /* "View.MemoryView":880
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     __pyx_t_2 = ((__pyx_v_new_shape < 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":883
+      /* "View.MemoryView":881
  * 
  *         if new_shape < 0:
  *             new_shape = 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_new_shape = 0;
 
-      /* "View.MemoryView":882
+      /* "View.MemoryView":880
  *                 new_shape += 1
  * 
  *         if new_shape < 0:             # <<<<<<<<<<<<<<
  *             new_shape = 0
  * 
  */
     }
 
-    /* "View.MemoryView":886
+    /* "View.MemoryView":884
  * 
  * 
  *         dst.strides[new_ndim] = stride * step             # <<<<<<<<<<<<<<
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset
  */
     (__pyx_v_dst->strides[__pyx_v_new_ndim]) = (__pyx_v_stride * __pyx_v_step);
 
-    /* "View.MemoryView":887
+    /* "View.MemoryView":885
  * 
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape             # <<<<<<<<<<<<<<
  *         dst.suboffsets[new_ndim] = suboffset
  * 
  */
     (__pyx_v_dst->shape[__pyx_v_new_ndim]) = __pyx_v_new_shape;
 
-    /* "View.MemoryView":888
+    /* "View.MemoryView":886
  *         dst.strides[new_ndim] = stride * step
  *         dst.shape[new_ndim] = new_shape
  *         dst.suboffsets[new_ndim] = suboffset             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_dst->suboffsets[__pyx_v_new_ndim]) = __pyx_v_suboffset;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":891
+  /* "View.MemoryView":889
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
   __pyx_t_2 = (((__pyx_v_suboffset_dim[0]) < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":892
+    /* "View.MemoryView":890
  * 
  *     if suboffset_dim[0] < 0:
  *         dst.data += start * stride             # <<<<<<<<<<<<<<
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  */
     __pyx_v_dst->data = (__pyx_v_dst->data + (__pyx_v_start * __pyx_v_stride));
 
-    /* "View.MemoryView":891
+    /* "View.MemoryView":889
  * 
  * 
  *     if suboffset_dim[0] < 0:             # <<<<<<<<<<<<<<
  *         dst.data += start * stride
  *     else:
  */
     goto __pyx_L23;
   }
 
-  /* "View.MemoryView":894
+  /* "View.MemoryView":892
  *         dst.data += start * stride
  *     else:
  *         dst.suboffsets[suboffset_dim[0]] += start * stride             # <<<<<<<<<<<<<<
  * 
  *     if suboffset >= 0:
  */
   /*else*/ {
     __pyx_t_3 = (__pyx_v_suboffset_dim[0]);
     (__pyx_v_dst->suboffsets[__pyx_t_3]) = ((__pyx_v_dst->suboffsets[__pyx_t_3]) + (__pyx_v_start * __pyx_v_stride));
   }
   __pyx_L23:;
 
-  /* "View.MemoryView":896
+  /* "View.MemoryView":894
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":897
+    /* "View.MemoryView":895
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
     __pyx_t_2 = ((!(__pyx_v_is_slice != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":898
+      /* "View.MemoryView":896
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
       __pyx_t_2 = ((__pyx_v_new_ndim == 0) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":899
+        /* "View.MemoryView":897
  *         if not is_slice:
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  */
         __pyx_v_dst->data = ((((char **)__pyx_v_dst->data)[0]) + __pyx_v_suboffset);
 
-        /* "View.MemoryView":898
+        /* "View.MemoryView":896
  *     if suboffset >= 0:
  *         if not is_slice:
  *             if new_ndim == 0:             # <<<<<<<<<<<<<<
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  */
         goto __pyx_L26;
       }
 
-      /* "View.MemoryView":901
+      /* "View.MemoryView":899
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "             # <<<<<<<<<<<<<<
  *                                      "must be indexed and not sliced", dim)
  *         else:
  */
       /*else*/ {
 
-        /* "View.MemoryView":902
+        /* "View.MemoryView":900
  *             else:
  *                 _err_dim(IndexError, "All dimensions preceding dimension %d "
  *                                      "must be indexed and not sliced", dim)             # <<<<<<<<<<<<<<
  *         else:
  *             suboffset_dim[0] = new_ndim
  */
-        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 901, __pyx_L1_error)
+        __pyx_t_3 = __pyx_memoryview_err_dim(__pyx_builtin_IndexError, ((char *)"All dimensions preceding dimension %d must be indexed and not sliced"), __pyx_v_dim); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 899, __pyx_L1_error)
       }
       __pyx_L26:;
 
-      /* "View.MemoryView":897
+      /* "View.MemoryView":895
  * 
  *     if suboffset >= 0:
  *         if not is_slice:             # <<<<<<<<<<<<<<
  *             if new_ndim == 0:
  *                 dst.data = (<char **> dst.data)[0] + suboffset
  */
       goto __pyx_L25;
     }
 
-    /* "View.MemoryView":904
+    /* "View.MemoryView":902
  *                                      "must be indexed and not sliced", dim)
  *         else:
  *             suboffset_dim[0] = new_ndim             # <<<<<<<<<<<<<<
  * 
  *     return 0
  */
     /*else*/ {
       (__pyx_v_suboffset_dim[0]) = __pyx_v_new_ndim;
     }
     __pyx_L25:;
 
-    /* "View.MemoryView":896
+    /* "View.MemoryView":894
  *         dst.suboffsets[suboffset_dim[0]] += start * stride
  * 
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         if not is_slice:
  *             if new_ndim == 0:
  */
   }
 
-  /* "View.MemoryView":906
+  /* "View.MemoryView":904
  *             suboffset_dim[0] = new_ndim
  * 
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":809
+  /* "View.MemoryView":807
  * 
  * @cname('__pyx_memoryview_slice_memviewslice')
  * cdef int slice_memviewslice(             # <<<<<<<<<<<<<<
  *         __Pyx_memviewslice *dst,
  *         Py_ssize_t shape, Py_ssize_t stride, Py_ssize_t suboffset,
  */
 
@@ -12877,15 +12708,15 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":912
+/* "View.MemoryView":910
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -12902,280 +12733,280 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pybuffer_index", 0);
 
-  /* "View.MemoryView":914
+  /* "View.MemoryView":912
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
  *     cdef char *resultp
  */
   __pyx_v_suboffset = -1L;
 
-  /* "View.MemoryView":915
+  /* "View.MemoryView":913
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  *     cdef Py_ssize_t itemsize = view.itemsize             # <<<<<<<<<<<<<<
  *     cdef char *resultp
  * 
  */
   __pyx_t_1 = __pyx_v_view->itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":918
+  /* "View.MemoryView":916
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
   __pyx_t_2 = ((__pyx_v_view->ndim == 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":919
+    /* "View.MemoryView":917
  * 
  *     if view.ndim == 0:
  *         shape = view.len / itemsize             # <<<<<<<<<<<<<<
  *         stride = itemsize
  *     else:
  */
     if (unlikely(__pyx_v_itemsize == 0)) {
       PyErr_SetString(PyExc_ZeroDivisionError, "integer division or modulo by zero");
-      __PYX_ERR(2, 919, __pyx_L1_error)
+      __PYX_ERR(2, 917, __pyx_L1_error)
     }
     else if (sizeof(Py_ssize_t) == sizeof(long) && (!(((Py_ssize_t)-1) > 0)) && unlikely(__pyx_v_itemsize == (Py_ssize_t)-1)  && unlikely(UNARY_NEG_WOULD_OVERFLOW(__pyx_v_view->len))) {
       PyErr_SetString(PyExc_OverflowError, "value too large to perform division");
-      __PYX_ERR(2, 919, __pyx_L1_error)
+      __PYX_ERR(2, 917, __pyx_L1_error)
     }
     __pyx_v_shape = __Pyx_div_Py_ssize_t(__pyx_v_view->len, __pyx_v_itemsize);
 
-    /* "View.MemoryView":920
+    /* "View.MemoryView":918
  *     if view.ndim == 0:
  *         shape = view.len / itemsize
  *         stride = itemsize             # <<<<<<<<<<<<<<
  *     else:
  *         shape = view.shape[dim]
  */
     __pyx_v_stride = __pyx_v_itemsize;
 
-    /* "View.MemoryView":918
+    /* "View.MemoryView":916
  *     cdef char *resultp
  * 
  *     if view.ndim == 0:             # <<<<<<<<<<<<<<
  *         shape = view.len / itemsize
  *         stride = itemsize
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":922
+  /* "View.MemoryView":920
  *         stride = itemsize
  *     else:
  *         shape = view.shape[dim]             # <<<<<<<<<<<<<<
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  */
   /*else*/ {
     __pyx_v_shape = (__pyx_v_view->shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":923
+    /* "View.MemoryView":921
  *     else:
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]             # <<<<<<<<<<<<<<
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]
  */
     __pyx_v_stride = (__pyx_v_view->strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":924
+    /* "View.MemoryView":922
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     __pyx_t_2 = ((__pyx_v_view->suboffsets != NULL) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":925
+      /* "View.MemoryView":923
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:
  *             suboffset = view.suboffsets[dim]             # <<<<<<<<<<<<<<
  * 
  *     if index < 0:
  */
       __pyx_v_suboffset = (__pyx_v_view->suboffsets[__pyx_v_dim]);
 
-      /* "View.MemoryView":924
+      /* "View.MemoryView":922
  *         shape = view.shape[dim]
  *         stride = view.strides[dim]
  *         if view.suboffsets != NULL:             # <<<<<<<<<<<<<<
  *             suboffset = view.suboffsets[dim]
  * 
  */
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":927
+  /* "View.MemoryView":925
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   __pyx_t_2 = ((__pyx_v_index < 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":928
+    /* "View.MemoryView":926
  * 
  *     if index < 0:
  *         index += view.shape[dim]             # <<<<<<<<<<<<<<
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  */
     __pyx_v_index = (__pyx_v_index + (__pyx_v_view->shape[__pyx_v_dim]));
 
-    /* "View.MemoryView":929
+    /* "View.MemoryView":927
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     __pyx_t_2 = ((__pyx_v_index < 0) != 0);
     if (unlikely(__pyx_t_2)) {
 
-      /* "View.MemoryView":930
+      /* "View.MemoryView":928
  *         index += view.shape[dim]
  *         if index < 0:
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     if index >= shape:
  */
-      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 930, __pyx_L1_error)
+      __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 928, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 930, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 928, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 930, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 928, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_3, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-      __PYX_ERR(2, 930, __pyx_L1_error)
+      __PYX_ERR(2, 928, __pyx_L1_error)
 
-      /* "View.MemoryView":929
+      /* "View.MemoryView":927
  *     if index < 0:
  *         index += view.shape[dim]
  *         if index < 0:             # <<<<<<<<<<<<<<
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
     }
 
-    /* "View.MemoryView":927
+    /* "View.MemoryView":925
  *             suboffset = view.suboffsets[dim]
  * 
  *     if index < 0:             # <<<<<<<<<<<<<<
  *         index += view.shape[dim]
  *         if index < 0:
  */
   }
 
-  /* "View.MemoryView":932
+  /* "View.MemoryView":930
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_index >= __pyx_v_shape) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "View.MemoryView":933
+    /* "View.MemoryView":931
  * 
  *     if index >= shape:
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)             # <<<<<<<<<<<<<<
  * 
  *     resultp = bufp + index * stride
  */
-    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 933, __pyx_L1_error)
+    __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 931, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 933, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 931, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 933, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_IndexError, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 931, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(2, 933, __pyx_L1_error)
+    __PYX_ERR(2, 931, __pyx_L1_error)
 
-    /* "View.MemoryView":932
+    /* "View.MemoryView":930
  *             raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     if index >= shape:             # <<<<<<<<<<<<<<
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  */
   }
 
-  /* "View.MemoryView":935
+  /* "View.MemoryView":933
  *         raise IndexError("Out of bounds on buffer access (axis %d)" % dim)
  * 
  *     resultp = bufp + index * stride             # <<<<<<<<<<<<<<
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset
  */
   __pyx_v_resultp = (__pyx_v_bufp + (__pyx_v_index * __pyx_v_stride));
 
-  /* "View.MemoryView":936
+  /* "View.MemoryView":934
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   __pyx_t_2 = ((__pyx_v_suboffset >= 0) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":937
+    /* "View.MemoryView":935
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:
  *         resultp = (<char **> resultp)[0] + suboffset             # <<<<<<<<<<<<<<
  * 
  *     return resultp
  */
     __pyx_v_resultp = ((((char **)__pyx_v_resultp)[0]) + __pyx_v_suboffset);
 
-    /* "View.MemoryView":936
+    /* "View.MemoryView":934
  * 
  *     resultp = bufp + index * stride
  *     if suboffset >= 0:             # <<<<<<<<<<<<<<
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  */
   }
 
-  /* "View.MemoryView":939
+  /* "View.MemoryView":937
  *         resultp = (<char **> resultp)[0] + suboffset
  * 
  *     return resultp             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_resultp;
   goto __pyx_L0;
 
-  /* "View.MemoryView":912
+  /* "View.MemoryView":910
  * 
  * @cname('__pyx_pybuffer_index')
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,             # <<<<<<<<<<<<<<
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1
  */
 
@@ -13186,15 +13017,15 @@
   __Pyx_AddTraceback("View.MemoryView.pybuffer_index", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":945
+/* "View.MemoryView":943
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -13214,90 +13045,90 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":946
+  /* "View.MemoryView":944
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  */
   __pyx_t_1 = __pyx_v_memslice->memview->view.ndim;
   __pyx_v_ndim = __pyx_t_1;
 
-  /* "View.MemoryView":948
+  /* "View.MemoryView":946
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  *     cdef Py_ssize_t *shape = memslice.shape             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t *strides = memslice.strides
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->shape;
   __pyx_v_shape = __pyx_t_2;
 
-  /* "View.MemoryView":949
+  /* "View.MemoryView":947
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
  *     cdef Py_ssize_t *strides = memslice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = __pyx_v_memslice->strides;
   __pyx_v_strides = __pyx_t_2;
 
-  /* "View.MemoryView":953
+  /* "View.MemoryView":951
  * 
  *     cdef int i, j
  *     for i in range(ndim / 2):             # <<<<<<<<<<<<<<
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  */
   __pyx_t_3 = __Pyx_div_long(__pyx_v_ndim, 2);
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_1 = 0; __pyx_t_1 < __pyx_t_4; __pyx_t_1+=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":954
+    /* "View.MemoryView":952
  *     cdef int i, j
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i             # <<<<<<<<<<<<<<
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]
  */
     __pyx_v_j = ((__pyx_v_ndim - 1) - __pyx_v_i);
 
-    /* "View.MemoryView":955
+    /* "View.MemoryView":953
  *     for i in range(ndim / 2):
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]             # <<<<<<<<<<<<<<
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  */
     __pyx_t_5 = (__pyx_v_strides[__pyx_v_j]);
     __pyx_t_6 = (__pyx_v_strides[__pyx_v_i]);
     (__pyx_v_strides[__pyx_v_i]) = __pyx_t_5;
     (__pyx_v_strides[__pyx_v_j]) = __pyx_t_6;
 
-    /* "View.MemoryView":956
+    /* "View.MemoryView":954
  *         j = ndim - 1 - i
  *         strides[i], strides[j] = strides[j], strides[i]
  *         shape[i], shape[j] = shape[j], shape[i]             # <<<<<<<<<<<<<<
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  */
     __pyx_t_6 = (__pyx_v_shape[__pyx_v_j]);
     __pyx_t_5 = (__pyx_v_shape[__pyx_v_i]);
     (__pyx_v_shape[__pyx_v_i]) = __pyx_t_6;
     (__pyx_v_shape[__pyx_v_j]) = __pyx_t_5;
 
-    /* "View.MemoryView":958
+    /* "View.MemoryView":956
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_i]) >= 0) != 0);
@@ -13307,44 +13138,44 @@
       goto __pyx_L6_bool_binop_done;
     }
     __pyx_t_8 = (((__pyx_v_memslice->suboffsets[__pyx_v_j]) >= 0) != 0);
     __pyx_t_7 = __pyx_t_8;
     __pyx_L6_bool_binop_done:;
     if (__pyx_t_7) {
 
-      /* "View.MemoryView":959
+      /* "View.MemoryView":957
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")             # <<<<<<<<<<<<<<
  * 
  *     return 1
  */
-      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 959, __pyx_L1_error)
+      __pyx_t_9 = __pyx_memoryview_err(__pyx_builtin_ValueError, ((char *)"Cannot transpose memoryview with indirect dimensions")); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(2, 957, __pyx_L1_error)
 
-      /* "View.MemoryView":958
+      /* "View.MemoryView":956
  *         shape[i], shape[j] = shape[j], shape[i]
  * 
  *         if memslice.suboffsets[i] >= 0 or memslice.suboffsets[j] >= 0:             # <<<<<<<<<<<<<<
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  */
     }
   }
 
-  /* "View.MemoryView":961
+  /* "View.MemoryView":959
  *             _err(ValueError, "Cannot transpose memoryview with indirect dimensions")
  * 
  *     return 1             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = 1;
   goto __pyx_L0;
 
-  /* "View.MemoryView":945
+  /* "View.MemoryView":943
  * 
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:             # <<<<<<<<<<<<<<
  *     cdef int ndim = memslice.memview.view.ndim
  * 
  */
 
@@ -13360,15 +13191,15 @@
     #endif
   }
   __pyx_r = 0;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":978
+/* "View.MemoryView":976
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
@@ -13383,36 +13214,36 @@
   __Pyx_RefNannyFinishContext();
 }
 
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "View.MemoryView":979
+  /* "View.MemoryView":977
  * 
  *     def __dealloc__(self):
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)             # <<<<<<<<<<<<<<
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  */
   __PYX_XDEC_MEMVIEW((&__pyx_v_self->from_slice), 1);
 
-  /* "View.MemoryView":978
+  /* "View.MemoryView":976
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":981
+/* "View.MemoryView":979
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -13422,64 +13253,64 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
-  /* "View.MemoryView":982
+  /* "View.MemoryView":980
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_object_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":983
+    /* "View.MemoryView":981
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)             # <<<<<<<<<<<<<<
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 983, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_object_func(__pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 981, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "View.MemoryView":982
+    /* "View.MemoryView":980
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
  *         else:
  */
   }
 
-  /* "View.MemoryView":985
+  /* "View.MemoryView":983
  *             return self.to_object_func(itemp)
  *         else:
  *             return memoryview.convert_item_to_object(self, itemp)             # <<<<<<<<<<<<<<
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 985, __pyx_L1_error)
+    __pyx_t_2 = __pyx_memoryview_convert_item_to_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 983, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":981
+  /* "View.MemoryView":979
  *         __PYX_XDEC_MEMVIEW(&self.from_slice, 1)
  * 
  *     cdef convert_item_to_object(self, char *itemp):             # <<<<<<<<<<<<<<
  *         if self.to_object_func != NULL:
  *             return self.to_object_func(itemp)
  */
 
@@ -13490,15 +13321,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":987
+/* "View.MemoryView":985
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -13509,58 +13340,58 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
-  /* "View.MemoryView":988
+  /* "View.MemoryView":986
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->to_dtype_func != NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":989
+    /* "View.MemoryView":987
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)             # <<<<<<<<<<<<<<
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)
  */
-    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 989, __pyx_L1_error)
+    __pyx_t_2 = __pyx_v_self->to_dtype_func(__pyx_v_itemp, __pyx_v_value); if (unlikely(__pyx_t_2 == ((int)0))) __PYX_ERR(2, 987, __pyx_L1_error)
 
-    /* "View.MemoryView":988
+    /* "View.MemoryView":986
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":991
+  /* "View.MemoryView":989
  *             self.to_dtype_func(itemp, value)
  *         else:
  *             memoryview.assign_item_from_object(self, itemp, value)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
-    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 991, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_assign_item_from_object(((struct __pyx_memoryview_obj *)__pyx_v_self), __pyx_v_itemp, __pyx_v_value); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 989, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":987
+  /* "View.MemoryView":985
  *             return memoryview.convert_item_to_object(self, itemp)
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):             # <<<<<<<<<<<<<<
  *         if self.to_dtype_func != NULL:
  *             self.to_dtype_func(itemp, value)
  */
 
@@ -13573,15 +13404,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":994
+/* "View.MemoryView":992
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -13599,27 +13430,27 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_16_memoryviewslice_4base___get__(struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "View.MemoryView":995
+  /* "View.MemoryView":993
  *     @property
  *     def base(self):
  *         return self.from_object             # <<<<<<<<<<<<<<
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->from_object);
   __pyx_r = __pyx_v_self->from_object;
   goto __pyx_L0;
 
-  /* "View.MemoryView":994
+  /* "View.MemoryView":992
  * 
  *     @property
  *     def base(self):             # <<<<<<<<<<<<<<
  *         return self.from_object
  * 
  */
 
@@ -13739,15 +13570,15 @@
   __Pyx_AddTraceback("View.MemoryView._memoryviewslice.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1001
+/* "View.MemoryView":999
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -13767,351 +13598,351 @@
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
 
-  /* "View.MemoryView":1009
+  /* "View.MemoryView":1007
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   __pyx_t_1 = ((((PyObject *)__pyx_v_memviewslice.memview) == Py_None) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1010
+    /* "View.MemoryView":1008
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:
  *         return None             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1009
+    /* "View.MemoryView":1007
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
  * 
  */
   }
 
-  /* "View.MemoryView":1015
+  /* "View.MemoryView":1013
  * 
  * 
  *     result = _memoryviewslice(None, 0, dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  *     result.from_slice = memviewslice
  */
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1015, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_v_dtype_is_object); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1015, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(3); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   PyTuple_SET_ITEM(__pyx_t_3, 0, Py_None);
   __Pyx_INCREF(__pyx_int_0);
   __Pyx_GIVEREF(__pyx_int_0);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_int_0);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 2, __pyx_t_2);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1015, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_memoryviewslice_type), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1013, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_result = ((struct __pyx_memoryviewslice_obj *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1017
+  /* "View.MemoryView":1015
  *     result = _memoryviewslice(None, 0, dtype_is_object)
  * 
  *     result.from_slice = memviewslice             # <<<<<<<<<<<<<<
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  */
   __pyx_v_result->from_slice = __pyx_v_memviewslice;
 
-  /* "View.MemoryView":1018
+  /* "View.MemoryView":1016
  * 
  *     result.from_slice = memviewslice
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)             # <<<<<<<<<<<<<<
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  */
   __PYX_INC_MEMVIEW((&__pyx_v_memviewslice), 1);
 
-  /* "View.MemoryView":1020
+  /* "View.MemoryView":1018
  *     __PYX_INC_MEMVIEW(&memviewslice, 1)
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base             # <<<<<<<<<<<<<<
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1020, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_memviewslice.memview), __pyx_n_s_base); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1018, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_result->from_object);
   __Pyx_DECREF(__pyx_v_result->from_object);
   __pyx_v_result->from_object = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "View.MemoryView":1021
+  /* "View.MemoryView":1019
  * 
  *     result.from_object = (<memoryview> memviewslice.memview).base
  *     result.typeinfo = memviewslice.memview.typeinfo             # <<<<<<<<<<<<<<
  * 
  *     result.view = memviewslice.memview.view
  */
   __pyx_t_4 = __pyx_v_memviewslice.memview->typeinfo;
   __pyx_v_result->__pyx_base.typeinfo = __pyx_t_4;
 
-  /* "View.MemoryView":1023
+  /* "View.MemoryView":1021
  *     result.typeinfo = memviewslice.memview.typeinfo
  * 
  *     result.view = memviewslice.memview.view             # <<<<<<<<<<<<<<
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  */
   __pyx_t_5 = __pyx_v_memviewslice.memview->view;
   __pyx_v_result->__pyx_base.view = __pyx_t_5;
 
-  /* "View.MemoryView":1024
+  /* "View.MemoryView":1022
  * 
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data             # <<<<<<<<<<<<<<
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  */
   __pyx_v_result->__pyx_base.view.buf = ((void *)__pyx_v_memviewslice.data);
 
-  /* "View.MemoryView":1025
+  /* "View.MemoryView":1023
  *     result.view = memviewslice.memview.view
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim             # <<<<<<<<<<<<<<
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)
  */
   __pyx_v_result->__pyx_base.view.ndim = __pyx_v_ndim;
 
-  /* "View.MemoryView":1026
+  /* "View.MemoryView":1024
  *     result.view.buf = <void *> memviewslice.data
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None             # <<<<<<<<<<<<<<
  *     Py_INCREF(Py_None)
  * 
  */
   ((Py_buffer *)(&__pyx_v_result->__pyx_base.view))->obj = Py_None;
 
-  /* "View.MemoryView":1027
+  /* "View.MemoryView":1025
  *     result.view.ndim = ndim
  *     (<__pyx_buffer *> &result.view).obj = Py_None
  *     Py_INCREF(Py_None)             # <<<<<<<<<<<<<<
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  */
   Py_INCREF(Py_None);
 
-  /* "View.MemoryView":1029
+  /* "View.MemoryView":1027
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
   __pyx_t_1 = ((((struct __pyx_memoryview_obj *)__pyx_v_memviewslice.memview)->flags & PyBUF_WRITABLE) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1030
+    /* "View.MemoryView":1028
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:
  *         result.flags = PyBUF_RECORDS             # <<<<<<<<<<<<<<
  *     else:
  *         result.flags = PyBUF_RECORDS_RO
  */
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS;
 
-    /* "View.MemoryView":1029
+    /* "View.MemoryView":1027
  *     Py_INCREF(Py_None)
  * 
  *     if (<memoryview>memviewslice.memview).flags & PyBUF_WRITABLE:             # <<<<<<<<<<<<<<
  *         result.flags = PyBUF_RECORDS
  *     else:
  */
     goto __pyx_L4;
   }
 
-  /* "View.MemoryView":1032
+  /* "View.MemoryView":1030
  *         result.flags = PyBUF_RECORDS
  *     else:
  *         result.flags = PyBUF_RECORDS_RO             # <<<<<<<<<<<<<<
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  */
   /*else*/ {
     __pyx_v_result->__pyx_base.flags = PyBUF_RECORDS_RO;
   }
   __pyx_L4:;
 
-  /* "View.MemoryView":1034
+  /* "View.MemoryView":1032
  *         result.flags = PyBUF_RECORDS_RO
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape             # <<<<<<<<<<<<<<
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides
  * 
  */
   __pyx_v_result->__pyx_base.view.shape = ((Py_ssize_t *)__pyx_v_result->from_slice.shape);
 
-  /* "View.MemoryView":1035
+  /* "View.MemoryView":1033
  * 
  *     result.view.shape = <Py_ssize_t *> result.from_slice.shape
  *     result.view.strides = <Py_ssize_t *> result.from_slice.strides             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_v_result->__pyx_base.view.strides = ((Py_ssize_t *)__pyx_v_result->from_slice.strides);
 
-  /* "View.MemoryView":1038
+  /* "View.MemoryView":1036
  * 
  * 
  *     result.view.suboffsets = NULL             # <<<<<<<<<<<<<<
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  */
   __pyx_v_result->__pyx_base.view.suboffsets = NULL;
 
-  /* "View.MemoryView":1039
+  /* "View.MemoryView":1037
  * 
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  */
   __pyx_t_7 = (__pyx_v_result->from_slice.suboffsets + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->from_slice.suboffsets; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
     __pyx_v_suboffset = (__pyx_t_6[0]);
 
-    /* "View.MemoryView":1040
+    /* "View.MemoryView":1038
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     __pyx_t_1 = ((__pyx_v_suboffset >= 0) != 0);
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1041
+      /* "View.MemoryView":1039
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_result->__pyx_base.view.suboffsets = ((Py_ssize_t *)__pyx_v_result->from_slice.suboffsets);
 
-      /* "View.MemoryView":1042
+      /* "View.MemoryView":1040
  *         if suboffset >= 0:
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break             # <<<<<<<<<<<<<<
  * 
  *     result.view.len = result.view.itemsize
  */
       goto __pyx_L6_break;
 
-      /* "View.MemoryView":1040
+      /* "View.MemoryView":1038
  *     result.view.suboffsets = NULL
  *     for suboffset in result.from_slice.suboffsets[:ndim]:
  *         if suboffset >= 0:             # <<<<<<<<<<<<<<
  *             result.view.suboffsets = <Py_ssize_t *> result.from_slice.suboffsets
  *             break
  */
     }
   }
   __pyx_L6_break:;
 
-  /* "View.MemoryView":1044
+  /* "View.MemoryView":1042
  *             break
  * 
  *     result.view.len = result.view.itemsize             # <<<<<<<<<<<<<<
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length
  */
   __pyx_t_9 = __pyx_v_result->__pyx_base.view.itemsize;
   __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
 
-  /* "View.MemoryView":1045
+  /* "View.MemoryView":1043
  * 
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         result.view.len *= length
  * 
  */
   __pyx_t_7 = (__pyx_v_result->__pyx_base.view.shape + __pyx_v_ndim);
   for (__pyx_t_8 = __pyx_v_result->__pyx_base.view.shape; __pyx_t_8 < __pyx_t_7; __pyx_t_8++) {
     __pyx_t_6 = __pyx_t_8;
-    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1045, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_6[0])); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1043, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_XDECREF_SET(__pyx_v_length, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "View.MemoryView":1046
+    /* "View.MemoryView":1044
  *     result.view.len = result.view.itemsize
  *     for length in result.view.shape[:ndim]:
  *         result.view.len *= length             # <<<<<<<<<<<<<<
  * 
  *     result.to_object_func = to_object_func
  */
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1046, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_result->__pyx_base.view.len); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1044, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1046, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_InPlaceMultiply(__pyx_t_2, __pyx_v_length); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1044, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 1046, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyIndex_AsSsize_t(__pyx_t_3); if (unlikely((__pyx_t_9 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(2, 1044, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_result->__pyx_base.view.len = __pyx_t_9;
   }
 
-  /* "View.MemoryView":1048
+  /* "View.MemoryView":1046
  *         result.view.len *= length
  * 
  *     result.to_object_func = to_object_func             # <<<<<<<<<<<<<<
  *     result.to_dtype_func = to_dtype_func
  * 
  */
   __pyx_v_result->to_object_func = __pyx_v_to_object_func;
 
-  /* "View.MemoryView":1049
+  /* "View.MemoryView":1047
  * 
  *     result.to_object_func = to_object_func
  *     result.to_dtype_func = to_dtype_func             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result->to_dtype_func = __pyx_v_to_dtype_func;
 
-  /* "View.MemoryView":1051
+  /* "View.MemoryView":1049
  *     result.to_dtype_func = to_dtype_func
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_result));
   __pyx_r = ((PyObject *)__pyx_v_result);
   goto __pyx_L0;
 
-  /* "View.MemoryView":1001
+  /* "View.MemoryView":999
  * 
  * @cname('__pyx_memoryview_fromslice')
  * cdef memoryview_fromslice(__Pyx_memviewslice memviewslice,             # <<<<<<<<<<<<<<
  *                           int ndim,
  *                           object (*to_object_func)(char *),
  */
 
@@ -14125,15 +13956,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_length);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1054
+/* "View.MemoryView":1052
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
 
@@ -14145,79 +13976,79 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
 
-  /* "View.MemoryView":1057
+  /* "View.MemoryView":1055
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1058
+    /* "View.MemoryView":1056
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview             # <<<<<<<<<<<<<<
  *         return &obj.from_slice
  *     else:
  */
-    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 1058, __pyx_L1_error)
+    if (!(likely(((((PyObject *)__pyx_v_memview)) == Py_None) || likely(__Pyx_TypeTest(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type))))) __PYX_ERR(2, 1056, __pyx_L1_error)
     __pyx_t_3 = ((PyObject *)__pyx_v_memview);
     __Pyx_INCREF(__pyx_t_3);
     __pyx_v_obj = ((struct __pyx_memoryviewslice_obj *)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "View.MemoryView":1059
+    /* "View.MemoryView":1057
  *     if isinstance(memview, _memoryviewslice):
  *         obj = memview
  *         return &obj.from_slice             # <<<<<<<<<<<<<<
  *     else:
  *         slice_copy(memview, mslice)
  */
     __pyx_r = (&__pyx_v_obj->from_slice);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1057
+    /* "View.MemoryView":1055
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
  *         return &obj.from_slice
  */
   }
 
-  /* "View.MemoryView":1061
+  /* "View.MemoryView":1059
  *         return &obj.from_slice
  *     else:
  *         slice_copy(memview, mslice)             # <<<<<<<<<<<<<<
  *         return mslice
  * 
  */
   /*else*/ {
     __pyx_memoryview_slice_copy(__pyx_v_memview, __pyx_v_mslice);
 
-    /* "View.MemoryView":1062
+    /* "View.MemoryView":1060
  *     else:
  *         slice_copy(memview, mslice)
  *         return mslice             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_slice_copy')
  */
     __pyx_r = __pyx_v_mslice;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1054
+  /* "View.MemoryView":1052
  * 
  * @cname('__pyx_memoryview_get_slice_from_memoryview')
  * cdef __Pyx_memviewslice *get_slice_from_memview(memoryview memview,             # <<<<<<<<<<<<<<
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  */
 
@@ -14228,15 +14059,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_obj);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1065
+/* "View.MemoryView":1063
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
@@ -14249,120 +14080,120 @@
   Py_ssize_t *__pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   __Pyx_RefNannySetupContext("slice_copy", 0);
 
-  /* "View.MemoryView":1069
+  /* "View.MemoryView":1067
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  * 
  *     shape = memview.view.shape             # <<<<<<<<<<<<<<
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets
  */
   __pyx_t_1 = __pyx_v_memview->view.shape;
   __pyx_v_shape = __pyx_t_1;
 
-  /* "View.MemoryView":1070
+  /* "View.MemoryView":1068
  * 
  *     shape = memview.view.shape
  *     strides = memview.view.strides             # <<<<<<<<<<<<<<
  *     suboffsets = memview.view.suboffsets
  * 
  */
   __pyx_t_1 = __pyx_v_memview->view.strides;
   __pyx_v_strides = __pyx_t_1;
 
-  /* "View.MemoryView":1071
+  /* "View.MemoryView":1069
  *     shape = memview.view.shape
  *     strides = memview.view.strides
  *     suboffsets = memview.view.suboffsets             # <<<<<<<<<<<<<<
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  */
   __pyx_t_1 = __pyx_v_memview->view.suboffsets;
   __pyx_v_suboffsets = __pyx_t_1;
 
-  /* "View.MemoryView":1073
+  /* "View.MemoryView":1071
  *     suboffsets = memview.view.suboffsets
  * 
  *     dst.memview = <__pyx_memoryview *> memview             # <<<<<<<<<<<<<<
  *     dst.data = <char *> memview.view.buf
  * 
  */
   __pyx_v_dst->memview = ((struct __pyx_memoryview_obj *)__pyx_v_memview);
 
-  /* "View.MemoryView":1074
+  /* "View.MemoryView":1072
  * 
  *     dst.memview = <__pyx_memoryview *> memview
  *     dst.data = <char *> memview.view.buf             # <<<<<<<<<<<<<<
  * 
  *     for dim in range(memview.view.ndim):
  */
   __pyx_v_dst->data = ((char *)__pyx_v_memview->view.buf);
 
-  /* "View.MemoryView":1076
+  /* "View.MemoryView":1074
  *     dst.data = <char *> memview.view.buf
  * 
  *     for dim in range(memview.view.ndim):             # <<<<<<<<<<<<<<
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  */
   __pyx_t_2 = __pyx_v_memview->view.ndim;
   __pyx_t_3 = __pyx_t_2;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_dim = __pyx_t_4;
 
-    /* "View.MemoryView":1077
+    /* "View.MemoryView":1075
  * 
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]             # <<<<<<<<<<<<<<
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  */
     (__pyx_v_dst->shape[__pyx_v_dim]) = (__pyx_v_shape[__pyx_v_dim]);
 
-    /* "View.MemoryView":1078
+    /* "View.MemoryView":1076
  *     for dim in range(memview.view.ndim):
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]             # <<<<<<<<<<<<<<
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1
  * 
  */
     (__pyx_v_dst->strides[__pyx_v_dim]) = (__pyx_v_strides[__pyx_v_dim]);
 
-    /* "View.MemoryView":1079
+    /* "View.MemoryView":1077
  *         dst.shape[dim] = shape[dim]
  *         dst.strides[dim] = strides[dim]
  *         dst.suboffsets[dim] = suboffsets[dim] if suboffsets else -1             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object')
  */
     if ((__pyx_v_suboffsets != 0)) {
       __pyx_t_5 = (__pyx_v_suboffsets[__pyx_v_dim]);
     } else {
       __pyx_t_5 = -1L;
     }
     (__pyx_v_dst->suboffsets[__pyx_v_dim]) = __pyx_t_5;
   }
 
-  /* "View.MemoryView":1065
+  /* "View.MemoryView":1063
  * 
  * @cname('__pyx_memoryview_slice_copy')
  * cdef void slice_copy(memoryview memview, __Pyx_memviewslice *dst):             # <<<<<<<<<<<<<<
  *     cdef int dim
  *     cdef (Py_ssize_t*) shape, strides, suboffsets
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1082
+/* "View.MemoryView":1080
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -14372,38 +14203,38 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy", 0);
 
-  /* "View.MemoryView":1085
+  /* "View.MemoryView":1083
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
  * 
  */
   __pyx_memoryview_slice_copy(__pyx_v_memview, (&__pyx_v_memviewslice));
 
-  /* "View.MemoryView":1086
+  /* "View.MemoryView":1084
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)
  *     return memoryview_copy_from_slice(memview, &memviewslice)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1086, __pyx_L1_error)
+  __pyx_t_1 = __pyx_memoryview_copy_object_from_slice(__pyx_v_memview, (&__pyx_v_memviewslice)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1084, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1082
+  /* "View.MemoryView":1080
  * 
  * @cname('__pyx_memoryview_copy_object')
  * cdef memoryview_copy(memoryview memview):             # <<<<<<<<<<<<<<
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  */
 
@@ -14414,15 +14245,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1089
+/* "View.MemoryView":1087
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -14437,99 +14268,99 @@
   int (*__pyx_t_4)(char *, PyObject *);
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
 
-  /* "View.MemoryView":1096
+  /* "View.MemoryView":1094
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
   __pyx_t_1 = __Pyx_TypeCheck(((PyObject *)__pyx_v_memview), __pyx_memoryviewslice_type); 
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1097
+    /* "View.MemoryView":1095
  * 
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func             # <<<<<<<<<<<<<<
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  */
     __pyx_t_3 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_object_func;
     __pyx_v_to_object_func = __pyx_t_3;
 
-    /* "View.MemoryView":1098
+    /* "View.MemoryView":1096
  *     if isinstance(memview, _memoryviewslice):
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func             # <<<<<<<<<<<<<<
  *     else:
  *         to_object_func = NULL
  */
     __pyx_t_4 = ((struct __pyx_memoryviewslice_obj *)__pyx_v_memview)->to_dtype_func;
     __pyx_v_to_dtype_func = __pyx_t_4;
 
-    /* "View.MemoryView":1096
+    /* "View.MemoryView":1094
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1100
+  /* "View.MemoryView":1098
  *         to_dtype_func = (<_memoryviewslice> memview).to_dtype_func
  *     else:
  *         to_object_func = NULL             # <<<<<<<<<<<<<<
  *         to_dtype_func = NULL
  * 
  */
   /*else*/ {
     __pyx_v_to_object_func = NULL;
 
-    /* "View.MemoryView":1101
+    /* "View.MemoryView":1099
  *     else:
  *         to_object_func = NULL
  *         to_dtype_func = NULL             # <<<<<<<<<<<<<<
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  */
     __pyx_v_to_dtype_func = NULL;
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1103
+  /* "View.MemoryView":1101
  *         to_dtype_func = NULL
  * 
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,             # <<<<<<<<<<<<<<
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)
  */
   __Pyx_XDECREF(__pyx_r);
 
-  /* "View.MemoryView":1105
+  /* "View.MemoryView":1103
  *     return memoryview_fromslice(memviewslice[0], memview.view.ndim,
  *                                 to_object_func, to_dtype_func,
  *                                 memview.dtype_is_object)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1103, __pyx_L1_error)
+  __pyx_t_5 = __pyx_memoryview_fromslice((__pyx_v_memviewslice[0]), __pyx_v_memview->view.ndim, __pyx_v_to_object_func, __pyx_v_to_dtype_func, __pyx_v_memview->dtype_is_object); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 1101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1089
+  /* "View.MemoryView":1087
  * 
  * @cname('__pyx_memoryview_copy_object_from_slice')
  * cdef memoryview_copy_from_slice(memoryview memview, __Pyx_memviewslice *memviewslice):             # <<<<<<<<<<<<<<
  *     """
  *     Create a new memoryview object from a given memoryview object and slice.
  */
 
@@ -14540,81 +14371,81 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "View.MemoryView":1111
+/* "View.MemoryView":1109
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
 static Py_ssize_t abs_py_ssize_t(Py_ssize_t __pyx_v_arg) {
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
 
-  /* "View.MemoryView":1112
+  /* "View.MemoryView":1110
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_arg < 0) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1113
+    /* "View.MemoryView":1111
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:
  *         return -arg             # <<<<<<<<<<<<<<
  *     else:
  *         return arg
  */
     __pyx_r = (-__pyx_v_arg);
     goto __pyx_L0;
 
-    /* "View.MemoryView":1112
+    /* "View.MemoryView":1110
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:
  *     if arg < 0:             # <<<<<<<<<<<<<<
  *         return -arg
  *     else:
  */
   }
 
-  /* "View.MemoryView":1115
+  /* "View.MemoryView":1113
  *         return -arg
  *     else:
  *         return arg             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_get_best_slice_order')
  */
   /*else*/ {
     __pyx_r = __pyx_v_arg;
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1111
+  /* "View.MemoryView":1109
  * 
  * 
  * cdef Py_ssize_t abs_py_ssize_t(Py_ssize_t arg) nogil:             # <<<<<<<<<<<<<<
  *     if arg < 0:
  *         return -arg
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1118
+/* "View.MemoryView":1116
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
@@ -14624,187 +14455,187 @@
   Py_ssize_t __pyx_v_f_stride;
   char __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1123
+  /* "View.MemoryView":1121
  *     """
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t f_stride = 0
  * 
  */
   __pyx_v_c_stride = 0;
 
-  /* "View.MemoryView":1124
+  /* "View.MemoryView":1122
  *     cdef int i
  *     cdef Py_ssize_t c_stride = 0
  *     cdef Py_ssize_t f_stride = 0             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_f_stride = 0;
 
-  /* "View.MemoryView":1126
+  /* "View.MemoryView":1124
  *     cdef Py_ssize_t f_stride = 0
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1127
+    /* "View.MemoryView":1125
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1128
+      /* "View.MemoryView":1126
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_c_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1129
+      /* "View.MemoryView":1127
  *         if mslice.shape[i] > 1:
  *             c_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
       goto __pyx_L4_break;
 
-      /* "View.MemoryView":1127
+      /* "View.MemoryView":1125
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             c_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L4_break:;
 
-  /* "View.MemoryView":1131
+  /* "View.MemoryView":1129
  *             break
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  */
   __pyx_t_1 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_1;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1132
+    /* "View.MemoryView":1130
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     __pyx_t_2 = (((__pyx_v_mslice->shape[__pyx_v_i]) > 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1133
+      /* "View.MemoryView":1131
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]             # <<<<<<<<<<<<<<
  *             break
  * 
  */
       __pyx_v_f_stride = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-      /* "View.MemoryView":1134
+      /* "View.MemoryView":1132
  *         if mslice.shape[i] > 1:
  *             f_stride = mslice.strides[i]
  *             break             # <<<<<<<<<<<<<<
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  */
       goto __pyx_L7_break;
 
-      /* "View.MemoryView":1132
+      /* "View.MemoryView":1130
  * 
  *     for i in range(ndim):
  *         if mslice.shape[i] > 1:             # <<<<<<<<<<<<<<
  *             f_stride = mslice.strides[i]
  *             break
  */
     }
   }
   __pyx_L7_break:;
 
-  /* "View.MemoryView":1136
+  /* "View.MemoryView":1134
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   __pyx_t_2 = ((abs_py_ssize_t(__pyx_v_c_stride) <= abs_py_ssize_t(__pyx_v_f_stride)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1137
+    /* "View.MemoryView":1135
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):
  *         return 'C'             # <<<<<<<<<<<<<<
  *     else:
  *         return 'F'
  */
     __pyx_r = 'C';
     goto __pyx_L0;
 
-    /* "View.MemoryView":1136
+    /* "View.MemoryView":1134
  *             break
  * 
  *     if abs_py_ssize_t(c_stride) <= abs_py_ssize_t(f_stride):             # <<<<<<<<<<<<<<
  *         return 'C'
  *     else:
  */
   }
 
-  /* "View.MemoryView":1139
+  /* "View.MemoryView":1137
  *         return 'C'
  *     else:
  *         return 'F'             # <<<<<<<<<<<<<<
  * 
  * @cython.cdivision(True)
  */
   /*else*/ {
     __pyx_r = 'F';
     goto __pyx_L0;
   }
 
-  /* "View.MemoryView":1118
+  /* "View.MemoryView":1116
  * 
  * @cname('__pyx_get_best_slice_order')
  * cdef char get_best_order(__Pyx_memviewslice *mslice, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     Figure out the best memory access order for a given slice.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1142
+/* "View.MemoryView":1140
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
@@ -14817,61 +14648,61 @@
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
 
-  /* "View.MemoryView":1149
+  /* "View.MemoryView":1147
  * 
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  */
   __pyx_v_src_extent = (__pyx_v_src_shape[0]);
 
-  /* "View.MemoryView":1150
+  /* "View.MemoryView":1148
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  */
   __pyx_v_dst_extent = (__pyx_v_dst_shape[0]);
 
-  /* "View.MemoryView":1151
+  /* "View.MemoryView":1149
  *     cdef Py_ssize_t src_extent = src_shape[0]
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  */
   __pyx_v_src_stride = (__pyx_v_src_strides[0]);
 
-  /* "View.MemoryView":1152
+  /* "View.MemoryView":1150
  *     cdef Py_ssize_t dst_extent = dst_shape[0]
  *     cdef Py_ssize_t src_stride = src_strides[0]
  *     cdef Py_ssize_t dst_stride = dst_strides[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_dst_stride = (__pyx_v_dst_strides[0]);
 
-  /* "View.MemoryView":1154
+  /* "View.MemoryView":1152
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1155
+    /* "View.MemoryView":1153
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     __pyx_t_2 = ((__pyx_v_src_stride > 0) != 0);
@@ -14883,195 +14714,195 @@
     __pyx_t_2 = ((__pyx_v_dst_stride > 0) != 0);
     if (__pyx_t_2) {
     } else {
       __pyx_t_1 = __pyx_t_2;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "View.MemoryView":1156
+    /* "View.MemoryView":1154
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):             # <<<<<<<<<<<<<<
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  */
     __pyx_t_2 = (((size_t)__pyx_v_src_stride) == __pyx_v_itemsize);
     if (__pyx_t_2) {
       __pyx_t_2 = (__pyx_v_itemsize == ((size_t)__pyx_v_dst_stride));
     }
     __pyx_t_3 = (__pyx_t_2 != 0);
     __pyx_t_1 = __pyx_t_3;
     __pyx_L5_bool_binop_done:;
 
-    /* "View.MemoryView":1155
+    /* "View.MemoryView":1153
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
     if (__pyx_t_1) {
 
-      /* "View.MemoryView":1157
+      /* "View.MemoryView":1155
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)             # <<<<<<<<<<<<<<
  *        else:
  *            for i in range(dst_extent):
  */
       (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, (__pyx_v_itemsize * __pyx_v_dst_extent)));
 
-      /* "View.MemoryView":1155
+      /* "View.MemoryView":1153
  * 
  *     if ndim == 1:
  *        if (src_stride > 0 and dst_stride > 0 and             # <<<<<<<<<<<<<<
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  */
       goto __pyx_L4;
     }
 
-    /* "View.MemoryView":1159
+    /* "View.MemoryView":1157
  *            memcpy(dst_data, src_data, itemsize * dst_extent)
  *        else:
  *            for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  */
     /*else*/ {
       __pyx_t_4 = __pyx_v_dst_extent;
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_v_i = __pyx_t_6;
 
-        /* "View.MemoryView":1160
+        /* "View.MemoryView":1158
  *        else:
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)             # <<<<<<<<<<<<<<
  *                src_data += src_stride
  *                dst_data += dst_stride
  */
         (void)(memcpy(__pyx_v_dst_data, __pyx_v_src_data, __pyx_v_itemsize));
 
-        /* "View.MemoryView":1161
+        /* "View.MemoryView":1159
  *            for i in range(dst_extent):
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride             # <<<<<<<<<<<<<<
  *                dst_data += dst_stride
  *     else:
  */
         __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-        /* "View.MemoryView":1162
+        /* "View.MemoryView":1160
  *                memcpy(dst_data, src_data, itemsize)
  *                src_data += src_stride
  *                dst_data += dst_stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(dst_extent):
  */
         __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
       }
     }
     __pyx_L4:;
 
-    /* "View.MemoryView":1154
+    /* "View.MemoryView":1152
  *     cdef Py_ssize_t dst_stride = dst_strides[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *        if (src_stride > 0 and dst_stride > 0 and
  *            <size_t> src_stride == itemsize == <size_t> dst_stride):
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1164
+  /* "View.MemoryView":1162
  *                dst_data += dst_stride
  *     else:
  *         for i in range(dst_extent):             # <<<<<<<<<<<<<<
  *             _copy_strided_to_strided(src_data, src_strides + 1,
  *                                      dst_data, dst_strides + 1,
  */
   /*else*/ {
     __pyx_t_4 = __pyx_v_dst_extent;
     __pyx_t_5 = __pyx_t_4;
     for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
       __pyx_v_i = __pyx_t_6;
 
-      /* "View.MemoryView":1165
+      /* "View.MemoryView":1163
  *     else:
  *         for i in range(dst_extent):
  *             _copy_strided_to_strided(src_data, src_strides + 1,             # <<<<<<<<<<<<<<
  *                                      dst_data, dst_strides + 1,
  *                                      src_shape + 1, dst_shape + 1,
  */
       _copy_strided_to_strided(__pyx_v_src_data, (__pyx_v_src_strides + 1), __pyx_v_dst_data, (__pyx_v_dst_strides + 1), (__pyx_v_src_shape + 1), (__pyx_v_dst_shape + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize);
 
-      /* "View.MemoryView":1169
+      /* "View.MemoryView":1167
  *                                      src_shape + 1, dst_shape + 1,
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride             # <<<<<<<<<<<<<<
  *             dst_data += dst_stride
  * 
  */
       __pyx_v_src_data = (__pyx_v_src_data + __pyx_v_src_stride);
 
-      /* "View.MemoryView":1170
+      /* "View.MemoryView":1168
  *                                      ndim - 1, itemsize)
  *             src_data += src_stride
  *             dst_data += dst_stride             # <<<<<<<<<<<<<<
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,
  */
       __pyx_v_dst_data = (__pyx_v_dst_data + __pyx_v_dst_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1142
+  /* "View.MemoryView":1140
  * 
  * @cython.cdivision(True)
  * cdef void _copy_strided_to_strided(char *src_data, Py_ssize_t *src_strides,             # <<<<<<<<<<<<<<
  *                                    char *dst_data, Py_ssize_t *dst_strides,
  *                                    Py_ssize_t *src_shape, Py_ssize_t *dst_shape,
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1172
+/* "View.MemoryView":1170
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
 static void copy_strided_to_strided(__Pyx_memviewslice *__pyx_v_src, __Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize) {
 
-  /* "View.MemoryView":1175
+  /* "View.MemoryView":1173
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  *     _copy_strided_to_strided(src.data, src.strides, dst.data, dst.strides,             # <<<<<<<<<<<<<<
  *                              src.shape, dst.shape, ndim, itemsize)
  * 
  */
   _copy_strided_to_strided(__pyx_v_src->data, __pyx_v_src->strides, __pyx_v_dst->data, __pyx_v_dst->strides, __pyx_v_src->shape, __pyx_v_dst->shape, __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1172
+  /* "View.MemoryView":1170
  *             dst_data += dst_stride
  * 
  * cdef void copy_strided_to_strided(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice *dst,
  *                                   int ndim, size_t itemsize) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1179
+/* "View.MemoryView":1177
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
 
@@ -15080,70 +14911,70 @@
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
 
-  /* "View.MemoryView":1181
+  /* "View.MemoryView":1179
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  * 
  *     for shape in src.shape[:ndim]:
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_size = __pyx_t_1;
 
-  /* "View.MemoryView":1183
+  /* "View.MemoryView":1181
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  * 
  *     for shape in src.shape[:ndim]:             # <<<<<<<<<<<<<<
  *         size *= shape
  * 
  */
   __pyx_t_3 = (__pyx_v_src->shape + __pyx_v_ndim);
   for (__pyx_t_4 = __pyx_v_src->shape; __pyx_t_4 < __pyx_t_3; __pyx_t_4++) {
     __pyx_t_2 = __pyx_t_4;
     __pyx_v_shape = (__pyx_t_2[0]);
 
-    /* "View.MemoryView":1184
+    /* "View.MemoryView":1182
  * 
  *     for shape in src.shape[:ndim]:
  *         size *= shape             # <<<<<<<<<<<<<<
  * 
  *     return size
  */
     __pyx_v_size = (__pyx_v_size * __pyx_v_shape);
   }
 
-  /* "View.MemoryView":1186
+  /* "View.MemoryView":1184
  *         size *= shape
  * 
  *     return size             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_fill_contig_strides_array')
  */
   __pyx_r = __pyx_v_size;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1179
+  /* "View.MemoryView":1177
  * 
  * @cname('__pyx_memoryview_slice_get_size')
  * cdef Py_ssize_t slice_get_size(__Pyx_memviewslice *src, int ndim) nogil:             # <<<<<<<<<<<<<<
  *     "Return the size of the memory occupied by the slice in number of bytes"
  *     cdef Py_ssize_t shape, size = src.memview.view.itemsize
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1189
+/* "View.MemoryView":1187
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
@@ -15151,121 +14982,121 @@
   int __pyx_v_idx;
   Py_ssize_t __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
 
-  /* "View.MemoryView":1198
+  /* "View.MemoryView":1196
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
   __pyx_t_1 = ((__pyx_v_order == 'F') != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1199
+    /* "View.MemoryView":1197
  * 
  *     if order == 'F':
  *         for idx in range(ndim):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride *= shape[idx]
  */
     __pyx_t_2 = __pyx_v_ndim;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_idx = __pyx_t_4;
 
-      /* "View.MemoryView":1200
+      /* "View.MemoryView":1198
  *     if order == 'F':
  *         for idx in range(ndim):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride *= shape[idx]
  *     else:
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1201
+      /* "View.MemoryView":1199
  *         for idx in range(ndim):
  *             strides[idx] = stride
  *             stride *= shape[idx]             # <<<<<<<<<<<<<<
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
 
-    /* "View.MemoryView":1198
+    /* "View.MemoryView":1196
  *     cdef int idx
  * 
  *     if order == 'F':             # <<<<<<<<<<<<<<
  *         for idx in range(ndim):
  *             strides[idx] = stride
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1203
+  /* "View.MemoryView":1201
  *             stride *= shape[idx]
  *     else:
  *         for idx in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *             strides[idx] = stride
  *             stride *= shape[idx]
  */
   /*else*/ {
     for (__pyx_t_2 = (__pyx_v_ndim - 1); __pyx_t_2 > -1; __pyx_t_2-=1) {
       __pyx_v_idx = __pyx_t_2;
 
-      /* "View.MemoryView":1204
+      /* "View.MemoryView":1202
  *     else:
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride             # <<<<<<<<<<<<<<
  *             stride *= shape[idx]
  * 
  */
       (__pyx_v_strides[__pyx_v_idx]) = __pyx_v_stride;
 
-      /* "View.MemoryView":1205
+      /* "View.MemoryView":1203
  *         for idx in range(ndim - 1, -1, -1):
  *             strides[idx] = stride
  *             stride *= shape[idx]             # <<<<<<<<<<<<<<
  * 
  *     return stride
  */
       __pyx_v_stride = (__pyx_v_stride * (__pyx_v_shape[__pyx_v_idx]));
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1207
+  /* "View.MemoryView":1205
  *             stride *= shape[idx]
  * 
  *     return stride             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  */
   __pyx_r = __pyx_v_stride;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1189
+  /* "View.MemoryView":1187
  * 
  * @cname('__pyx_fill_contig_strides_array')
  * cdef Py_ssize_t fill_contig_strides_array(             # <<<<<<<<<<<<<<
  *                 Py_ssize_t *shape, Py_ssize_t *strides, Py_ssize_t stride,
  *                 int ndim, char order) nogil:
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1210
+/* "View.MemoryView":1208
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -15281,222 +15112,222 @@
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":1221
+  /* "View.MemoryView":1219
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  */
   __pyx_t_1 = __pyx_v_src->memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1222
+  /* "View.MemoryView":1220
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef size_t size = slice_get_size(src, ndim)             # <<<<<<<<<<<<<<
  * 
  *     result = malloc(size)
  */
   __pyx_v_size = __pyx_memoryview_slice_get_size(__pyx_v_src, __pyx_v_ndim);
 
-  /* "View.MemoryView":1224
+  /* "View.MemoryView":1222
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
  *     result = malloc(size)             # <<<<<<<<<<<<<<
  *     if not result:
  *         _err(MemoryError, NULL)
  */
   __pyx_v_result = malloc(__pyx_v_size);
 
-  /* "View.MemoryView":1225
+  /* "View.MemoryView":1223
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_result != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1226
+    /* "View.MemoryView":1224
  *     result = malloc(size)
  *     if not result:
  *         _err(MemoryError, NULL)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 1226, __pyx_L1_error)
+    __pyx_t_3 = __pyx_memoryview_err(__pyx_builtin_MemoryError, NULL); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(2, 1224, __pyx_L1_error)
 
-    /* "View.MemoryView":1225
+    /* "View.MemoryView":1223
  * 
  *     result = malloc(size)
  *     if not result:             # <<<<<<<<<<<<<<
  *         _err(MemoryError, NULL)
  * 
  */
   }
 
-  /* "View.MemoryView":1229
+  /* "View.MemoryView":1227
  * 
  * 
  *     tmpslice.data = <char *> result             # <<<<<<<<<<<<<<
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  */
   __pyx_v_tmpslice->data = ((char *)__pyx_v_result);
 
-  /* "View.MemoryView":1230
+  /* "View.MemoryView":1228
  * 
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview             # <<<<<<<<<<<<<<
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  */
   __pyx_t_4 = __pyx_v_src->memview;
   __pyx_v_tmpslice->memview = __pyx_t_4;
 
-  /* "View.MemoryView":1231
+  /* "View.MemoryView":1229
  *     tmpslice.data = <char *> result
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1232
+    /* "View.MemoryView":1230
  *     tmpslice.memview = src.memview
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]             # <<<<<<<<<<<<<<
  *         tmpslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_tmpslice->shape[__pyx_v_i]) = (__pyx_v_src->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1233
+    /* "View.MemoryView":1231
  *     for i in range(ndim):
  *         tmpslice.shape[i] = src.shape[i]
  *         tmpslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,
  */
     (__pyx_v_tmpslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1235
+  /* "View.MemoryView":1233
  *         tmpslice.suboffsets[i] = -1
  * 
  *     fill_contig_strides_array(&tmpslice.shape[0], &tmpslice.strides[0], itemsize,             # <<<<<<<<<<<<<<
  *                               ndim, order)
  * 
  */
   (void)(__pyx_fill_contig_strides_array((&(__pyx_v_tmpslice->shape[0])), (&(__pyx_v_tmpslice->strides[0])), __pyx_v_itemsize, __pyx_v_ndim, __pyx_v_order));
 
-  /* "View.MemoryView":1239
+  /* "View.MemoryView":1237
  * 
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0
  */
   __pyx_t_3 = __pyx_v_ndim;
   __pyx_t_5 = __pyx_t_3;
   for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
     __pyx_v_i = __pyx_t_6;
 
-    /* "View.MemoryView":1240
+    /* "View.MemoryView":1238
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     __pyx_t_2 = (((__pyx_v_tmpslice->shape[__pyx_v_i]) == 1) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1241
+      /* "View.MemoryView":1239
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:
  *             tmpslice.strides[i] = 0             # <<<<<<<<<<<<<<
  * 
  *     if slice_is_contig(src[0], order, ndim):
  */
       (__pyx_v_tmpslice->strides[__pyx_v_i]) = 0;
 
-      /* "View.MemoryView":1240
+      /* "View.MemoryView":1238
  * 
  *     for i in range(ndim):
  *         if tmpslice.shape[i] == 1:             # <<<<<<<<<<<<<<
  *             tmpslice.strides[i] = 0
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1243
+  /* "View.MemoryView":1241
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
   __pyx_t_2 = (__pyx_memviewslice_is_contig((__pyx_v_src[0]), __pyx_v_order, __pyx_v_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1244
+    /* "View.MemoryView":1242
  * 
  *     if slice_is_contig(src[0], order, ndim):
  *         memcpy(result, src.data, size)             # <<<<<<<<<<<<<<
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  */
     (void)(memcpy(__pyx_v_result, __pyx_v_src->data, __pyx_v_size));
 
-    /* "View.MemoryView":1243
+    /* "View.MemoryView":1241
  *             tmpslice.strides[i] = 0
  * 
  *     if slice_is_contig(src[0], order, ndim):             # <<<<<<<<<<<<<<
  *         memcpy(result, src.data, size)
  *     else:
  */
     goto __pyx_L9;
   }
 
-  /* "View.MemoryView":1246
+  /* "View.MemoryView":1244
  *         memcpy(result, src.data, size)
  *     else:
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   /*else*/ {
     copy_strided_to_strided(__pyx_v_src, __pyx_v_tmpslice, __pyx_v_ndim, __pyx_v_itemsize);
   }
   __pyx_L9:;
 
-  /* "View.MemoryView":1248
+  /* "View.MemoryView":1246
  *         copy_strided_to_strided(src, tmpslice, ndim, itemsize)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1210
+  /* "View.MemoryView":1208
  * 
  * @cname('__pyx_memoryview_copy_data_to_temp')
  * cdef void *copy_data_to_temp(__Pyx_memviewslice *src,             # <<<<<<<<<<<<<<
  *                              __Pyx_memviewslice *tmpslice,
  *                              char order,
  */
 
@@ -15512,15 +15343,15 @@
     #endif
   }
   __pyx_r = NULL;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1253
+/* "View.MemoryView":1251
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -15535,57 +15366,57 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_extents", 0);
 
-  /* "View.MemoryView":1256
+  /* "View.MemoryView":1254
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  *                                                         (i, extent1, extent2))             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err_dim')
  */
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1256, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1256, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_extent1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1256, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t(__pyx_v_extent2); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1256, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_3);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
 
-  /* "View.MemoryView":1255
+  /* "View.MemoryView":1253
  * cdef int _err_extents(int i, Py_ssize_t extent1,
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %             # <<<<<<<<<<<<<<
  *                                                         (i, extent1, extent2))
  * 
  */
-  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1255, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyString_Format(__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1255, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_4, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __PYX_ERR(2, 1255, __pyx_L1_error)
+  __PYX_ERR(2, 1253, __pyx_L1_error)
 
-  /* "View.MemoryView":1253
+  /* "View.MemoryView":1251
  * 
  * @cname('__pyx_memoryview_err_extents')
  * cdef int _err_extents(int i, Py_ssize_t extent1,             # <<<<<<<<<<<<<<
  *                              Py_ssize_t extent2) except -1 with gil:
  *     raise ValueError("got differing extents in dimension %d (got %d and %d)" %
  */
 
@@ -15600,15 +15431,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1259
+/* "View.MemoryView":1257
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -15624,26 +15455,26 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_dim", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1260
+  /* "View.MemoryView":1258
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:
  *     raise error(msg.decode('ascii') % dim)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_err')
  */
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1260, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1260, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_dim); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1260, __pyx_L1_error)
+  __pyx_t_4 = PyUnicode_Format(__pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 1258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_v_error);
   __pyx_t_3 = __pyx_v_error; __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -15653,22 +15484,22 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1260, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 1258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __PYX_ERR(2, 1260, __pyx_L1_error)
+  __PYX_ERR(2, 1258, __pyx_L1_error)
 
-  /* "View.MemoryView":1259
+  /* "View.MemoryView":1257
  * 
  * @cname('__pyx_memoryview_err_dim')
  * cdef int _err_dim(object error, char *msg, int dim) except -1 with gil:             # <<<<<<<<<<<<<<
  *     raise error(msg.decode('ascii') % dim)
  * 
  */
 
@@ -15684,15 +15515,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1263
+/* "View.MemoryView":1261
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -15709,32 +15540,32 @@
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err", 0);
   __Pyx_INCREF(__pyx_v_error);
 
-  /* "View.MemoryView":1264
+  /* "View.MemoryView":1262
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   __pyx_t_1 = ((__pyx_v_msg != NULL) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "View.MemoryView":1265
+    /* "View.MemoryView":1263
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))             # <<<<<<<<<<<<<<
  *     else:
  *         raise error
  */
-    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1265, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_decode_c_string(__pyx_v_msg, 0, strlen(__pyx_v_msg), NULL, NULL, PyUnicode_DecodeASCII); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 1263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_v_error);
     __pyx_t_4 = __pyx_v_error; __pyx_t_5 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_5)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -15742,43 +15573,43 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_2 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_5, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_t_3);
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1265, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 1263, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(2, 1265, __pyx_L1_error)
+    __PYX_ERR(2, 1263, __pyx_L1_error)
 
-    /* "View.MemoryView":1264
+    /* "View.MemoryView":1262
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:
  *     if msg != NULL:             # <<<<<<<<<<<<<<
  *         raise error(msg.decode('ascii'))
  *     else:
  */
   }
 
-  /* "View.MemoryView":1267
+  /* "View.MemoryView":1265
  *         raise error(msg.decode('ascii'))
  *     else:
  *         raise error             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_copy_contents')
  */
   /*else*/ {
     __Pyx_Raise(__pyx_v_error, 0, 0, 0);
-    __PYX_ERR(2, 1267, __pyx_L1_error)
+    __PYX_ERR(2, 1265, __pyx_L1_error)
   }
 
-  /* "View.MemoryView":1263
+  /* "View.MemoryView":1261
  * 
  * @cname('__pyx_memoryview_err')
  * cdef int _err(object error, char *msg) except -1 with gil:             # <<<<<<<<<<<<<<
  *     if msg != NULL:
  *         raise error(msg.decode('ascii'))
  */
 
@@ -15794,15 +15625,15 @@
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   return __pyx_r;
 }
 
-/* "View.MemoryView":1270
+/* "View.MemoryView":1268
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -15824,119 +15655,119 @@
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "View.MemoryView":1278
+  /* "View.MemoryView":1276
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  */
   __pyx_v_tmpdata = NULL;
 
-  /* "View.MemoryView":1279
+  /* "View.MemoryView":1277
  *     """
  *     cdef void *tmpdata = NULL
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  */
   __pyx_t_1 = __pyx_v_src.memview->view.itemsize;
   __pyx_v_itemsize = __pyx_t_1;
 
-  /* "View.MemoryView":1281
+  /* "View.MemoryView":1279
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)             # <<<<<<<<<<<<<<
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False
  */
   __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_src), __pyx_v_src_ndim);
 
-  /* "View.MemoryView":1282
+  /* "View.MemoryView":1280
  *     cdef int i
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False             # <<<<<<<<<<<<<<
  *     cdef bint direct_copy = False
  *     cdef __Pyx_memviewslice tmp
  */
   __pyx_v_broadcasting = 0;
 
-  /* "View.MemoryView":1283
+  /* "View.MemoryView":1281
  *     cdef char order = get_best_order(&src, src_ndim)
  *     cdef bint broadcasting = False
  *     cdef bint direct_copy = False             # <<<<<<<<<<<<<<
  *     cdef __Pyx_memviewslice tmp
  * 
  */
   __pyx_v_direct_copy = 0;
 
-  /* "View.MemoryView":1286
+  /* "View.MemoryView":1284
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
   __pyx_t_2 = ((__pyx_v_src_ndim < __pyx_v_dst_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1287
+    /* "View.MemoryView":1285
  * 
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_src), __pyx_v_src_ndim, __pyx_v_dst_ndim);
 
-    /* "View.MemoryView":1286
+    /* "View.MemoryView":1284
  *     cdef __Pyx_memviewslice tmp
  * 
  *     if src_ndim < dst_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1288
+  /* "View.MemoryView":1286
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   __pyx_t_2 = ((__pyx_v_dst_ndim < __pyx_v_src_ndim) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1289
+    /* "View.MemoryView":1287
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:
  *         broadcast_leading(&dst, dst_ndim, src_ndim)             # <<<<<<<<<<<<<<
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)
  */
     __pyx_memoryview_broadcast_leading((&__pyx_v_dst), __pyx_v_dst_ndim, __pyx_v_src_ndim);
 
-    /* "View.MemoryView":1288
+    /* "View.MemoryView":1286
  *     if src_ndim < dst_ndim:
  *         broadcast_leading(&src, src_ndim, dst_ndim)
  *     elif dst_ndim < src_ndim:             # <<<<<<<<<<<<<<
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  */
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1291
+  /* "View.MemoryView":1289
  *         broadcast_leading(&dst, dst_ndim, src_ndim)
  * 
  *     cdef int ndim = max(src_ndim, dst_ndim)             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim):
  */
   __pyx_t_3 = __pyx_v_dst_ndim;
@@ -15944,420 +15775,420 @@
   if (((__pyx_t_3 > __pyx_t_4) != 0)) {
     __pyx_t_5 = __pyx_t_3;
   } else {
     __pyx_t_5 = __pyx_t_4;
   }
   __pyx_v_ndim = __pyx_t_5;
 
-  /* "View.MemoryView":1293
+  /* "View.MemoryView":1291
  *     cdef int ndim = max(src_ndim, dst_ndim)
  * 
  *     for i in range(ndim):             # <<<<<<<<<<<<<<
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  */
   __pyx_t_5 = __pyx_v_ndim;
   __pyx_t_3 = __pyx_t_5;
   for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
     __pyx_v_i = __pyx_t_4;
 
-    /* "View.MemoryView":1294
+    /* "View.MemoryView":1292
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) != (__pyx_v_dst.shape[__pyx_v_i])) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1295
+      /* "View.MemoryView":1293
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
       __pyx_t_2 = (((__pyx_v_src.shape[__pyx_v_i]) == 1) != 0);
       if (__pyx_t_2) {
 
-        /* "View.MemoryView":1296
+        /* "View.MemoryView":1294
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:
  *                 broadcasting = True             # <<<<<<<<<<<<<<
  *                 src.strides[i] = 0
  *             else:
  */
         __pyx_v_broadcasting = 1;
 
-        /* "View.MemoryView":1297
+        /* "View.MemoryView":1295
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  *                 src.strides[i] = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  */
         (__pyx_v_src.strides[__pyx_v_i]) = 0;
 
-        /* "View.MemoryView":1295
+        /* "View.MemoryView":1293
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:
  *             if src.shape[i] == 1:             # <<<<<<<<<<<<<<
  *                 broadcasting = True
  *                 src.strides[i] = 0
  */
         goto __pyx_L7;
       }
 
-      /* "View.MemoryView":1299
+      /* "View.MemoryView":1297
  *                 src.strides[i] = 0
  *             else:
  *                 _err_extents(i, dst.shape[i], src.shape[i])             # <<<<<<<<<<<<<<
  * 
  *         if src.suboffsets[i] >= 0:
  */
       /*else*/ {
-        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1299, __pyx_L1_error)
+        __pyx_t_6 = __pyx_memoryview_err_extents(__pyx_v_i, (__pyx_v_dst.shape[__pyx_v_i]), (__pyx_v_src.shape[__pyx_v_i])); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1297, __pyx_L1_error)
       }
       __pyx_L7:;
 
-      /* "View.MemoryView":1294
+      /* "View.MemoryView":1292
  * 
  *     for i in range(ndim):
  *         if src.shape[i] != dst.shape[i]:             # <<<<<<<<<<<<<<
  *             if src.shape[i] == 1:
  *                 broadcasting = True
  */
     }
 
-    /* "View.MemoryView":1301
+    /* "View.MemoryView":1299
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     __pyx_t_2 = (((__pyx_v_src.suboffsets[__pyx_v_i]) >= 0) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1302
+      /* "View.MemoryView":1300
  * 
  *         if src.suboffsets[i] >= 0:
  *             _err_dim(ValueError, "Dimension %d is not direct", i)             # <<<<<<<<<<<<<<
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  */
-      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1302, __pyx_L1_error)
+      __pyx_t_6 = __pyx_memoryview_err_dim(__pyx_builtin_ValueError, ((char *)"Dimension %d is not direct"), __pyx_v_i); if (unlikely(__pyx_t_6 == ((int)-1))) __PYX_ERR(2, 1300, __pyx_L1_error)
 
-      /* "View.MemoryView":1301
+      /* "View.MemoryView":1299
  *                 _err_extents(i, dst.shape[i], src.shape[i])
  * 
  *         if src.suboffsets[i] >= 0:             # <<<<<<<<<<<<<<
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  */
     }
   }
 
-  /* "View.MemoryView":1304
+  /* "View.MemoryView":1302
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   __pyx_t_2 = (__pyx_slices_overlap((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1306
+    /* "View.MemoryView":1304
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     __pyx_t_2 = ((!(__pyx_memviewslice_is_contig(__pyx_v_src, __pyx_v_order, __pyx_v_ndim) != 0)) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1307
+      /* "View.MemoryView":1305
  * 
  *         if not slice_is_contig(src, order, ndim):
  *             order = get_best_order(&dst, ndim)             # <<<<<<<<<<<<<<
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  */
       __pyx_v_order = __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim);
 
-      /* "View.MemoryView":1306
+      /* "View.MemoryView":1304
  *     if slices_overlap(&src, &dst, ndim, itemsize):
  * 
  *         if not slice_is_contig(src, order, ndim):             # <<<<<<<<<<<<<<
  *             order = get_best_order(&dst, ndim)
  * 
  */
     }
 
-    /* "View.MemoryView":1309
+    /* "View.MemoryView":1307
  *             order = get_best_order(&dst, ndim)
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)             # <<<<<<<<<<<<<<
  *         src = tmp
  * 
  */
-    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(2, 1309, __pyx_L1_error)
+    __pyx_t_7 = __pyx_memoryview_copy_data_to_temp((&__pyx_v_src), (&__pyx_v_tmp), __pyx_v_order, __pyx_v_ndim); if (unlikely(__pyx_t_7 == ((void *)NULL))) __PYX_ERR(2, 1307, __pyx_L1_error)
     __pyx_v_tmpdata = __pyx_t_7;
 
-    /* "View.MemoryView":1310
+    /* "View.MemoryView":1308
  * 
  *         tmpdata = copy_data_to_temp(&src, &tmp, order, ndim)
  *         src = tmp             # <<<<<<<<<<<<<<
  * 
  *     if not broadcasting:
  */
     __pyx_v_src = __pyx_v_tmp;
 
-    /* "View.MemoryView":1304
+    /* "View.MemoryView":1302
  *             _err_dim(ValueError, "Dimension %d is not direct", i)
  * 
  *     if slices_overlap(&src, &dst, ndim, itemsize):             # <<<<<<<<<<<<<<
  * 
  *         if not slice_is_contig(src, order, ndim):
  */
   }
 
-  /* "View.MemoryView":1312
+  /* "View.MemoryView":1310
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = ((!(__pyx_v_broadcasting != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "View.MemoryView":1315
+    /* "View.MemoryView":1313
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'C', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1316
+      /* "View.MemoryView":1314
  * 
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)             # <<<<<<<<<<<<<<
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'C', __pyx_v_ndim);
 
-      /* "View.MemoryView":1315
+      /* "View.MemoryView":1313
  * 
  * 
  *         if slice_is_contig(src, 'C', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  */
       goto __pyx_L12;
     }
 
-    /* "View.MemoryView":1317
+    /* "View.MemoryView":1315
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     __pyx_t_2 = (__pyx_memviewslice_is_contig(__pyx_v_src, 'F', __pyx_v_ndim) != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1318
+      /* "View.MemoryView":1316
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):
  *             direct_copy = slice_is_contig(dst, 'F', ndim)             # <<<<<<<<<<<<<<
  * 
  *         if direct_copy:
  */
       __pyx_v_direct_copy = __pyx_memviewslice_is_contig(__pyx_v_dst, 'F', __pyx_v_ndim);
 
-      /* "View.MemoryView":1317
+      /* "View.MemoryView":1315
  *         if slice_is_contig(src, 'C', ndim):
  *             direct_copy = slice_is_contig(dst, 'C', ndim)
  *         elif slice_is_contig(src, 'F', ndim):             # <<<<<<<<<<<<<<
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  */
     }
     __pyx_L12:;
 
-    /* "View.MemoryView":1320
+    /* "View.MemoryView":1318
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     __pyx_t_2 = (__pyx_v_direct_copy != 0);
     if (__pyx_t_2) {
 
-      /* "View.MemoryView":1322
+      /* "View.MemoryView":1320
  *         if direct_copy:
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-      /* "View.MemoryView":1323
+      /* "View.MemoryView":1321
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))             # <<<<<<<<<<<<<<
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  */
       (void)(memcpy(__pyx_v_dst.data, __pyx_v_src.data, __pyx_memoryview_slice_get_size((&__pyx_v_src), __pyx_v_ndim)));
 
-      /* "View.MemoryView":1324
+      /* "View.MemoryView":1322
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  *             free(tmpdata)
  *             return 0
  */
       __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-      /* "View.MemoryView":1325
+      /* "View.MemoryView":1323
  *             memcpy(dst.data, src.data, slice_get_size(&src, ndim))
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)             # <<<<<<<<<<<<<<
  *             return 0
  * 
  */
       free(__pyx_v_tmpdata);
 
-      /* "View.MemoryView":1326
+      /* "View.MemoryView":1324
  *             refcount_copying(&dst, dtype_is_object, ndim, True)
  *             free(tmpdata)
  *             return 0             # <<<<<<<<<<<<<<
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):
  */
       __pyx_r = 0;
       goto __pyx_L0;
 
-      /* "View.MemoryView":1320
+      /* "View.MemoryView":1318
  *             direct_copy = slice_is_contig(dst, 'F', ndim)
  * 
  *         if direct_copy:             # <<<<<<<<<<<<<<
  * 
  *             refcount_copying(&dst, dtype_is_object, ndim, False)
  */
     }
 
-    /* "View.MemoryView":1312
+    /* "View.MemoryView":1310
  *         src = tmp
  * 
  *     if not broadcasting:             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1328
+  /* "View.MemoryView":1326
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_2 = (__pyx_v_order == 'F');
   if (__pyx_t_2) {
     __pyx_t_2 = ('F' == __pyx_get_best_slice_order((&__pyx_v_dst), __pyx_v_ndim));
   }
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (__pyx_t_8) {
 
-    /* "View.MemoryView":1331
+    /* "View.MemoryView":1329
  * 
  * 
  *         transpose_memslice(&src)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&dst)
  * 
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1331, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_src)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1329, __pyx_L1_error)
 
-    /* "View.MemoryView":1332
+    /* "View.MemoryView":1330
  * 
  *         transpose_memslice(&src)
  *         transpose_memslice(&dst)             # <<<<<<<<<<<<<<
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  */
-    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1332, __pyx_L1_error)
+    __pyx_t_5 = __pyx_memslice_transpose((&__pyx_v_dst)); if (unlikely(__pyx_t_5 == ((int)0))) __PYX_ERR(2, 1330, __pyx_L1_error)
 
-    /* "View.MemoryView":1328
+    /* "View.MemoryView":1326
  *             return 0
  * 
  *     if order == 'F' == get_best_order(&dst, ndim):             # <<<<<<<<<<<<<<
  * 
  * 
  */
   }
 
-  /* "View.MemoryView":1334
+  /* "View.MemoryView":1332
  *         transpose_memslice(&dst)
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1335
+  /* "View.MemoryView":1333
  * 
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)             # <<<<<<<<<<<<<<
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  */
   copy_strided_to_strided((&__pyx_v_src), (&__pyx_v_dst), __pyx_v_ndim, __pyx_v_itemsize);
 
-  /* "View.MemoryView":1336
+  /* "View.MemoryView":1334
  *     refcount_copying(&dst, dtype_is_object, ndim, False)
  *     copy_strided_to_strided(&src, &dst, ndim, itemsize)
  *     refcount_copying(&dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  *     free(tmpdata)
  */
   __pyx_memoryview_refcount_copying((&__pyx_v_dst), __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1338
+  /* "View.MemoryView":1336
  *     refcount_copying(&dst, dtype_is_object, ndim, True)
  * 
  *     free(tmpdata)             # <<<<<<<<<<<<<<
  *     return 0
  * 
  */
   free(__pyx_v_tmpdata);
 
-  /* "View.MemoryView":1339
+  /* "View.MemoryView":1337
  * 
  *     free(tmpdata)
  *     return 0             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  */
   __pyx_r = 0;
   goto __pyx_L0;
 
-  /* "View.MemoryView":1270
+  /* "View.MemoryView":1268
  * 
  * @cname('__pyx_memoryview_copy_contents')
  * cdef int memoryview_copy_contents(__Pyx_memviewslice src,             # <<<<<<<<<<<<<<
  *                                   __Pyx_memviewslice dst,
  *                                   int src_ndim, int dst_ndim,
  */
 
@@ -16373,217 +16204,217 @@
     #endif
   }
   __pyx_r = -1;
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "View.MemoryView":1342
+/* "View.MemoryView":1340
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
 static void __pyx_memoryview_broadcast_leading(__Pyx_memviewslice *__pyx_v_mslice, int __pyx_v_ndim, int __pyx_v_ndim_other) {
   int __pyx_v_i;
   int __pyx_v_offset;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
 
-  /* "View.MemoryView":1346
+  /* "View.MemoryView":1344
  *                             int ndim_other) nogil:
  *     cdef int i
  *     cdef int offset = ndim_other - ndim             # <<<<<<<<<<<<<<
  * 
  *     for i in range(ndim - 1, -1, -1):
  */
   __pyx_v_offset = (__pyx_v_ndim_other - __pyx_v_ndim);
 
-  /* "View.MemoryView":1348
+  /* "View.MemoryView":1346
  *     cdef int offset = ndim_other - ndim
  * 
  *     for i in range(ndim - 1, -1, -1):             # <<<<<<<<<<<<<<
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  */
   for (__pyx_t_1 = (__pyx_v_ndim - 1); __pyx_t_1 > -1; __pyx_t_1-=1) {
     __pyx_v_i = __pyx_t_1;
 
-    /* "View.MemoryView":1349
+    /* "View.MemoryView":1347
  * 
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]             # <<<<<<<<<<<<<<
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  */
     (__pyx_v_mslice->shape[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->shape[__pyx_v_i]);
 
-    /* "View.MemoryView":1350
+    /* "View.MemoryView":1348
  *     for i in range(ndim - 1, -1, -1):
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  */
     (__pyx_v_mslice->strides[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->strides[__pyx_v_i]);
 
-    /* "View.MemoryView":1351
+    /* "View.MemoryView":1349
  *         mslice.shape[i + offset] = mslice.shape[i]
  *         mslice.strides[i + offset] = mslice.strides[i]
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]             # <<<<<<<<<<<<<<
  * 
  *     for i in range(offset):
  */
     (__pyx_v_mslice->suboffsets[(__pyx_v_i + __pyx_v_offset)]) = (__pyx_v_mslice->suboffsets[__pyx_v_i]);
   }
 
-  /* "View.MemoryView":1353
+  /* "View.MemoryView":1351
  *         mslice.suboffsets[i + offset] = mslice.suboffsets[i]
  * 
  *     for i in range(offset):             # <<<<<<<<<<<<<<
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  */
   __pyx_t_1 = __pyx_v_offset;
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1354
+    /* "View.MemoryView":1352
  * 
  *     for i in range(offset):
  *         mslice.shape[i] = 1             # <<<<<<<<<<<<<<
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1
  */
     (__pyx_v_mslice->shape[__pyx_v_i]) = 1;
 
-    /* "View.MemoryView":1355
+    /* "View.MemoryView":1353
  *     for i in range(offset):
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]             # <<<<<<<<<<<<<<
  *         mslice.suboffsets[i] = -1
  * 
  */
     (__pyx_v_mslice->strides[__pyx_v_i]) = (__pyx_v_mslice->strides[0]);
 
-    /* "View.MemoryView":1356
+    /* "View.MemoryView":1354
  *         mslice.shape[i] = 1
  *         mslice.strides[i] = mslice.strides[0]
  *         mslice.suboffsets[i] = -1             # <<<<<<<<<<<<<<
  * 
  * 
  */
     (__pyx_v_mslice->suboffsets[__pyx_v_i]) = -1L;
   }
 
-  /* "View.MemoryView":1342
+  /* "View.MemoryView":1340
  * 
  * @cname('__pyx_memoryview_broadcast_leading')
  * cdef void broadcast_leading(__Pyx_memviewslice *mslice,             # <<<<<<<<<<<<<<
  *                             int ndim,
  *                             int ndim_other) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1364
+/* "View.MemoryView":1362
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
 static void __pyx_memoryview_refcount_copying(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_dtype_is_object, int __pyx_v_ndim, int __pyx_v_inc) {
   int __pyx_t_1;
 
-  /* "View.MemoryView":1368
+  /* "View.MemoryView":1366
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   __pyx_t_1 = (__pyx_v_dtype_is_object != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1369
+    /* "View.MemoryView":1367
  * 
  *     if dtype_is_object:
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,             # <<<<<<<<<<<<<<
  *                                            dst.strides, ndim, inc)
  * 
  */
     __pyx_memoryview_refcount_objects_in_slice_with_gil(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_inc);
 
-    /* "View.MemoryView":1368
+    /* "View.MemoryView":1366
  * 
  * 
  *     if dtype_is_object:             # <<<<<<<<<<<<<<
  *         refcount_objects_in_slice_with_gil(dst.data, dst.shape,
  *                                            dst.strides, ndim, inc)
  */
   }
 
-  /* "View.MemoryView":1364
+  /* "View.MemoryView":1362
  * 
  * @cname('__pyx_memoryview_refcount_copying')
  * cdef void refcount_copying(__Pyx_memviewslice *dst, bint dtype_is_object,             # <<<<<<<<<<<<<<
  *                            int ndim, bint inc) nogil:
  * 
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1373
+/* "View.MemoryView":1371
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
 static void __pyx_memoryview_refcount_objects_in_slice_with_gil(char *__pyx_v_data, Py_ssize_t *__pyx_v_shape, Py_ssize_t *__pyx_v_strides, int __pyx_v_ndim, int __pyx_v_inc) {
   __Pyx_RefNannyDeclarations
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("refcount_objects_in_slice_with_gil", 0);
 
-  /* "View.MemoryView":1376
+  /* "View.MemoryView":1374
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  *     refcount_objects_in_slice(data, shape, strides, ndim, inc)             # <<<<<<<<<<<<<<
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  */
   __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, __pyx_v_shape, __pyx_v_strides, __pyx_v_ndim, __pyx_v_inc);
 
-  /* "View.MemoryView":1373
+  /* "View.MemoryView":1371
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice_with_gil')
  * cdef void refcount_objects_in_slice_with_gil(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                              Py_ssize_t *strides, int ndim,
  *                                              bint inc) with gil:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "View.MemoryView":1379
+/* "View.MemoryView":1377
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
@@ -16592,178 +16423,178 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   __Pyx_RefNannySetupContext("refcount_objects_in_slice", 0);
 
-  /* "View.MemoryView":1383
+  /* "View.MemoryView":1381
  *     cdef Py_ssize_t i
  * 
  *     for i in range(shape[0]):             # <<<<<<<<<<<<<<
  *         if ndim == 1:
  *             if inc:
  */
   __pyx_t_1 = (__pyx_v_shape[0]);
   __pyx_t_2 = __pyx_t_1;
   for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
     __pyx_v_i = __pyx_t_3;
 
-    /* "View.MemoryView":1384
+    /* "View.MemoryView":1382
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
     __pyx_t_4 = ((__pyx_v_ndim == 1) != 0);
     if (__pyx_t_4) {
 
-      /* "View.MemoryView":1385
+      /* "View.MemoryView":1383
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
       __pyx_t_4 = (__pyx_v_inc != 0);
       if (__pyx_t_4) {
 
-        /* "View.MemoryView":1386
+        /* "View.MemoryView":1384
  *         if ndim == 1:
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])
  */
         Py_INCREF((((PyObject **)__pyx_v_data)[0]));
 
-        /* "View.MemoryView":1385
+        /* "View.MemoryView":1383
  *     for i in range(shape[0]):
  *         if ndim == 1:
  *             if inc:             # <<<<<<<<<<<<<<
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  */
         goto __pyx_L6;
       }
 
-      /* "View.MemoryView":1388
+      /* "View.MemoryView":1386
  *                 Py_INCREF((<PyObject **> data)[0])
  *             else:
  *                 Py_DECREF((<PyObject **> data)[0])             # <<<<<<<<<<<<<<
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  */
       /*else*/ {
         Py_DECREF((((PyObject **)__pyx_v_data)[0]));
       }
       __pyx_L6:;
 
-      /* "View.MemoryView":1384
+      /* "View.MemoryView":1382
  * 
  *     for i in range(shape[0]):
  *         if ndim == 1:             # <<<<<<<<<<<<<<
  *             if inc:
  *                 Py_INCREF((<PyObject **> data)[0])
  */
       goto __pyx_L5;
     }
 
-    /* "View.MemoryView":1390
+    /* "View.MemoryView":1388
  *                 Py_DECREF((<PyObject **> data)[0])
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                       ndim - 1, inc)
  * 
  */
     /*else*/ {
 
-      /* "View.MemoryView":1391
+      /* "View.MemoryView":1389
  *         else:
  *             refcount_objects_in_slice(data, shape + 1, strides + 1,
  *                                       ndim - 1, inc)             # <<<<<<<<<<<<<<
  * 
  *         data += strides[0]
  */
       __pyx_memoryview_refcount_objects_in_slice(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_inc);
     }
     __pyx_L5:;
 
-    /* "View.MemoryView":1393
+    /* "View.MemoryView":1391
  *                                       ndim - 1, inc)
  * 
  *         data += strides[0]             # <<<<<<<<<<<<<<
  * 
  * 
  */
     __pyx_v_data = (__pyx_v_data + (__pyx_v_strides[0]));
   }
 
-  /* "View.MemoryView":1379
+  /* "View.MemoryView":1377
  * 
  * @cname('__pyx_memoryview_refcount_objects_in_slice')
  * cdef void refcount_objects_in_slice(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                                     Py_ssize_t *strides, int ndim, bint inc):
  *     cdef Py_ssize_t i
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "View.MemoryView":1399
+/* "View.MemoryView":1397
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
 static void __pyx_memoryview_slice_assign_scalar(__Pyx_memviewslice *__pyx_v_dst, int __pyx_v_ndim, size_t __pyx_v_itemsize, void *__pyx_v_item, int __pyx_v_dtype_is_object) {
 
-  /* "View.MemoryView":1402
+  /* "View.MemoryView":1400
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)             # <<<<<<<<<<<<<<
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 0);
 
-  /* "View.MemoryView":1403
+  /* "View.MemoryView":1401
  *                               bint dtype_is_object) nogil:
  *     refcount_copying(dst, dtype_is_object, ndim, False)
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,             # <<<<<<<<<<<<<<
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)
  */
   __pyx_memoryview__slice_assign_scalar(__pyx_v_dst->data, __pyx_v_dst->shape, __pyx_v_dst->strides, __pyx_v_ndim, __pyx_v_itemsize, __pyx_v_item);
 
-  /* "View.MemoryView":1405
+  /* "View.MemoryView":1403
  *     _slice_assign_scalar(dst.data, dst.shape, dst.strides, ndim,
  *                          itemsize, item)
  *     refcount_copying(dst, dtype_is_object, ndim, True)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_memoryview_refcount_copying(__pyx_v_dst, __pyx_v_dtype_is_object, __pyx_v_ndim, 1);
 
-  /* "View.MemoryView":1399
+  /* "View.MemoryView":1397
  * 
  * @cname('__pyx_memoryview_slice_assign_scalar')
  * cdef void slice_assign_scalar(__Pyx_memviewslice *dst, int ndim,             # <<<<<<<<<<<<<<
  *                               size_t itemsize, void *item,
  *                               bint dtype_is_object) nogil:
  */
 
   /* function exit code */
 }
 
-/* "View.MemoryView":1409
+/* "View.MemoryView":1407
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -16772,118 +16603,118 @@
   Py_ssize_t __pyx_v_stride;
   Py_ssize_t __pyx_v_extent;
   int __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
 
-  /* "View.MemoryView":1413
+  /* "View.MemoryView":1411
  *                               size_t itemsize, void *item) nogil:
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t extent = shape[0]
  * 
  */
   __pyx_v_stride = (__pyx_v_strides[0]);
 
-  /* "View.MemoryView":1414
+  /* "View.MemoryView":1412
  *     cdef Py_ssize_t i
  *     cdef Py_ssize_t stride = strides[0]
  *     cdef Py_ssize_t extent = shape[0]             # <<<<<<<<<<<<<<
  * 
  *     if ndim == 1:
  */
   __pyx_v_extent = (__pyx_v_shape[0]);
 
-  /* "View.MemoryView":1416
+  /* "View.MemoryView":1414
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
   __pyx_t_1 = ((__pyx_v_ndim == 1) != 0);
   if (__pyx_t_1) {
 
-    /* "View.MemoryView":1417
+    /* "View.MemoryView":1415
  * 
  *     if ndim == 1:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             memcpy(data, item, itemsize)
  *             data += stride
  */
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1418
+      /* "View.MemoryView":1416
  *     if ndim == 1:
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)             # <<<<<<<<<<<<<<
  *             data += stride
  *     else:
  */
       (void)(memcpy(__pyx_v_data, __pyx_v_item, __pyx_v_itemsize));
 
-      /* "View.MemoryView":1419
+      /* "View.MemoryView":1417
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  *             data += stride             # <<<<<<<<<<<<<<
  *     else:
  *         for i in range(extent):
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
 
-    /* "View.MemoryView":1416
+    /* "View.MemoryView":1414
  *     cdef Py_ssize_t extent = shape[0]
  * 
  *     if ndim == 1:             # <<<<<<<<<<<<<<
  *         for i in range(extent):
  *             memcpy(data, item, itemsize)
  */
     goto __pyx_L3;
   }
 
-  /* "View.MemoryView":1421
+  /* "View.MemoryView":1419
  *             data += stride
  *     else:
  *         for i in range(extent):             # <<<<<<<<<<<<<<
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  */
   /*else*/ {
     __pyx_t_2 = __pyx_v_extent;
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_v_i = __pyx_t_4;
 
-      /* "View.MemoryView":1422
+      /* "View.MemoryView":1420
  *     else:
  *         for i in range(extent):
  *             _slice_assign_scalar(data, shape + 1, strides + 1,             # <<<<<<<<<<<<<<
  *                                 ndim - 1, itemsize, item)
  *             data += stride
  */
       __pyx_memoryview__slice_assign_scalar(__pyx_v_data, (__pyx_v_shape + 1), (__pyx_v_strides + 1), (__pyx_v_ndim - 1), __pyx_v_itemsize, __pyx_v_item);
 
-      /* "View.MemoryView":1424
+      /* "View.MemoryView":1422
  *             _slice_assign_scalar(data, shape + 1, strides + 1,
  *                                 ndim - 1, itemsize, item)
  *             data += stride             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_v_data = (__pyx_v_data + __pyx_v_stride);
     }
   }
   __pyx_L3:;
 
-  /* "View.MemoryView":1409
+  /* "View.MemoryView":1407
  * 
  * @cname('__pyx_memoryview__slice_assign_scalar')
  * cdef void _slice_assign_scalar(char *data, Py_ssize_t *shape,             # <<<<<<<<<<<<<<
  *                               Py_ssize_t *strides, int ndim,
  *                               size_t itemsize, void *item) nogil:
  */
 
@@ -16973,155 +16804,151 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  int __pyx_t_3;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum != 0xb068931:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__21, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (__pyx_t_3) {
+  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xb068931) != 0);
+  if (__pyx_t_1) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
+ *     if __pyx_checksum != 0xb068931:
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
-    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_t_1);
-    __pyx_v___pyx_PickleError = __pyx_t_1;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
+    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_t_2);
+    __pyx_v___pyx_PickleError = __pyx_t_2;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
+ *     if __pyx_checksum != 0xb068931:
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_6);
+    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(2, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum != 0xb068931:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_5);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v___pyx_result = __pyx_t_3;
+  __pyx_t_3 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_2 = (__pyx_t_3 != 0);
-  if (__pyx_t_2) {
+  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_6 = (__pyx_t_1 != 0);
+  if (__pyx_t_6) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
-    __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_3 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(2, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17141,18 +16968,18 @@
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("View.MemoryView.__pyx_unpickle_Enum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -17468,23 +17295,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -17590,23 +17414,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -17854,23 +17675,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
   PyObject *o = __pyx_tp_new_memoryview(t, a, k);
   if (unlikely(!o)) return 0;
@@ -18003,23 +17821,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -18069,15 +17884,15 @@
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
-  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_k_Incompatible_checksums_s_vs_0xb0, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xb0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
@@ -18173,105 +17988,105 @@
   {&__pyx_n_s_word1, __pyx_k_word1, sizeof(__pyx_k_word1), 0, 0, 1, 1},
   {&__pyx_n_s_word2, __pyx_k_word2, sizeof(__pyx_k_word2), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 14, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
-  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 133, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 148, __pyx_L1_error)
+  __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 151, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
-  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
-  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
-  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
+  __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 404, __pyx_L1_error)
+  __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 613, __pyx_L1_error)
+  __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 832, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "View.MemoryView":134
+  /* "View.MemoryView":133
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 134, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(2, 133, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
-  /* "View.MemoryView":137
+  /* "View.MemoryView":136
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 137, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(2, 136, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "View.MemoryView":149
+  /* "View.MemoryView":148
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 149, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(2, 148, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
-  /* "View.MemoryView":177
+  /* "View.MemoryView":176
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 177, __pyx_L1_error)
+  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(2, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "View.MemoryView":193
+  /* "View.MemoryView":192
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 193, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(2, 192, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -18286,66 +18101,66 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "View.MemoryView":420
+  /* "View.MemoryView":418
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 420, __pyx_L1_error)
+  __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__10);
   __Pyx_GIVEREF(__pyx_tuple__10);
 
-  /* "View.MemoryView":497
+  /* "View.MemoryView":495
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 497, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(2, 495, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
-  /* "View.MemoryView":522
+  /* "View.MemoryView":520
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 522, __pyx_L1_error)
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(2, 520, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__12);
   __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "View.MemoryView":572
+  /* "View.MemoryView":570
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 572, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(2, 570, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__13);
   __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "View.MemoryView":579
+  /* "View.MemoryView":577
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 579, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_New(1); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(2, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__14);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
   PyTuple_SET_ITEM(__pyx_tuple__14, 0, __pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "(tree fragment)":2
@@ -18363,33 +18178,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__16);
   __Pyx_GIVEREF(__pyx_tuple__16);
 
-  /* "View.MemoryView":684
+  /* "View.MemoryView":682
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(2, 684, __pyx_L1_error)
+  __pyx_slice__17 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__17)) __PYX_ERR(2, 682, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice__17);
   __Pyx_GIVEREF(__pyx_slice__17);
 
-  /* "View.MemoryView":705
+  /* "View.MemoryView":703
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 705, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(2, 703, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -18403,107 +18218,102 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "shorttext/metrics/dynprog/dldist.pyx":5
  * cimport numpy as np
  * 
  * def damerau_levenshtein(str word1, str word2):             # <<<<<<<<<<<<<<
  *     cdef int len1 = len(word1)
  *     cdef int len2 = len(word2)
  */
-  __pyx_tuple__22 = PyTuple_Pack(12, __pyx_n_s_word1, __pyx_n_s_word2, __pyx_n_s_len1, __pyx_n_s_len2, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_cost, __pyx_n_s_delcost, __pyx_n_s_inscost, __pyx_n_s_subcost, __pyx_n_s_score, __pyx_n_s_matrix); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 5, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_shorttext_metrics_dynprog_dldist, __pyx_n_s_damerau_levenshtein, 5, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(12, __pyx_n_s_word1, __pyx_n_s_word2, __pyx_n_s_len1, __pyx_n_s_len2, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_cost, __pyx_n_s_delcost, __pyx_n_s_inscost, __pyx_n_s_subcost, __pyx_n_s_score, __pyx_n_s_matrix); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 5, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(2, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_shorttext_metrics_dynprog_dldist, __pyx_n_s_damerau_levenshtein, 5, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 5, __pyx_L1_error)
 
-  /* "View.MemoryView":287
+  /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(2, 286, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
-  /* "View.MemoryView":288
+  /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
-  /* "View.MemoryView":289
+  /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
-  /* "View.MemoryView":292
+  /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(2, 291, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__26);
+  __Pyx_GIVEREF(__pyx_tuple__26);
 
-  /* "View.MemoryView":293
+  /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__29 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 2, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 2, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -18549,62 +18359,62 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
-  if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
   #endif
-  if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 106, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_array.tp_dict, __pyx_vtabptr_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_array) < 0) __PYX_ERR(2, 105, __pyx_L1_error)
   __pyx_array_type = &__pyx_type___pyx_array;
-  if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 280, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 279, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_MemviewEnum.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_MemviewEnum.tp_dictoffset && __pyx_type___pyx_MemviewEnum.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_MemviewEnum.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 280, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_MemviewEnum) < 0) __PYX_ERR(2, 279, __pyx_L1_error)
   __pyx_MemviewEnum_type = &__pyx_type___pyx_MemviewEnum;
   __pyx_vtabptr_memoryview = &__pyx_vtable_memoryview;
   __pyx_vtable_memoryview.get_item_pointer = (char *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_get_item_pointer;
   __pyx_vtable_memoryview.is_slice = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_is_slice;
   __pyx_vtable_memoryview.setitem_slice_assignment = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_slice_assignment;
   __pyx_vtable_memoryview.setitem_slice_assign_scalar = (PyObject *(*)(struct __pyx_memoryview_obj *, struct __pyx_memoryview_obj *, PyObject *))__pyx_memoryview_setitem_slice_assign_scalar;
   __pyx_vtable_memoryview.setitem_indexed = (PyObject *(*)(struct __pyx_memoryview_obj *, PyObject *, PyObject *))__pyx_memoryview_setitem_indexed;
   __pyx_vtable_memoryview.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryview_convert_item_to_object;
   __pyx_vtable_memoryview.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryview_assign_item_from_object;
-  if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryview.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryview.tp_dictoffset && __pyx_type___pyx_memoryview.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryview.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 331, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryview.tp_dict, __pyx_vtabptr_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryview) < 0) __PYX_ERR(2, 330, __pyx_L1_error)
   __pyx_memoryview_type = &__pyx_type___pyx_memoryview;
   __pyx_vtabptr__memoryviewslice = &__pyx_vtable__memoryviewslice;
   __pyx_vtable__memoryviewslice.__pyx_base = *__pyx_vtabptr_memoryview;
   __pyx_vtable__memoryviewslice.__pyx_base.convert_item_to_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *))__pyx_memoryviewslice_convert_item_to_object;
   __pyx_vtable__memoryviewslice.__pyx_base.assign_item_from_object = (PyObject *(*)(struct __pyx_memoryview_obj *, char *, PyObject *))__pyx_memoryviewslice_assign_item_from_object;
   __pyx_type___pyx_memoryviewslice.tp_base = __pyx_memoryview_type;
-  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
+  if (PyType_Ready(&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_memoryviewslice.tp_print = 0;
   #endif
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type___pyx_memoryviewslice.tp_dictoffset && __pyx_type___pyx_memoryviewslice.tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_type___pyx_memoryviewslice.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 967, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type___pyx_memoryviewslice.tp_dict, __pyx_vtabptr__memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type___pyx_memoryviewslice) < 0) __PYX_ERR(2, 965, __pyx_L1_error)
   __pyx_memoryviewslice_type = &__pyx_type___pyx_memoryviewslice;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
@@ -18624,46 +18434,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -18827,17 +18637,19 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
+  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("dldist", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -18916,107 +18728,107 @@
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "View.MemoryView":210
+  /* "View.MemoryView":209
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(array self):
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 210, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_array_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 209, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 210, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_array_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 209, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_array_type);
 
-  /* "View.MemoryView":287
+  /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":288
+  /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":289
+  /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":292
+  /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":293
+  /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "View.MemoryView":317
+  /* "View.MemoryView":316
  * 
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0             # <<<<<<<<<<<<<<
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [
  *     PyThread_allocate_lock(),
  */
   __pyx_memoryview_thread_locks_used = 0;
 
-  /* "View.MemoryView":318
+  /* "View.MemoryView":317
  * DEF THREAD_LOCKS_PREALLOCATED = 8
  * cdef int __pyx_memoryview_thread_locks_used = 0
  * cdef PyThread_type_lock[THREAD_LOCKS_PREALLOCATED] __pyx_memoryview_thread_locks = [             # <<<<<<<<<<<<<<
  *     PyThread_allocate_lock(),
  *     PyThread_allocate_lock(),
  */
   __pyx_t_2[0] = PyThread_allocate_lock();
@@ -19025,37 +18837,37 @@
   __pyx_t_2[3] = PyThread_allocate_lock();
   __pyx_t_2[4] = PyThread_allocate_lock();
   __pyx_t_2[5] = PyThread_allocate_lock();
   __pyx_t_2[6] = PyThread_allocate_lock();
   __pyx_t_2[7] = PyThread_allocate_lock();
   memcpy(&(__pyx_memoryview_thread_locks[0]), __pyx_t_2, sizeof(__pyx_memoryview_thread_locks[0]) * (8));
 
-  /* "View.MemoryView":551
+  /* "View.MemoryView":549
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 551, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 549, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 551, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryview_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 549, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryview_type);
 
-  /* "View.MemoryView":997
+  /* "View.MemoryView":995
  *         return self.from_object
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_memoryview_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 997, __pyx_L1_error)
+  __pyx_t_1 = __pyx_capsule_create(((void *)(&__pyx_memoryview_getbuffer)), ((char *)"getbuffer(obj, view, flags)")); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 995, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 997, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_memoryviewslice_type->tp_dict, __pyx_n_s_pyx_getbuffer, __pyx_t_1) < 0) __PYX_ERR(2, 995, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   PyType_Modified(__pyx_memoryviewslice_type);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
@@ -19367,15 +19179,15 @@
     return __Pyx_GetBuiltinName(name);
 }
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
+    ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -19532,15 +19344,15 @@
 }
 #ifndef Py_NO_RETURN
 #define Py_NO_RETURN
 #endif
 static void __pyx_fatalerror(const char *fmt, ...) Py_NO_RETURN {
     va_list vargs;
     char msg[200];
-#if PY_VERSION_HEX >= 0x030A0000 || defined(HAVE_STDARG_PROTOTYPES)
+#ifdef HAVE_STDARG_PROTOTYPES
     va_start(vargs, fmt);
 #else
     va_start(vargs);
 #endif
     vsnprintf(msg, 200, fmt, vargs);
     va_end(vargs);
     Py_FatalError(msg);
@@ -20197,15 +20009,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+#if CYTHON_USE_UNICODE_INTERNALS
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -20326,15 +20138,15 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
-/* DivInt[Py_ssize_t] */
+/* None */
 static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t a, Py_ssize_t b) {
     Py_ssize_t q = a / b;
     Py_ssize_t r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
@@ -20784,15 +20596,15 @@
 #endif
 
 /* None */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
     PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
 }
 
-/* DivInt[long] */
+/* None */
 static CYTHON_INLINE long __Pyx_div_long(long a, long b) {
     long q = a / b;
     long r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
@@ -20934,43 +20746,25 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
-    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
-    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
 #else
-    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
-    if (!getstate && PyErr_Occurred()) {
-        goto __PYX_BAD;
-    }
+    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
 #endif
-    if (getstate) {
-#if CYTHON_USE_PYTYPE_LOOKUP
-        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
-#else
-        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
-        if (!object_getstate && PyErr_Occurred()) {
-            goto __PYX_BAD;
-        }
-#endif
-        if (object_getstate != getstate) {
-            goto __PYX_GOOD;
-        }
-    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -21007,16 +20801,14 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
-    Py_XDECREF(object_getstate);
-    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -21111,15 +20903,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -21205,48 +20997,41 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = NULL;
-    PyObject *py_funcname = NULL;
+    PyCodeObject *py_code = 0;
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
     #if PY_MAJOR_VERSION < 3
-    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    if (!py_srcfile) goto bad;
+    #else
+    py_srcfile = PyUnicode_FromString(filename);
     #endif
+    if (!py_srcfile) goto bad;
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
-        funcname = PyUnicode_AsUTF8(py_funcname);
-        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        if (!py_funcname) goto bad;
+        #else
+        py_funcname = PyUnicode_FromString(funcname);
         #endif
     }
-    #if PY_MAJOR_VERSION < 3
+    if (!py_funcname) goto bad;
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -21257,49 +21042,34 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    #else
-    py_code = PyCode_NewEmpty(filename, funcname, py_line);
-    #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_DECREF(py_funcname);
     return py_code;
 bad:
-    Py_XDECREF(py_funcname);
-    #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
-    #endif
+    Py_XDECREF(py_funcname);
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -21401,774 +21171,16 @@
     cobj = PyCapsule_New(p, sig, NULL);
 #else
     cobj = PyCObject_FromVoidPtr(p, NULL);
 #endif
     return cobj;
 }
 
-/* IsLittleEndian */
-static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
-{
-  union {
-    uint32_t u32;
-    uint8_t u8[4];
-  } S;
-  S.u32 = 0x01020304;
-  return S.u8[0] == 4;
-}
-
-/* BufferFormatCheck */
-static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
-                              __Pyx_BufFmt_StackElem* stack,
-                              __Pyx_TypeInfo* type) {
-  stack[0].field = &ctx->root;
-  stack[0].parent_offset = 0;
-  ctx->root.type = type;
-  ctx->root.name = "buffer dtype";
-  ctx->root.offset = 0;
-  ctx->head = stack;
-  ctx->head->field = &ctx->root;
-  ctx->fmt_offset = 0;
-  ctx->head->parent_offset = 0;
-  ctx->new_packmode = '@';
-  ctx->enc_packmode = '@';
-  ctx->new_count = 1;
-  ctx->enc_count = 0;
-  ctx->enc_type = 0;
-  ctx->is_complex = 0;
-  ctx->is_valid_array = 0;
-  ctx->struct_alignment = 0;
-  while (type->typegroup == 'S') {
-    ++ctx->head;
-    ctx->head->field = type->fields;
-    ctx->head->parent_offset = 0;
-    type = type->fields->type;
-  }
-}
-static int __Pyx_BufFmt_ParseNumber(const char** ts) {
-    int count;
-    const char* t = *ts;
-    if (*t < '0' || *t > '9') {
-      return -1;
-    } else {
-        count = *t++ - '0';
-        while (*t >= '0' && *t <= '9') {
-            count *= 10;
-            count += *t++ - '0';
-        }
-    }
-    *ts = t;
-    return count;
-}
-static int __Pyx_BufFmt_ExpectNumber(const char **ts) {
-    int number = __Pyx_BufFmt_ParseNumber(ts);
-    if (number == -1)
-        PyErr_Format(PyExc_ValueError,\
-                     "Does not understand character buffer dtype format string ('%c')", **ts);
-    return number;
-}
-static void __Pyx_BufFmt_RaiseUnexpectedChar(char ch) {
-  PyErr_Format(PyExc_ValueError,
-               "Unexpected format string character: '%c'", ch);
-}
-static const char* __Pyx_BufFmt_DescribeTypeChar(char ch, int is_complex) {
-  switch (ch) {
-    case '?': return "'bool'";
-    case 'c': return "'char'";
-    case 'b': return "'signed char'";
-    case 'B': return "'unsigned char'";
-    case 'h': return "'short'";
-    case 'H': return "'unsigned short'";
-    case 'i': return "'int'";
-    case 'I': return "'unsigned int'";
-    case 'l': return "'long'";
-    case 'L': return "'unsigned long'";
-    case 'q': return "'long long'";
-    case 'Q': return "'unsigned long long'";
-    case 'f': return (is_complex ? "'complex float'" : "'float'");
-    case 'd': return (is_complex ? "'complex double'" : "'double'");
-    case 'g': return (is_complex ? "'complex long double'" : "'long double'");
-    case 'T': return "a struct";
-    case 'O': return "Python object";
-    case 'P': return "a pointer";
-    case 's': case 'p': return "a string";
-    case 0: return "end";
-    default: return "unparseable format string";
-  }
-}
-static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return 2;
-    case 'i': case 'I': case 'l': case 'L': return 4;
-    case 'q': case 'Q': return 8;
-    case 'f': return (is_complex ? 8 : 4);
-    case 'd': return (is_complex ? 16 : 8);
-    case 'g': {
-      PyErr_SetString(PyExc_ValueError, "Python does not define a standard format string size for long double ('g')..");
-      return 0;
-    }
-    case 'O': case 'P': return sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-}
-static size_t __Pyx_BufFmt_TypeCharToNativeSize(char ch, int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(short);
-    case 'i': case 'I': return sizeof(int);
-    case 'l': case 'L': return sizeof(long);
-    #ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(PY_LONG_LONG);
-    #endif
-    case 'f': return sizeof(float) * (is_complex ? 2 : 1);
-    case 'd': return sizeof(double) * (is_complex ? 2 : 1);
-    case 'g': return sizeof(long double) * (is_complex ? 2 : 1);
-    case 'O': case 'P': return sizeof(void*);
-    default: {
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-  }
-}
-typedef struct { char c; short x; } __Pyx_st_short;
-typedef struct { char c; int x; } __Pyx_st_int;
-typedef struct { char c; long x; } __Pyx_st_long;
-typedef struct { char c; float x; } __Pyx_st_float;
-typedef struct { char c; double x; } __Pyx_st_double;
-typedef struct { char c; long double x; } __Pyx_st_longdouble;
-typedef struct { char c; void *x; } __Pyx_st_void_p;
-#ifdef HAVE_LONG_LONG
-typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
-#endif
-static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
-    case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
-    case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
-#ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
-#endif
-    case 'f': return sizeof(__Pyx_st_float) - sizeof(float);
-    case 'd': return sizeof(__Pyx_st_double) - sizeof(double);
-    case 'g': return sizeof(__Pyx_st_longdouble) - sizeof(long double);
-    case 'P': case 'O': return sizeof(__Pyx_st_void_p) - sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-}
-/* These are for computing the padding at the end of the struct to align
-   on the first member of the struct. This will probably the same as above,
-   but we don't have any guarantees.
- */
-typedef struct { short x; char c; } __Pyx_pad_short;
-typedef struct { int x; char c; } __Pyx_pad_int;
-typedef struct { long x; char c; } __Pyx_pad_long;
-typedef struct { float x; char c; } __Pyx_pad_float;
-typedef struct { double x; char c; } __Pyx_pad_double;
-typedef struct { long double x; char c; } __Pyx_pad_longdouble;
-typedef struct { void *x; char c; } __Pyx_pad_void_p;
-#ifdef HAVE_LONG_LONG
-typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
-#endif
-static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
-  switch (ch) {
-    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
-    case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
-    case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
-    case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
-#ifdef HAVE_LONG_LONG
-    case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
-#endif
-    case 'f': return sizeof(__Pyx_pad_float) - sizeof(float);
-    case 'd': return sizeof(__Pyx_pad_double) - sizeof(double);
-    case 'g': return sizeof(__Pyx_pad_longdouble) - sizeof(long double);
-    case 'P': case 'O': return sizeof(__Pyx_pad_void_p) - sizeof(void*);
-    default:
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-}
-static char __Pyx_BufFmt_TypeCharToGroup(char ch, int is_complex) {
-  switch (ch) {
-    case 'c':
-        return 'H';
-    case 'b': case 'h': case 'i':
-    case 'l': case 'q': case 's': case 'p':
-        return 'I';
-    case '?': case 'B': case 'H': case 'I': case 'L': case 'Q':
-        return 'U';
-    case 'f': case 'd': case 'g':
-        return (is_complex ? 'C' : 'R');
-    case 'O':
-        return 'O';
-    case 'P':
-        return 'P';
-    default: {
-      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
-      return 0;
-    }
-  }
-}
-static void __Pyx_BufFmt_RaiseExpected(__Pyx_BufFmt_Context* ctx) {
-  if (ctx->head == NULL || ctx->head->field == &ctx->root) {
-    const char* expected;
-    const char* quote;
-    if (ctx->head == NULL) {
-      expected = "end";
-      quote = "";
-    } else {
-      expected = ctx->head->field->type->name;
-      quote = "'";
-    }
-    PyErr_Format(PyExc_ValueError,
-                 "Buffer dtype mismatch, expected %s%s%s but got %s",
-                 quote, expected, quote,
-                 __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex));
-  } else {
-    __Pyx_StructField* field = ctx->head->field;
-    __Pyx_StructField* parent = (ctx->head - 1)->field;
-    PyErr_Format(PyExc_ValueError,
-                 "Buffer dtype mismatch, expected '%s' but got %s in '%s.%s'",
-                 field->type->name, __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex),
-                 parent->type->name, field->name);
-  }
-}
-static int __Pyx_BufFmt_ProcessTypeChunk(__Pyx_BufFmt_Context* ctx) {
-  char group;
-  size_t size, offset, arraysize = 1;
-  if (ctx->enc_type == 0) return 0;
-  if (ctx->head->field->type->arraysize[0]) {
-    int i, ndim = 0;
-    if (ctx->enc_type == 's' || ctx->enc_type == 'p') {
-        ctx->is_valid_array = ctx->head->field->type->ndim == 1;
-        ndim = 1;
-        if (ctx->enc_count != ctx->head->field->type->arraysize[0]) {
-            PyErr_Format(PyExc_ValueError,
-                         "Expected a dimension of size %zu, got %zu",
-                         ctx->head->field->type->arraysize[0], ctx->enc_count);
-            return -1;
-        }
-    }
-    if (!ctx->is_valid_array) {
-      PyErr_Format(PyExc_ValueError, "Expected %d dimensions, got %d",
-                   ctx->head->field->type->ndim, ndim);
-      return -1;
-    }
-    for (i = 0; i < ctx->head->field->type->ndim; i++) {
-      arraysize *= ctx->head->field->type->arraysize[i];
-    }
-    ctx->is_valid_array = 0;
-    ctx->enc_count = 1;
-  }
-  group = __Pyx_BufFmt_TypeCharToGroup(ctx->enc_type, ctx->is_complex);
-  do {
-    __Pyx_StructField* field = ctx->head->field;
-    __Pyx_TypeInfo* type = field->type;
-    if (ctx->enc_packmode == '@' || ctx->enc_packmode == '^') {
-      size = __Pyx_BufFmt_TypeCharToNativeSize(ctx->enc_type, ctx->is_complex);
-    } else {
-      size = __Pyx_BufFmt_TypeCharToStandardSize(ctx->enc_type, ctx->is_complex);
-    }
-    if (ctx->enc_packmode == '@') {
-      size_t align_at = __Pyx_BufFmt_TypeCharToAlignment(ctx->enc_type, ctx->is_complex);
-      size_t align_mod_offset;
-      if (align_at == 0) return -1;
-      align_mod_offset = ctx->fmt_offset % align_at;
-      if (align_mod_offset > 0) ctx->fmt_offset += align_at - align_mod_offset;
-      if (ctx->struct_alignment == 0)
-          ctx->struct_alignment = __Pyx_BufFmt_TypeCharToPadding(ctx->enc_type,
-                                                                 ctx->is_complex);
-    }
-    if (type->size != size || type->typegroup != group) {
-      if (type->typegroup == 'C' && type->fields != NULL) {
-        size_t parent_offset = ctx->head->parent_offset + field->offset;
-        ++ctx->head;
-        ctx->head->field = type->fields;
-        ctx->head->parent_offset = parent_offset;
-        continue;
-      }
-      if ((type->typegroup == 'H' || group == 'H') && type->size == size) {
-      } else {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return -1;
-      }
-    }
-    offset = ctx->head->parent_offset + field->offset;
-    if (ctx->fmt_offset != offset) {
-      PyErr_Format(PyExc_ValueError,
-                   "Buffer dtype mismatch; next field is at offset %" CYTHON_FORMAT_SSIZE_T "d but %" CYTHON_FORMAT_SSIZE_T "d expected",
-                   (Py_ssize_t)ctx->fmt_offset, (Py_ssize_t)offset);
-      return -1;
-    }
-    ctx->fmt_offset += size;
-    if (arraysize)
-      ctx->fmt_offset += (arraysize - 1) * size;
-    --ctx->enc_count;
-    while (1) {
-      if (field == &ctx->root) {
-        ctx->head = NULL;
-        if (ctx->enc_count != 0) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return -1;
-        }
-        break;
-      }
-      ctx->head->field = ++field;
-      if (field->type == NULL) {
-        --ctx->head;
-        field = ctx->head->field;
-        continue;
-      } else if (field->type->typegroup == 'S') {
-        size_t parent_offset = ctx->head->parent_offset + field->offset;
-        if (field->type->fields->type == NULL) continue;
-        field = field->type->fields;
-        ++ctx->head;
-        ctx->head->field = field;
-        ctx->head->parent_offset = parent_offset;
-        break;
-      } else {
-        break;
-      }
-    }
-  } while (ctx->enc_count);
-  ctx->enc_type = 0;
-  ctx->is_complex = 0;
-  return 0;
-}
-static PyObject *
-__pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
-{
-    const char *ts = *tsp;
-    int i = 0, number, ndim;
-    ++ts;
-    if (ctx->new_count != 1) {
-        PyErr_SetString(PyExc_ValueError,
-                        "Cannot handle repeated arrays in format string");
-        return NULL;
-    }
-    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-    ndim = ctx->head->field->type->ndim;
-    while (*ts && *ts != ')') {
-        switch (*ts) {
-            case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
-            default:  break;
-        }
-        number = __Pyx_BufFmt_ExpectNumber(&ts);
-        if (number == -1) return NULL;
-        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
-            return PyErr_Format(PyExc_ValueError,
-                        "Expected a dimension of size %zu, got %d",
-                        ctx->head->field->type->arraysize[i], number);
-        if (*ts != ',' && *ts != ')')
-            return PyErr_Format(PyExc_ValueError,
-                                "Expected a comma in format string, got '%c'", *ts);
-        if (*ts == ',') ts++;
-        i++;
-    }
-    if (i != ndim)
-        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
-                            ctx->head->field->type->ndim, i);
-    if (!*ts) {
-        PyErr_SetString(PyExc_ValueError,
-                        "Unexpected end of format string, expected ')'");
-        return NULL;
-    }
-    ctx->is_valid_array = 1;
-    ctx->new_count = 1;
-    *tsp = ++ts;
-    return Py_None;
-}
-static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
-  int got_Z = 0;
-  while (1) {
-    switch(*ts) {
-      case 0:
-        if (ctx->enc_type != 0 && ctx->head == NULL) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return NULL;
-        }
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        if (ctx->head != NULL) {
-          __Pyx_BufFmt_RaiseExpected(ctx);
-          return NULL;
-        }
-        return ts;
-      case ' ':
-      case '\r':
-      case '\n':
-        ++ts;
-        break;
-      case '<':
-        if (!__Pyx_Is_Little_Endian()) {
-          PyErr_SetString(PyExc_ValueError, "Little-endian buffer not supported on big-endian compiler");
-          return NULL;
-        }
-        ctx->new_packmode = '=';
-        ++ts;
-        break;
-      case '>':
-      case '!':
-        if (__Pyx_Is_Little_Endian()) {
-          PyErr_SetString(PyExc_ValueError, "Big-endian buffer not supported on little-endian compiler");
-          return NULL;
-        }
-        ctx->new_packmode = '=';
-        ++ts;
-        break;
-      case '=':
-      case '@':
-      case '^':
-        ctx->new_packmode = *ts++;
-        break;
-      case 'T':
-        {
-          const char* ts_after_sub;
-          size_t i, struct_count = ctx->new_count;
-          size_t struct_alignment = ctx->struct_alignment;
-          ctx->new_count = 1;
-          ++ts;
-          if (*ts != '{') {
-            PyErr_SetString(PyExc_ValueError, "Buffer acquisition: Expected '{' after 'T'");
-            return NULL;
-          }
-          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-          ctx->enc_type = 0;
-          ctx->enc_count = 0;
-          ctx->struct_alignment = 0;
-          ++ts;
-          ts_after_sub = ts;
-          for (i = 0; i != struct_count; ++i) {
-            ts_after_sub = __Pyx_BufFmt_CheckString(ctx, ts);
-            if (!ts_after_sub) return NULL;
-          }
-          ts = ts_after_sub;
-          if (struct_alignment) ctx->struct_alignment = struct_alignment;
-        }
-        break;
-      case '}':
-        {
-          size_t alignment = ctx->struct_alignment;
-          ++ts;
-          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-          ctx->enc_type = 0;
-          if (alignment && ctx->fmt_offset % alignment) {
-            ctx->fmt_offset += alignment - (ctx->fmt_offset % alignment);
-          }
-        }
-        return ts;
-      case 'x':
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        ctx->fmt_offset += ctx->new_count;
-        ctx->new_count = 1;
-        ctx->enc_count = 0;
-        ctx->enc_type = 0;
-        ctx->enc_packmode = ctx->new_packmode;
-        ++ts;
-        break;
-      case 'Z':
-        got_Z = 1;
-        ++ts;
-        if (*ts != 'f' && *ts != 'd' && *ts != 'g') {
-          __Pyx_BufFmt_RaiseUnexpectedChar('Z');
-          return NULL;
-        }
-        CYTHON_FALLTHROUGH;
-      case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
-      case 'l': case 'L': case 'q': case 'Q':
-      case 'f': case 'd': case 'g':
-      case 'O': case 'p':
-        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
-            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
-          ctx->enc_count += ctx->new_count;
-          ctx->new_count = 1;
-          got_Z = 0;
-          ++ts;
-          break;
-        }
-        CYTHON_FALLTHROUGH;
-      case 's':
-        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-        ctx->enc_count = ctx->new_count;
-        ctx->enc_packmode = ctx->new_packmode;
-        ctx->enc_type = *ts;
-        ctx->is_complex = got_Z;
-        ++ts;
-        ctx->new_count = 1;
-        got_Z = 0;
-        break;
-      case ':':
-        ++ts;
-        while(*ts != ':') ++ts;
-        ++ts;
-        break;
-      case '(':
-        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
-        break;
-      default:
-        {
-          int number = __Pyx_BufFmt_ExpectNumber(&ts);
-          if (number == -1) return NULL;
-          ctx->new_count = (size_t)number;
-        }
-    }
-  }
-}
-
-/* TypeInfoCompare */
-  static int
-__pyx_typeinfo_cmp(__Pyx_TypeInfo *a, __Pyx_TypeInfo *b)
-{
-    int i;
-    if (!a || !b)
-        return 0;
-    if (a == b)
-        return 1;
-    if (a->size != b->size || a->typegroup != b->typegroup ||
-            a->is_unsigned != b->is_unsigned || a->ndim != b->ndim) {
-        if (a->typegroup == 'H' || b->typegroup == 'H') {
-            return a->size == b->size;
-        } else {
-            return 0;
-        }
-    }
-    if (a->ndim) {
-        for (i = 0; i < a->ndim; i++)
-            if (a->arraysize[i] != b->arraysize[i])
-                return 0;
-    }
-    if (a->typegroup == 'S') {
-        if (a->flags != b->flags)
-            return 0;
-        if (a->fields || b->fields) {
-            if (!(a->fields && b->fields))
-                return 0;
-            for (i = 0; a->fields[i].type && b->fields[i].type; i++) {
-                __Pyx_StructField *field_a = a->fields + i;
-                __Pyx_StructField *field_b = b->fields + i;
-                if (field_a->offset != field_b->offset ||
-                    !__pyx_typeinfo_cmp(field_a->type, field_b->type))
-                    return 0;
-            }
-            return !a->fields[i].type && !b->fields[i].type;
-        }
-    }
-    return 1;
-}
-
-/* MemviewSliceValidateAndInit */
-  static int
-__pyx_check_strides(Py_buffer *buf, int dim, int ndim, int spec)
-{
-    if (buf->shape[dim] <= 1)
-        return 1;
-    if (buf->strides) {
-        if (spec & __Pyx_MEMVIEW_CONTIG) {
-            if (spec & (__Pyx_MEMVIEW_PTR|__Pyx_MEMVIEW_FULL)) {
-                if (unlikely(buf->strides[dim] != sizeof(void *))) {
-                    PyErr_Format(PyExc_ValueError,
-                                 "Buffer is not indirectly contiguous "
-                                 "in dimension %d.", dim);
-                    goto fail;
-                }
-            } else if (unlikely(buf->strides[dim] != buf->itemsize)) {
-                PyErr_SetString(PyExc_ValueError,
-                                "Buffer and memoryview are not contiguous "
-                                "in the same dimension.");
-                goto fail;
-            }
-        }
-        if (spec & __Pyx_MEMVIEW_FOLLOW) {
-            Py_ssize_t stride = buf->strides[dim];
-            if (stride < 0)
-                stride = -stride;
-            if (unlikely(stride < buf->itemsize)) {
-                PyErr_SetString(PyExc_ValueError,
-                                "Buffer and memoryview are not contiguous "
-                                "in the same dimension.");
-                goto fail;
-            }
-        }
-    } else {
-        if (unlikely(spec & __Pyx_MEMVIEW_CONTIG && dim != ndim - 1)) {
-            PyErr_Format(PyExc_ValueError,
-                         "C-contiguous buffer is not contiguous in "
-                         "dimension %d", dim);
-            goto fail;
-        } else if (unlikely(spec & (__Pyx_MEMVIEW_PTR))) {
-            PyErr_Format(PyExc_ValueError,
-                         "C-contiguous buffer is not indirect in "
-                         "dimension %d", dim);
-            goto fail;
-        } else if (unlikely(buf->suboffsets)) {
-            PyErr_SetString(PyExc_ValueError,
-                            "Buffer exposes suboffsets but no strides");
-            goto fail;
-        }
-    }
-    return 1;
-fail:
-    return 0;
-}
-static int
-__pyx_check_suboffsets(Py_buffer *buf, int dim, CYTHON_UNUSED int ndim, int spec)
-{
-    if (spec & __Pyx_MEMVIEW_DIRECT) {
-        if (unlikely(buf->suboffsets && buf->suboffsets[dim] >= 0)) {
-            PyErr_Format(PyExc_ValueError,
-                         "Buffer not compatible with direct access "
-                         "in dimension %d.", dim);
-            goto fail;
-        }
-    }
-    if (spec & __Pyx_MEMVIEW_PTR) {
-        if (unlikely(!buf->suboffsets || (buf->suboffsets[dim] < 0))) {
-            PyErr_Format(PyExc_ValueError,
-                         "Buffer is not indirectly accessible "
-                         "in dimension %d.", dim);
-            goto fail;
-        }
-    }
-    return 1;
-fail:
-    return 0;
-}
-static int
-__pyx_verify_contig(Py_buffer *buf, int ndim, int c_or_f_flag)
-{
-    int i;
-    if (c_or_f_flag & __Pyx_IS_F_CONTIG) {
-        Py_ssize_t stride = 1;
-        for (i = 0; i < ndim; i++) {
-            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
-                PyErr_SetString(PyExc_ValueError,
-                    "Buffer not fortran contiguous.");
-                goto fail;
-            }
-            stride = stride * buf->shape[i];
-        }
-    } else if (c_or_f_flag & __Pyx_IS_C_CONTIG) {
-        Py_ssize_t stride = 1;
-        for (i = ndim - 1; i >- 1; i--) {
-            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
-                PyErr_SetString(PyExc_ValueError,
-                    "Buffer not C contiguous.");
-                goto fail;
-            }
-            stride = stride * buf->shape[i];
-        }
-    }
-    return 1;
-fail:
-    return 0;
-}
-static int __Pyx_ValidateAndInit_memviewslice(
-                int *axes_specs,
-                int c_or_f_flag,
-                int buf_flags,
-                int ndim,
-                __Pyx_TypeInfo *dtype,
-                __Pyx_BufFmt_StackElem stack[],
-                __Pyx_memviewslice *memviewslice,
-                PyObject *original_obj)
-{
-    struct __pyx_memoryview_obj *memview, *new_memview;
-    __Pyx_RefNannyDeclarations
-    Py_buffer *buf;
-    int i, spec = 0, retval = -1;
-    __Pyx_BufFmt_Context ctx;
-    int from_memoryview = __pyx_memoryview_check(original_obj);
-    __Pyx_RefNannySetupContext("ValidateAndInit_memviewslice", 0);
-    if (from_memoryview && __pyx_typeinfo_cmp(dtype, ((struct __pyx_memoryview_obj *)
-                                                            original_obj)->typeinfo)) {
-        memview = (struct __pyx_memoryview_obj *) original_obj;
-        new_memview = NULL;
-    } else {
-        memview = (struct __pyx_memoryview_obj *) __pyx_memoryview_new(
-                                            original_obj, buf_flags, 0, dtype);
-        new_memview = memview;
-        if (unlikely(!memview))
-            goto fail;
-    }
-    buf = &memview->view;
-    if (unlikely(buf->ndim != ndim)) {
-        PyErr_Format(PyExc_ValueError,
-                "Buffer has wrong number of dimensions (expected %d, got %d)",
-                ndim, buf->ndim);
-        goto fail;
-    }
-    if (new_memview) {
-        __Pyx_BufFmt_Init(&ctx, stack, dtype);
-        if (unlikely(!__Pyx_BufFmt_CheckString(&ctx, buf->format))) goto fail;
-    }
-    if (unlikely((unsigned) buf->itemsize != dtype->size)) {
-        PyErr_Format(PyExc_ValueError,
-                     "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "u byte%s) "
-                     "does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "u byte%s)",
-                     buf->itemsize,
-                     (buf->itemsize > 1) ? "s" : "",
-                     dtype->name,
-                     dtype->size,
-                     (dtype->size > 1) ? "s" : "");
-        goto fail;
-    }
-    if (buf->len > 0) {
-        for (i = 0; i < ndim; i++) {
-            spec = axes_specs[i];
-            if (unlikely(!__pyx_check_strides(buf, i, ndim, spec)))
-                goto fail;
-            if (unlikely(!__pyx_check_suboffsets(buf, i, ndim, spec)))
-                goto fail;
-        }
-        if (unlikely(buf->strides && !__pyx_verify_contig(buf, ndim, c_or_f_flag)))
-            goto fail;
-    }
-    if (unlikely(__Pyx_init_memviewslice(memview, ndim, memviewslice,
-                                         new_memview != NULL) == -1)) {
-        goto fail;
-    }
-    retval = 0;
-    goto no_fail;
-fail:
-    Py_XDECREF(new_memview);
-    retval = -1;
-no_fail:
-    __Pyx_RefNannyFinishContext();
-    return retval;
-}
-
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_int(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
-    }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
-                                                 PyBUF_RECORDS_RO | writable_flag, 2,
-                                                 &__Pyx_TypeInfo_int, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
-}
-
 /* CIntFromPyVerify */
-  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+#define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
     {\
         func_type value = func_value;\
         if (sizeof(target_type) < sizeof(func_type)) {\
@@ -22182,15 +21194,15 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return x + y*(__pyx_t_float_complex)_Complex_I;
@@ -22202,15 +21214,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX
 #else
     static CYTHON_INLINE int __Pyx_c_eq_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_float_complex __Pyx_c_sum_float(__pyx_t_float_complex a, __pyx_t_float_complex b) {
         __pyx_t_float_complex z;
         z.real = a.real + b.real;
@@ -22336,15 +21348,15 @@
             z.imag = z_r * sinf(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* Declarations */
-  #if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return ::std::complex< double >(x, y);
     }
   #else
     static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double x, double y) {
       return x + y*(__pyx_t_double_complex)_Complex_I;
@@ -22356,15 +21368,15 @@
       z.real = x;
       z.imag = y;
       return z;
     }
 #endif
 
 /* Arithmetic */
-  #if CYTHON_CCOMPLEX
+#if CYTHON_CCOMPLEX
 #else
     static CYTHON_INLINE int __Pyx_c_eq_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
        return (a.real == b.real) && (a.imag == b.imag);
     }
     static CYTHON_INLINE __pyx_t_double_complex __Pyx_c_sum_double(__pyx_t_double_complex a, __pyx_t_double_complex b) {
         __pyx_t_double_complex z;
         z.real = a.real + b.real;
@@ -22490,15 +21502,15 @@
             z.imag = z_r * sin(z_theta);
             return z;
         }
     #endif
 #endif
 
 /* MemviewSliceCopyTemplate */
-  static __Pyx_memviewslice
+static __Pyx_memviewslice
 __pyx_memoryview_copy_new_contig(const __Pyx_memviewslice *from_mvs,
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object)
 {
     __Pyx_RefNannyDeclarations
     int i;
@@ -22557,15 +21569,15 @@
     __Pyx_XDECREF(temp_int);
     __Pyx_XDECREF(array_obj);
     __Pyx_RefNannyFinishContext();
     return new_mvs;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -22595,15 +21607,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
+static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -22791,15 +21803,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -22829,15 +21841,15 @@
         unsigned char *bytes = (unsigned char *)&value;
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
+static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -23025,15 +22037,15 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntFromPy */
-  static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
+static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const char neg_one = (char) -1, const_zero = (char) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic pop
@@ -23220,43 +22232,779 @@
     return (char) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to char");
     return (char) -1;
 }
 
-/* CheckBinaryVersion */
-  static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
+/* IsLittleEndian */
+static CYTHON_INLINE int __Pyx_Is_Little_Endian(void)
+{
+  union {
+    uint32_t u32;
+    uint8_t u8[4];
+  } S;
+  S.u32 = 0x01020304;
+  return S.u8[0] == 4;
+}
+
+/* BufferFormatCheck */
+static void __Pyx_BufFmt_Init(__Pyx_BufFmt_Context* ctx,
+                              __Pyx_BufFmt_StackElem* stack,
+                              __Pyx_TypeInfo* type) {
+  stack[0].field = &ctx->root;
+  stack[0].parent_offset = 0;
+  ctx->root.type = type;
+  ctx->root.name = "buffer dtype";
+  ctx->root.offset = 0;
+  ctx->head = stack;
+  ctx->head->field = &ctx->root;
+  ctx->fmt_offset = 0;
+  ctx->head->parent_offset = 0;
+  ctx->new_packmode = '@';
+  ctx->enc_packmode = '@';
+  ctx->new_count = 1;
+  ctx->enc_count = 0;
+  ctx->enc_type = 0;
+  ctx->is_complex = 0;
+  ctx->is_valid_array = 0;
+  ctx->struct_alignment = 0;
+  while (type->typegroup == 'S') {
+    ++ctx->head;
+    ctx->head->field = type->fields;
+    ctx->head->parent_offset = 0;
+    type = type->fields->type;
+  }
+}
+static int __Pyx_BufFmt_ParseNumber(const char** ts) {
+    int count;
+    const char* t = *ts;
+    if (*t < '0' || *t > '9') {
+      return -1;
+    } else {
+        count = *t++ - '0';
+        while (*t >= '0' && *t <= '9') {
+            count *= 10;
+            count += *t++ - '0';
         }
     }
-    if (!same) {
-        char rtversion[5] = {'\0'};
-        char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
+    *ts = t;
+    return count;
+}
+static int __Pyx_BufFmt_ExpectNumber(const char **ts) {
+    int number = __Pyx_BufFmt_ParseNumber(ts);
+    if (number == -1)
+        PyErr_Format(PyExc_ValueError,\
+                     "Does not understand character buffer dtype format string ('%c')", **ts);
+    return number;
+}
+static void __Pyx_BufFmt_RaiseUnexpectedChar(char ch) {
+  PyErr_Format(PyExc_ValueError,
+               "Unexpected format string character: '%c'", ch);
+}
+static const char* __Pyx_BufFmt_DescribeTypeChar(char ch, int is_complex) {
+  switch (ch) {
+    case '?': return "'bool'";
+    case 'c': return "'char'";
+    case 'b': return "'signed char'";
+    case 'B': return "'unsigned char'";
+    case 'h': return "'short'";
+    case 'H': return "'unsigned short'";
+    case 'i': return "'int'";
+    case 'I': return "'unsigned int'";
+    case 'l': return "'long'";
+    case 'L': return "'unsigned long'";
+    case 'q': return "'long long'";
+    case 'Q': return "'unsigned long long'";
+    case 'f': return (is_complex ? "'complex float'" : "'float'");
+    case 'd': return (is_complex ? "'complex double'" : "'double'");
+    case 'g': return (is_complex ? "'complex long double'" : "'long double'");
+    case 'T': return "a struct";
+    case 'O': return "Python object";
+    case 'P': return "a pointer";
+    case 's': case 'p': return "a string";
+    case 0: return "end";
+    default: return "unparseable format string";
+  }
+}
+static size_t __Pyx_BufFmt_TypeCharToStandardSize(char ch, int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return 2;
+    case 'i': case 'I': case 'l': case 'L': return 4;
+    case 'q': case 'Q': return 8;
+    case 'f': return (is_complex ? 8 : 4);
+    case 'd': return (is_complex ? 16 : 8);
+    case 'g': {
+      PyErr_SetString(PyExc_ValueError, "Python does not define a standard format string size for long double ('g')..");
+      return 0;
+    }
+    case 'O': case 'P': return sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+}
+static size_t __Pyx_BufFmt_TypeCharToNativeSize(char ch, int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(short);
+    case 'i': case 'I': return sizeof(int);
+    case 'l': case 'L': return sizeof(long);
+    #ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(PY_LONG_LONG);
+    #endif
+    case 'f': return sizeof(float) * (is_complex ? 2 : 1);
+    case 'd': return sizeof(double) * (is_complex ? 2 : 1);
+    case 'g': return sizeof(long double) * (is_complex ? 2 : 1);
+    case 'O': case 'P': return sizeof(void*);
+    default: {
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+  }
+}
+typedef struct { char c; short x; } __Pyx_st_short;
+typedef struct { char c; int x; } __Pyx_st_int;
+typedef struct { char c; long x; } __Pyx_st_long;
+typedef struct { char c; float x; } __Pyx_st_float;
+typedef struct { char c; double x; } __Pyx_st_double;
+typedef struct { char c; long double x; } __Pyx_st_longdouble;
+typedef struct { char c; void *x; } __Pyx_st_void_p;
+#ifdef HAVE_LONG_LONG
+typedef struct { char c; PY_LONG_LONG x; } __Pyx_st_longlong;
+#endif
+static size_t __Pyx_BufFmt_TypeCharToAlignment(char ch, CYTHON_UNUSED int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(__Pyx_st_short) - sizeof(short);
+    case 'i': case 'I': return sizeof(__Pyx_st_int) - sizeof(int);
+    case 'l': case 'L': return sizeof(__Pyx_st_long) - sizeof(long);
+#ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(__Pyx_st_longlong) - sizeof(PY_LONG_LONG);
+#endif
+    case 'f': return sizeof(__Pyx_st_float) - sizeof(float);
+    case 'd': return sizeof(__Pyx_st_double) - sizeof(double);
+    case 'g': return sizeof(__Pyx_st_longdouble) - sizeof(long double);
+    case 'P': case 'O': return sizeof(__Pyx_st_void_p) - sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+}
+/* These are for computing the padding at the end of the struct to align
+   on the first member of the struct. This will probably the same as above,
+   but we don't have any guarantees.
+ */
+typedef struct { short x; char c; } __Pyx_pad_short;
+typedef struct { int x; char c; } __Pyx_pad_int;
+typedef struct { long x; char c; } __Pyx_pad_long;
+typedef struct { float x; char c; } __Pyx_pad_float;
+typedef struct { double x; char c; } __Pyx_pad_double;
+typedef struct { long double x; char c; } __Pyx_pad_longdouble;
+typedef struct { void *x; char c; } __Pyx_pad_void_p;
+#ifdef HAVE_LONG_LONG
+typedef struct { PY_LONG_LONG x; char c; } __Pyx_pad_longlong;
+#endif
+static size_t __Pyx_BufFmt_TypeCharToPadding(char ch, CYTHON_UNUSED int is_complex) {
+  switch (ch) {
+    case '?': case 'c': case 'b': case 'B': case 's': case 'p': return 1;
+    case 'h': case 'H': return sizeof(__Pyx_pad_short) - sizeof(short);
+    case 'i': case 'I': return sizeof(__Pyx_pad_int) - sizeof(int);
+    case 'l': case 'L': return sizeof(__Pyx_pad_long) - sizeof(long);
+#ifdef HAVE_LONG_LONG
+    case 'q': case 'Q': return sizeof(__Pyx_pad_longlong) - sizeof(PY_LONG_LONG);
+#endif
+    case 'f': return sizeof(__Pyx_pad_float) - sizeof(float);
+    case 'd': return sizeof(__Pyx_pad_double) - sizeof(double);
+    case 'g': return sizeof(__Pyx_pad_longdouble) - sizeof(long double);
+    case 'P': case 'O': return sizeof(__Pyx_pad_void_p) - sizeof(void*);
+    default:
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+}
+static char __Pyx_BufFmt_TypeCharToGroup(char ch, int is_complex) {
+  switch (ch) {
+    case 'c':
+        return 'H';
+    case 'b': case 'h': case 'i':
+    case 'l': case 'q': case 's': case 'p':
+        return 'I';
+    case '?': case 'B': case 'H': case 'I': case 'L': case 'Q':
+        return 'U';
+    case 'f': case 'd': case 'g':
+        return (is_complex ? 'C' : 'R');
+    case 'O':
+        return 'O';
+    case 'P':
+        return 'P';
+    default: {
+      __Pyx_BufFmt_RaiseUnexpectedChar(ch);
+      return 0;
+    }
+  }
+}
+static void __Pyx_BufFmt_RaiseExpected(__Pyx_BufFmt_Context* ctx) {
+  if (ctx->head == NULL || ctx->head->field == &ctx->root) {
+    const char* expected;
+    const char* quote;
+    if (ctx->head == NULL) {
+      expected = "end";
+      quote = "";
+    } else {
+      expected = ctx->head->field->type->name;
+      quote = "'";
+    }
+    PyErr_Format(PyExc_ValueError,
+                 "Buffer dtype mismatch, expected %s%s%s but got %s",
+                 quote, expected, quote,
+                 __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex));
+  } else {
+    __Pyx_StructField* field = ctx->head->field;
+    __Pyx_StructField* parent = (ctx->head - 1)->field;
+    PyErr_Format(PyExc_ValueError,
+                 "Buffer dtype mismatch, expected '%s' but got %s in '%s.%s'",
+                 field->type->name, __Pyx_BufFmt_DescribeTypeChar(ctx->enc_type, ctx->is_complex),
+                 parent->type->name, field->name);
+  }
+}
+static int __Pyx_BufFmt_ProcessTypeChunk(__Pyx_BufFmt_Context* ctx) {
+  char group;
+  size_t size, offset, arraysize = 1;
+  if (ctx->enc_type == 0) return 0;
+  if (ctx->head->field->type->arraysize[0]) {
+    int i, ndim = 0;
+    if (ctx->enc_type == 's' || ctx->enc_type == 'p') {
+        ctx->is_valid_array = ctx->head->field->type->ndim == 1;
+        ndim = 1;
+        if (ctx->enc_count != ctx->head->field->type->arraysize[0]) {
+            PyErr_Format(PyExc_ValueError,
+                         "Expected a dimension of size %zu, got %zu",
+                         ctx->head->field->type->arraysize[0], ctx->enc_count);
+            return -1;
+        }
+    }
+    if (!ctx->is_valid_array) {
+      PyErr_Format(PyExc_ValueError, "Expected %d dimensions, got %d",
+                   ctx->head->field->type->ndim, ndim);
+      return -1;
+    }
+    for (i = 0; i < ctx->head->field->type->ndim; i++) {
+      arraysize *= ctx->head->field->type->arraysize[i];
+    }
+    ctx->is_valid_array = 0;
+    ctx->enc_count = 1;
+  }
+  group = __Pyx_BufFmt_TypeCharToGroup(ctx->enc_type, ctx->is_complex);
+  do {
+    __Pyx_StructField* field = ctx->head->field;
+    __Pyx_TypeInfo* type = field->type;
+    if (ctx->enc_packmode == '@' || ctx->enc_packmode == '^') {
+      size = __Pyx_BufFmt_TypeCharToNativeSize(ctx->enc_type, ctx->is_complex);
+    } else {
+      size = __Pyx_BufFmt_TypeCharToStandardSize(ctx->enc_type, ctx->is_complex);
+    }
+    if (ctx->enc_packmode == '@') {
+      size_t align_at = __Pyx_BufFmt_TypeCharToAlignment(ctx->enc_type, ctx->is_complex);
+      size_t align_mod_offset;
+      if (align_at == 0) return -1;
+      align_mod_offset = ctx->fmt_offset % align_at;
+      if (align_mod_offset > 0) ctx->fmt_offset += align_at - align_mod_offset;
+      if (ctx->struct_alignment == 0)
+          ctx->struct_alignment = __Pyx_BufFmt_TypeCharToPadding(ctx->enc_type,
+                                                                 ctx->is_complex);
+    }
+    if (type->size != size || type->typegroup != group) {
+      if (type->typegroup == 'C' && type->fields != NULL) {
+        size_t parent_offset = ctx->head->parent_offset + field->offset;
+        ++ctx->head;
+        ctx->head->field = type->fields;
+        ctx->head->parent_offset = parent_offset;
+        continue;
+      }
+      if ((type->typegroup == 'H' || group == 'H') && type->size == size) {
+      } else {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return -1;
+      }
+    }
+    offset = ctx->head->parent_offset + field->offset;
+    if (ctx->fmt_offset != offset) {
+      PyErr_Format(PyExc_ValueError,
+                   "Buffer dtype mismatch; next field is at offset %" CYTHON_FORMAT_SSIZE_T "d but %" CYTHON_FORMAT_SSIZE_T "d expected",
+                   (Py_ssize_t)ctx->fmt_offset, (Py_ssize_t)offset);
+      return -1;
+    }
+    ctx->fmt_offset += size;
+    if (arraysize)
+      ctx->fmt_offset += (arraysize - 1) * size;
+    --ctx->enc_count;
+    while (1) {
+      if (field == &ctx->root) {
+        ctx->head = NULL;
+        if (ctx->enc_count != 0) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return -1;
+        }
+        break;
+      }
+      ctx->head->field = ++field;
+      if (field->type == NULL) {
+        --ctx->head;
+        field = ctx->head->field;
+        continue;
+      } else if (field->type->typegroup == 'S') {
+        size_t parent_offset = ctx->head->parent_offset + field->offset;
+        if (field->type->fields->type == NULL) continue;
+        field = field->type->fields;
+        ++ctx->head;
+        ctx->head->field = field;
+        ctx->head->parent_offset = parent_offset;
+        break;
+      } else {
+        break;
+      }
+    }
+  } while (ctx->enc_count);
+  ctx->enc_type = 0;
+  ctx->is_complex = 0;
+  return 0;
+}
+static PyObject *
+__pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
+{
+    const char *ts = *tsp;
+    int i = 0, number, ndim;
+    ++ts;
+    if (ctx->new_count != 1) {
+        PyErr_SetString(PyExc_ValueError,
+                        "Cannot handle repeated arrays in format string");
+        return NULL;
+    }
+    if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+    ndim = ctx->head->field->type->ndim;
+    while (*ts && *ts != ')') {
+        switch (*ts) {
+            case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
+            default:  break;
+        }
+        number = __Pyx_BufFmt_ExpectNumber(&ts);
+        if (number == -1) return NULL;
+        if (i < ndim && (size_t) number != ctx->head->field->type->arraysize[i])
+            return PyErr_Format(PyExc_ValueError,
+                        "Expected a dimension of size %zu, got %d",
+                        ctx->head->field->type->arraysize[i], number);
+        if (*ts != ',' && *ts != ')')
+            return PyErr_Format(PyExc_ValueError,
+                                "Expected a comma in format string, got '%c'", *ts);
+        if (*ts == ',') ts++;
+        i++;
+    }
+    if (i != ndim)
+        return PyErr_Format(PyExc_ValueError, "Expected %d dimension(s), got %d",
+                            ctx->head->field->type->ndim, i);
+    if (!*ts) {
+        PyErr_SetString(PyExc_ValueError,
+                        "Unexpected end of format string, expected ')'");
+        return NULL;
+    }
+    ctx->is_valid_array = 1;
+    ctx->new_count = 1;
+    *tsp = ++ts;
+    return Py_None;
+}
+static const char* __Pyx_BufFmt_CheckString(__Pyx_BufFmt_Context* ctx, const char* ts) {
+  int got_Z = 0;
+  while (1) {
+    switch(*ts) {
+      case 0:
+        if (ctx->enc_type != 0 && ctx->head == NULL) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return NULL;
+        }
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        if (ctx->head != NULL) {
+          __Pyx_BufFmt_RaiseExpected(ctx);
+          return NULL;
+        }
+        return ts;
+      case ' ':
+      case '\r':
+      case '\n':
+        ++ts;
+        break;
+      case '<':
+        if (!__Pyx_Is_Little_Endian()) {
+          PyErr_SetString(PyExc_ValueError, "Little-endian buffer not supported on big-endian compiler");
+          return NULL;
+        }
+        ctx->new_packmode = '=';
+        ++ts;
+        break;
+      case '>':
+      case '!':
+        if (__Pyx_Is_Little_Endian()) {
+          PyErr_SetString(PyExc_ValueError, "Big-endian buffer not supported on little-endian compiler");
+          return NULL;
+        }
+        ctx->new_packmode = '=';
+        ++ts;
+        break;
+      case '=':
+      case '@':
+      case '^':
+        ctx->new_packmode = *ts++;
+        break;
+      case 'T':
+        {
+          const char* ts_after_sub;
+          size_t i, struct_count = ctx->new_count;
+          size_t struct_alignment = ctx->struct_alignment;
+          ctx->new_count = 1;
+          ++ts;
+          if (*ts != '{') {
+            PyErr_SetString(PyExc_ValueError, "Buffer acquisition: Expected '{' after 'T'");
+            return NULL;
+          }
+          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+          ctx->enc_type = 0;
+          ctx->enc_count = 0;
+          ctx->struct_alignment = 0;
+          ++ts;
+          ts_after_sub = ts;
+          for (i = 0; i != struct_count; ++i) {
+            ts_after_sub = __Pyx_BufFmt_CheckString(ctx, ts);
+            if (!ts_after_sub) return NULL;
+          }
+          ts = ts_after_sub;
+          if (struct_alignment) ctx->struct_alignment = struct_alignment;
+        }
+        break;
+      case '}':
+        {
+          size_t alignment = ctx->struct_alignment;
+          ++ts;
+          if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+          ctx->enc_type = 0;
+          if (alignment && ctx->fmt_offset % alignment) {
+            ctx->fmt_offset += alignment - (ctx->fmt_offset % alignment);
+          }
+        }
+        return ts;
+      case 'x':
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        ctx->fmt_offset += ctx->new_count;
+        ctx->new_count = 1;
+        ctx->enc_count = 0;
+        ctx->enc_type = 0;
+        ctx->enc_packmode = ctx->new_packmode;
+        ++ts;
+        break;
+      case 'Z':
+        got_Z = 1;
+        ++ts;
+        if (*ts != 'f' && *ts != 'd' && *ts != 'g') {
+          __Pyx_BufFmt_RaiseUnexpectedChar('Z');
+          return NULL;
+        }
+        CYTHON_FALLTHROUGH;
+      case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
+      case 'l': case 'L': case 'q': case 'Q':
+      case 'f': case 'd': case 'g':
+      case 'O': case 'p':
+        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
+            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
+          ctx->enc_count += ctx->new_count;
+          ctx->new_count = 1;
+          got_Z = 0;
+          ++ts;
+          break;
+        }
+        CYTHON_FALLTHROUGH;
+      case 's':
+        if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
+        ctx->enc_count = ctx->new_count;
+        ctx->enc_packmode = ctx->new_packmode;
+        ctx->enc_type = *ts;
+        ctx->is_complex = got_Z;
+        ++ts;
+        ctx->new_count = 1;
+        got_Z = 0;
+        break;
+      case ':':
+        ++ts;
+        while(*ts != ':') ++ts;
+        ++ts;
+        break;
+      case '(':
+        if (!__pyx_buffmt_parse_array(ctx, &ts)) return NULL;
+        break;
+      default:
+        {
+          int number = __Pyx_BufFmt_ExpectNumber(&ts);
+          if (number == -1) return NULL;
+          ctx->new_count = (size_t)number;
+        }
+    }
+  }
+}
+
+/* TypeInfoCompare */
+  static int
+__pyx_typeinfo_cmp(__Pyx_TypeInfo *a, __Pyx_TypeInfo *b)
+{
+    int i;
+    if (!a || !b)
+        return 0;
+    if (a == b)
+        return 1;
+    if (a->size != b->size || a->typegroup != b->typegroup ||
+            a->is_unsigned != b->is_unsigned || a->ndim != b->ndim) {
+        if (a->typegroup == 'H' || b->typegroup == 'H') {
+            return a->size == b->size;
+        } else {
+            return 0;
+        }
+    }
+    if (a->ndim) {
+        for (i = 0; i < a->ndim; i++)
+            if (a->arraysize[i] != b->arraysize[i])
+                return 0;
+    }
+    if (a->typegroup == 'S') {
+        if (a->flags != b->flags)
+            return 0;
+        if (a->fields || b->fields) {
+            if (!(a->fields && b->fields))
+                return 0;
+            for (i = 0; a->fields[i].type && b->fields[i].type; i++) {
+                __Pyx_StructField *field_a = a->fields + i;
+                __Pyx_StructField *field_b = b->fields + i;
+                if (field_a->offset != field_b->offset ||
+                    !__pyx_typeinfo_cmp(field_a->type, field_b->type))
+                    return 0;
+            }
+            return !a->fields[i].type && !b->fields[i].type;
+        }
+    }
+    return 1;
+}
+
+/* MemviewSliceValidateAndInit */
+  static int
+__pyx_check_strides(Py_buffer *buf, int dim, int ndim, int spec)
+{
+    if (buf->shape[dim] <= 1)
+        return 1;
+    if (buf->strides) {
+        if (spec & __Pyx_MEMVIEW_CONTIG) {
+            if (spec & (__Pyx_MEMVIEW_PTR|__Pyx_MEMVIEW_FULL)) {
+                if (unlikely(buf->strides[dim] != sizeof(void *))) {
+                    PyErr_Format(PyExc_ValueError,
+                                 "Buffer is not indirectly contiguous "
+                                 "in dimension %d.", dim);
+                    goto fail;
+                }
+            } else if (unlikely(buf->strides[dim] != buf->itemsize)) {
+                PyErr_SetString(PyExc_ValueError,
+                                "Buffer and memoryview are not contiguous "
+                                "in the same dimension.");
+                goto fail;
+            }
+        }
+        if (spec & __Pyx_MEMVIEW_FOLLOW) {
+            Py_ssize_t stride = buf->strides[dim];
+            if (stride < 0)
+                stride = -stride;
+            if (unlikely(stride < buf->itemsize)) {
+                PyErr_SetString(PyExc_ValueError,
+                                "Buffer and memoryview are not contiguous "
+                                "in the same dimension.");
+                goto fail;
             }
-            rtversion[i] = rt_from_call[i];
         }
+    } else {
+        if (unlikely(spec & __Pyx_MEMVIEW_CONTIG && dim != ndim - 1)) {
+            PyErr_Format(PyExc_ValueError,
+                         "C-contiguous buffer is not contiguous in "
+                         "dimension %d", dim);
+            goto fail;
+        } else if (unlikely(spec & (__Pyx_MEMVIEW_PTR))) {
+            PyErr_Format(PyExc_ValueError,
+                         "C-contiguous buffer is not indirect in "
+                         "dimension %d", dim);
+            goto fail;
+        } else if (unlikely(buf->suboffsets)) {
+            PyErr_SetString(PyExc_ValueError,
+                            "Buffer exposes suboffsets but no strides");
+            goto fail;
+        }
+    }
+    return 1;
+fail:
+    return 0;
+}
+static int
+__pyx_check_suboffsets(Py_buffer *buf, int dim, CYTHON_UNUSED int ndim, int spec)
+{
+    if (spec & __Pyx_MEMVIEW_DIRECT) {
+        if (unlikely(buf->suboffsets && buf->suboffsets[dim] >= 0)) {
+            PyErr_Format(PyExc_ValueError,
+                         "Buffer not compatible with direct access "
+                         "in dimension %d.", dim);
+            goto fail;
+        }
+    }
+    if (spec & __Pyx_MEMVIEW_PTR) {
+        if (unlikely(!buf->suboffsets || (buf->suboffsets[dim] < 0))) {
+            PyErr_Format(PyExc_ValueError,
+                         "Buffer is not indirectly accessible "
+                         "in dimension %d.", dim);
+            goto fail;
+        }
+    }
+    return 1;
+fail:
+    return 0;
+}
+static int
+__pyx_verify_contig(Py_buffer *buf, int ndim, int c_or_f_flag)
+{
+    int i;
+    if (c_or_f_flag & __Pyx_IS_F_CONTIG) {
+        Py_ssize_t stride = 1;
+        for (i = 0; i < ndim; i++) {
+            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
+                PyErr_SetString(PyExc_ValueError,
+                    "Buffer not fortran contiguous.");
+                goto fail;
+            }
+            stride = stride * buf->shape[i];
+        }
+    } else if (c_or_f_flag & __Pyx_IS_C_CONTIG) {
+        Py_ssize_t stride = 1;
+        for (i = ndim - 1; i >- 1; i--) {
+            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
+                PyErr_SetString(PyExc_ValueError,
+                    "Buffer not C contiguous.");
+                goto fail;
+            }
+            stride = stride * buf->shape[i];
+        }
+    }
+    return 1;
+fail:
+    return 0;
+}
+static int __Pyx_ValidateAndInit_memviewslice(
+                int *axes_specs,
+                int c_or_f_flag,
+                int buf_flags,
+                int ndim,
+                __Pyx_TypeInfo *dtype,
+                __Pyx_BufFmt_StackElem stack[],
+                __Pyx_memviewslice *memviewslice,
+                PyObject *original_obj)
+{
+    struct __pyx_memoryview_obj *memview, *new_memview;
+    __Pyx_RefNannyDeclarations
+    Py_buffer *buf;
+    int i, spec = 0, retval = -1;
+    __Pyx_BufFmt_Context ctx;
+    int from_memoryview = __pyx_memoryview_check(original_obj);
+    __Pyx_RefNannySetupContext("ValidateAndInit_memviewslice", 0);
+    if (from_memoryview && __pyx_typeinfo_cmp(dtype, ((struct __pyx_memoryview_obj *)
+                                                            original_obj)->typeinfo)) {
+        memview = (struct __pyx_memoryview_obj *) original_obj;
+        new_memview = NULL;
+    } else {
+        memview = (struct __pyx_memoryview_obj *) __pyx_memoryview_new(
+                                            original_obj, buf_flags, 0, dtype);
+        new_memview = memview;
+        if (unlikely(!memview))
+            goto fail;
+    }
+    buf = &memview->view;
+    if (unlikely(buf->ndim != ndim)) {
+        PyErr_Format(PyExc_ValueError,
+                "Buffer has wrong number of dimensions (expected %d, got %d)",
+                ndim, buf->ndim);
+        goto fail;
+    }
+    if (new_memview) {
+        __Pyx_BufFmt_Init(&ctx, stack, dtype);
+        if (unlikely(!__Pyx_BufFmt_CheckString(&ctx, buf->format))) goto fail;
+    }
+    if (unlikely((unsigned) buf->itemsize != dtype->size)) {
+        PyErr_Format(PyExc_ValueError,
+                     "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "u byte%s) "
+                     "does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "u byte%s)",
+                     buf->itemsize,
+                     (buf->itemsize > 1) ? "s" : "",
+                     dtype->name,
+                     dtype->size,
+                     (dtype->size > 1) ? "s" : "");
+        goto fail;
+    }
+    if (buf->len > 0) {
+        for (i = 0; i < ndim; i++) {
+            spec = axes_specs[i];
+            if (unlikely(!__pyx_check_strides(buf, i, ndim, spec)))
+                goto fail;
+            if (unlikely(!__pyx_check_suboffsets(buf, i, ndim, spec)))
+                goto fail;
+        }
+        if (unlikely(buf->strides && !__pyx_verify_contig(buf, ndim, c_or_f_flag)))
+            goto fail;
+    }
+    if (unlikely(__Pyx_init_memviewslice(memview, ndim, memviewslice,
+                                         new_memview != NULL) == -1)) {
+        goto fail;
+    }
+    retval = 0;
+    goto no_fail;
+fail:
+    Py_XDECREF(new_memview);
+    retval = -1;
+no_fail:
+    __Pyx_RefNannyFinishContext();
+    return retval;
+}
+
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_int(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, 0,
+                                                 PyBUF_RECORDS_RO | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_int, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
+/* CheckBinaryVersion */
+  static int __Pyx_check_binary_version(void) {
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+        char message[200];
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -23506,31 +23254,14 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
-  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
-    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
-#if PY_MAJOR_VERSION < 3
-  } else if (likely(PyInt_CheckExact(o))) {
-    return PyInt_AS_LONG(o);
-#endif
-  } else {
-    Py_ssize_t ival;
-    PyObject *x;
-    x = PyNumber_Index(o);
-    if (!x) return -1;
-    ival = PyInt_AsLong(x);
-    Py_DECREF(x);
-    return ival;
-  }
-}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `shorttext-1.5.8/shorttext/metrics/dynprog/dldist.pyx` & `shorttext-1.5.9/shorttext/metrics/dynprog/dldist.pyx`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/metrics/dynprog/jaccard.py` & `shorttext-1.5.9/shorttext/metrics/dynprog/jaccard.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/metrics/dynprog/lcp.c` & `shorttext-1.5.9/shorttext/metrics/dynprog/lcp.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.22 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "shorttext.metrics.dynprog.lcp",
         "sources": [
             "shorttext/metrics/dynprog/lcp.pyx"
         ]
     },
     "module_name": "shorttext.metrics.dynprog.lcp"
 }
 END: Cython Metadata */
 
-#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
-#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_22"
+#define CYTHON_HEX_VERSION 0x001D16F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -58,15 +56,14 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -95,22 +92,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -140,67 +133,18 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_PYSTON 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
-  #ifndef CYTHON_USE_TYPE_SLOTS
-    #define CYTHON_USE_TYPE_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_INTERNALS
-    #define CYTHON_USE_UNICODE_INTERNALS 1
-  #endif
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #ifndef CYTHON_ASSUME_SAFE_MACROS
-    #define CYTHON_ASSUME_SAFE_MACROS 1
-  #endif
-  #ifndef CYTHON_UNPACK_METHODS
-    #define CYTHON_UNPACK_METHODS 1
-  #endif
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -220,64 +164,53 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
+  #if PY_VERSION_HEX < 0x030300F0
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+  #ifndef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #if PY_MAJOR_VERSION < 3
-    #include "longintrepr.h"
-  #endif
+  #include "longintrepr.h"
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -386,76 +319,17 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-  #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
-                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
-                                                    PyObject *fv, PyObject *cell, PyObject* fn,
-                                                    PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
-        PyObject *type, *value, *traceback;
-        PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(call_result);
-        Py_XDECREF(empty);
-        if (type) {
-            PyErr_Restore(type, value, traceback);
-        }
-        return co;
-    }
+#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -561,33 +435,25 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
-  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
   #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
   #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
@@ -685,18 +551,18 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
@@ -713,18 +579,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -856,15 +720,14 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -996,195 +859,195 @@
 
 static const char *__pyx_f[] = {
   "shorttext/metrics/dynprog/lcp.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":689
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":690
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":691
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":692
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":696
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":697
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":698
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":699
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":703
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":704
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":713
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":714
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":715
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":717
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":718
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":719
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":721
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":722
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":724
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":725
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":726
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1211,42 +1074,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":728
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":729
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":730
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":732
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1965,15 +1828,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":734
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -1982,29 +1845,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":735
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":734
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -2015,15 +1878,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":737
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2032,29 +1895,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":738
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":737
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -2065,15 +1928,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":740
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2082,29 +1945,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":741
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":740
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -2115,15 +1978,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":743
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2132,29 +1995,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":744
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":743
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -2165,15 +2028,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":746
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2182,29 +2045,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":747
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":746
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -2215,212 +2078,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":749
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":750
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":751
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":750
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":753
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":749
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":928
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":929
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":930
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":928
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":932
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":933
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":934
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":935
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":934
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":936
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":932
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":940
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2436,15 +2299,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -2452,84 +2315,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":942
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":943
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":944
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":941
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":940
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -2544,15 +2407,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":946
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2568,15 +2431,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2584,84 +2447,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":948
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":949
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":950
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":947
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":946
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2676,15 +2539,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":952
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2700,15 +2563,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -2716,84 +2579,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":954
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":955
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":956
+      /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":953
+    /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":952
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -2808,176 +2671,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":966
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":978
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":966
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":981
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":993
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":981
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":996
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1003
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":996
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1010
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1006
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+/* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1017
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3052,43 +2915,43 @@
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_word1, __pyx_k_word1, sizeof(__pyx_k_word1), 0, 0, 1, 1},
   {&__pyx_n_s_word2, __pyx_k_word2, sizeof(__pyx_k_word2), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 12, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 945, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":944
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":950
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 951, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "shorttext/metrics/dynprog/lcp.pyx":5
  * cimport numpy as np
  * 
  * def longest_common_prefix(str word1, str word2):             # <<<<<<<<<<<<<<
@@ -3168,46 +3031,46 @@
   sizeof(PyTypeObject),
   #else
   sizeof(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 200, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 200, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 223, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 227, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 239, __pyx_L1_error)
   __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 771, __pyx_L1_error)
   __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 773, __pyx_L1_error)
   __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 775, __pyx_L1_error)
   __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 777, __pyx_L1_error)
   __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 779, __pyx_L1_error)
   __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 781, __pyx_L1_error)
   __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 783, __pyx_L1_error)
   __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 785, __pyx_L1_error)
   __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 787, __pyx_L1_error)
   __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 789, __pyx_L1_error)
   __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 827, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -3370,17 +3233,19 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
+  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("lcp", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -3459,15 +3324,15 @@
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../private/var/folders/rg/x22ydmg16jx944ktmgv7r1d80000gn/T/pip-build-env-byoru83a/overlay/lib/python3.8/site-packages/numpy/__init__.pxd":1013
+  /* "../../opt/anaconda3/envs/nlp/lib/python3.8/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -3946,15 +3811,15 @@
     return -1;
 }
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
+    ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -4329,15 +4194,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -4423,48 +4288,41 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = NULL;
-    PyObject *py_funcname = NULL;
+    PyCodeObject *py_code = 0;
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
     #if PY_MAJOR_VERSION < 3
-    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    if (!py_srcfile) goto bad;
+    #else
+    py_srcfile = PyUnicode_FromString(filename);
     #endif
+    if (!py_srcfile) goto bad;
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
-        funcname = PyUnicode_AsUTF8(py_funcname);
-        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        if (!py_funcname) goto bad;
+        #else
+        py_funcname = PyUnicode_FromString(funcname);
         #endif
     }
-    #if PY_MAJOR_VERSION < 3
+    if (!py_funcname) goto bad;
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -4475,49 +4333,34 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    #else
-    py_code = PyCode_NewEmpty(filename, funcname, py_line);
-    #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_DECREF(py_funcname);
     return py_code;
 bad:
-    Py_XDECREF(py_funcname);
-    #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
-    #endif
+    Py_XDECREF(py_funcname);
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -5426,41 +5269,19 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -5710,31 +5531,14 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
-  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
-    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
-#if PY_MAJOR_VERSION < 3
-  } else if (likely(PyInt_CheckExact(o))) {
-    return PyInt_AS_LONG(o);
-#endif
-  } else {
-    Py_ssize_t ival;
-    PyObject *x;
-    x = PyNumber_Index(o);
-    if (!x) return -1;
-    ival = PyInt_AsLong(x);
-    Py_DECREF(x);
-    return ival;
-  }
-}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `shorttext-1.5.8/shorttext/metrics/embedfuzzy/jaccard.py` & `shorttext-1.5.9/shorttext/metrics/embedfuzzy/jaccard.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/metrics/transformers/bertscore.py` & `shorttext-1.5.9/shorttext/metrics/transformers/bertscore.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/metrics/wasserstein/wordmoverdist.py` & `shorttext-1.5.9/shorttext/metrics/wasserstein/wordmoverdist.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/smartload.py` & `shorttext-1.5.9/shorttext/smartload.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/spell/basespellcorrector.py` & `shorttext-1.5.9/shorttext/spell/basespellcorrector.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/spell/binarize.py` & `shorttext-1.5.9/shorttext/spell/binarize.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/spell/editor.py` & `shorttext-1.5.9/shorttext/spell/editor.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/spell/norvig.py` & `shorttext-1.5.9/shorttext/spell/norvig.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/spell/sakaguchi.py` & `shorttext-1.5.9/shorttext/spell/sakaguchi.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/stack/stacking.py` & `shorttext-1.5.9/shorttext/stack/stacking.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/__init__.py` & `shorttext-1.5.9/shorttext/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/classification_exceptions.py` & `shorttext-1.5.9/shorttext/utils/classification_exceptions.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/compactmodel_io.py` & `shorttext-1.5.9/shorttext/utils/compactmodel_io.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/deprecation.py` & `shorttext-1.5.9/shorttext/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/dtm.py` & `shorttext-1.5.9/shorttext/utils/dtm.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/gensim_corpora.py` & `shorttext-1.5.9/shorttext/utils/gensim_corpora.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/kerasmodel_io.py` & `shorttext-1.5.9/shorttext/utils/kerasmodel_io.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/misc.py` & `shorttext-1.5.9/shorttext/utils/misc.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/nonneg_stopwords.txt` & `shorttext-1.5.9/shorttext/utils/nonneg_stopwords.txt`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/stopwords.txt` & `shorttext-1.5.9/shorttext/utils/stopwords.txt`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/textpreprocessing.py` & `shorttext-1.5.9/shorttext/utils/textpreprocessing.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/transformers.py` & `shorttext-1.5.9/shorttext/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext/utils/wordembed.py` & `shorttext-1.5.9/shorttext/utils/wordembed.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/shorttext.egg-info/PKG-INFO` & `shorttext-1.5.9/shorttext.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shorttext
-Version: 1.5.8
+Version: 1.5.9
 Summary: Short Text Mining
 Home-page: https://github.com/stephenhky/PyShortTextCategorization
 Author: Kwan-Yuet Ho
 Author-email: stephenhky@yahoo.com.hk
 License: MIT
 Description: ## Introduction
         
@@ -85,14 +85,15 @@
         * "Python Package for Short Text Mining", [WordPress](https://datawarrior.wordpress.com/2016/12/22/python-package-for-short-text-mining/)
         * "Document-Term Matrix: Text Mining in R and Python," [WordPress](https://datawarrior.wordpress.com/2018/01/22/document-term-matrix-text-mining-in-r-and-python/)
         * An [earlier version](https://github.com/stephenhky/PyShortTextCategorization/tree/b298d3ce7d06a9b4e0f7d32f27bab66064ba7afa) of this repository is a demonstration of the following blog post: [Short Text Categorization using Deep Neural Networks and Word-Embedding Models](https://datawarrior.wordpress.com/2016/10/12/short-text-categorization-using-deep-neural-networks-and-word-embedding-models/)
         
         
         ## News
         
+        * 06/19/2023: `shorttext` 1.5.9 released.
         * 09/23/2022: `shorttext` 1.5.8 released.
         * 09/22/2022: `shorttext` 1.5.7 released.
         * 08/29/2022: `shorttext` 1.5.6 released.
         * 05/28/2022: `shorttext` 1.5.5 released.
         * 12/15/2021: `shorttext` 1.5.4 released.
         * 07/11/2021: `shorttext` 1.5.3 released.
         * 07/06/2021: `shorttext` 1.5.2 released.
```

### Comparing `shorttext-1.5.8/shorttext.egg-info/SOURCES.txt` & `shorttext-1.5.9/shorttext.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 requirements.txt
 setup.cfg
 setup.py
 setup_requirements.txt
 test_requirements.txt
 bin/ShortTextCategorizerConsole
 bin/ShortTextWordEmbedSimilarity
-bin/WordEmbedAPI
 shorttext/__init__.py
 shorttext/smartload.py
 shorttext.egg-info/PKG-INFO
 shorttext.egg-info/SOURCES.txt
 shorttext.egg-info/dependency_links.txt
 shorttext.egg-info/not-zip-safe
 shorttext.egg-info/requires.txt
```

### Comparing `shorttext-1.5.8/test/test_bertrepresentations.py` & `shorttext-1.5.9/test/test_bertrepresentations.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_charonehot.py` & `shorttext-1.5.9/test/test_charonehot.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_dtm.py` & `shorttext-1.5.9/test/test_dtm.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_fuzzylogic.py` & `shorttext-1.5.9/test/test_fuzzylogic.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_norvigspell.py` & `shorttext-1.5.9/test/test_norvigspell.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_sakaguchispell.py` & `shorttext-1.5.9/test/test_sakaguchispell.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_stacking.py` & `shorttext-1.5.9/test/test_stacking.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_textpreprocessing.py` & `shorttext-1.5.9/test/test_textpreprocessing.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_var_nn_embedded_vec_classifier.py` & `shorttext-1.5.9/test/test_var_nn_embedded_vec_classifier.py`

 * *Files identical despite different names*

### Comparing `shorttext-1.5.8/test/test_wmd.py` & `shorttext-1.5.9/test/test_wmd.py`

 * *Files identical despite different names*

