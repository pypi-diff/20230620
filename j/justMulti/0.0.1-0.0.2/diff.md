# Comparing `tmp/justMulti-0.0.1.tar.gz` & `tmp/justMulti-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justMulti-0.0.1.tar", last modified: Tue Jun 20 05:17:05 2023, max compression
+gzip compressed data, was "justMulti-0.0.2.tar", last modified: Tue Jun 20 05:38:30 2023, max compression
```

## Comparing `justMulti-0.0.1.tar` & `justMulti-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,118 @@
-drwxrwxr-x   0 vrushank  (1000) vrushank  (1000)        0 2023-06-20 05:17:05.119338 justMulti-0.0.1/
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      306 2023-06-20 05:17:05.119338 justMulti-0.0.1/PKG-INFO
-drwxrwxr-x   0 vrushank  (1000) vrushank  (1000)        0 2023-06-20 05:17:05.115337 justMulti-0.0.1/justMulti/
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      271 2023-06-20 04:54:45.000000 justMulti-0.0.1/justMulti/__init__.py
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    12640 2023-06-20 04:54:50.000000 justMulti-0.0.1/justMulti/__main__.py
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      802 2023-06-18 18:29:39.000000 justMulti-0.0.1/justMulti/_compat.py
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    14518 2023-06-20 04:54:36.000000 justMulti-0.0.1/justMulti/core.py
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1700 2023-06-19 02:18:04.000000 justMulti-0.0.1/justMulti/paragraph.py
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1969 2023-06-20 04:55:00.000000 justMulti-0.0.1/justMulti/utils.py
-drwxrwxr-x   0 vrushank  (1000) vrushank  (1000)        0 2023-06-20 05:17:05.119338 justMulti-0.0.1/justMulti.egg-info/
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      306 2023-06-20 05:17:05.000000 justMulti-0.0.1/justMulti.egg-info/PKG-INFO
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      297 2023-06-20 05:17:05.000000 justMulti-0.0.1/justMulti.egg-info/SOURCES.txt
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)        1 2023-06-20 05:17:05.000000 justMulti-0.0.1/justMulti.egg-info/dependency_links.txt
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)        5 2023-06-20 05:17:05.000000 justMulti-0.0.1/justMulti.egg-info/requires.txt
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)       10 2023-06-20 05:17:05.000000 justMulti-0.0.1/justMulti.egg-info/top_level.txt
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)       38 2023-06-20 05:17:05.119338 justMulti-0.0.1/setup.cfg
--rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      571 2023-06-20 05:17:02.000000 justMulti-0.0.1/setup.py
+drwxrwxr-x   0 vrushank  (1000) vrushank  (1000)        0 2023-06-20 05:38:30.433931 justMulti-0.0.2/
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      361 2023-06-20 05:38:30.433931 justMulti-0.0.2/PKG-INFO
+drwxrwxr-x   0 vrushank  (1000) vrushank  (1000)        0 2023-06-20 05:38:30.425930 justMulti-0.0.2/justMulti/
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      271 2023-06-20 04:54:45.000000 justMulti-0.0.2/justMulti/__init__.py
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    12640 2023-06-20 04:54:50.000000 justMulti-0.0.2/justMulti/__main__.py
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      802 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/_compat.py
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    14518 2023-06-20 04:54:36.000000 justMulti-0.0.2/justMulti/core.py
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1700 2023-06-19 02:18:04.000000 justMulti-0.0.2/justMulti/paragraph.py
+drwxrwxr-x   0 vrushank  (1000) vrushank  (1000)        0 2023-06-20 05:38:30.433931 justMulti-0.0.2/justMulti/stoplists/
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1205 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Afrikaans.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3424 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Albanian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    30217 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Arabic.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      918 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Aragonese.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    45410 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Armenian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3544 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Aromanian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     4379 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Asturian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    33201 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Azerbaijani.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    17791 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Basque.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    65883 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Belarusian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    62122 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Belarusian_Taraskievica.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    18721 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Bengali.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      950 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Bishnupriya_Manipuri.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    16143 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Bosnian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1649 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Breton.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    15206 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Bulgarian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1344 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Catalan.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)       57 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Cebuano.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    35124 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Chuvash.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    17928 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Croatian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    25564 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Czech.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3504 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Danish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1756 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Dutch.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3123 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/English.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3657 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Esperanto.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    50849 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Estonian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    66511 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Finnish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     2656 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/French.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     2857 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Galician.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)   128465 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Georgian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     4653 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/German.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     7796 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Greek.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     6073 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Gujarati.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      175 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Haitian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    45229 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Hebrew.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     4944 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Hindi.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    29227 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Hungarian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     4813 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Icelandic.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      249 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Ido.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      733 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Igbo.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     6758 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Indonesian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1191 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Irish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3715 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Italian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     4533 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Javanese.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)   161220 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Kannada.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    52789 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Kazakh.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)   131487 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Korean.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3530 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Kurdish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    54729 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Kyrgyz.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    14282 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Latin.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    30561 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Latvian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    43497 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Lithuanian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      738 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Lombard.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1051 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Low_Saxon.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     2374 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Luxembourgish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    11982 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Macedonian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     6368 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Malay.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)   309082 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Malayalam.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    11115 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Maltese.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    39588 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Marathi.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1749 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Neapolitan.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    26543 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Nepali.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1465 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Newar.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     2850 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Norwegian_Bokmal.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     2002 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Norwegian_Nynorsk.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3109 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Occitan.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     4642 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Persian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      419 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Piedmontese.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    29632 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Polish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3261 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Portuguese.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     2237 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Quechua.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     7067 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Romanian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    77600 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Russian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    14867 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Samogitian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    21052 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Serbian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    17311 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Serbo_Croatian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3167 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Sicilian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1567 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Simple_English.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    28930 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Slovak.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    17179 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Slovenian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1851 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Spanish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     5971 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Sundanese.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     2406 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Swahili.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     4870 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Swedish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      980 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Tagalog.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)   154484 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Tamil.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    95849 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Telugu.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    25673 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Turkish.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    27602 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Turkmen.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    75370 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Ukrainian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1900 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Urdu.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)    51738 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Uzbek.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1769 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Vietnamese.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      533 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Volapuk.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      910 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Walloon.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)       47 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Waray_Waray.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3338 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Welsh.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1353 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/West_Frisian.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     2230 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Western_Panjabi.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1748 2023-06-18 18:29:39.000000 justMulti-0.0.2/justMulti/stoplists/Yoruba.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     1969 2023-06-20 04:55:00.000000 justMulti-0.0.2/justMulti/utils.py
+drwxrwxr-x   0 vrushank  (1000) vrushank  (1000)        0 2023-06-20 05:38:30.425930 justMulti-0.0.2/justMulti.egg-info/
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      361 2023-06-20 05:38:30.000000 justMulti-0.0.2/justMulti.egg-info/PKG-INFO
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)     3602 2023-06-20 05:38:30.000000 justMulti-0.0.2/justMulti.egg-info/SOURCES.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)        1 2023-06-20 05:38:30.000000 justMulti-0.0.2/justMulti.egg-info/dependency_links.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)        5 2023-06-20 05:38:30.000000 justMulti-0.0.2/justMulti.egg-info/requires.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)       10 2023-06-20 05:38:30.000000 justMulti-0.0.2/justMulti.egg-info/top_level.txt
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)       38 2023-06-20 05:38:30.433931 justMulti-0.0.2/setup.cfg
+-rw-rw-r--   0 vrushank  (1000) vrushank  (1000)      630 2023-06-20 05:36:47.000000 justMulti-0.0.2/setup.py
```

### Comparing `justMulti-0.0.1/justMulti/__main__.py` & `justMulti-0.0.2/justMulti/__main__.py`

 * *Files identical despite different names*

### Comparing `justMulti-0.0.1/justMulti/_compat.py` & `justMulti-0.0.2/justMulti/_compat.py`

 * *Files identical despite different names*

### Comparing `justMulti-0.0.1/justMulti/core.py` & `justMulti-0.0.2/justMulti/core.py`

 * *Files identical despite different names*

### Comparing `justMulti-0.0.1/justMulti/paragraph.py` & `justMulti-0.0.2/justMulti/paragraph.py`

 * *Files identical despite different names*

### Comparing `justMulti-0.0.1/justMulti/utils.py` & `justMulti-0.0.2/justMulti/utils.py`

 * *Files identical despite different names*

### Comparing `justMulti-0.0.1/setup.py` & `justMulti-0.0.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Parse html strings'
 LONG_DESCRIPTION = 'Parse html strings and remove boilerplate material while extracting useful text/images/video/audio.'
 
 # Setting up
 setup(
     name="justMulti",
     version=VERSION,
@@ -12,8 +12,11 @@
     author_email="<vrushdesai0@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['lxml'],
     keywords=['html', 'parsing'],
-)
+    package_data={
+        '': ['stoplists/*.txt'],
+    }
+)
```

