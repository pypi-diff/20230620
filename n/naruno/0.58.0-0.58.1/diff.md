# Comparing `tmp/naruno-0.58.0.tar.gz` & `tmp/naruno-0.58.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno-0.58.0.tar", last modified: Mon May 22 16:17:57 2023, max compression
+gzip compressed data, was "naruno-0.58.1.tar", last modified: Tue Jun 20 12:51:03 2023, max compression
```

## Comparing `naruno-0.58.0.tar` & `naruno-0.58.1.tar`

### file list

```diff
@@ -1,302 +1,302 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.877287 naruno-0.58.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-22 16:17:45.000000 naruno-0.58.0/LICENCE-naruno-gui_lib__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-22 16:17:45.000000 naruno-0.58.0/LICENCE-naruno-lib-mix__.md
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-22 16:17:45.000000 naruno-0.58.0/LICENCE-naruno-wallet-elipticcurve__.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-22 16:17:45.000000 naruno-0.58.0/LICENSE-others__.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 16:17:45.000000 naruno-0.58.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-22 16:17:57.877287 naruno-0.58.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-22 16:17:45.000000 naruno-0.58.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.849286 naruno-0.58.0/naruno/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.849286 naruno-0.58.0/naruno/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/accounts/account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.849286 naruno-0.58.0/naruno/accounts/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/accounts/commanders/delete_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/accounts/commanders/get_comnder.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/accounts/commanders/save_commander.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/accounts/get_accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/accounts/get_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/accounts/get_sequence_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/accounts/save_accounts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.849286 naruno-0.58.0/naruno/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.849286 naruno-0.58.0/naruno/api/buildozer/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/api/buildozer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    26091 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/api/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.849286 naruno-0.58.0/naruno/apps/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/apps/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)    29108 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/apps/remote_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.841286 naruno-0.58.0/naruno/blockchain/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/blockchain/block/
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/block_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/change_transaction_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/create_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/get_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/get_block_from_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/get_minumum_transfer_amount.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/blockchain/block/hash/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/hash/accounts_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/hash/blocks_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/hash/calculate_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/hash/tx_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/just_one_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/max_data_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/max_tx_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/save_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/save_block_to_blockchain_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/block/shares.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/blockchain/candidate_block/
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/blockchain/candidate_block/candidate_block_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/cli/
--rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/consensus_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/finished/
--rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/finished/finished_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/finished/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/finished/transactions/transactions_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/finished/true_time/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/finished/true_time/true_time_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/ongoing/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/ongoing/ongoing_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.845286 naruno-0.58.0/naruno/consensus/rounds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.841286 naruno-0.58.0/naruno/consensus/rounds/round_1/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/process/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/checks/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_1/round_1_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_2/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_2/checks/checks_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.845286 naruno-0.58.0/naruno/consensus/rounds/round_2/checks/time/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_2/checks/time/time_difference/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_2/process/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_2/process/process_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_2/process/rescue/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.853286 naruno-0.58.0/naruno/consensus/rounds/round_2/process/validate/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/rounds/round_2/round_2_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/consensus/sync/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/sync/send_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/sync/send_block_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/consensus/sync/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/blocks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/commanders/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/commanders/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/connected_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/connected_nodes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/connected_nodes_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/connected_nodes_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/connected_nodes_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/connected_nodes_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/connected_nodes_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/connected_nodes_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/extracted_proofs/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/extracted_proofs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/my_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/pending_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/pending_transactions/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/pending_transactions_test_0/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/pending_transactions_test_0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/pending_transactions_test_1/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/pending_transactions_test_1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/pending_transactions_test_2/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/pending_transactions_test_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/proof/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/proof/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/qrs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/qrs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/remote_app_cache/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/remote_app_cache/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/signs/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/signs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_consensus_trigger_finished/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_consensus_trigger_finished/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_finished_main/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_finished_main/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_finished_main_2/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_finished_main_2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_finished_main_3/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_finished_main_3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_finished_main_false_time/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_finished_main_false_time/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_finished_main_no_reset/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_finished_main_no_reset/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/db/test_proof_extracted/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/db/test_proof_extracted/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.857286 naruno-0.58.0/naruno/gui/
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui/popup.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui/the_naruno_gui_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.845286 naruno-0.58.0/naruno/gui_lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.865286 naruno-0.58.0/naruno/gui_lib/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/POPPINS_LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Black.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Light.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-LightItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Medium.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-SemiBold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Thin.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.865286 naruno-0.58.0/naruno/gui_lib/images/
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/images/logo.ico
--rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/images/logo_sm_orb_fw.png
--rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/images/logo_w_bc.png
--rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/images/logo_win.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.845286 naruno-0.58.0/naruno/gui_lib/libs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.865286 naruno-0.58.0/naruno/gui_lib/libs/baseclass/
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/baseclass/node_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/baseclass/operations_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/baseclass/root_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/baseclass/settings_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/baseclass/tabnavigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/baseclass/wallet_screen.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/baseclass/welcome_screen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.865286 naruno-0.58.0/naruno/gui_lib/libs/kv/
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/kv/node_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/kv/operations_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/kv/root_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/kv/settings_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/kv/tabnavigation.kv
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/kv/wallet_screen.kv
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/gui_lib/libs/kv/welcome_screen.kv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/lib/backup/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/backup/naruno_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/backup/naruno_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/clean_up.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/config_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/lib/mix/
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/mix/merkle_root.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/mix/mixlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/lib/performance_analyzers/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/performance_analyzers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/performance_analyzers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/performance_analyzers/blockshash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/performance_analyzers/blockshash_part.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/performance_analyzers/heartbeat_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/performance_analyzers/transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/perpetualtimer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/qr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/safety.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/settings_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/sign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/lib/verify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/logs/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/logs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/node/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/node/client/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/node/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/node/get_candidate_blocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/node/server/
--rw-r--r--   0 runner    (1001) docker     (123)    29480 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/node/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/node/unl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/transactions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.869286 naruno-0.58.0/naruno/transactions/check/
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/check/check_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/transactions/check/datas/
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/check/datas/check_datas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/transactions/check/len/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/check/len/check_len.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/transactions/check/sign/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/check/sign/check_sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/transactions/check/type/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/check/type/check_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/get_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/transactions/my_transactions/
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/my_transactions/check_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/my_transactions/get_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/my_transactions/get_proof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/my_transactions/save_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/my_transactions/save_to_my_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/my_transactions/sended_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/my_transactions/validate_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/transactions/pending/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/pending/delete_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/pending/get_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/pending/save_pending.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/pending_to_validating.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/print_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/process_the_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/send.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/transactions/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/wallet/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/delete_current_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/wallet/ellipticcurve/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/ecdsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/math.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/privateKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/publicKey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/signature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.873287 naruno-0.58.0/naruno/wallet/ellipticcurve/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/utils/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/utils/der.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/utils/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/utils/oid.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/ellipticcurve/utils/pem.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/get_saved_wallet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/print_wallets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/save_wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/wallet_create.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/wallet_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/wallet_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-22 16:17:45.000000 naruno-0.58.0/naruno/wallet/wallet_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:17:57.849286 naruno-0.58.0/naruno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-05-22 16:17:57.000000 naruno-0.58.0/naruno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-22 16:17:57.000000 naruno-0.58.0/naruno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:17:57.000000 naruno-0.58.0/naruno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 16:17:57.000000 naruno-0.58.0/naruno.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 16:17:57.000000 naruno-0.58.0/naruno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:17:57.877287 naruno-0.58.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 16:17:45.000000 naruno-0.58.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.410224 naruno-0.58.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-06-20 12:50:53.000000 naruno-0.58.1/LICENCE-naruno-gui_lib__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-20 12:50:53.000000 naruno-0.58.1/LICENCE-naruno-lib-mix__.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 12:50:53.000000 naruno-0.58.1/LICENCE-naruno-wallet-elipticcurve__.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-20 12:50:53.000000 naruno-0.58.1/LICENSE-others__.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-20 12:50:53.000000 naruno-0.58.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-20 12:51:03.410224 naruno-0.58.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-06-20 12:50:53.000000 naruno-0.58.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.386223 naruno-0.58.1/naruno/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/accounts/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/accounts/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/accounts/commanders/delete_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/accounts/commanders/get_comnder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/accounts/commanders/save_commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/accounts/get_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/accounts/get_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/accounts/get_sequence_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/accounts/save_accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/api/buildozer/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/api/buildozer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26091 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/api/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/apps/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29108 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/apps/remote_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.382223 naruno-0.58.1/naruno/blockchain/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/blockchain/block/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/block_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/change_transaction_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/create_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/get_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/get_block_from_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/get_minumum_transfer_amount.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/blockchain/block/hash/
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/hash/accounts_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/hash/blocks_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/hash/calculate_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/hash/tx_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/just_one_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/max_data_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/max_tx_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13888 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/save_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/save_block_to_blockchain_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/block/shares.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/blockchain/candidate_block/
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/blockchain/candidate_block/candidate_block_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/consensus_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/finished/
+-rw-r--r--   0 runner    (1001) docker     (123)     7333 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/finished/finished_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/finished/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/finished/transactions/transactions_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/finished/true_time/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/finished/true_time/true_time_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/ongoing/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/ongoing/ongoing_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.382223 naruno-0.58.1/naruno/consensus/rounds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/rounds/round_1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/rounds/round_1/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.382223 naruno-0.58.1/naruno/consensus/rounds/round_1/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/rounds/round_1/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/rounds/round_1/process/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.390224 naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/checks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_1/round_1_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_2/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_2/checks/checks_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.382223 naruno-0.58.1/naruno/consensus/rounds/round_2/checks/time/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_2/checks/time/time_difference/
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_2/process/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_2/process/process_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_2/process/rescue/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/rounds/round_2/process/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_2/process/validate/validate_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/rounds/round_2/round_2_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/consensus/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/sync/send_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/sync/send_block_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/consensus/sync/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/blocks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/commanders/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/commanders/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/connected_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/connected_nodes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/connected_nodes_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/connected_nodes_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/connected_nodes_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/connected_nodes_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/connected_nodes_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/connected_nodes_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/extracted_proofs/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/extracted_proofs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/my_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/pending_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/pending_transactions/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/pending_transactions_test_0/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/pending_transactions_test_0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/pending_transactions_test_1/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/pending_transactions_test_1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/pending_transactions_test_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/pending_transactions_test_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/proof/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/proof/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/qrs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/qrs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/remote_app_cache/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/remote_app_cache/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/signs/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/signs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_SaveBlockstoBlockchainDB_GetBlockstoBlockchainDB_not_our_transaction/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_consensus_trigger_finished/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_consensus_trigger_finished/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_finished_main/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_finished_main/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_finished_main_2/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_finished_main_2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_finished_main_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_finished_main_3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_finished_main_false_time/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_finished_main_false_time/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_finished_main_no_reset/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_finished_main_no_reset/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.394224 naruno-0.58.1/naruno/db/test_proof_extracted/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/db/test_proof_extracted/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.398224 naruno-0.58.1/naruno/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.386223 naruno-0.58.1/naruno/gui/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.402224 naruno-0.58.1/naruno/gui/lib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/POPPINS_LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)   151396 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Black.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   171604 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   153944 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   176588 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   152764 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   173916 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161456 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   186168 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   182012 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   159892 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Light.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   184460 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-LightItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   156520 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Medium.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   180444 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   158240 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   155232 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-SemiBold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   178584 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   161652 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Thin.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   187044 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.402224 naruno-0.58.1/naruno/gui/lib/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/images/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    19780 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16238 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/images/logo_sm_orb_fw.png
+-rw-r--r--   0 runner    (1001) docker     (123)    21468 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/images/logo_w_bc.png
+-rw-r--r--   0 runner    (1001) docker     (123)   254014 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/images/logo_win.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.386223 naruno-0.58.1/naruno/gui/lib/libs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.402224 naruno-0.58.1/naruno/gui/lib/libs/baseclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/baseclass/node_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/baseclass/operations_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/baseclass/root_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/baseclass/settings_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/baseclass/tabnavigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/baseclass/wallet_screen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/baseclass/welcome_screen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.402224 naruno-0.58.1/naruno/gui/lib/libs/kv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/kv/node_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/kv/operations_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/kv/root_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/kv/settings_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/kv/tabnavigation.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/kv/wallet_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/lib/libs/kv/welcome_screen.kv
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/popup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/gui/the_naruno_gui_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/lib/backup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/backup/naruno_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/backup/naruno_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/clean_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/config_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/lib/mix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/mix/merkle_root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/mix/mixlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/lib/performance_analyzers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/performance_analyzers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/performance_analyzers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/performance_analyzers/blockshash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/performance_analyzers/blockshash_part.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/performance_analyzers/heartbeat_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/performance_analyzers/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/perpetualtimer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/qr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/safety.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/settings_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/sign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/lib/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/logs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/node/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/node/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/node/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/node/get_candidate_blocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/node/server/
+-rw-r--r--   0 runner    (1001) docker     (123)    29480 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/node/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/node/unl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/transactions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/transactions/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/check/check_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/transactions/check/datas/
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/check/datas/check_datas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/transactions/check/len/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/check/len/check_len.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/transactions/check/sign/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/check/sign/check_sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/transactions/check/type/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/check/type/check_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/get_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.406224 naruno-0.58.1/naruno/transactions/my_transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/my_transactions/check_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/my_transactions/get_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/my_transactions/get_proof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/my_transactions/save_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/my_transactions/save_to_my_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/my_transactions/sended_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/my_transactions/validate_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.410224 naruno-0.58.1/naruno/transactions/pending/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/pending/delete_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/pending/get_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/pending/save_pending.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/pending_to_validating.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/print_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/process_the_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/transactions/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.410224 naruno-0.58.1/naruno/wallet/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/delete_current_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.410224 naruno-0.58.1/naruno/wallet/ellipticcurve/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/ecdsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5022 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/privateKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/publicKey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/signature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.410224 naruno-0.58.1/naruno/wallet/ellipticcurve/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/utils/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/utils/der.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/utils/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/utils/oid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/ellipticcurve/utils/pem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/get_saved_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/print_wallets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/save_wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/wallet_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/wallet_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/wallet_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-20 12:50:53.000000 naruno-0.58.1/naruno/wallet/wallet_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:51:03.386223 naruno-0.58.1/naruno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-20 12:51:03.000000 naruno-0.58.1/naruno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-06-20 12:51:03.000000 naruno-0.58.1/naruno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:51:03.000000 naruno-0.58.1/naruno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 12:51:03.000000 naruno-0.58.1/naruno.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 12:51:03.000000 naruno-0.58.1/naruno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 12:51:03.410224 naruno-0.58.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-20 12:50:53.000000 naruno-0.58.1/setup.py
```

### Comparing `naruno-0.58.0/LICENCE-naruno-gui_lib__.md` & `naruno-0.58.1/LICENCE-naruno-gui_lib__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/LICENCE-naruno-lib-mix__.md` & `naruno-0.58.1/LICENCE-naruno-lib-mix__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/LICENCE-naruno-wallet-elipticcurve__.md` & `naruno-0.58.1/LICENCE-naruno-wallet-elipticcurve__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/LICENSE-others__.md` & `naruno-0.58.1/LICENSE-others__.md`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/PKG-INFO` & `naruno-0.58.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.58.0
+Version: 0.58.1
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.58.0 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.58.1 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.58.0/README.md` & `naruno-0.58.1/README.md`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/accounts/account.py` & `naruno-0.58.1/naruno/accounts/account.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/accounts/commanders/delete_commander.py` & `naruno-0.58.1/naruno/accounts/commanders/delete_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/accounts/commanders/get_comnder.py` & `naruno-0.58.1/naruno/accounts/commanders/get_comnder.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/accounts/commanders/save_commander.py` & `naruno-0.58.1/naruno/accounts/commanders/save_commander.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/accounts/get_accounts.py` & `naruno-0.58.1/naruno/accounts/get_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/accounts/get_balance.py` & `naruno-0.58.1/naruno/accounts/get_balance.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
                 return None
 
         balance = -block.minumum_transfer_amount
 
         the_account_list = GetAccounts(
         ) if account_list is None else account_list
         the_account_list.execute(
-            f"SELECT * FROM account_list WHERE address = '{address}'")
+            f"SELECT * FROM account_list WHERE address = ?", (address,))
         for row in the_account_list.fetchall():
             balance += row[2]
             break
         if not block.just_one_tx:
             for tx in block.validating_list + GetPending():
                 if Address(tx.fromUser) == user:
                     balance -= float(tx.amount) + float(tx.transaction_fee)
```

### Comparing `naruno-0.58.0/naruno/accounts/get_sequence_number.py` & `naruno-0.58.1/naruno/accounts/get_sequence_number.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 def GetSequanceNumber(user, account_list=None, dont_convert=False, block=None):
     user = Address(user) if not dont_convert else user
     sequence_number = 0
     the_account_list = GetAccounts() if account_list is None else account_list
     the_account_list.execute(
-        f"SELECT * FROM account_list WHERE address = '{user}'")
+        f"SELECT * FROM account_list WHERE address = ?", (user,))
     for Accounts in the_account_list.fetchall():
         sequence_number = Accounts[1]
         break
     if block is not None:
         if not block.just_one_tx:
             for tx in block.validating_list + GetPending():
                 if Address(tx.fromUser) == user:
```

### Comparing `naruno-0.58.0/naruno/accounts/save_accounts.py` & `naruno-0.58.1/naruno/accounts/save_accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/api/buildozer/main.py` & `naruno-0.58.1/naruno/api/buildozer/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/api/main.py` & `naruno-0.58.1/naruno/api/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/apps/checker.py` & `naruno-0.58.1/naruno/apps/checker.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/apps/remote_app.py` & `naruno-0.58.1/naruno/apps/remote_app.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/block_main.py` & `naruno-0.58.1/naruno/blockchain/block/block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/blocks_hash.py` & `naruno-0.58.1/naruno/blockchain/block/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/change_transaction_fee.py` & `naruno-0.58.1/naruno/blockchain/block/change_transaction_fee.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/create_block.py` & `naruno-0.58.1/naruno/blockchain/block/create_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/get_block.py` & `naruno-0.58.1/naruno/blockchain/block/get_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/get_block_from_blockchain_db.py` & `naruno-0.58.1/naruno/blockchain/block/get_block_from_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/get_minumum_transfer_amount.py` & `naruno-0.58.1/naruno/blockchain/block/get_minumum_transfer_amount.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/hash/accounts_hash.py` & `naruno-0.58.1/naruno/blockchain/block/hash/accounts_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/hash/blocks_hash.py` & `naruno-0.58.1/naruno/blockchain/block/hash/blocks_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/hash/calculate_hash.py` & `naruno-0.58.1/naruno/blockchain/block/hash/calculate_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/hash/tx_hash.py` & `naruno-0.58.1/naruno/blockchain/block/hash/tx_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/just_one_tx.py` & `naruno-0.58.1/naruno/blockchain/block/just_one_tx.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/max_data_size.py` & `naruno-0.58.1/naruno/blockchain/block/max_data_size.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/max_tx_number.py` & `naruno-0.58.1/naruno/blockchain/block/max_tx_number.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/save_block.py` & `naruno-0.58.1/naruno/blockchain/block/save_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/save_block_to_blockchain_db.py` & `naruno-0.58.1/naruno/blockchain/block/save_block_to_blockchain_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/block/shares.py` & `naruno-0.58.1/naruno/blockchain/block/shares.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/blockchain/candidate_block/candidate_block_main.py` & `naruno-0.58.1/naruno/blockchain/candidate_block/candidate_block_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/cli/main.py` & `naruno-0.58.1/naruno/cli/main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/config.py` & `naruno-0.58.1/naruno/config.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/consensus_main.py` & `naruno-0.58.1/naruno/consensus/consensus_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/finished/finished_main.py` & `naruno-0.58.1/naruno/consensus/finished/finished_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/finished/transactions/transactions_main.py` & `naruno-0.58.1/naruno/consensus/finished/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/finished/true_time/true_time_main.py` & `naruno-0.58.1/naruno/consensus/finished/true_time/true_time_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/ongoing/ongoing_main.py` & `naruno-0.58.1/naruno/consensus/ongoing/ongoing_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/checks/candidate_blocks/candidate_blocks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/checks/checks_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/process/process_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/checks/duplicated.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/find_newly/find_newly_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/find_validated/find_validated_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/process/transactions/transactions_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_1/round_1_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_1/round_1_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_2/checks/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_2/checks/checks_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_2/checks/checks_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_2/checks/time/time_difference/time_difference_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_2/process/candidate_blocks_hashes/candidate_blocks_hashes_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_2/process/process_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_2/process/process_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_2/process/rescue/rescue_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_2/process/validate/validate_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_2/process/validate/validate_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/rounds/round_2/round_2_main.py` & `naruno-0.58.1/naruno/consensus/rounds/round_2/round_2_main.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/sync/send_block.py` & `naruno-0.58.1/naruno/consensus/sync/send_block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/sync/send_block_hash.py` & `naruno-0.58.1/naruno/consensus/sync/send_block_hash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/consensus/sync/sync.py` & `naruno-0.58.1/naruno/consensus/sync/sync.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui/main.py` & `naruno-0.58.1/naruno/gui/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,27 @@
 from naruno.lib.safety import safety_check
 from naruno.lib.settings_system import the_settings
 
 Config.set("graphics", "width", "700")
 Config.set("graphics", "height", "450")
 Config.set("graphics", "minimum_width", "700")
 Config.set("graphics", "minimum_height", "450")
-Config.set("input", "mouse", "mouse,disable_multitouch")
 
 os.environ["NARUNO_ROOT"] = get_config()["main_folder"]
 
-KV_DIR = f"{os.environ['NARUNO_ROOT']}/gui_lib/libs/kv/"
+KV_DIR = f"{os.environ['NARUNO_ROOT']}/gui/lib/libs/kv/"
 
 for kv_file in os.listdir(KV_DIR):
     with open(os.path.join(KV_DIR, kv_file), encoding="utf-8") as kv:
         Builder.load_string(kv.read())
 
 KV = """
 #:import FadeTransition kivy.uix.screenmanager.FadeTransition
-#:import NarunoWelcomeScreen naruno.gui_lib.libs.baseclass.welcome_screen.NarunoWelcomeScreen
-#:import NarunoRootScreen naruno.gui_lib.libs.baseclass.root_screen.NarunoRootScreen
+#:import NarunoWelcomeScreen naruno.gui.lib.libs.baseclass.welcome_screen.NarunoWelcomeScreen
+#:import NarunoRootScreen naruno.gui.lib.libs.baseclass.root_screen.NarunoRootScreen
 
 ScreenManager:
     transition: FadeTransition()
 
     NarunoWelcomeScreen:
         name: "naruno register screen"
 
@@ -51,45 +50,43 @@
         name: "naruno root screen"
 
 """
 
 logger = get_logger("GUI")
 
 
-
 class GUI(MDApp):
     """
     An MDApp based  GUI class.
     GUI class consists of 2 elements:
       * title: Title of the app.
       * icon: icon of the app.
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.title = "Naruno"
-        self.icon = f"{os.environ['NARUNO_ROOT']}/gui_lib/images/logo.ico"
+        self.icon = f"{os.environ['NARUNO_ROOT']}/gui/lib/images/logo.ico"
 
     def build(self):
         """
         Some configurations.
         """
         Window.borderless = True
         value = the_settings()["dark_mode"]
 
-
         for i in self.theme_cls.colors["Yellow"]:
             self.theme_cls.colors["Yellow"][i] = "#5C6BC0"
         for i in self.theme_cls.colors["Dark"]:
             self.theme_cls.colors["Dark"][i] = "#303030"
 
         self.theme_cls.theme_style = "Dark" if value else "Light"
         self.theme_cls.primary_palette = "Yellow"  # "Purple", "Red"
 
-        self.FONT_PATH = os.path.join(os.environ["NARUNO_ROOT"], "gui_lib",
+        self.FONT_PATH = os.path.join(os.environ["NARUNO_ROOT"], "gui", "lib",
                                       "fonts")
 
         self.theme_cls.font_styles.update({
             "H1":
             [os.path.join(self.FONT_PATH, "Poppins-Light"), 96, False, -1.5],
             "H2":
             [os.path.join(self.FONT_PATH, "Poppins-Light"), 60, False, -0.5],
@@ -150,18 +147,16 @@
         })
 
         return Builder.load_string(KV)
 
     def restart(self):
         self.root.clear_widgets()
         self.stop()
-        naruno.gui.the_naruno_gui_app.the_naruno_gui = (
-            GUI())
-        return (naruno.gui.the_naruno_gui_app.
-                the_naruno_gui.run())
+        naruno.gui.the_naruno_gui_app.the_naruno_gui = GUI()
+        return naruno.gui.the_naruno_gui_app.the_naruno_gui.run()
 
 
 def arguments():
     """
     This function parses the arguments and makes the directions.
     """
 
@@ -184,19 +179,17 @@
         help="Timeout",
     )
 
     args = parser.parse_args()
 
     safety_check(args.interface, args.timeout)
 
-    naruno.gui.the_naruno_gui_app.the_naruno_gui = GUI(
-    )
+    naruno.gui.the_naruno_gui_app.the_naruno_gui = GUI()
 
-    naruno.gui.the_naruno_gui_app.the_naruno_gui.run(
-    )
+    naruno.gui.the_naruno_gui_app.the_naruno_gui.run()
 
 
 def start():
     """
     Start the GUI mode.
     """
```

### Comparing `naruno-0.58.0/naruno/gui/popup.py` & `naruno-0.58.1/naruno/gui/popup.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/POPPINS_LICENCE` & `naruno-0.58.1/naruno/gui/lib/fonts/POPPINS_LICENCE`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Black.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Black.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-BlackItalic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Bold.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Bold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-BoldItalic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ExtraBold.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ExtraLight.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Italic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Italic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Light.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Light.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-LightItalic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Medium.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Medium.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-MediumItalic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Regular.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Regular.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-SemiBold.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-Thin.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-Thin.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/fonts/Poppins-ThinItalic.ttf` & `naruno-0.58.1/naruno/gui/lib/fonts/Poppins-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/images/logo.ico` & `naruno-0.58.1/naruno/gui/lib/images/logo.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/images/logo.png` & `naruno-0.58.1/naruno/gui/lib/images/logo.png`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/images/logo_sm_orb_fw.png` & `naruno-0.58.1/naruno/gui/lib/images/logo_sm_orb_fw.png`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/images/logo_w_bc.png` & `naruno-0.58.1/naruno/gui/lib/images/logo_w_bc.png`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/images/logo_win.ico` & `naruno-0.58.1/naruno/gui/lib/images/logo_win.ico`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/baseclass/node_screen.py` & `naruno-0.58.1/naruno/gui/lib/libs/baseclass/node_screen.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 from naruno.node.server.server import server
 
 
 class NodeScreen(MDScreen):
     pass
 
 
-
 class NodeBox(MDGridLayout):
     cols = 2
 
     def start_node_server_func(self):
         server(
             self.start_node_server_dialog.input_results["IP"],
             int(self.start_node_server_dialog.input_results["PORT"]),
@@ -56,15 +55,14 @@
             return False
         server.Server.stop()
 
     def connect_to_know_node(self):
         server.connectionfrommixdb()
 
     def connect_a_node_func(self):
-
         if not self.check_node_server():
             return False
         server.Server.connect(
             self.connect_a_node_dialog.input_results["IP"],
             int(self.connect_a_node_dialog.input_results["PORT"]),
         )
 
@@ -75,15 +73,14 @@
             inputs=[
                 ["IP", False],
                 ["PORT", False],
             ],
         )
 
     def add_unl_node_func(self):
-
         from naruno.node.unl import Unl
 
         Unl.save_new_unl_node(
             self.add_unl_node_dialog.input_results["PublicKey"])
 
     def show_add_unl_node_dialog(self):
         self.add_unl_node_dialog = popup(
```

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/baseclass/operations_screen.py` & `naruno-0.58.1/naruno/gui/lib/libs/baseclass/operations_screen.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,30 +33,29 @@
 
 class OperationBox(MDGridLayout):
     cols = 2
 
     def sent_the_coins(self):
         the_block = GetBlock()
 
-        if (float(self.send_coin_dialog.input_results["Amount"]) >=
-                the_block.minumum_transfer_amount):
+        if (float(self.send_coin_dialog.input_results["Amount"])
+                >= the_block.minumum_transfer_amount):
             if (wallet_import(int(the_settings()["wallet"]), 2) == sha256(
                     self.send_coin_dialog.input_results["Password"].encode(
                         "utf-8")).hexdigest()):
                 block = the_block
                 send_tx = send(
                     self.send_coin_dialog.input_results["Password"],
                     self.send_coin_dialog.input_results["Receiver"],
                     amount=float(
                         self.send_coin_dialog.input_results["Amount"]),
                     data=str(self.send_coin_dialog.input_results["Data"]),
                     block=block,
                 )
                 if send_tx != False:
-
                     from naruno.node.server.server import server
 
                     if server.Server is None:
                         popup(title="Please start the node server",
                               type="failure")
                         return False
```

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/baseclass/root_screen.py` & `naruno-0.58.1/naruno/gui/lib/libs/baseclass/root_screen.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,22 +12,20 @@
 
 
 class NarunoRootScreen(MDScreen):
 
     def close_app(self, widget=None):
         self.close_app_dialog = popup(
             text="Are you sure you want to close ?",
-            target=naruno.gui.the_naruno_gui_app.
-            the_naruno_gui.stop,
+            target=naruno.gui.the_naruno_gui_app.the_naruno_gui.stop,
             type="question",
         )
 
 
-class NarunoListItem(ThemableBehavior, RectangularRippleBehavior,
-                       MDBoxLayout):
+class NarunoListItem(ThemableBehavior, RectangularRippleBehavior, MDBoxLayout):
     text = StringProperty()
     secondary_text = StringProperty()
     tertiary_text = StringProperty()
     bar_color = ColorProperty((1, 0, 0, 1))
 
 
 class NarunoSeeAllButton(RectangularRippleBehavior, MDBoxLayout):
```

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/baseclass/settings_screen.py` & `naruno-0.58.1/naruno/gui/lib/libs/baseclass/settings_screen.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,17 +56,15 @@
             type="info",
         )
 
     def callback(self, instance_button):
         if instance_button.text == "OK":
             self.alert.dismiss()
             SettingsBox.dark_mode_first_status = the_settings()["dark_mode"]
-            naruno.gui.the_naruno_gui_app.the_naruno_gui.restart(
-            )
+            naruno.gui.the_naruno_gui_app.the_naruno_gui.restart()
 
         else:
             self.alert.dismiss()
 
     def DARK_MODE_Status_Changing(self, instance, value):
-
         dark_mode_settings(value)
         self.show_dialog()
```

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/baseclass/tabnavigation.py` & `naruno-0.58.1/naruno/gui/lib/libs/baseclass/tabnavigation.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
             t="linear",
             duration=self.duration,
             icon_color=self.theme_cls.text_color,
         )
         anim.start(self)
 
     def _button_shrink(self):
-
         label_anim = Animation(opacity=0,
                                transition="out_sine",
                                duration=self.duration)
         label_anim.start(self.ids._label)
 
         but_anim = Animation(
             width=self.height,
```

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/baseclass/wallet_screen.py` & `naruno-0.58.1/naruno/gui/lib/libs/baseclass/wallet_screen.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
 
 class WalletBox(MDGridLayout):
     cols = 2
     text = StringProperty()
 
     def reflesh_balance(self):
-
         self.text = f"Balance: {str(GetBalance(wallet_import(-1, 0)))}"
 
     def create_the_wallet(self):
         wallet_create(self.wallet_alert_dialog.input_results["Password"])
 
     def show_wallet_alert_dialog(self):
         self.wallet_alert_dialog = popup(
```

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/baseclass/welcome_screen.py` & `naruno-0.58.1/naruno/gui/lib/libs/baseclass/welcome_screen.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/kv/node_screen.kv` & `naruno-0.58.1/naruno/gui/lib/libs/kv/node_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/kv/operations_screen.kv` & `naruno-0.58.1/naruno/gui/lib/libs/kv/operations_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/kv/root_screen.kv` & `naruno-0.58.1/naruno/gui/lib/libs/kv/root_screen.kv`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #: import environ os.environ
 #: import gch kivy.utils.get_color_from_hex
-#: import NavigationItem naruno.gui_lib.libs.baseclass.tabnavigation.NavigationItem
-#: import NavigationBar naruno.gui_lib.libs.baseclass.tabnavigation.NavigationBar
+#: import NavigationItem naruno.gui.lib.libs.baseclass.tabnavigation.NavigationItem
+#: import NavigationBar naruno.gui.lib.libs.baseclass.tabnavigation.NavigationBar
 
-#: import WalletScreen naruno.gui_lib.libs.baseclass.wallet_screen.WalletScreen
-#: import OperationScreen naruno.gui_lib.libs.baseclass.operations_screen.OperationScreen
-#: import NodeScreen naruno.gui_lib.libs.baseclass.node_screen.NodeScreen
-#: import SettingsScreen naruno.gui_lib.libs.baseclass.settings_screen.SettingsScreen
+#: import WalletScreen naruno.gui.lib.libs.baseclass.wallet_screen.WalletScreen
+#: import OperationScreen naruno.gui.lib.libs.baseclass.operations_screen.OperationScreen
+#: import NodeScreen naruno.gui.lib.libs.baseclass.node_screen.NodeScreen
+#: import SettingsScreen naruno.gui.lib.libs.baseclass.settings_screen.SettingsScreen
 
 
 <NarunoRootScreen>
 
     MDBoxLayout:
         orientation: 'vertical'
```

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/kv/settings_screen.kv` & `naruno-0.58.1/naruno/gui/lib/libs/kv/settings_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/kv/tabnavigation.kv` & `naruno-0.58.1/naruno/gui/lib/libs/kv/tabnavigation.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/kv/wallet_screen.kv` & `naruno-0.58.1/naruno/gui/lib/libs/kv/wallet_screen.kv`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/gui_lib/libs/kv/welcome_screen.kv` & `naruno-0.58.1/naruno/gui/lib/libs/kv/welcome_screen.kv`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         padding: dp(50)
         cols: 1
 
         AnchorLayout:
             anchor_x: 'center'
             anchor_y: 'center'
             Image:
-                source: f"{environ['NARUNO_ROOT']}/gui_lib/images/logo.ico"
+                source: f"{environ['NARUNO_ROOT']}/gui/lib/images/logo.ico"
 
 
 
         AnchorLayout:
             anchor_x: 'center'
             anchor_y: 'bottom'
             MDProgressBar:
```

### Comparing `naruno-0.58.0/naruno/lib/backup/naruno_export.py` & `naruno-0.58.1/naruno/lib/backup/naruno_export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/backup/naruno_import.py` & `naruno-0.58.1/naruno/lib/backup/naruno_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/clean_up.py` & `naruno-0.58.1/naruno/lib/clean_up.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/config_system.py` & `naruno-0.58.1/naruno/lib/config_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/encryption.py` & `naruno-0.58.1/naruno/lib/encryption.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/export.py` & `naruno-0.58.1/naruno/lib/export.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/log.py` & `naruno-0.58.1/naruno/lib/log.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/mix/merkle_root.py` & `naruno-0.58.1/naruno/lib/mix/merkle_root.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/mix/mixlib.py` & `naruno-0.58.1/naruno/lib/mix/mixlib.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/notification.py` & `naruno-0.58.1/naruno/lib/notification.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,16 +35,16 @@
         timeout = 10
         logger.debug(f"app_name: {app_name}")
         logger.debug(f"timeout: {timeout}")
         logger.debug(f"title: {title}")
         logger.debug(f"message: {message}")
         main_folder = get_config()["main_folder"]
 
-        icon = (f"{main_folder}/gui_lib/images/logo_win.ico" if platform
-                == "win" else f"{main_folder}/gui_lib/images/logo.png")
+        icon = (f"{main_folder}/gui/lib/images/logo_win.ico" if platform
+                == "win" else f"{main_folder}/gui/lib/images/logo.png")
 
         logger.debug(f"icon: {icon}")
         plyer_notification.notify(
             title=title,
             message=message,
             app_icon=icon,
             app_name=app_name,
```

### Comparing `naruno-0.58.0/naruno/lib/performance_analyzers/accounts.py` & `naruno-0.58.1/naruno/lib/performance_analyzers/accounts.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/performance_analyzers/block.py` & `naruno-0.58.1/naruno/lib/performance_analyzers/block.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/performance_analyzers/blockshash.py` & `naruno-0.58.1/naruno/lib/performance_analyzers/blockshash.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/performance_analyzers/blockshash_part.py` & `naruno-0.58.1/naruno/lib/performance_analyzers/blockshash_part.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/performance_analyzers/heartbeat_db.py` & `naruno-0.58.1/naruno/lib/performance_analyzers/heartbeat_db.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/performance_analyzers/transactions.py` & `naruno-0.58.1/naruno/lib/performance_analyzers/transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/perpetualtimer.py` & `naruno-0.58.1/naruno/lib/perpetualtimer.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/qr.py` & `naruno-0.58.1/naruno/lib/qr.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,46 +9,46 @@
 
 import qrcode
 from qrcode.image.styledpil import StyledPilImage
 from qrcode.image.styles.colormasks import SolidFillColorMask
 
 sys.path.append(os.path.join(os.path.dirname(__file__), "..", ".."))
 
+from hashlib import sha256
+
 from naruno.config import QR_CODE_PATH
 from naruno.lib.config_system import get_config
 from naruno.lib.log import get_logger
-from hashlib import sha256
-
 
 logger = get_logger("LIB")
 
 
 def qr(data):
     logger.info("Qr code generator is started")
     logger.debug(f"data: {data}")
     main_folder = get_config()["main_folder"]
     data_sha256 = sha256(data.encode("utf-8")).hexdigest()
     location = f"{main_folder}/{QR_CODE_PATH}{data_sha256}.png"
-    
 
     if not os.path.exists(location):
         logger.info("Qr code is not exist, it will be created")
         qr = qrcode.QRCode(error_correction=qrcode.constants.ERROR_CORRECT_H)
         qr.add_data(data)
         qr.make(fit=True)
-        icon = f"{main_folder}/gui_lib/images/logo_sm_orb_fw.png"
+        icon = f"{main_folder}/gui/lib/images/logo_sm_orb_fw.png"
         logger.debug(f"icon: {icon}")
         qr_img = qr.make_image(
             image_factory=StyledPilImage,
             embeded_image_path=icon,
             color_mask=SolidFillColorMask(front_color=(92, 107, 192)),
         )
         qr_img.save(location)
     else:
         logger.info("Qr code already exists")
 
     logger.info(f"location: {location}")
     logger.info("Qr code generator is finished.")
     return location
 
+
 if __name__ == "__main__":
-    qr("Ali_Eren_TABAK")
+    qr("Ali_Eren_TABAK")
```

### Comparing `naruno-0.58.0/naruno/lib/safety.py` & `naruno-0.58.1/naruno/lib/safety.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/settings_system.py` & `naruno-0.58.1/naruno/lib/settings_system.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/sign.py` & `naruno-0.58.1/naruno/lib/sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/status.py` & `naruno-0.58.1/naruno/lib/status.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/lib/verify.py` & `naruno-0.58.1/naruno/lib/verify.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/node/client/client.py` & `naruno-0.58.1/naruno/node/client/client.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/node/get_candidate_blocks.py` & `naruno-0.58.1/naruno/node/get_candidate_blocks.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/node/server/server.py` & `naruno-0.58.1/naruno/node/server/server.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/node/unl.py` & `naruno-0.58.1/naruno/node/unl.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/check/check_transaction.py` & `naruno-0.58.1/naruno/transactions/check/check_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/check/datas/check_datas.py` & `naruno-0.58.1/naruno/transactions/check/datas/check_datas.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/check/len/check_len.py` & `naruno-0.58.1/naruno/transactions/check/len/check_len.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/check/sign/check_sign.py` & `naruno-0.58.1/naruno/transactions/check/sign/check_sign.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/check/type/check_type.py` & `naruno-0.58.1/naruno/transactions/check/type/check_type.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/cleaner.py` & `naruno-0.58.1/naruno/transactions/cleaner.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/get_transaction.py` & `naruno-0.58.1/naruno/transactions/get_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/my_transactions/check_proof.py` & `naruno-0.58.1/naruno/transactions/my_transactions/check_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/my_transactions/get_my_transaction.py` & `naruno-0.58.1/naruno/transactions/my_transactions/get_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/my_transactions/get_proof.py` & `naruno-0.58.1/naruno/transactions/my_transactions/get_proof.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/my_transactions/save_my_transaction.py` & `naruno-0.58.1/naruno/transactions/my_transactions/save_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/my_transactions/save_to_my_transaction.py` & `naruno-0.58.1/naruno/transactions/my_transactions/save_to_my_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/my_transactions/sended_transaction.py` & `naruno-0.58.1/naruno/transactions/my_transactions/sended_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/my_transactions/validate_transaction.py` & `naruno-0.58.1/naruno/transactions/my_transactions/validate_transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/pending/delete_pending.py` & `naruno-0.58.1/naruno/transactions/pending/delete_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/pending/get_pending.py` & `naruno-0.58.1/naruno/transactions/pending/get_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/pending/save_pending.py` & `naruno-0.58.1/naruno/transactions/pending/save_pending.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/pending_to_validating.py` & `naruno-0.58.1/naruno/transactions/pending_to_validating.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/print_transactions.py` & `naruno-0.58.1/naruno/transactions/print_transactions.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/process_the_transaction.py` & `naruno-0.58.1/naruno/transactions/process_the_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,19 +73,19 @@
 
         touser_inlist = True
         to_user_in_new_list = False
 
         address_of_fromUser = Address(trans.fromUser)
         logger.debug(f"FromUser address: {address_of_fromUser}")
         the_account_list.execute(
-            f"SELECT * FROM account_list WHERE address = '{address_of_fromUser}'"
+            "SELECT * FROM account_list WHERE address = ?", (address_of_fromUser,)
         )
         first_list = the_account_list.fetchall()
         the_account_list.execute(
-            f"SELECT * FROM account_list WHERE address = '{trans.toUser}'")
+            "SELECT * FROM account_list WHERE address = ?", (trans.toUser,))
         second_list = the_account_list.fetchall()
 
         for the_pulled_account in first_list + second_list:
             account_list.append(
                 Account(the_pulled_account[0], the_pulled_account[2],
                         the_pulled_account[1]))
 
@@ -135,15 +135,15 @@
     new_added_accounts_list = sorted(new_added_accounts_list,
                                      key=lambda x: x.Address)
 
     conn = sqlite3.connect(the_TEMP_ACCOUNTS_PATH)
     c = conn.cursor()
     for changed_account in edited_accounts:
         c.execute(
-            f"UPDATE account_list SET balance = {changed_account.balance}, sequence_number = {changed_account.sequence_number} WHERE address = '{changed_account.Address}'"
-        )
+            "UPDATE account_list SET balance = ?, sequence_number = ? WHERE address = ?"
+        ,(changed_account.balance,changed_account.sequence_number,changed_account.Address))
         conn.commit()
     conn.close()
 
     SaveAccounts(new_added_accounts_list, the_TEMP_ACCOUNTS_PATH)
 
     return block
```

### Comparing `naruno-0.58.0/naruno/transactions/send.py` & `naruno-0.58.1/naruno/transactions/send.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/transactions/transaction.py` & `naruno-0.58.1/naruno/transactions/transaction.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/delete_current_wallet.py` & `naruno-0.58.1/naruno/wallet/delete_current_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/curve.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/curve.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/ecdsa.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/ecdsa.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/math.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/math.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/privateKey.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/privateKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/publicKey.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/publicKey.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/signature.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/signature.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/utils/binary.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/utils/binary.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/utils/compatibility.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/utils/der.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/utils/der.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/ellipticcurve/utils/oid.py` & `naruno-0.58.1/naruno/wallet/ellipticcurve/utils/oid.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/get_saved_wallet.py` & `naruno-0.58.1/naruno/wallet/get_saved_wallet.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/print_wallets.py` & `naruno-0.58.1/naruno/wallet/print_wallets.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/save_wallet_list.py` & `naruno-0.58.1/naruno/wallet/save_wallet_list.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/wallet_create.py` & `naruno-0.58.1/naruno/wallet/wallet_create.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/wallet_delete.py` & `naruno-0.58.1/naruno/wallet/wallet_delete.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/wallet_import.py` & `naruno-0.58.1/naruno/wallet/wallet_import.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno/wallet/wallet_selector.py` & `naruno-0.58.1/naruno/wallet/wallet_selector.py`

 * *Files identical despite different names*

### Comparing `naruno-0.58.0/naruno.egg-info/PKG-INFO` & `naruno-0.58.1/naruno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naruno
-Version: 0.58.0
+Version: 0.58.1
 Summary: Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.
 Home-page: https://github.com/Naruno/Naruno
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MPL-2.0
 Description: <p align="center">
           <a href="https://github.com/Naruno/Naruno">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: naruno Version: 0.58.0 Summary: Naruno is a
+Metadata-Version: 2.1 Name: naruno Version: 0.58.1 Summary: Naruno is a
 lightning-fast, secure, and scalable blockchain that is able to create
 transaction proofs and verification via raw data and timestamp. We remove the
 archive nodes and lazy web3 integrations. With Naruno everyone can get the
 proof (5-10MB) of their transactions via their nodes and after everyone can use
 in another node for verification the raw data and timestamp. Also you can
 integrate your web3 applications with 4 code lines (just python for now) via
 our remote app system. Home-page: https://github.com/Naruno/Naruno Author:
```

### Comparing `naruno-0.58.0/naruno.egg-info/SOURCES.txt` & `naruno-0.58.1/naruno.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -93,52 +93,52 @@
 naruno/db/test_finished_main_3/README.md
 naruno/db/test_finished_main_false_time/README.md
 naruno/db/test_finished_main_no_reset/README.md
 naruno/db/test_proof_extracted/README.md
 naruno/gui/main.py
 naruno/gui/popup.py
 naruno/gui/the_naruno_gui_app.py
-naruno/gui_lib/fonts/POPPINS_LICENCE
-naruno/gui_lib/fonts/Poppins-Black.ttf
-naruno/gui_lib/fonts/Poppins-BlackItalic.ttf
-naruno/gui_lib/fonts/Poppins-Bold.ttf
-naruno/gui_lib/fonts/Poppins-BoldItalic.ttf
-naruno/gui_lib/fonts/Poppins-ExtraBold.ttf
-naruno/gui_lib/fonts/Poppins-ExtraBoldItalic.ttf
-naruno/gui_lib/fonts/Poppins-ExtraLight.ttf
-naruno/gui_lib/fonts/Poppins-ExtraLightItalic.ttf
-naruno/gui_lib/fonts/Poppins-Italic.ttf
-naruno/gui_lib/fonts/Poppins-Light.ttf
-naruno/gui_lib/fonts/Poppins-LightItalic.ttf
-naruno/gui_lib/fonts/Poppins-Medium.ttf
-naruno/gui_lib/fonts/Poppins-MediumItalic.ttf
-naruno/gui_lib/fonts/Poppins-Regular.ttf
-naruno/gui_lib/fonts/Poppins-SemiBold.ttf
-naruno/gui_lib/fonts/Poppins-SemiBoldItalic.ttf
-naruno/gui_lib/fonts/Poppins-Thin.ttf
-naruno/gui_lib/fonts/Poppins-ThinItalic.ttf
-naruno/gui_lib/images/logo.ico
-naruno/gui_lib/images/logo.png
-naruno/gui_lib/images/logo_sm_orb_fw.png
-naruno/gui_lib/images/logo_w_bc.png
-naruno/gui_lib/images/logo_win.ico
-naruno/gui_lib/libs/baseclass/node_screen.py
-naruno/gui_lib/libs/baseclass/operations_screen.py
-naruno/gui_lib/libs/baseclass/root_screen.py
-naruno/gui_lib/libs/baseclass/settings_screen.py
-naruno/gui_lib/libs/baseclass/tabnavigation.py
-naruno/gui_lib/libs/baseclass/wallet_screen.py
-naruno/gui_lib/libs/baseclass/welcome_screen.py
-naruno/gui_lib/libs/kv/node_screen.kv
-naruno/gui_lib/libs/kv/operations_screen.kv
-naruno/gui_lib/libs/kv/root_screen.kv
-naruno/gui_lib/libs/kv/settings_screen.kv
-naruno/gui_lib/libs/kv/tabnavigation.kv
-naruno/gui_lib/libs/kv/wallet_screen.kv
-naruno/gui_lib/libs/kv/welcome_screen.kv
+naruno/gui/lib/fonts/POPPINS_LICENCE
+naruno/gui/lib/fonts/Poppins-Black.ttf
+naruno/gui/lib/fonts/Poppins-BlackItalic.ttf
+naruno/gui/lib/fonts/Poppins-Bold.ttf
+naruno/gui/lib/fonts/Poppins-BoldItalic.ttf
+naruno/gui/lib/fonts/Poppins-ExtraBold.ttf
+naruno/gui/lib/fonts/Poppins-ExtraBoldItalic.ttf
+naruno/gui/lib/fonts/Poppins-ExtraLight.ttf
+naruno/gui/lib/fonts/Poppins-ExtraLightItalic.ttf
+naruno/gui/lib/fonts/Poppins-Italic.ttf
+naruno/gui/lib/fonts/Poppins-Light.ttf
+naruno/gui/lib/fonts/Poppins-LightItalic.ttf
+naruno/gui/lib/fonts/Poppins-Medium.ttf
+naruno/gui/lib/fonts/Poppins-MediumItalic.ttf
+naruno/gui/lib/fonts/Poppins-Regular.ttf
+naruno/gui/lib/fonts/Poppins-SemiBold.ttf
+naruno/gui/lib/fonts/Poppins-SemiBoldItalic.ttf
+naruno/gui/lib/fonts/Poppins-Thin.ttf
+naruno/gui/lib/fonts/Poppins-ThinItalic.ttf
+naruno/gui/lib/images/logo.ico
+naruno/gui/lib/images/logo.png
+naruno/gui/lib/images/logo_sm_orb_fw.png
+naruno/gui/lib/images/logo_w_bc.png
+naruno/gui/lib/images/logo_win.ico
+naruno/gui/lib/libs/baseclass/node_screen.py
+naruno/gui/lib/libs/baseclass/operations_screen.py
+naruno/gui/lib/libs/baseclass/root_screen.py
+naruno/gui/lib/libs/baseclass/settings_screen.py
+naruno/gui/lib/libs/baseclass/tabnavigation.py
+naruno/gui/lib/libs/baseclass/wallet_screen.py
+naruno/gui/lib/libs/baseclass/welcome_screen.py
+naruno/gui/lib/libs/kv/node_screen.kv
+naruno/gui/lib/libs/kv/operations_screen.kv
+naruno/gui/lib/libs/kv/root_screen.kv
+naruno/gui/lib/libs/kv/settings_screen.kv
+naruno/gui/lib/libs/kv/tabnavigation.kv
+naruno/gui/lib/libs/kv/wallet_screen.kv
+naruno/gui/lib/libs/kv/welcome_screen.kv
 naruno/lib/clean_up.py
 naruno/lib/config_system.py
 naruno/lib/encryption.py
 naruno/lib/export.py
 naruno/lib/log.py
 naruno/lib/notification.py
 naruno/lib/perpetualtimer.py
```

### Comparing `naruno-0.58.0/setup.py` & `naruno-0.58.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup
 
 setup(
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     packages=["naruno"],
     name="naruno",
-    version="0.58.0",
+    version="0.58.1",
     url="https://github.com/Naruno/Naruno",
     description=
     "Naruno is a lightning-fast, secure, and scalable blockchain that is able to create transaction proofs and verification via raw data and timestamp. We remove the archive nodes and lazy web3 integrations. With Naruno everyone can get the proof (5-10MB) of their transactions via their nodes and after everyone can use in another node for verification the raw data and timestamp. Also you can integrate your web3 applications with 4 code lines (just python for now) via our remote app system.",
     keywords=[
         "python",
         "cryptography",
         "blockchain",
```

