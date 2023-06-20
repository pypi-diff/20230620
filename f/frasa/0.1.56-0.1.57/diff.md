# Comparing `tmp/frasa-0.1.56.tar.gz` & `tmp/frasa-0.1.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frasa-0.1.56.tar", last modified: Tue Jun 20 15:38:43 2023, max compression
+gzip compressed data, was "frasa-0.1.57.tar", last modified: Tue Jun 20 16:02:35 2023, max compression
```

## Comparing `frasa-0.1.56.tar` & `frasa-0.1.57.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.895701 frasa-0.1.56/
--rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.1.56/LICENSE
--rw-r--r--   0 novay      (501) staff       (20)      691 2023-06-04 18:05:03.000000 frasa-0.1.56/MANIFEST.in
--rw-r--r--   0 novay      (501) staff       (20)     1323 2023-06-20 15:38:43.895533 frasa-0.1.56/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)      613 2023-04-28 16:40:32.000000 frasa-0.1.56/README.md
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.837942 frasa-0.1.56/frasa/
--rw-r--r--   0 novay      (501) staff       (20)      698 2023-06-20 15:38:38.000000 frasa-0.1.56/frasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.841391 frasa-0.1.56/frasa/azlyrics/
--rw-r--r--   0 novay      (501) staff       (20)       82 2023-06-20 15:32:49.000000 frasa-0.1.56/frasa/azlyrics/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     6005 2023-06-20 15:32:28.000000 frasa-0.1.56/frasa/azlyrics/azlyrics.py
--rw-r--r--   0 novay      (501) staff       (20)     1081 2023-06-20 15:27:37.000000 frasa-0.1.56/frasa/azlyrics/jaro.py
--rw-r--r--   0 novay      (501) staff       (20)     5071 2023-06-20 15:27:46.000000 frasa-0.1.56/frasa/azlyrics/requester.py
--rw-r--r--   0 novay      (501) staff       (20)     5339 2023-06-20 15:31:38.000000 frasa-0.1.56/frasa/azlyrics/tools.py
--rw-r--r--   0 novay      (501) staff       (20)      794 2023-06-08 10:08:17.000000 frasa-0.1.56/frasa/base.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.841681 frasa-0.1.56/frasa/datasets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.1.56/frasa/datasets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.841873 frasa-0.1.56/frasa/datasets/corpus/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.1.56/frasa/datasets/corpus/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.842007 frasa-0.1.56/frasa/datasets/corpus/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.1.56/frasa/datasets/corpus/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.842246 frasa-0.1.56/frasa/datasets/corpus/indonesia/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.1.56/frasa/datasets/corpus/indonesia/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.867190 frasa-0.1.56/frasa/datasets/corpus/indonesia/lemma/
--rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-15 21:44:57.000000 frasa-0.1.56/frasa/datasets/corpus/indonesia/lemma/clitics.txt
--rw-r--r--   0 novay      (501) staff       (20) 19937523 2023-04-04 17:44:44.000000 frasa-0.1.56/frasa/datasets/corpus/indonesia/lemma/dict.json
--rw-r--r--   0 novay      (501) staff       (20)   236286 2023-04-04 17:43:21.000000 frasa-0.1.56/frasa/datasets/corpus/indonesia/lemma/root.txt
--rw-r--r--   0 novay      (501) staff       (20)    10520 2023-04-15 22:25:42.000000 frasa-0.1.56/frasa/datasets/corpus/indonesia/stopword.txt
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.870669 frasa-0.1.56/frasa/datasets/corpus/sensor/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.1.56/frasa/datasets/corpus/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)    71076 2023-04-14 16:22:53.000000 frasa-0.1.56/frasa/datasets/corpus/sensor/alphabetic_unicode.json
--rw-r--r--   0 novay      (501) staff       (20)      118 2023-04-15 23:06:01.000000 frasa-0.1.56/frasa/datasets/corpus/sensor/sensor-aturan.csv
--rw-r--r--   0 novay      (501) staff       (20)     7997 2023-04-15 23:06:01.000000 frasa-0.1.56/frasa/datasets/corpus/sensor/sensor-kata.csv
--rw-r--r--   0 novay      (501) staff       (20)      112 2023-04-15 23:06:01.000000 frasa-0.1.56/frasa/datasets/corpus/sensor/sensor-pengganti.csv
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.870948 frasa-0.1.56/frasa/datasets/corpus/tweets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.1.56/frasa/datasets/corpus/tweets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.871230 frasa-0.1.56/frasa/datasets/models/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.1.56/frasa/datasets/models/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)   121561 2023-04-15 23:49:13.000000 frasa-0.1.56/frasa/datasets/models/frasa-gender.pickle
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.886036 frasa-0.1.56/frasa/datasets/models/nusax/
--rw-r--r--   0 novay      (501) staff       (20)   141300 2023-06-04 17:03:55.000000 frasa-0.1.56/frasa/datasets/models/nusax/aceh_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    33057 2023-06-04 17:03:57.000000 frasa-0.1.56/frasa/datasets/models/nusax/aceh_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   164436 2023-06-04 17:03:59.000000 frasa-0.1.56/frasa/datasets/models/nusax/bali_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    39361 2023-06-04 17:04:01.000000 frasa-0.1.56/frasa/datasets/models/nusax/bali_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   154020 2023-06-04 17:04:04.000000 frasa-0.1.56/frasa/datasets/models/nusax/banjar_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    37829 2023-06-04 17:04:05.000000 frasa-0.1.56/frasa/datasets/models/nusax/banjar_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   153924 2023-06-04 17:04:07.000000 frasa-0.1.56/frasa/datasets/models/nusax/batak_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    37447 2023-06-04 17:04:08.000000 frasa-0.1.56/frasa/datasets/models/nusax/batak_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   164004 2023-06-04 17:04:10.000000 frasa-0.1.56/frasa/datasets/models/nusax/bugis_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    40991 2023-06-04 17:04:12.000000 frasa-0.1.56/frasa/datasets/models/nusax/bugis_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   144948 2023-06-04 17:04:16.000000 frasa-0.1.56/frasa/datasets/models/nusax/indo_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    35227 2023-06-04 17:04:17.000000 frasa-0.1.56/frasa/datasets/models/nusax/indo_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   154404 2023-06-04 17:04:19.000000 frasa-0.1.56/frasa/datasets/models/nusax/jawa_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    36524 2023-06-04 17:04:20.000000 frasa-0.1.56/frasa/datasets/models/nusax/jawa_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   159828 2023-06-04 17:04:23.000000 frasa-0.1.56/frasa/datasets/models/nusax/madura_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    38306 2023-06-04 17:04:24.000000 frasa-0.1.56/frasa/datasets/models/nusax/madura_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   149268 2023-06-04 17:04:26.000000 frasa-0.1.56/frasa/datasets/models/nusax/minang_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    36144 2023-06-04 17:04:27.000000 frasa-0.1.56/frasa/datasets/models/nusax/minang_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   135204 2023-06-04 17:04:31.000000 frasa-0.1.56/frasa/datasets/models/nusax/ngaju_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    31596 2023-06-04 17:04:32.000000 frasa-0.1.56/frasa/datasets/models/nusax/ngaju_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   157332 2023-06-04 17:04:34.000000 frasa-0.1.56/frasa/datasets/models/nusax/sunda_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    38239 2023-06-04 17:04:36.000000 frasa-0.1.56/frasa/datasets/models/nusax/sunda_vectorizer.pkl
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.886286 frasa-0.1.56/frasa/deteksi/
--rw-r--r--   0 novay      (501) staff       (20)      865 2023-04-16 00:07:31.000000 frasa-0.1.56/frasa/deteksi/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.886570 frasa-0.1.56/frasa/deteksi/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.1.56/frasa/deteksi/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.886709 frasa-0.1.56/frasa/deteksi/bahasa/data/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.1.56/frasa/deteksi/bahasa/data/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.887526 frasa-0.1.56/frasa/deteksi/gender/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:39:09.000000 frasa-0.1.56/frasa/deteksi/gender/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     3129 2023-04-18 19:44:26.000000 frasa-0.1.56/frasa/deteksi/gender/classify.py
--rw-r--r--   0 novay      (501) staff       (20)      992 2023-04-16 00:06:23.000000 frasa-0.1.56/frasa/deteksi/gender/gender.py
--rw-r--r--   0 novay      (501) staff       (20)      747 2023-04-15 23:49:34.000000 frasa-0.1.56/frasa/deteksi/gender/utils.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.888806 frasa-0.1.56/frasa/deteksi/plagiat/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:14:54.000000 frasa-0.1.56/frasa/deteksi/plagiat/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     1363 2023-04-16 09:16:31.000000 frasa-0.1.56/frasa/deteksi/plagiat/cosine.py
--rw-r--r--   0 novay      (501) staff       (20)      911 2023-04-16 09:14:51.000000 frasa-0.1.56/frasa/deteksi/plagiat/jaccard.py
--rw-r--r--   0 novay      (501) staff       (20)     4247 2023-04-16 11:45:48.000000 frasa-0.1.56/frasa/deteksi/plagiat/plagiat.py
--rw-r--r--   0 novay      (501) staff       (20)     1176 2023-04-16 01:06:12.000000 frasa-0.1.56/frasa/deteksi/plagiat/rabin_karp.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.890398 frasa-0.1.56/frasa/preprocess/
--rw-r--r--   0 novay      (501) staff       (20)      286 2023-06-20 15:29:31.000000 frasa-0.1.56/frasa/preprocess/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     8758 2023-04-15 21:37:48.000000 frasa-0.1.56/frasa/preprocess/lemma.py
--rw-r--r--   0 novay      (501) staff       (20)     1476 2023-06-04 18:04:23.000000 frasa-0.1.56/frasa/preprocess/sentimen.py
--rw-r--r--   0 novay      (501) staff       (20)      850 2023-04-15 22:28:40.000000 frasa-0.1.56/frasa/preprocess/stopword.py
--rw-r--r--   0 novay      (501) staff       (20)     9372 2023-04-16 13:15:30.000000 frasa-0.1.56/frasa/preprocess/token.py
--rw-r--r--   0 novay      (501) staff       (20)     5129 2023-06-08 12:52:05.000000 frasa-0.1.56/frasa/preprocess/tweet.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.894423 frasa-0.1.56/frasa/scrap/
--rw-r--r--   0 novay      (501) staff       (20)      778 2023-06-20 15:30:31.000000 frasa-0.1.56/frasa/scrap/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     3214 2023-06-08 16:58:22.000000 frasa-0.1.56/frasa/scrap/antara.py
--rw-r--r--   0 novay      (501) staff       (20)     1251 2023-06-08 17:23:32.000000 frasa-0.1.56/frasa/scrap/cnbc.py
--rw-r--r--   0 novay      (501) staff       (20)     1201 2023-06-08 17:26:45.000000 frasa-0.1.56/frasa/scrap/cnn.py
--rw-r--r--   0 novay      (501) staff       (20)     7902 2023-06-08 09:49:52.000000 frasa-0.1.56/frasa/scrap/detiknews.py
--rw-r--r--   0 novay      (501) staff       (20)      359 2023-06-08 17:28:05.000000 frasa-0.1.56/frasa/scrap/jpnn.py
--rw-r--r--   0 novay      (501) staff       (20)      367 2023-06-08 17:28:15.000000 frasa-0.1.56/frasa/scrap/kumparan.py
--rw-r--r--   0 novay      (501) staff       (20)     8492 2023-06-08 09:49:43.000000 frasa-0.1.56/frasa/scrap/liputan6.py
--rw-r--r--   0 novay      (501) staff       (20)     1243 2023-06-08 17:51:32.000000 frasa-0.1.56/frasa/scrap/merdeka.py
--rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:52:54.000000 frasa-0.1.56/frasa/scrap/okezone.py
--rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:53:27.000000 frasa-0.1.56/frasa/scrap/republika.py
--rw-r--r--   0 novay      (501) staff       (20)     1329 2023-06-08 17:54:41.000000 frasa-0.1.56/frasa/scrap/sindonews.py
--rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:55:25.000000 frasa-0.1.56/frasa/scrap/suara.py
--rw-r--r--   0 novay      (501) staff       (20)     1192 2023-06-08 17:56:57.000000 frasa-0.1.56/frasa/scrap/tempo.py
--rw-r--r--   0 novay      (501) staff       (20)     1251 2023-06-08 17:57:59.000000 frasa-0.1.56/frasa/scrap/tribun.py
--rw-r--r--   0 novay      (501) staff       (20)      776 2023-06-08 15:49:48.000000 frasa-0.1.56/frasa/scrap/utils.py
--rw-r--r--   0 novay      (501) staff       (20)      454 2023-06-08 15:39:44.000000 frasa-0.1.56/frasa/scrap/viva.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.895291 frasa-0.1.56/frasa/sensor/
--rw-r--r--   0 novay      (501) staff       (20)       76 2023-04-15 23:12:29.000000 frasa-0.1.56/frasa/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      428 2023-04-15 23:10:24.000000 frasa-0.1.56/frasa/sensor/constants.py
--rw-r--r--   0 novay      (501) staff       (20)     9267 2023-04-15 23:12:36.000000 frasa-0.1.56/frasa/sensor/sensor.py
--rw-r--r--   0 novay      (501) staff       (20)     1584 2023-04-15 23:10:52.000000 frasa-0.1.56/frasa/sensor/utils.py
--rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.1.56/frasa/sensor/variasi.py
--rw-r--r--   0 novay      (501) staff       (20)     1640 2023-04-19 21:40:39.000000 frasa-0.1.56/frasa/update.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 15:38:43.838982 frasa-0.1.56/frasa.egg-info/
--rw-r--r--   0 novay      (501) staff       (20)     1323 2023-06-20 15:38:43.000000 frasa-0.1.56/frasa.egg-info/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     3097 2023-06-20 15:38:43.000000 frasa-0.1.56/frasa.egg-info/SOURCES.txt
--rw-r--r--   0 novay      (501) staff       (20)        1 2023-06-20 15:38:43.000000 frasa-0.1.56/frasa.egg-info/dependency_links.txt
--rw-r--r--   0 novay      (501) staff       (20)       12 2023-06-20 15:38:43.000000 frasa-0.1.56/frasa.egg-info/top_level.txt
--rw-r--r--   0 novay      (501) staff       (20)       38 2023-06-20 15:38:43.895751 frasa-0.1.56/setup.cfg
--rw-r--r--   0 novay      (501) staff       (20)     1599 2023-06-20 15:38:34.000000 frasa-0.1.56/setup.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.631598 frasa-0.1.57/
+-rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.1.57/LICENSE
+-rw-r--r--   0 novay      (501) staff       (20)      691 2023-06-04 18:05:03.000000 frasa-0.1.57/MANIFEST.in
+-rw-r--r--   0 novay      (501) staff       (20)     1323 2023-06-20 16:02:35.631423 frasa-0.1.57/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)      613 2023-04-28 16:40:32.000000 frasa-0.1.57/README.md
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.571087 frasa-0.1.57/frasa/
+-rw-r--r--   0 novay      (501) staff       (20)      698 2023-06-20 16:02:17.000000 frasa-0.1.57/frasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.573478 frasa-0.1.57/frasa/azlyrics/
+-rw-r--r--   0 novay      (501) staff       (20)       82 2023-06-20 15:32:49.000000 frasa-0.1.57/frasa/azlyrics/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     5993 2023-06-20 16:00:58.000000 frasa-0.1.57/frasa/azlyrics/azlyrics.py
+-rw-r--r--   0 novay      (501) staff       (20)     1081 2023-06-20 15:27:37.000000 frasa-0.1.57/frasa/azlyrics/jaro.py
+-rw-r--r--   0 novay      (501) staff       (20)     5071 2023-06-20 15:27:46.000000 frasa-0.1.57/frasa/azlyrics/requester.py
+-rw-r--r--   0 novay      (501) staff       (20)     4806 2023-06-20 16:00:54.000000 frasa-0.1.57/frasa/azlyrics/tools.py
+-rw-r--r--   0 novay      (501) staff       (20)      794 2023-06-08 10:08:17.000000 frasa-0.1.57/frasa/base.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.573741 frasa-0.1.57/frasa/datasets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.1.57/frasa/datasets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.573861 frasa-0.1.57/frasa/datasets/corpus/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.1.57/frasa/datasets/corpus/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.573966 frasa-0.1.57/frasa/datasets/corpus/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.1.57/frasa/datasets/corpus/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.574195 frasa-0.1.57/frasa/datasets/corpus/indonesia/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.1.57/frasa/datasets/corpus/indonesia/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.586403 frasa-0.1.57/frasa/datasets/corpus/indonesia/lemma/
+-rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-15 21:44:57.000000 frasa-0.1.57/frasa/datasets/corpus/indonesia/lemma/clitics.txt
+-rw-r--r--   0 novay      (501) staff       (20) 19937523 2023-04-04 17:44:44.000000 frasa-0.1.57/frasa/datasets/corpus/indonesia/lemma/dict.json
+-rw-r--r--   0 novay      (501) staff       (20)   236286 2023-04-04 17:43:21.000000 frasa-0.1.57/frasa/datasets/corpus/indonesia/lemma/root.txt
+-rw-r--r--   0 novay      (501) staff       (20)    10520 2023-04-15 22:25:42.000000 frasa-0.1.57/frasa/datasets/corpus/indonesia/stopword.txt
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.591787 frasa-0.1.57/frasa/datasets/corpus/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.1.57/frasa/datasets/corpus/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)    71076 2023-04-14 16:22:53.000000 frasa-0.1.57/frasa/datasets/corpus/sensor/alphabetic_unicode.json
+-rw-r--r--   0 novay      (501) staff       (20)      118 2023-04-15 23:06:01.000000 frasa-0.1.57/frasa/datasets/corpus/sensor/sensor-aturan.csv
+-rw-r--r--   0 novay      (501) staff       (20)     7997 2023-04-15 23:06:01.000000 frasa-0.1.57/frasa/datasets/corpus/sensor/sensor-kata.csv
+-rw-r--r--   0 novay      (501) staff       (20)      112 2023-04-15 23:06:01.000000 frasa-0.1.57/frasa/datasets/corpus/sensor/sensor-pengganti.csv
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.592123 frasa-0.1.57/frasa/datasets/corpus/tweets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.1.57/frasa/datasets/corpus/tweets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.592392 frasa-0.1.57/frasa/datasets/models/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.1.57/frasa/datasets/models/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)   121561 2023-04-15 23:49:13.000000 frasa-0.1.57/frasa/datasets/models/frasa-gender.pickle
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.619816 frasa-0.1.57/frasa/datasets/models/nusax/
+-rw-r--r--   0 novay      (501) staff       (20)   141300 2023-06-04 17:03:55.000000 frasa-0.1.57/frasa/datasets/models/nusax/aceh_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    33057 2023-06-04 17:03:57.000000 frasa-0.1.57/frasa/datasets/models/nusax/aceh_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   164436 2023-06-04 17:03:59.000000 frasa-0.1.57/frasa/datasets/models/nusax/bali_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    39361 2023-06-04 17:04:01.000000 frasa-0.1.57/frasa/datasets/models/nusax/bali_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   154020 2023-06-04 17:04:04.000000 frasa-0.1.57/frasa/datasets/models/nusax/banjar_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    37829 2023-06-04 17:04:05.000000 frasa-0.1.57/frasa/datasets/models/nusax/banjar_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   153924 2023-06-04 17:04:07.000000 frasa-0.1.57/frasa/datasets/models/nusax/batak_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    37447 2023-06-04 17:04:08.000000 frasa-0.1.57/frasa/datasets/models/nusax/batak_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   164004 2023-06-04 17:04:10.000000 frasa-0.1.57/frasa/datasets/models/nusax/bugis_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    40991 2023-06-04 17:04:12.000000 frasa-0.1.57/frasa/datasets/models/nusax/bugis_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   144948 2023-06-04 17:04:16.000000 frasa-0.1.57/frasa/datasets/models/nusax/indo_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    35227 2023-06-04 17:04:17.000000 frasa-0.1.57/frasa/datasets/models/nusax/indo_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   154404 2023-06-04 17:04:19.000000 frasa-0.1.57/frasa/datasets/models/nusax/jawa_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    36524 2023-06-04 17:04:20.000000 frasa-0.1.57/frasa/datasets/models/nusax/jawa_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   159828 2023-06-04 17:04:23.000000 frasa-0.1.57/frasa/datasets/models/nusax/madura_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    38306 2023-06-04 17:04:24.000000 frasa-0.1.57/frasa/datasets/models/nusax/madura_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   149268 2023-06-04 17:04:26.000000 frasa-0.1.57/frasa/datasets/models/nusax/minang_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    36144 2023-06-04 17:04:27.000000 frasa-0.1.57/frasa/datasets/models/nusax/minang_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   135204 2023-06-04 17:04:31.000000 frasa-0.1.57/frasa/datasets/models/nusax/ngaju_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    31596 2023-06-04 17:04:32.000000 frasa-0.1.57/frasa/datasets/models/nusax/ngaju_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   157332 2023-06-04 17:04:34.000000 frasa-0.1.57/frasa/datasets/models/nusax/sunda_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    38239 2023-06-04 17:04:36.000000 frasa-0.1.57/frasa/datasets/models/nusax/sunda_vectorizer.pkl
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.620199 frasa-0.1.57/frasa/deteksi/
+-rw-r--r--   0 novay      (501) staff       (20)      865 2023-04-16 00:07:31.000000 frasa-0.1.57/frasa/deteksi/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.620766 frasa-0.1.57/frasa/deteksi/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.1.57/frasa/deteksi/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.620903 frasa-0.1.57/frasa/deteksi/bahasa/data/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.1.57/frasa/deteksi/bahasa/data/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.622313 frasa-0.1.57/frasa/deteksi/gender/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:39:09.000000 frasa-0.1.57/frasa/deteksi/gender/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     3129 2023-04-18 19:44:26.000000 frasa-0.1.57/frasa/deteksi/gender/classify.py
+-rw-r--r--   0 novay      (501) staff       (20)      992 2023-04-16 00:06:23.000000 frasa-0.1.57/frasa/deteksi/gender/gender.py
+-rw-r--r--   0 novay      (501) staff       (20)      747 2023-04-15 23:49:34.000000 frasa-0.1.57/frasa/deteksi/gender/utils.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.624438 frasa-0.1.57/frasa/deteksi/plagiat/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:14:54.000000 frasa-0.1.57/frasa/deteksi/plagiat/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     1363 2023-04-16 09:16:31.000000 frasa-0.1.57/frasa/deteksi/plagiat/cosine.py
+-rw-r--r--   0 novay      (501) staff       (20)      911 2023-04-16 09:14:51.000000 frasa-0.1.57/frasa/deteksi/plagiat/jaccard.py
+-rw-r--r--   0 novay      (501) staff       (20)     4247 2023-04-16 11:45:48.000000 frasa-0.1.57/frasa/deteksi/plagiat/plagiat.py
+-rw-r--r--   0 novay      (501) staff       (20)     1176 2023-04-16 01:06:12.000000 frasa-0.1.57/frasa/deteksi/plagiat/rabin_karp.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.626206 frasa-0.1.57/frasa/preprocess/
+-rw-r--r--   0 novay      (501) staff       (20)      286 2023-06-20 15:29:31.000000 frasa-0.1.57/frasa/preprocess/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     8758 2023-04-15 21:37:48.000000 frasa-0.1.57/frasa/preprocess/lemma.py
+-rw-r--r--   0 novay      (501) staff       (20)     1476 2023-06-04 18:04:23.000000 frasa-0.1.57/frasa/preprocess/sentimen.py
+-rw-r--r--   0 novay      (501) staff       (20)      850 2023-04-15 22:28:40.000000 frasa-0.1.57/frasa/preprocess/stopword.py
+-rw-r--r--   0 novay      (501) staff       (20)     9372 2023-04-16 13:15:30.000000 frasa-0.1.57/frasa/preprocess/token.py
+-rw-r--r--   0 novay      (501) staff       (20)     5129 2023-06-08 12:52:05.000000 frasa-0.1.57/frasa/preprocess/tweet.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.630418 frasa-0.1.57/frasa/scrap/
+-rw-r--r--   0 novay      (501) staff       (20)      778 2023-06-20 15:30:31.000000 frasa-0.1.57/frasa/scrap/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     3214 2023-06-08 16:58:22.000000 frasa-0.1.57/frasa/scrap/antara.py
+-rw-r--r--   0 novay      (501) staff       (20)     1251 2023-06-08 17:23:32.000000 frasa-0.1.57/frasa/scrap/cnbc.py
+-rw-r--r--   0 novay      (501) staff       (20)     1201 2023-06-08 17:26:45.000000 frasa-0.1.57/frasa/scrap/cnn.py
+-rw-r--r--   0 novay      (501) staff       (20)     7902 2023-06-08 09:49:52.000000 frasa-0.1.57/frasa/scrap/detiknews.py
+-rw-r--r--   0 novay      (501) staff       (20)      359 2023-06-08 17:28:05.000000 frasa-0.1.57/frasa/scrap/jpnn.py
+-rw-r--r--   0 novay      (501) staff       (20)      367 2023-06-08 17:28:15.000000 frasa-0.1.57/frasa/scrap/kumparan.py
+-rw-r--r--   0 novay      (501) staff       (20)     8492 2023-06-08 09:49:43.000000 frasa-0.1.57/frasa/scrap/liputan6.py
+-rw-r--r--   0 novay      (501) staff       (20)     1243 2023-06-08 17:51:32.000000 frasa-0.1.57/frasa/scrap/merdeka.py
+-rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:52:54.000000 frasa-0.1.57/frasa/scrap/okezone.py
+-rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:53:27.000000 frasa-0.1.57/frasa/scrap/republika.py
+-rw-r--r--   0 novay      (501) staff       (20)     1329 2023-06-08 17:54:41.000000 frasa-0.1.57/frasa/scrap/sindonews.py
+-rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:55:25.000000 frasa-0.1.57/frasa/scrap/suara.py
+-rw-r--r--   0 novay      (501) staff       (20)     1192 2023-06-08 17:56:57.000000 frasa-0.1.57/frasa/scrap/tempo.py
+-rw-r--r--   0 novay      (501) staff       (20)     1251 2023-06-08 17:57:59.000000 frasa-0.1.57/frasa/scrap/tribun.py
+-rw-r--r--   0 novay      (501) staff       (20)      776 2023-06-08 15:49:48.000000 frasa-0.1.57/frasa/scrap/utils.py
+-rw-r--r--   0 novay      (501) staff       (20)      454 2023-06-08 15:39:44.000000 frasa-0.1.57/frasa/scrap/viva.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.631164 frasa-0.1.57/frasa/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)       76 2023-04-15 23:12:29.000000 frasa-0.1.57/frasa/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      428 2023-04-15 23:10:24.000000 frasa-0.1.57/frasa/sensor/constants.py
+-rw-r--r--   0 novay      (501) staff       (20)     9267 2023-04-15 23:12:36.000000 frasa-0.1.57/frasa/sensor/sensor.py
+-rw-r--r--   0 novay      (501) staff       (20)     1584 2023-04-15 23:10:52.000000 frasa-0.1.57/frasa/sensor/utils.py
+-rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.1.57/frasa/sensor/variasi.py
+-rw-r--r--   0 novay      (501) staff       (20)     1640 2023-04-19 21:40:39.000000 frasa-0.1.57/frasa/update.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-20 16:02:35.572072 frasa-0.1.57/frasa.egg-info/
+-rw-r--r--   0 novay      (501) staff       (20)     1323 2023-06-20 16:02:35.000000 frasa-0.1.57/frasa.egg-info/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     3097 2023-06-20 16:02:35.000000 frasa-0.1.57/frasa.egg-info/SOURCES.txt
+-rw-r--r--   0 novay      (501) staff       (20)        1 2023-06-20 16:02:35.000000 frasa-0.1.57/frasa.egg-info/dependency_links.txt
+-rw-r--r--   0 novay      (501) staff       (20)       12 2023-06-20 16:02:35.000000 frasa-0.1.57/frasa.egg-info/top_level.txt
+-rw-r--r--   0 novay      (501) staff       (20)       38 2023-06-20 16:02:35.631654 frasa-0.1.57/setup.cfg
+-rw-r--r--   0 novay      (501) staff       (20)     1599 2023-06-20 16:02:12.000000 frasa-0.1.57/setup.py
```

### Comparing `frasa-0.1.56/LICENSE` & `frasa-0.1.57/LICENSE`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/MANIFEST.in` & `frasa-0.1.57/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/PKG-INFO` & `frasa-0.1.57/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.1.56
+Version: 0.1.57
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.1.56/README.md` & `frasa-0.1.57/README.md`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/__init__.py` & `frasa-0.1.57/frasa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Kunjungi http://frasa.id untuk informasi selengkapnya.
 """
 
 import os
 
 __name__ = "frasa"
-__version__ = "0.1.56"
+__version__ = "0.1.57"
 __license__ = 'MIT'
 __author__ = 'Novianto Rahmadi'
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 DATASET_DIR = PACKAGE_DIR + '/datasets/corpus'
 MODELS_DIR = PACKAGE_DIR + '/datasets/models'
```

### Comparing `frasa-0.1.56/frasa/azlyrics/azlyrics.py` & `frasa-0.1.57/frasa/azlyrics/azlyrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         
         self.proxies = proxies
 
         self.lyrics_history = []
         self.lyrics = ''
         self.songs = {}
 
-    def getLyrics(self, url=None, ext='txt', save=False, path='', sleep=3):
+    def lirik(self, url=None, ext='txt', save=False, path='', sleep=3):
         """
         Retrieve Lyrics for a given song details.
         
         Parameters: 
             url (str): url of the song's Azlyrics page. 
             ext (str): extension of the lyrics saved file, default is ".txt".
             save (bool): allow to or not to save lyrics in a file.
@@ -77,15 +77,15 @@
                             0)
 
         page = self.get(link, self.proxies)
         if page.status_code != 200:
             if not self.search_engine:
                 print('Failed to find lyrics. Trying to get link from Google')
                 self.search_engine = 'google'
-                lyrics = self.getLyrics(url=url, ext=ext, save=save, path=path, sleep=sleep)
+                lyrics = self.lirik(url=url, ext=ext, save=save, path=path, sleep=sleep)
                 self.search_engine = ''
                 return lyrics
             else:
                 print('Error',page.status_code)
                 return 1
 
         # Getting Basic metadata from azlyrics
@@ -122,15 +122,15 @@
             # Store lyrics for later usage
             self.lyrics_history.append(self.lyrics)
             return self.lyrics
 
         self.lyrics = 'No lyrics found :('
         return 2
 
-    def getSongs(self, sleep=3):
+    def lagu(self, sleep=3):
         """
         Retrieve a dictionary of songs with their links.
 
         Parameters:
             sleep (float): cooldown before next request.  
         
         Returns:
@@ -162,17 +162,17 @@
                         1)
         
         albums_page = self.get(link, self.proxies)
         if albums_page.status_code != 200:
             if not self.search_engine:
                 print('Failed to find songs. Trying to get link from Google')
                 self.search_engine = 'google'
-                songs = self.getLyrics(sleep=sleep)
+                songs = self.lirik(sleep=sleep)
                 self.search_engine = ''
                 return songs
             else:
                 print('Error',albums_page.status_code)
                 return {}
         
-        # Store songs for later usage
+        # Store songs for later usage    
         self.songs = parseSongs(albums_page)
         return self.songs
```

### Comparing `frasa-0.1.56/frasa/azlyrics/jaro.py` & `frasa-0.1.57/frasa/azlyrics/jaro.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/azlyrics/requester.py` & `frasa-0.1.57/frasa/azlyrics/requester.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/azlyrics/tools.py` & `frasa-0.1.57/frasa/azlyrics/tools.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 import bs4, re, time, os
 from urllib.parse import quote
 from .jaro import jaro_distance
 
 letters = 'abcdefghijklmnopqrstuvwxyz0123456789'
 
 def htmlFind(page):
-    # v3.0
-    # Changed page.text -> page.content.decode() to support variant unicodes
     soup = bs4.BeautifulSoup(
                         page.content.decode(),
                         "html.parser"
                         )
     return soup.find
 
 def htmlFindAll(page):
-    # v3.0
-    # Changed page.text -> page.content.decode() to support variant unicodes
     soup = bs4.BeautifulSoup(
                         page.content.decode(),
                         "html.parser"
                         )
     return soup.findAll
 
 def filtr(inpt, isFile=False):
     if isFile:
         return ''.join(i for i in inpt if i not in r'<>:"/\|?*')
     return ''.join(i.lower() for i in inpt if i.lower() in letters)
 
 def normalGet(artist='', title='', _type=0):
     art, tit = filtr(artist), filtr(title)
     if _type:
-        print('https://www.azlyrics.com/{}/{}.html'.format(art[0], art))
+        # print('https://www.azlyrics.com/{}/{}.html'.format(art[0], art))
         return 'https://www.azlyrics.com/{}/{}.html'.format(art[0], art)
     return 'https://www.azlyrics.com/lyrics/{}/{}.html'.format(art, tit)
 
 def googleGet(srch_eng, acc, get_func, artist='', title='', _type=0, proxies={}):
     # Encode artist and title to avoid url encoding errors
     data = artist + ' ' * (title != '' and artist != '') + title
     encoded_data = quote(data.replace(' ', '+'))
@@ -104,20 +100,14 @@
     Parent = htmlFind(page)('div', {'id':'listAlbum'})
     if Parent:
         Raw_Data = Parent.findChildren()
 
         curType, curName, curYear = '', '', ''
 
         for elmnt in Raw_Data:
-
-            # v3.0.3: Removed break after script due to google ads inside listAlbum
-            # is using script tag, which results in not all songs retrieved
-            #if elmnt.name == 'script':
-            #    break
-            
             # album info are inside divs
             if elmnt.name == 'div':
                 if elmnt.text == 'other songs:':
                     curType, curName, curYear = 'Others', '', ''
                 else:
                     # Separating to (album, name, year)
                     rgx = re.findall(r'(.*):\s"(.*)"\s\(([0-9]+)\)', elmnt.text)
@@ -128,21 +118,20 @@
                     'year': curYear,
                     'album': curName,
                     'type': curType,
                     # Azlyrics puts hrefs with/without base url
                     'url': 'http://www.azlyrics.com' + elmnt['href'].strip('.') \
                             if elmnt['href'].startswith('/lyrics/') else elmnt['href']
                 }
-    # v 3.0
-    # Some artists have no albums, so we cover this
+
     else:
         for div in htmlFindAll(page)('div', {'class':'listalbum-item'}):
             a = div.find('a')
             songs[a.text] = {
                 'year': '',
                 'album': '',
                 'type': '',
-                # v3.0.1: fix relative urls -> absolute url
                 'url': 'http://www.azlyrics.com' + a['href'][2:] \
                         if a['href'][:2] == '..' else a['href']
                 }
+
     return songs
```

### Comparing `frasa-0.1.56/frasa/base.py` & `frasa-0.1.57/frasa/base.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/corpus/indonesia/lemma/dict.json` & `frasa-0.1.57/frasa/datasets/corpus/indonesia/lemma/dict.json`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/corpus/indonesia/lemma/root.txt` & `frasa-0.1.57/frasa/datasets/corpus/indonesia/lemma/root.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/corpus/indonesia/stopword.txt` & `frasa-0.1.57/frasa/datasets/corpus/indonesia/stopword.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/corpus/sensor/alphabetic_unicode.json` & `frasa-0.1.57/frasa/datasets/corpus/sensor/alphabetic_unicode.json`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/corpus/sensor/sensor-kata.csv` & `frasa-0.1.57/frasa/datasets/corpus/sensor/sensor-kata.csv`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/frasa-gender.pickle` & `frasa-0.1.57/frasa/datasets/models/frasa-gender.pickle`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/aceh_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/aceh_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/aceh_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/aceh_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/bali_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/bali_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/bali_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/bali_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/banjar_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/banjar_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/banjar_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/banjar_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/batak_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/batak_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/batak_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/batak_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/bugis_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/bugis_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/bugis_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/bugis_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/indo_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/indo_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/indo_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/indo_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/jawa_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/jawa_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/jawa_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/jawa_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/madura_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/madura_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/madura_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/madura_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/minang_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/minang_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/minang_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/minang_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/ngaju_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/ngaju_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/ngaju_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/ngaju_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/sunda_model.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/sunda_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/datasets/models/nusax/sunda_vectorizer.pkl` & `frasa-0.1.57/frasa/datasets/models/nusax/sunda_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/deteksi/__init__.py` & `frasa-0.1.57/frasa/deteksi/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/deteksi/gender/classify.py` & `frasa-0.1.57/frasa/deteksi/gender/classify.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/deteksi/gender/gender.py` & `frasa-0.1.57/frasa/deteksi/gender/gender.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/deteksi/gender/utils.py` & `frasa-0.1.57/frasa/deteksi/gender/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/deteksi/plagiat/cosine.py` & `frasa-0.1.57/frasa/deteksi/plagiat/cosine.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/deteksi/plagiat/jaccard.py` & `frasa-0.1.57/frasa/deteksi/plagiat/jaccard.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/deteksi/plagiat/plagiat.py` & `frasa-0.1.57/frasa/deteksi/plagiat/plagiat.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/deteksi/plagiat/rabin_karp.py` & `frasa-0.1.57/frasa/deteksi/plagiat/rabin_karp.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/preprocess/lemma.py` & `frasa-0.1.57/frasa/preprocess/lemma.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/preprocess/sentimen.py` & `frasa-0.1.57/frasa/preprocess/sentimen.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/preprocess/stopword.py` & `frasa-0.1.57/frasa/preprocess/stopword.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/preprocess/token.py` & `frasa-0.1.57/frasa/preprocess/token.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/preprocess/tweet.py` & `frasa-0.1.57/frasa/preprocess/tweet.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/__init__.py` & `frasa-0.1.57/frasa/scrap/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/antara.py` & `frasa-0.1.57/frasa/scrap/antara.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/cnbc.py` & `frasa-0.1.57/frasa/scrap/cnbc.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/cnn.py` & `frasa-0.1.57/frasa/scrap/cnn.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/detiknews.py` & `frasa-0.1.57/frasa/scrap/detiknews.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/liputan6.py` & `frasa-0.1.57/frasa/scrap/liputan6.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/merdeka.py` & `frasa-0.1.57/frasa/scrap/merdeka.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/okezone.py` & `frasa-0.1.57/frasa/scrap/okezone.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/republika.py` & `frasa-0.1.57/frasa/scrap/republika.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/sindonews.py` & `frasa-0.1.57/frasa/scrap/sindonews.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/suara.py` & `frasa-0.1.57/frasa/scrap/suara.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/tempo.py` & `frasa-0.1.57/frasa/scrap/tempo.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/tribun.py` & `frasa-0.1.57/frasa/scrap/tribun.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/scrap/utils.py` & `frasa-0.1.57/frasa/scrap/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/sensor/sensor.py` & `frasa-0.1.57/frasa/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/sensor/utils.py` & `frasa-0.1.57/frasa/sensor/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/sensor/variasi.py` & `frasa-0.1.57/frasa/sensor/variasi.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa/update.py` & `frasa-0.1.57/frasa/update.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/frasa.egg-info/PKG-INFO` & `frasa-0.1.57/frasa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.1.56
+Version: 0.1.57
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.1.56/frasa.egg-info/SOURCES.txt` & `frasa-0.1.57/frasa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.56/setup.py` & `frasa-0.1.57/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="frasa",
-    version="0.1.56",
+    version="0.1.57",
     description="Koleksi NLP Pribadi untuk Bahasa Indonesia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novay/frasa",
     author="Novianto Rahmadi",
     author_email="novay@btekno.id",
     license="MIT",
```

