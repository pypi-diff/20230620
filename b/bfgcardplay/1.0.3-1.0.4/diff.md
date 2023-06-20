# Comparing `tmp/bfgcardplay-1.0.3.tar.gz` & `tmp/bfgcardplay-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgcardplay-1.0.3.tar", last modified: Thu May 11 08:45:27 2023, max compression
+gzip compressed data, was "bfgcardplay-1.0.4.tar", last modified: Tue Jun 20 11:37:28 2023, max compression
```

## Comparing `bfgcardplay-1.0.3.tar` & `bfgcardplay-1.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.798407 bfgcardplay-1.0.3/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3757 2023-05-11 08:45:27.798407 bfgcardplay-1.0.3/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.3/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.768407 bfgcardplay-1.0.3/bfgcardplay/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      227 2021-10-01 11:09:27.000000 bfgcardplay-1.0.3/bfgcardplay/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/_version.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.3/bfgcardplay/logger.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.791740 bfgcardplay-1.0.3/bfgcardplay/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-12-22 17:41:36.000000 bfgcardplay-1.0.3/bfgcardplay/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3402 2021-12-22 17:41:36.000000 bfgcardplay-1.0.3/bfgcardplay/source/card_player_components.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2347 2023-01-20 16:29:14.000000 bfgcardplay-1.0.3/bfgcardplay/source/cards.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    19631 2023-01-05 11:19:24.000000 bfgcardplay-1.0.3/bfgcardplay/source/dashboard.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4714 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/source/data_classes.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    12323 2023-02-10 13:38:26.000000 bfgcardplay-1.0.3/bfgcardplay/source/declarer_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4085 2023-03-08 17:55:15.000000 bfgcardplay-1.0.3/bfgcardplay/source/defender_play.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9806 2023-02-10 13:38:26.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16175 2023-02-03 17:43:49.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17044 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer_nt.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    22029 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    16559 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/first_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2791 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     5957 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     4836 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2021-12-22 17:41:36.000000 bfgcardplay-1.0.3/bfgcardplay/source/global_variables.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3966 2022-01-04 17:55:18.000000 bfgcardplay-1.0.3/bfgcardplay/source/manager.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      667 2022-06-27 17:02:41.000000 bfgcardplay-1.0.3/bfgcardplay/source/opening_lead.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     6981 2023-01-20 16:49:44.000000 bfgcardplay-1.0.3/bfgcardplay/source/opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    43121 2023-03-08 17:55:15.000000 bfgcardplay-1.0.3/bfgcardplay/source/opening_lead_suit.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    24518 2023-05-11 08:43:28.000000 bfgcardplay-1.0.3/bfgcardplay/source/player.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3052 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/second_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     9977 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/second_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     7234 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/second_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3672 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/suggested_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2428 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/third_seat.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17717 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/third_seat_declarer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    13898 2023-02-02 07:57:08.000000 bfgcardplay-1.0.3/bfgcardplay/source/third_seat_defender.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1483 2023-01-20 11:07:39.000000 bfgcardplay-1.0.3/bfgcardplay/source/utilities.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.798407 bfgcardplay-1.0.3/bfgcardplay/test/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-10-25 15:12:22.000000 bfgcardplay-1.0.3/bfgcardplay/test/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    11741 2023-01-20 16:48:53.000000 bfgcardplay-1.0.3/bfgcardplay/test/test_opening_lead_card.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14967 2023-01-20 17:51:03.000000 bfgcardplay-1.0.3/bfgcardplay/test/test_opening_lead_suit.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-11 08:45:27.768407 bfgcardplay-1.0.3/bfgcardplay.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     3757 2023-05-11 08:45:27.000000 bfgcardplay-1.0.3/bfgcardplay.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1434 2023-05-11 08:45:27.000000 bfgcardplay-1.0.3/bfgcardplay.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-11 08:45:27.000000 bfgcardplay-1.0.3/bfgcardplay.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-05-11 08:45:27.000000 bfgcardplay-1.0.3/bfgcardplay.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-11 08:45:27.798407 bfgcardplay-1.0.3/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.3/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:37:28.630135 bfgcardplay-1.0.4/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3800 2023-06-20 11:37:28.630135 bfgcardplay-1.0.4/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        2 2021-07-03 11:00:43.000000 bfgcardplay-1.0.4/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:37:28.620135 bfgcardplay-1.0.4/bfgcardplay/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      227 2021-10-01 11:09:27.000000 bfgcardplay-1.0.4/bfgcardplay/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-20 11:36:59.000000 bfgcardplay-1.0.4/bfgcardplay/_version.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      912 2021-11-08 15:49:35.000000 bfgcardplay-1.0.4/bfgcardplay/logger.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:37:28.626801 bfgcardplay-1.0.4/bfgcardplay/source/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-12-22 17:41:36.000000 bfgcardplay-1.0.4/bfgcardplay/source/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3402 2021-12-22 17:41:36.000000 bfgcardplay-1.0.4/bfgcardplay/source/card_player_components.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2347 2023-01-20 16:29:14.000000 bfgcardplay-1.0.4/bfgcardplay/source/cards.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    19631 2023-01-05 11:19:24.000000 bfgcardplay-1.0.4/bfgcardplay/source/dashboard.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4714 2023-05-11 08:43:28.000000 bfgcardplay-1.0.4/bfgcardplay/source/data_classes.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    12323 2023-02-10 13:38:26.000000 bfgcardplay-1.0.4/bfgcardplay/source/declarer_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     4022 2023-06-20 11:36:59.000000 bfgcardplay-1.0.4/bfgcardplay/source/defender_play.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9806 2023-02-10 13:38:26.000000 bfgcardplay-1.0.4/bfgcardplay/source/first_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16175 2023-02-03 17:43:49.000000 bfgcardplay-1.0.4/bfgcardplay/source/first_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17044 2023-05-11 08:43:28.000000 bfgcardplay-1.0.4/bfgcardplay/source/first_seat_declarer_nt.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    22029 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/first_seat_declarer_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    16559 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/first_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2791 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/fourth_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5957 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/fourth_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     5359 2023-06-20 11:36:59.000000 bfgcardplay-1.0.4/bfgcardplay/source/fourth_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      134 2021-12-22 17:41:36.000000 bfgcardplay-1.0.4/bfgcardplay/source/global_variables.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3966 2022-01-04 17:55:18.000000 bfgcardplay-1.0.4/bfgcardplay/source/manager.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      667 2022-06-27 17:02:41.000000 bfgcardplay-1.0.4/bfgcardplay/source/opening_lead.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     6981 2023-01-20 16:49:44.000000 bfgcardplay-1.0.4/bfgcardplay/source/opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    43121 2023-03-08 17:55:15.000000 bfgcardplay-1.0.4/bfgcardplay/source/opening_lead_suit.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    24518 2023-05-11 08:43:28.000000 bfgcardplay-1.0.4/bfgcardplay/source/player.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3052 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/second_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9977 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/second_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     7234 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/second_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3672 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/suggested_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     2428 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/third_seat.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17717 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/third_seat_declarer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    13898 2023-02-02 07:57:08.000000 bfgcardplay-1.0.4/bfgcardplay/source/third_seat_defender.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1483 2023-01-20 11:07:39.000000 bfgcardplay-1.0.4/bfgcardplay/source/utilities.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:37:28.626801 bfgcardplay-1.0.4/bfgcardplay/test/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2021-10-25 15:12:22.000000 bfgcardplay-1.0.4/bfgcardplay/test/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    11741 2023-01-20 16:48:53.000000 bfgcardplay-1.0.4/bfgcardplay/test/test_opening_lead_card.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14967 2023-01-20 17:51:03.000000 bfgcardplay-1.0.4/bfgcardplay/test/test_opening_lead_suit.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:37:28.620135 bfgcardplay-1.0.4/bfgcardplay.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     3800 2023-06-20 11:37:28.000000 bfgcardplay-1.0.4/bfgcardplay.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1434 2023-06-20 11:37:28.000000 bfgcardplay-1.0.4/bfgcardplay.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-20 11:37:28.000000 bfgcardplay-1.0.4/bfgcardplay.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       12 2023-06-20 11:37:28.000000 bfgcardplay-1.0.4/bfgcardplay.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-20 11:37:28.630135 bfgcardplay-1.0.4/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1284 2021-07-03 11:10:30.000000 bfgcardplay-1.0.4/setup.py
```

### Comparing `bfgcardplay-1.0.3/PKG-INFO` & `bfgcardplay-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.0.4 20 Jun 2023
+
+1. xxx
+
+------
+
 Version 1.0.3 11 May 2023
 
 1. Correct manager.suit_to_develop
 
 ------
 
 Version 1.0.2 08 Mar 2023
```

### Comparing `bfgcardplay-1.0.3/bfgcardplay/logger.py` & `bfgcardplay-1.0.4/bfgcardplay/logger.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/card_player_components.py` & `bfgcardplay-1.0.4/bfgcardplay/source/card_player_components.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/cards.py` & `bfgcardplay-1.0.4/bfgcardplay/source/cards.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/dashboard.py` & `bfgcardplay-1.0.4/bfgcardplay/source/dashboard.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/data_classes.py` & `bfgcardplay-1.0.4/bfgcardplay/source/data_classes.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/declarer_play.py` & `bfgcardplay-1.0.4/bfgcardplay/source/declarer_play.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/defender_play.py` & `bfgcardplay-1.0.4/bfgcardplay/source/defender_play.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
 def get_hilo_signal_card(player, cards: List[Card]) -> Card:
     """Return a signal card denoting even/odd"""
     manager = global_vars.manager
     trick = player.board.tricks[-1]
     if len(cards) % 2 == 0:
         if len(cards) == 2:
-            cprint(f"{cards} {cards[-2].rank}", MODULE_COLOUR)
             if not cards[-2].is_honour and cards[-2].rank != 'T':
                 manager.set_even_odd(player.seat, trick.suit.name, 0)
                 return log(inspect.stack(), cards[-2])
             return log(inspect.stack(), cards[-1])
 
     manager.set_even_odd(player.seat, trick.suit.name, 1)
     return log(inspect.stack(), cards[-1])
```

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/first_seat.py` & `bfgcardplay-1.0.4/bfgcardplay/source/first_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer.py` & `bfgcardplay-1.0.4/bfgcardplay/source/first_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer_nt.py` & `bfgcardplay-1.0.4/bfgcardplay/source/first_seat_declarer_nt.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/first_seat_declarer_suit.py` & `bfgcardplay-1.0.4/bfgcardplay/source/first_seat_declarer_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/first_seat_defender.py` & `bfgcardplay-1.0.4/bfgcardplay/source/first_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat.py` & `bfgcardplay-1.0.4/bfgcardplay/source/fourth_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat_declarer.py` & `bfgcardplay-1.0.4/bfgcardplay/source/fourth_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/fourth_seat_defender.py` & `bfgcardplay-1.0.4/bfgcardplay/source/fourth_seat_defender.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,20 +50,32 @@
         unplayed_cards = player.total_unplayed_cards[trick.suit.name]
         if winning_card:
             value = winning_card.value
             play_winner = False
             while value > 1:
                 value -= 1
                 card = Card(CARD_VALUES[value], trick.suit.name)
-                if card in unplayed_cards and card not in player.dummys_unplayed_cards[trick.suit.name]:
+                if (card in unplayed_cards and
+                        card not in player.dummys_unplayed_cards[trick.suit.name]):
                     play_winner = True
                     break
             if play_winner:
                 return log(inspect.stack(), winning_card)
 
+        # Play low if higher card is winner after trick played
+        # losing_trick = (trick.cards[0].value > trick.cards[1].value or
+        #                     trick.cards[2].value > trick.cards[1].value)
+        # if len(cards) == 2 and losing_trick:
+        #     winner = True
+        #     for card in unplayed_cards:
+        #         if card.value > cards[0].value:
+        #             winner = False
+        #     if winner:
+        #         return log(inspect.stack(), cards[1])
+
         # Signal even/odd
         return get_hilo_signal_card(player, cards)
 
     def _select_card_if_void(self, player: Player, trick: Trick) -> Card:
         """Return card if cannot follow suit."""
         player.record_void(trick.suit)
         manager = global_vars.manager
```

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/manager.py` & `bfgcardplay-1.0.4/bfgcardplay/source/manager.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/opening_lead.py` & `bfgcardplay-1.0.4/bfgcardplay/source/opening_lead.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/opening_lead_card.py` & `bfgcardplay-1.0.4/bfgcardplay/source/opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/opening_lead_suit.py` & `bfgcardplay-1.0.4/bfgcardplay/source/opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/player.py` & `bfgcardplay-1.0.4/bfgcardplay/source/player.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/second_seat.py` & `bfgcardplay-1.0.4/bfgcardplay/source/second_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/second_seat_declarer.py` & `bfgcardplay-1.0.4/bfgcardplay/source/second_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/second_seat_defender.py` & `bfgcardplay-1.0.4/bfgcardplay/source/second_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/suggested_card.py` & `bfgcardplay-1.0.4/bfgcardplay/source/suggested_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/third_seat.py` & `bfgcardplay-1.0.4/bfgcardplay/source/third_seat.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/third_seat_declarer.py` & `bfgcardplay-1.0.4/bfgcardplay/source/third_seat_declarer.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/third_seat_defender.py` & `bfgcardplay-1.0.4/bfgcardplay/source/third_seat_defender.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/source/utilities.py` & `bfgcardplay-1.0.4/bfgcardplay/source/utilities.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/test/test_opening_lead_card.py` & `bfgcardplay-1.0.4/bfgcardplay/test/test_opening_lead_card.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay/test/test_opening_lead_suit.py` & `bfgcardplay-1.0.4/bfgcardplay/test/test_opening_lead_suit.py`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/bfgcardplay.egg-info/PKG-INFO` & `bfgcardplay-1.0.4/bfgcardplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 Metadata-Version: 2.1
 Name: bfgcardplay
-Version: 1.0.3
+Version: 1.0.4
 Summary: A collection of modules that facilitate cardplay in the BfG environment.
 Home-page: https://psionman@bitbucket.org/psionman/bfgcardplay.git
 Download-URL: https://pypi.org/project/bfgcardplay/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, duplicate bridge, contract bridge, hand, board, suit, auction, contract, card
 Description-Content-Type: text/markdown
 
  
 
 
 # Version History
 
+Version 1.0.4 20 Jun 2023
+
+1. xxx
+
+------
+
 Version 1.0.3 11 May 2023
 
 1. Correct manager.suit_to_develop
 
 ------
 
 Version 1.0.2 08 Mar 2023
```

### Comparing `bfgcardplay-1.0.3/bfgcardplay.egg-info/SOURCES.txt` & `bfgcardplay-1.0.4/bfgcardplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bfgcardplay-1.0.3/setup.py` & `bfgcardplay-1.0.4/setup.py`

 * *Files identical despite different names*

