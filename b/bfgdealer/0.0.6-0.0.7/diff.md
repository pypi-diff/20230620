# Comparing `tmp/bfgdealer-0.0.6.tar.gz` & `tmp/bfgdealer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfgdealer-0.0.6.tar", last modified: Sun Jun 18 12:51:47 2023, max compression
+gzip compressed data, was "bfgdealer-0.0.7.tar", last modified: Tue Jun 20 11:31:05 2023, max compression
```

## Comparing `bfgdealer-0.0.6.tar` & `bfgdealer-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 12:51:47.986682 bfgdealer-0.0.6/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.6/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1028 2023-06-18 12:51:47.986682 bfgdealer-0.0.6/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.6/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 12:51:47.983348 bfgdealer-0.0.6/bfgdealer/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.6/bfgdealer/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-18 12:50:16.000000 bfgdealer-0.0.6/bfgdealer/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 12:51:47.986682 bfgdealer-0.0.6/bfgdealer/source/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.6/bfgdealer/source/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    20266 2023-05-05 16:12:36.000000 bfgdealer-0.0.6/bfgdealer/source/board.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    10586 2023-05-05 16:12:36.000000 bfgdealer-0.0.6/bfgdealer/source/dealer.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    27873 2023-06-18 12:50:16.000000 bfgdealer-0.0.6/bfgdealer/source/dealer_duo.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.6/bfgdealer/source/dealer_engine.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)    14324 2023-05-05 16:12:36.000000 bfgdealer-0.0.6/bfgdealer/source/dealer_solo.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-18 12:51:47.983348 bfgdealer-0.0.6/bfgdealer.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1028 2023-06-18 12:51:47.000000 bfgdealer-0.0.6/bfgdealer.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-06-18 12:51:47.000000 bfgdealer-0.0.6/bfgdealer.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-18 12:51:47.000000 bfgdealer-0.0.6/bfgdealer.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-06-18 12:51:47.000000 bfgdealer-0.0.6/bfgdealer.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-18 12:51:47.986682 bfgdealer-0.0.6/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.6/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:31:05.398234 bfgdealer-0.0.7/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 bfgdealer-0.0.7/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1097 2023-06-20 11:31:05.398234 bfgdealer-0.0.7/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      141 2023-02-01 12:53:56.000000 bfgdealer-0.0.7/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:31:05.394901 bfgdealer-0.0.7/bfgdealer/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      548 2023-05-11 08:35:00.000000 bfgdealer-0.0.7/bfgdealer/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:31:05.398234 bfgdealer-0.0.7/bfgdealer/source/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-01-30 17:36:30.000000 bfgdealer-0.0.7/bfgdealer/source/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    22867 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/source/board.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     9879 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/source/dealer.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    28485 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/source/dealer_duo.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    17454 2023-02-01 13:02:59.000000 bfgdealer-0.0.7/bfgdealer/source/dealer_engine.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)    14271 2023-06-20 11:28:53.000000 bfgdealer-0.0.7/bfgdealer/source/dealer_solo.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-06-20 11:31:05.394901 bfgdealer-0.0.7/bfgdealer.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1097 2023-06-20 11:31:05.000000 bfgdealer-0.0.7/bfgdealer.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      395 2023-06-20 11:31:05.000000 bfgdealer-0.0.7/bfgdealer.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-06-20 11:31:05.000000 bfgdealer-0.0.7/bfgdealer.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       10 2023-06-20 11:31:05.000000 bfgdealer-0.0.7/bfgdealer.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-06-20 11:31:05.398234 bfgdealer-0.0.7/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1186 2023-02-01 12:55:15.000000 bfgdealer-0.0.7/setup.py
```

### Comparing `bfgdealer-0.0.6/LICENSE.txt` & `bfgdealer-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.6/PKG-INFO` & `bfgdealer-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.6
+Version: 0.0.7
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.7 20 Jun 2023
+
+1. Various refactor and Lucas 2s
+
+------
+
 Version 0.0.6 18 Jun 2023
 
 1. Multi-2D
 
 ------
```

### Comparing `bfgdealer-0.0.6/bfgdealer/__init__.py` & `bfgdealer-0.0.7/bfgdealer/__init__.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.6/bfgdealer/source/board.py` & `bfgdealer-0.0.7/bfgdealer/source/board.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 """
 
 from datetime import datetime
 import json
 from termcolor import cprint
 
 from bfgbidding import Player, Hand
-from bridgeobjects import (Board as bfg_Board, RANKS, SEATS, SUITS,
-                            parse_pbn, Contract,
-                            Auction, Trick)
-
+from bridgeobjects import (Board as bfg_Board, RANKS, SEATS, SUITS, SUIT_NAMES,
+                           parse_pbn, Contract, Call,
+                           Auction, Trick)
 
 MODULE_COLOUR = 'green'
-
 DEFAULT_SUIT_ORDER = ['S', 'H', 'C', 'D']
+SEPARATOR = 100
 
 
 class Board(bfg_Board):
     """Define BfG Board class."""
     def __init__(self, *args, **kwargs):
         super(Board, self).__init__(*args, **kwargs)
         self.auction = Auction()
@@ -31,16 +30,16 @@
         for index in range(4):
             self.players[index] = Player(self, None, index)
             self.players[SEATS[index]] = Player(self, None, index)
         self._dealer = None
         self.leader = None
         self.current_player = None
         self.current_trick = Trick()
-        self.unplayed_cards = {seat:[] for seat in SEATS}
-        self.hands = {seat:Hand() for seat in SEATS}
+        self.unplayed_cards = {seat: [] for seat in SEATS}
+        self.hands = {seat: Hand() for seat in SEATS}
         self.hand_cards = {seat: [card.name for card in self.hands[seat].cards] for seat in SEATS}
         self.unplayed_card_names = []
         self.current_player = ''
         self.NS_tricks = 0
         self.EW_tricks = 0
         self.score = 0
         self.suit_order = self._get_suit_order()
@@ -206,15 +205,14 @@
         """Create a deal from pbn_string."""
         pass
 
     def set_description(self, description):
         """Set the Board description."""
         self.description = description
 
-
     def get_auction(self, test=False):
         """Generate the auction."""
         if test:
             player_index = 0
         else:
             player_index = self.dealer_index
         auction_calls = []
@@ -229,23 +227,14 @@
         auction = Auction()
         auction.calls = auction_calls
         auction.first_caller = self.dealer
         self.bid_history = bid_history
         return auction
 
     @staticmethod
-    def three_final_passes(calls):
-        """Return True if there have been three consecutive passes."""
-        three_passes = False
-        if len(calls) >= 4:
-            if calls[-1].is_pass and calls[-2].is_pass and calls[-3].is_pass:
-                three_passes = True
-        return three_passes
-
-    @staticmethod
     def _default_hands():
         hands = []
         dummy_hand = ['AS', 'KS', 'QS', 'JS', 'TS', '9S', '8S',
                       '7S', '6S', '5S', '4S', '3S', '2S']
         hands.append(Hand(dummy_hand))
         dummy_hand = [hand.replace('S', 'H') for hand in dummy_hand]
         hands.append(Hand(dummy_hand))
@@ -253,26 +242,14 @@
         hands.append(Hand(dummy_hand))
         dummy_hand = [hand.replace('D', 'C') for hand in dummy_hand]
         hands.append(Hand(dummy_hand))
         return hands
 
     def parse_pbn_board(self, pbn_board, delimiter=":"):
         """Return a list of hands from a pbn deal string."""
-        # example deal
-        #   ['[Board "Board 1"]', '[Dealer "N"]',
-        #    '[Deal "N:JT84.A987.8.T982 AKQ.KQ54.KQ2.A76 7652.JT3.T9.KQJ5 93.62.AJ76543.43"]']
-        # hands = [None, None, None, None]
-        # # Assign hands to board in correct position
-        # self._dealer = deal[0]
-        # hand_index = self._get_pbn_dealer_index(deal)
-        # raw_hands = deal[2:].split(delimiter)
-        # for card_list in raw_hands:
-        #     hand = Hand(card_list)
-        #     hands[hand_index] = hand
-        #     hand_index = (hand_index + 1) % 4
         events = parse_pbn(pbn_board)
         board = events[0].boards[0]
         self.description = board.description
         self.dealer = board.dealer
         self.hands = {}
         for key, hand in board.hands.items():
             self.hands[key] = Hand(hand.cards)
@@ -329,25 +306,25 @@
         hands = board.hands
         for index in range(4):
             rotated_index = (index + increment) % 4
             if index in hands:
                 rotated_hands[rotated_index] = hands[index]
                 board.players[rotated_index].hand = hands[index]
             if SEATS[index] in hands:
-                rotated_hands[SEATS[rotated_index] ] = hands[SEATS[index]]
+                rotated_hands[SEATS[rotated_index]] = hands[SEATS[index]]
         board.hands = rotated_hands
         return board
 
     def get_contract(self):
         """Return a contract from the auction."""
         contract = Contract()
         if not self._auction:
             return contract
 
-        if not (self._three_final_passes(self._auction.calls) and
+        if not (self.three_final_passes(self._auction.calls) and
                 not self._passed_out(self._auction.calls)):
             return contract
 
         (call, modifier, declarer_partition) = self._analyse_auction()
 
         declarer_index = self._get_declarer_index(call, declarer_partition)
         declarer = SEATS[declarer_index]
@@ -374,28 +351,26 @@
             if (check_call.denomination == call.denomination and
                     (declarer_partition - index) % 2 == 0):
                 break
         dealer_index = SEATS.index(self.dealer)
         declarer_index = (dealer_index + index) % 4
         return declarer_index
 
-
-
     @staticmethod
     def _passed_out(calls):
         """Return True if the board has been passed out."""
         if len(calls) != 4:
             return False
         for call in calls:
             if not call.is_pass:
                 return False
         return True
 
     @staticmethod
-    def _three_final_passes(calls):
+    def three_final_passes(calls):
         """Return True if there have been three consecutive passes."""
         three_passes = False
         if len(calls) >= 4:
             if calls[-1].is_pass and calls[-2].is_pass and calls[-3].is_pass:
                 three_passes = True
         return three_passes
 
@@ -448,15 +423,15 @@
         self.max_suit_length = max_suit_length
         self.hand_suit_length = hand_suit_length
         self.current_player = self.current_player
         self.NS_tricks = self.NS_tricks
         self.EW_tricks = self.EW_tricks
         self.score = score
         context = {
-            'hand_cards': { seat: [card.name for card in self.hands[seat].cards] for seat in SEATS},
+            'hand_cards': {seat: [card.name for card in self.hands[seat].cards] for seat in SEATS},
             'unplayed_card_names': unplayed_cards,
             'max_suit_length': max_suit_length,
             'hand_suit_length': hand_suit_length,
             'current_player': self.current_player,
             'NS_tricks': self.NS_tricks,
             'EW_tricks': self.EW_tricks,
             # 'board_status': self.status,
@@ -490,15 +465,15 @@
                 suit_length.append(hand_for_shape.suit_length(suit))
             hand_suit_length[seat] = suit_length
             max_suit_length[seat] = hand_for_shape.shape[0]
         return (hand_suit_length, max_suit_length, unplayed_cards)
 
     def _get_suit_order(self):
         """Return a list of suit order."""
-        if self._three_passes():
+        if self.three_passes(self.bid_history):
             bid_history = self.bid_history[:-3]
             while bid_history and bid_history[-1] in ['D', 'R']:
                 bid_history = self.bid_history[:-1]
             contract = bid_history[-1]
             suit = contract[-1]
             if suit in DEFAULT_SUIT_ORDER:
                 if suit == 'S':
@@ -510,20 +485,21 @@
                 if suit == 'C':
                     return ['C', 'H', 'S', 'D']
             else:
                 return DEFAULT_SUIT_ORDER
         else:
             return DEFAULT_SUIT_ORDER
 
-    def _three_passes(self):
+    @staticmethod
+    def three_passes(bid_history: list[str]) -> bool:  # X
         """Return True if there are 3 passes."""
-        if len(self.bid_history) >= 4:
-            if (self.bid_history[-1] == 'P' and
-                    self.bid_history[-2] == 'P' and
-                    self.bid_history[-3] == 'P'):
+        if len(bid_history) >= 4:
+            if (bid_history[-1] == 'P' and
+                    bid_history[-2] == 'P' and
+                    bid_history[-3] == 'P'):
                 return True
         return False
 
     def _get_score(self):
         """Return the score for the board."""
         vulnerable = False
         if self.contract.declarer in 'NS':
@@ -531,7 +507,94 @@
             if self.vulnerable in ['NS', 'Both', 'All']:
                 vulnerable = True
         else:
             declarers_tricks = self.EW_tricks
             if self.vulnerable in ['EW', 'Both', 'All']:
                 vulnerable = True
         return self.contract.score(declarers_tricks, vulnerable)
+
+    def display_stats(self):
+        hand_card_dict = self._get_hand_card_dict()
+        # suits = [suit for suit in SUIT_NAMES]
+        # suits.reverse()
+        max_cards = self._get_suit_lengths(hand_card_dict)
+        auction = self.auction
+        if not self.auction.calls:
+            auction = self.get_auction([])
+        calls = [call.name for call in auction.calls]
+        contract = Contract('', '', auction)
+        self._display(hand_card_dict, max_cards, calls, contract)
+
+    def _display(self, hand_card_dict, max_cards, calls, contract):
+        cprint(f"{'='*SEPARATOR}", MODULE_COLOUR)
+        spades = f"{'S':-<{max_cards['S']}}"
+        hearts = f"{'H':-<{max_cards['H']}}"
+        diams = f"{'D':-<{max_cards['D']}}"
+        clubs = f"{'C':-<{max_cards['C']}}"
+        cprint(f"{' '} {spades} {hearts} {diams} {clubs}", MODULE_COLOUR)
+
+        for seat in range(4):
+            hand = self.hands[seat]
+            hand_cards = hand_card_dict[seat]
+            spades = f"{hand_cards['S']:<{max_cards['S']}}"
+            hearts = f"{hand_cards['H']:<{max_cards['H']}}"
+            clubs = f"{hand_cards['C']:<{max_cards['C']}}"
+            diams = f"{hand_cards['D']:<{max_cards['D']}}"
+            cards = f'{spades} {hearts} {diams} {clubs}'
+            hand_details = f'{SEATS[seat]} {cards} {hand.shape} {hand.hcp:>2}'
+            cprint(hand_details, MODULE_COLOUR)
+
+        cprint(f"{'-'*SEPARATOR}", MODULE_COLOUR)
+        cprint(f"Dealer: {self.dealer}", MODULE_COLOUR)
+
+        cprint(f"{', '.join(calls)}", MODULE_COLOUR)
+        cprint(f"{contract}", MODULE_COLOUR)
+        cprint(f"{'='*SEPARATOR}", MODULE_COLOUR)
+
+    def _get_hand_cards(self):
+        suits = [suit for suit in SUIT_NAMES]
+        suits.reverse()
+        hand_cards_list = self._sort_hand_cards()
+        hands = {}
+        for seat in range(4):
+            hand_cards = hand_cards_list[seat]
+            cards = {}
+            for suit in suits:
+                suit_cards = [card[0] for card in hand_cards if card[1] == suit]
+                cards[suit] = ('').join(suit_cards)
+            hands[seat] = cards
+        return hands
+
+    def _get_hand_card_dict(self):
+        hands = self._sort_hand_cards()
+        hand_card_dict = {}
+        for seat in range(4):
+            cards = {}
+            for suit in SUIT_NAMES:
+                card_list = []
+                for card in hands[seat]:
+                    if card[1] == suit:
+                        card_list.append(card[0])
+                cards[suit] = ''.join(card_list)
+            hand_card_dict[seat] = cards
+        return hand_card_dict
+
+    @staticmethod
+    def _get_suit_lengths(hands):
+        max_cards = {'S': 0, 'H': 0, 'D': 0, 'C': 0}
+        for seat in range(4):
+            cards = hands[seat]
+            for suit in SUIT_NAMES:
+                if len(cards[suit]) > max_cards[suit]:
+                    max_cards[suit] = len(cards[suit])
+        return max_cards
+
+    def _sort_hand_cards(self) -> list[str]:
+        hands = []
+        hand_cards = []
+        suit_order = self._get_suit_order()
+        for index in range(4):
+            hand = str(self.hands[index])
+            hands.append(hand.replace('Hand(', '').replace(')', '').replace('"', ''))
+            sorted_hand = Hand.sort_card_list(self.hands[index].cards, suit_order)
+            hand_cards.append([card.name for card in sorted_hand])
+        return hand_cards
```

### Comparing `bfgdealer-0.0.6/bfgdealer/source/dealer.py` & `bfgdealer-0.0.7/bfgdealer/source/dealer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """The dealer object for the bridgeobjects module."""
 
 import random
 from termcolor import cprint
 
-from bridgeobjects import (SEATS, SHAPES, BALANCED_SHAPES, Call)
-from bfgbidding import Bid
+from bridgeobjects import (SEATS, SHAPES, BALANCED_SHAPES)
 
 from .dealer_engine import DealerEngine
-from .board import Board, Auction
+from .board import Board
 
 
 MODULE_COLOUR = 'cyan'
 
+
 class Dealer(object):
     """The dealer object for the bridgeobjects module."""
     DEFAULT_POINTS_RANGE = [12, 14]
     #: the maximum number of points allowed in a hand
     MAX_POINTS = 26
 
     #: shapes suitable for single suited rebids
@@ -74,15 +74,15 @@
             seat = self.dealer
         else:
             seat = SEATS[random.choice(range(4))]
         valid_overcalls = False
         while not valid_overcalls:
             hands = {0: hand}
             board = self.engine.create_board_from_hands(hands, seat)
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             valid_overcalls = self._valid_overcalls(auction)
         return board
 
     def deal_balanced_hand(self, points_range=None):
         """Return a board with balanced hand in the given points range."""
         hand = self.engine.get_hand_from_points_and_shape(points_range,
                                                           BALANCED_SHAPES)
@@ -135,22 +135,22 @@
         return board
 
     def deal_opening_one_hand(self):
         """Return a hand suitable for an opening one."""
         get_hand = self.engine.get_hand_from_points_and_shape
         found = False
         loop = 0
-        openers_hand =  None
+        openers_hand = None
         while not found:
             loop += 1
             openers_hand = get_hand([12, 22])
             responders_hand = get_hand([0, 22], None, openers_hand)
             hands = {0: openers_hand, 2: responders_hand}
             board = self.engine.create_board_from_hands(hands)
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             openers_bid = auction[0]
             if openers_bid.level == 1 and self._valid_overcalls(auction):
                 found = True
         return openers_hand
 
     @staticmethod
     def _openers_bid(hand):
@@ -178,15 +178,14 @@
                 found = True
         hands = {0: openers_hand, 2: responders_hand}
         board = self.engine.create_board_from_hands(hands)
         return board
 
     def deal_defence_to_one_nt_board(self):
         """Return a board with 1NT opponents and positive response."""
-        dealer = random.choice([1, 3])
         openers_hand = self.deal_balanced_hand([12, 14])
         hands = {0: openers_hand}
         board = self.engine.create_board_from_hands(hands)
         found = False
         while not found:
             hand_one = board.hands[1]
             hand_three = board.hands[3]
@@ -210,34 +209,18 @@
                         result = True
                 elif second_bid.is_no_trumps:
                     result = True
             else:
                 result = False
         return result
 
-    def _generate_auction_calls(self, board):
+    def _get_auction_calls(self, board):
         """Return the auction calls as a list."""
-        board.auction = Auction()
-        player_index = SEATS.index(board.dealer)
-        board.auction.calls = []
-        while not self._three_passes(board.bid_history):
-            player = board.players[player_index]
-            bid = player.make_bid(board)
-            board.auction.calls.append(bid)
-            player_index = (player_index + 1) % 4
-        return board.auction.calls
-
-    @staticmethod
-    def _three_passes(calls):
-        """Return True if there have been three consecutive passes."""
-        three_passes = False
-        if len(calls) >= 4:
-            if calls[-3:] == ['P', 'P', 'P']:
-                three_passes = True
-        return three_passes
+        auction = board.get_auction()
+        return auction.calls
 
     def _valid_overcalls(self, auction):
         """Return True if the overcalls in the auction match self.allow_overcalls."""
         if self.allow_overcalls == 1:
             return True
         elif self.allow_overcalls == 0:
             return self._no_overcall_present(self._strip_auction(auction))
@@ -272,8 +255,8 @@
     def _overcall_present(auction):
         """Return True if there is an overcall in the auction."""
         value = False
         for call in auction[1::2]:
             if not call.is_pass:
                 value = True
                 break
-        return value
+        return value
```

### Comparing `bfgdealer-0.0.6/bfgdealer/source/dealer_duo.py` & `bfgdealer-0.0.7/bfgdealer/source/dealer_duo.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
             ('Take-out doubles', self.take_out_double_board),
             ('Defending against weak 1NT', self.defend_weak_nt_board),
             ('Fourth suit forcing', self.fourth_suit_forcing_board),
             ('Response to preemptive opening', self.respond_to_preempt_board),
             ('Defending preemptive opening', self.defend_preempt_board),
             ('Support for a minor', self.minor_support_board),
             ('Multi-2D', self.multi_two_diamond),
+            ('Lucas-2s', self.lucas_2s),
         ]
         self.generate_hand = self.engine.get_hand_from_points_and_shape
         self.create_board = self.engine.create_board_from_hands
         self.random_shape = self.engine.select_random_shape_from_list
         self._dealer = ''
 
     def get_set_hand(self, stages, dealer):
@@ -120,15 +121,15 @@
         """Deal a hand with slam potential."""
         found = False
         board = None
         while not found:
             hand = self.generate_hand([16, 35])
             hands = {self._first_seat(): hand}
             board = self.create_board(hands)
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if auction[-4].level >= 6:
                 found = True
         return board
 
     def jacoby_2nt_board(self):
         """
             Deal a hand with jacoby 2NT response.
@@ -149,40 +150,39 @@
                 continue
             if openers_hand.shape[0] == 4 and openers_hand.hcp <= 14:
                 continue
             board = self.create_board(hands)
 
             # board.dealer = self._dealer
             # cprint(f"{board.dealer}", MODULE_COLOUR)
-            auction = self._generate_auction_calls(board)
-            if self._dealer in 'EW': # and auction.calls[0].name != 'P':
-                auction_2 = self._generate_auction_calls(board)
-                # cprint(f"{board.dealer=}", MODULE_COLOUR)
-                # cprint(f"{auction}", MODULE_COLOUR)
-                # cprint(f"{auction_2}", 'green')
-                # continue
+            auction = self._get_auction_calls(board)
+            # if self._dealer in 'EW': # and auction.calls[0].name != 'P':
+            #     auction_2 = self._get_auction_calls(board)
+            #     cprint(f"{board.dealer=}", MODULE_COLOUR)
+            #     cprint(f"{auction}", MODULE_COLOUR)
+            #     cprint(f"{auction_2}", 'green')
+            #     continue
 
             partners_hand = board.hands[responder]
             if partners_hand.spades < 4 and partners_hand.hearts < 4:
                 continue
             if not (partners_hand.hcp >= 12 and partners_hand.shape[3] >= 2):
                 continue
             if self._four_of_openers_major(partners_hand, auction):
                 found = True
         return board
 
     @staticmethod
     def _four_of_openers_major(partner, auction):
         """Return True if hand has 4 of partner's major."""
         if ((auction[0].name == '1S' and partner.spades >= 4) or
-            (auction[0].name == '1H' and partner.hearts >= 4)):
+           (auction[0].name == '1H' and partner.hearts >= 4)):
             return True
         return False
 
-
     def negative_double_hand(self):
         """
             Deal a hand with negative double response.
 
             The negative double (aka "Sputnik") is a conventional double
             used by responder after opener starts the bidding with
             one-of-a-suit and the next player makes a suit overcall.
@@ -237,15 +237,15 @@
                                                             responders_hand):
                 continue
             found = True
         return board
 
     def _negative_double_auction(self, board):
         """Return the first two relevant bids in the auction."""
-        auction = self._generate_auction_calls(board)
+        auction = self._get_auction_calls(board)
         if board.dealer in ('N', 'S'):
             start = 0
         else:
             start = 1
         # openers_bid is the first bid on our side
         openers_bid = auction[start]
         overcallers_bid = auction[start+1]
@@ -263,23 +263,23 @@
             If both majors are bid, the double promises both minors.
             If a minor and a major are bid, the double promises the other major.
         """
         # Check S and a minor bid
         if ((openers_bid.denomination.name == 'S' and
                 overcallers_bid.denomination.is_minor) or
                 (overcallers_bid.denomination.name == 'S' and
-                openers_bid.denomination.is_minor) and
+                 openers_bid.denomination.is_minor) and
                 responders_hand.hearts != 4):
             return False
 
         # Check H and a minor bid
         if ((openers_bid.denomination.name == 'H' and
                 overcallers_bid.denomination.is_minor) or
                 (overcallers_bid.denomination.name == 'H' and
-                openers_bid.denomination.is_minor) and
+                 openers_bid.denomination.is_minor) and
                 responders_hand.spades != 4):
             return False
 
         # Check 2 minors bid
         if (openers_bid.denomination.is_minor and
                 overcallers_bid.denomination.is_minor and
                 (responders_hand.hearts != 4 or
@@ -328,15 +328,15 @@
             if responders_hand.hcp > 12:
                 continue
             if not 6 < responders_hand.losers < 8:
                 continue
             # print(responders_hand.losers)
 
             # Ensure N or S are the opener
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             openers_call = (opener - dealer_index) % 4
             if not self._opener_is_ns(auction, openers_call):
                 continue
 
             # Opener' call
             if not self._opener_is_suit_at_level_one(auction[openers_call]):
                 continue
@@ -357,15 +357,15 @@
     def _get_splinter_board(self, responders_min_hcp):
         """Return a board with suitable NS hands."""
         found = False
         while not found:
             openers_hand = self.generate_hand([12, 19])
             responders_hand_max = 34 - openers_hand.hcp
             responders_hand = self.generate_hand([0, responders_hand_max],
-                                            partners_hand=openers_hand)
+                                                 partners_hand=openers_hand)
             distribution_points = self._get_distribution_points(responders_hand)
             if responders_hand.hcp + distribution_points >= responders_min_hcp:
                 found = True
         # The first hand to bid on NS gets the opening hand.
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener=True)
         del check_bid
         hands = {
@@ -400,15 +400,15 @@
         while not found:
             (board, opener) = self._get_opener_overcaller_board(ns_opener=False)
             # Advancer's suit holding
             advancer = (opener + 3) % 4
             if board.hands[advancer].hcp < 10:
                 continue
 
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
 
             # Ensure that N/S pass if they are the opener.
             if self._dealer in ('N', 'S') and auction[0].name != 'P':
                 continue
 
             # Ensure E or W are the opener
             openers_call = (opener - dealer_index) % 4
@@ -450,22 +450,22 @@
             }
             # generate a new board where either N or S might be overcaller.
             board = self.create_board(hands)
             board.dealer = self._dealer
 
             # These checks seem to slow it down!
             # Responders hand
-            responder = (opener + 2) % 4
+            # responder = (opener + 2) % 4
             # responders_hand = board.hands[responder]
             # if responders_hand.hcp < 11:
             #     continue
             # if responders_hand.shape[2] < 3:
             #     continue
 
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
 
             # Ensure that N/S pass if they are the opener.
             if self._dealer in ('N', 'S') and auction[0].name != 'P':
                 continue
 
             # Ensure E or W are the opener
             openers_call = (opener - dealer_index) % 4
@@ -511,20 +511,20 @@
 
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener=False)
         del responder
         overcaller = (opener + 1) % 4
 
         while not found:
             hand = self.generate_hand([12, 14], BALANCED_SHAPES)
-            hands = {opener: hand,}
+            hands = {opener: hand}
             # generate a new board where E or W open 1NT.
             board = self.create_board(hands)
             board.dealer = self._dealer
 
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if auction[check_bid].name != '1NT':
                 found = False
             elif board.hands[overcaller].hcp < 9 or board.hands[overcaller].shape[0] < 5:
                 found = False
             else:
                 found = True
         return board
@@ -535,18 +535,18 @@
         board = None
 
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener=True)
         del responder
 
         while not found:
             hand = self.generate_hand([12, 19])
-            hands = {opener: hand,}
+            hands = {opener: hand}
             board = self.create_board(hands)
             board.dealer = self._dealer
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
 
             denominations = []
             nt_bid = False
             for index, call in enumerate(auction):
                 # Get a list of suits called in the auction by N/S
                 if not (index + check_bid) % 2:
                     if call.is_suit_call:
@@ -579,24 +579,24 @@
         else:
             points = [0, 9]
 
         (check_bid, opener, responder) = self._opener_given_dealer(ns_opener=True)
 
         while not found:
             openers_hand = self.generate_hand(points, [shape])
-            if openers_hand.suit_length(SUITS['C']) >=6:
+            if openers_hand.suit_length(SUITS['C']) >= 6:
                 continue
             responders_hand = self.generate_hand([14, 25], partners_hand=openers_hand)
             hands = {
                 opener: openers_hand,
                 responder: responders_hand,
                 }
             board = self.create_board(hands)
             board.dealer = self._dealer
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
 
             # Check first bid is valid
             call = auction[check_bid]
             if call.level in (2, 3, 4):
                 found = True
         return board
 
@@ -622,19 +622,19 @@
             responders_hand = self.generate_hand([0, 8], partners_hand=openers_hand)
             hands = {
                 opener: openers_hand,
                 responder: responders_hand,
                 }
             board = self.create_board(hands)
             board.dealer = self._dealer
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
 
             # Check first bid is valid
             if check_bid:
-                if auction[0].name  != 'P':
+                if auction[0].name != 'P':
                     continue
             if auction[check_bid].level in (2, 3, 4):
                 found = True
         return board
 
     def minor_support_board(self):
         """Minor support look for NT."""
@@ -648,43 +648,59 @@
             responders_hand = self.generate_hand(responders_points, partners_hand=openers_hand)
             hands = {
                 opener: openers_hand,
                 responder: responders_hand,
                 }
             board = self.create_board(hands)
             board.dealer = self._dealer
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
 
             # Check first bid is valid
             if check_bid:
                 if auction[0].name != 'P':
                     continue
             if auction[check_bid].is_minor:
                 suit = auction[check_bid].denomination.name
                 if responders_hand.suit_holding[suit] >= 4:
                     found = True
         return board
 
     def multi_two_diamond(self):
-        """Return 19-20 balanced or weak 5/4."""
+        """Return 19-20 balanced or weak 6 card major."""
         choice = random.randint(0, 1)
         if choice == 0:
             hand = self.generate_hand([19, 20], BALANCED_SHAPES)
         else:
             found = False
-            hand = None
             while not found:
                 hand = self.generate_hand([6, 10])
-                if hand.spades >= 5 or hand.hearts >= 5:
-                    if hand.shape[0] == 5 and hand.shape[1] == 4:
-                        found = True
+                if hand.spades == 6 or hand.hearts == 6:
+                    found = True
         hands = {self._first_seat(): hand}
         board = self.create_board(hands)
         return board
 
+    def lucas_2s(self):
+        """Generate hand suitable for Lucas 2 opening."""
+        found = False
+        while not found:
+            hand = self.generate_hand([6, 10])
+            if hand.spades == 5 or hand.hearts == 5:
+                if hand.shape[1] == 4:
+                    hands = {self._first_seat(): hand}
+                    board = self.create_board(hands)
+                    board.dealer = self._dealer
+                    auction = self._get_auction_calls(board)
+                    if board.dealer in 'NS':
+                        found = True
+                    else:
+                        if auction[0].name == 'P':
+                            found = True
+        return board
+
     def _opener_given_dealer(self, ns_opener):
         """Return the seat indices given dealer and opener orientation."""
         # E.g if we want N or S to bid and E is dealer then the opener will be S.
         # If on the other hand W is dealer, the opener will be N.
 
         # check_bid returns True (1) if N/S are to be opener and E/W are dealer
         # or if E/W are to be opener and N/S are dealer
```

### Comparing `bfgdealer-0.0.6/bfgdealer/source/dealer_engine.py` & `bfgdealer-0.0.7/bfgdealer/source/dealer_engine.py`

 * *Files identical despite different names*

### Comparing `bfgdealer-0.0.6/bfgdealer/source/dealer_solo.py` & `bfgdealer-0.0.7/bfgdealer/source/dealer_solo.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 from bridgeobjects import SEATS, BALANCED_SHAPES, SEMI_BALANCED_SHAPES, Call
 
 from .dealer import Dealer as DealerBase, Board
 
 MODULE_COLOUR = 'green'
 
+
 class Dealer(DealerBase):
     """Generate deals for Solo stages."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
         self.set_hands = [
@@ -43,15 +44,15 @@
         board = None
         while not found:
             loop += 1
             openers_hand = self.generate_hand([12, 22])
             hands = {seat_index: openers_hand}
             board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if auction[0].level == 1 and self._valid_overcalls(auction):
                 found = True
         return board
 
     def limit_bids_responder_board(self, seat_index):
         """Return a board suitable for limited responses to opener."""
         found = False
@@ -65,15 +66,15 @@
                 responders_hand = self._deal_limit_bids_responder_nt(openers_hand)
             else:
                 responders_hand = self._deal_limit_bids_responder_support(openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
             board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if self._valid_overcalls(auction):
                 found = True
         return board
 
     def _deal_limit_bids_responder_nt(self, openers_hand):
         """Return a hand suitable for an NT response after opening one."""
         shapes = BALANCED_SHAPES.extend(SEMI_BALANCED_SHAPES)
@@ -114,15 +115,15 @@
             loop += 1
             openers_hand = get_hand([15, 19], BALANCED_SHAPES)
             responders_hand = get_hand([3, 20], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
             board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if len(auction) >= 5:
                 openers_bid = auction[0]
                 responders_bid = auction[2]
                 if (openers_bid.denomination != responders_bid.denomination and
                         not responders_bid.is_no_trumps):
                     if self._valid_overcalls(auction):
                         found = True
@@ -138,15 +139,15 @@
             loop += 1
             openers_hand = get_hand([12, 19], self.SINGLE_SUITED_SHAPES)
             responders_hand = get_hand([6, 15], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
             board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if len(auction) >= 5:
                 openers_bid_one = auction[0]
                 responders_bid = auction[2]
                 openers_bid_two = auction[4]
                 if (openers_bid_one.denomination == openers_bid_two.denomination and
                         responders_bid.denomination != openers_bid_one.denomination and
                         responders_bid.denomination != openers_bid_two.denomination):
@@ -162,15 +163,15 @@
         while not found:
             openers_hand = get_hand([12, 19], self.TWO_SUITED_SHAPES)
             responders_hand = get_hand([6, 15], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
             board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             openers_bid_one = auction[0]
             if len(auction) >= 5:
                 openers_bid_two = auction[4]
             else:
                 # dummy inserted to ensure a 2 level bid
                 openers_bid_two = Call('2C')
             responders_bid = auction[2]
@@ -210,15 +211,15 @@
         while not found:
             loop += 1
             responders_hand = get_hand([6, 16], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
             board = self.create_board(hands, SEATS[seat_index])
             board.dealer = SEATS[seat_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             openers_bid = auction[0]
             responders_bid = auction[2]
             if responders_bid.is_suit_call:
                 if self._valid_overcalls(auction):
                     responders_suit = responders_bid.denomination
                     if (openers_bid.denomination != responders_suit and
                             openers_hand.suit_holding[responders_suit] >= 4):
@@ -236,15 +237,15 @@
         while not found:
             loop += 1
             responders_hand = get_hand([6, 16], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
             board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             openers_bid = auction[0]
             responders_bid = auction[2]
             if responders_bid.is_suit_call:
                 if self._valid_overcalls(auction):
                     responders_suit = responders_bid.denomination
                     if openers_bid.denomination != responders_suit:
                         found = True
@@ -260,15 +261,15 @@
             loop += 1
             openers_hand = get_hand([12, 19], SEMI_BALANCED_SHAPES)
             responders_hand = get_hand([6, 16], BALANCED_SHAPES, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {seat_index: openers_hand, partners_index: responders_hand}
             board = self.create_board(hands)
             board.dealer = SEATS[seat_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if len(auction) >= 5:
                 openers_bid = auction[0]
                 responders_bid = auction[2]
                 openers_rebid = auction[4]
                 if (openers_bid.is_suit_call and
                         responders_bid.is_no_trumps and
                         openers_rebid.is_no_trumps):
@@ -286,15 +287,15 @@
             loop += 1
             openers_hand = get_hand([6, 10], self.WEAK_TWO_SHAPES)
             responders_hand = get_hand([12, 19], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
             board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             openers_bid = auction[0]
             if openers_bid.level == 2:
                 if self._valid_overcalls(auction):
                     found = True
         return board
 
     def response_to_two_nt_board(self, seat_index):
@@ -307,15 +308,15 @@
             loop += 1
             openers_hand = get_hand([20, 22], BALANCED_SHAPES)
             responders_hand = get_hand([0, 12], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
             board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if self._valid_overcalls(auction):
                 found = True
         return board
 
     def response_to_two_clubs_board(self, seat_index):
         """Return a board requiring a response to two clubs opening."""
         get_hand = self.generate_hand
@@ -326,11 +327,11 @@
             loop += 1
             openers_hand = get_hand([23, 30])
             responders_hand = get_hand([0, 12], None, openers_hand)
             partners_index = (seat_index + 2) % 4
             hands = {partners_index: openers_hand, seat_index: responders_hand}
             board = self.create_board(hands, SEATS[partners_index])
             board.dealer = SEATS[partners_index]
-            auction = self._generate_auction_calls(board)
+            auction = self._get_auction_calls(board)
             if self._valid_overcalls(auction):
                 found = True
-        return board
+        return board
```

### Comparing `bfgdealer-0.0.6/bfgdealer.egg-info/PKG-INFO` & `bfgdealer-0.0.7/bfgdealer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bfgdealer
-Version: 0.0.6
+Version: 0.0.7
 Summary: """A collection of modules that supports dealing Bid for Game applications."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: bridge, dealing
@@ -20,14 +20,20 @@
 ```bash
 pip install bfgdealer
 ```
 
 
 # Version History
 
+Version 0.0.7 20 Jun 2023
+
+1. Various refactor and Lucas 2s
+
+------
+
 Version 0.0.6 18 Jun 2023
 
 1. Multi-2D
 
 ------
```

### Comparing `bfgdealer-0.0.6/setup.py` & `bfgdealer-0.0.7/setup.py`

 * *Files identical despite different names*

