# Comparing `tmp/dexteritysdk-0.2.3.tar.gz` & `tmp/dexteritysdk-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexteritysdk-0.2.3.tar", max compression
+gzip compressed data, was "dexteritysdk-0.2.8.tar", max compression
```

## Comparing `dexteritysdk-0.2.3.tar` & `dexteritysdk-0.2.8.tar`

### file list

```diff
@@ -1,225 +1,238 @@
--rw-r--r--   0        0        0     4751 2022-11-21 11:32:49.669721 dexteritysdk-0.2.3/README.md
--rw-r--r--   0        0        0        0 2022-08-24 13:49:21.974698 dexteritysdk-0.2.3/dexteritysdk/__init__.py
--rw-r--r--   0        0        0    18461 2022-09-08 12:11:13.318564 dexteritysdk-0.2.3/dexteritysdk/bots/bootstrap.py
--rw-r--r--   0        0        0     8829 2022-08-24 13:49:21.975096 dexteritysdk-0.2.3/dexteritysdk/bots/consume_events_crank.py
--rw-r--r--   0        0        0     6278 2022-08-24 13:49:21.975214 dexteritysdk-0.2.3/dexteritysdk/bots/expiration_routine.py
--rwxr-xr-x   0        0        0     3042 2022-08-24 13:49:21.975334 dexteritysdk-0.2.3/dexteritysdk/bots/new_connect.py
--rw-r--r--   0        0        0     7395 2022-08-24 13:49:21.975452 dexteritysdk-0.2.3/dexteritysdk/bots/oracle_price_crank.py
--rwxr-xr-x   0        0        0     9098 2023-01-24 19:47:07.942386 dexteritysdk-0.2.3/dexteritysdk/bots/quoter_bot.py
--rw-r--r--   0        0        0     4676 2022-08-24 13:49:21.975738 dexteritysdk-0.2.3/dexteritysdk/bots/settle_crank.py
--rw-r--r--   0        0        0        0 2022-08-24 13:49:21.975778 dexteritysdk-0.2.3/dexteritysdk/bots/solmate_bootstrap.py
--rw-r--r--   0        0        0     6329 2022-08-24 13:49:21.975918 dexteritysdk-0.2.3/dexteritysdk/bots/taker_bot.py
--rw-r--r--   0        0        0       84 2022-09-07 16:16:02.404150 dexteritysdk-0.2.3/dexteritysdk/codegen/__init__.py
--rw-r--r--   0        0        0      253 2022-09-07 16:16:02.404420 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/__init__.py
--rw-r--r--   0        0        0      595 2022-09-07 16:16:02.404559 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/accounts.py
--rw-r--r--   0        0        0      138 2022-09-07 16:16:02.404667 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/addrs.py
--rw-r--r--   0        0        0      409 2022-09-07 16:16:02.404821 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/instructions/__init__.py
--rw-r--r--   0        0        0     3269 2022-09-07 16:16:02.404965 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/instructions/create_risk_state_account.py
--rw-r--r--   0        0        0      437 2022-09-07 16:16:02.405092 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/instructions/instruction_tag.py
--rw-r--r--   0        0        0     3816 2022-09-07 16:16:02.405234 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/instructions/validate_account_health.py
--rw-r--r--   0        0        0     3846 2022-09-07 16:16:02.405340 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/instructions/validate_account_liquidation.py
--rw-r--r--   0        0        0       75 2022-09-07 16:16:02.405485 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/types/__init__.py
--rw-r--r--   0        0        0      606 2022-09-07 16:16:02.405612 dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/types/health.py
--rw-r--r--   0        0        0      264 2023-01-24 18:58:48.242097 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/__init__.py
--rw-r--r--   0        0        0      264 2022-10-26 11:38:44.406419 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/__init__.py.py
--rw-r--r--   0        0        0     1942 2023-01-24 18:58:48.247713 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/accounts.py
--rw-r--r--   0        0        0      138 2023-01-24 18:58:48.242196 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/addrs.py
--rw-r--r--   0        0        0      624 2023-01-24 18:58:48.247644 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/constants.py
--rw-r--r--   0        0        0     2609 2023-01-24 18:58:48.247821 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/__init__.py
--rw-r--r--   0        0        0     7007 2023-01-25 14:46:55.406403 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/cancel_order.py
--rw-r--r--   0        0        0     2533 2023-01-24 18:58:48.256696 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/choose_successor.py
--rw-r--r--   0        0        0     2206 2023-01-24 18:58:48.256780 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/claim_authority.py
--rw-r--r--   0        0        0     4397 2023-01-24 18:58:48.256114 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/clear_expired_orderbook.py
--rw-r--r--   0        0        0     2872 2023-01-24 18:58:48.250386 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/clear_open_orders.py
--rw-r--r--   0        0        0     5856 2023-01-24 18:58:48.252405 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/consume_orderbook_events.py
--rw-r--r--   0        0        0     4451 2023-01-25 14:46:55.406637 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/deactivate_market_product.py
--rw-r--r--   0        0        0     4762 2023-01-24 18:58:48.252900 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/deposit_funds.py
--rw-r--r--   0        0        0     2754 2023-01-24 18:58:48.253515 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_combo.py
--rw-r--r--   0        0        0     3143 2023-01-24 18:58:48.248882 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_market_product.py
--rw-r--r--   0        0        0     7893 2023-01-24 18:58:48.248507 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_market_product_group.py
--rw-r--r--   0        0        0     4459 2023-01-24 18:58:48.249748 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_print_trade.py
--rw-r--r--   0        0        0     4587 2023-01-24 18:58:48.250039 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_trader_risk_group.py
--rw-r--r--   0        0        0     1746 2023-01-24 18:58:48.257174 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/instruction_tag.py
--rw-r--r--   0        0        0     9123 2023-01-25 14:46:55.406762 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/new_order.py
--rw-r--r--   0        0        0     4033 2023-01-24 18:58:48.256396 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/pop_events.py
--rw-r--r--   0        0        0     2193 2023-01-24 18:58:48.249583 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/remove_market_product.py
--rw-r--r--   0        0        0     2242 2023-01-24 18:58:48.249667 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/remove_market_product_group.py
--rw-r--r--   0        0        0     3019 2023-01-24 18:58:48.256856 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/setup_capital_limits.py
--rw-r--r--   0        0        0     9361 2023-01-25 14:46:55.406894 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/sign_print_trade.py
--rw-r--r--   0        0        0     4454 2023-01-24 18:58:48.256502 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/sweep_fees.py
--rw-r--r--   0        0        0     5721 2023-01-25 14:46:55.407006 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/transfer_full_position.py
--rw-r--r--   0        0        0     3270 2023-01-24 18:58:48.256945 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_capital_limits.py
--rw-r--r--   0        0        0     3709 2023-01-24 18:58:48.248702 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_market_product_group.py
--rw-r--r--   0        0        0     2471 2023-01-24 18:58:48.253249 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_product_funding.py
--rw-r--r--   0        0        0     4387 2023-01-25 14:46:55.407109 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_trader_funding.py
--rw-r--r--   0        0        0     2523 2023-01-24 18:58:48.257094 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_trader_risk_group_owner.py
--rw-r--r--   0        0        0     5083 2023-01-25 14:46:55.407385 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_variance_cache.py
--rw-r--r--   0        0        0     6429 2023-01-25 14:46:55.407512 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/withdraw_funds.py
--rw-r--r--   0        0        0     2339 2023-01-24 18:58:48.242439 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/__init__.py
--rw-r--r--   0        0        0     1031 2023-01-24 18:58:48.246653 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/account_tag.py
--rw-r--r--   0        0        0      858 2023-01-24 18:58:48.247119 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/action_status.py
--rw-r--r--   0        0        0      453 2023-01-24 18:58:48.244571 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/bitset.py
--rw-r--r--   0        0        0      503 2023-01-24 18:58:48.242584 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/call_back_info.py
--rw-r--r--   0        0        0      458 2023-01-24 18:58:48.245226 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/cancel_order_params.py
--rw-r--r--   0        0        0      628 2023-01-24 18:58:48.247182 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/capital_limits.py
--rw-r--r--   0        0        0      535 2023-01-24 18:58:48.247584 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/capital_limits_params.py
--rw-r--r--   0        0        0      469 2023-01-24 18:58:48.246403 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/clear_expired_orderbook_params.py
--rw-r--r--   0        0        0      670 2023-01-24 18:58:48.244066 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/combo.py
--rw-r--r--   0        0        0      467 2023-01-24 18:58:48.245153 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/consume_orderbook_events_params.py
--rw-r--r--   0        0        0      495 2023-01-24 18:58:48.245291 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/deposit_funds_params.py
--rw-r--r--   0        0        0     3169 2023-01-24 18:58:48.246584 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/dex_error.py
--rw-r--r--   0        0        0     3335 2023-01-24 18:58:48.244639 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/fractional.py
--rw-r--r--   0        0        0      583 2023-01-24 18:58:48.244223 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/health_info.py
--rw-r--r--   0        0        0      778 2023-01-24 18:58:48.246996 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/health_result.py
--rw-r--r--   0        0        0      906 2023-01-24 18:58:48.247059 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/health_status.py
--rw-r--r--   0        0        0      668 2023-01-24 18:58:48.245787 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/initialize_combo_params.py
--rw-r--r--   0        0        0      955 2023-01-24 18:58:48.244707 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/initialize_market_product_group_params.py
--rw-r--r--   0        0        0      647 2023-01-24 18:58:48.245012 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/initialize_market_product_params.py
--rw-r--r--   0        0        0      767 2023-01-24 18:58:48.244844 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/initialize_print_trade_params.py
--rw-r--r--   0        0        0      545 2023-01-24 18:58:48.244150 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/leg.py
--rw-r--r--   0        0        0      875 2023-01-24 18:58:48.244299 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/liquidation_info.py
--rw-r--r--   0        0        0     3438 2023-01-24 18:58:48.247251 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/market_product_group.py
--rw-r--r--   0        0        0      791 2023-01-24 18:58:48.245092 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/new_order_params.py
--rw-r--r--   0        0        0      786 2023-01-24 18:58:48.242918 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/open_orders.py
--rw-r--r--   0        0        0      649 2023-01-24 18:58:48.242851 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/open_orders_metadata.py
--rw-r--r--   0        0        0      548 2023-01-24 18:58:48.243241 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/open_orders_node.py
--rw-r--r--   0        0        0      940 2023-01-24 18:58:48.246925 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/operation_type.py
--rw-r--r--   0        0        0      868 2023-01-24 18:58:48.244438 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/order_info.py
--rw-r--r--   0        0        0      901 2023-01-24 18:58:48.246790 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/order_type.py
--rw-r--r--   0        0        0     1190 2023-01-24 18:58:48.243687 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/outright.py
--rw-r--r--   0        0        0      473 2023-01-24 18:58:48.242519 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/params.py
--rw-r--r--   0        0        0      444 2023-01-24 18:58:48.246319 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/pop_events_params.py
--rw-r--r--   0        0        0      691 2023-01-24 18:58:48.242783 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/price_ewma.py
--rw-r--r--   0        0        0      892 2023-01-24 18:58:48.247381 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/print_trade.py
--rw-r--r--   0        0        0     1644 2023-01-24 18:58:48.246860 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/product.py
--rw-r--r--   0        0        0      519 2023-01-24 18:58:48.247318 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/product_array.py
--rw-r--r--   0        0        0      855 2023-01-24 18:58:48.243763 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/product_metadata.py
--rw-r--r--   0        0        0      903 2023-01-24 18:58:48.246723 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/product_status.py
--rw-r--r--   0        0        0      512 2023-01-24 18:58:48.247444 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/risk_output_register.py
--rw-r--r--   0        0        0      755 2023-01-24 18:58:48.244923 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/sign_print_trade_params.py
--rw-r--r--   0        0        0      550 2023-01-24 18:58:48.244372 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/social_loss.py
--rw-r--r--   0        0        0      686 2023-01-24 18:58:48.242715 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/trader_fee_params.py
--rw-r--r--   0        0        0      538 2023-01-24 18:58:48.242652 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/trader_fees.py
--rw-r--r--   0        0        0      837 2023-01-24 18:58:48.244505 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/trader_position.py
--rw-r--r--   0        0        0     1352 2023-01-24 18:58:48.247513 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/trader_risk_group.py
--rw-r--r--   0        0        0      438 2023-01-24 18:58:48.244776 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/update_market_product_group_params.py
--rw-r--r--   0        0        0      621 2023-01-24 18:58:48.245664 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/update_product_funding_params.py
--rw-r--r--   0        0        0     1385 2023-01-24 18:58:48.246496 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/util_error.py
--rw-r--r--   0        0        0      497 2023-01-24 18:58:48.245349 dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/withdraw_funds_params.py
--rw-r--r--   0        0        0      234 2023-01-24 18:58:48.259755 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/__init__.py
--rw-r--r--   0        0        0      639 2023-01-24 18:58:48.260439 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/accounts.py
--rw-r--r--   0        0        0      138 2023-01-24 18:58:48.259838 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/addrs.py
--rw-r--r--   0        0        0      370 2023-01-24 18:58:48.260509 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/__init__.py
--rw-r--r--   0        0        0     2603 2023-01-24 18:58:48.260732 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/close_derivative_account.py
--rw-r--r--   0        0        0     3613 2023-01-25 14:46:55.407719 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/initialize_derivative.py
--rw-r--r--   0        0        0     3299 2022-09-07 16:16:02.407477 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/initialize_fixed_income.py
--rw-r--r--   0        0        0      423 2023-01-24 18:58:48.260796 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/instruction_tag.py
--rw-r--r--   0        0        0     2948 2023-01-25 14:46:55.407889 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/settle_derivative.py
--rw-r--r--   0        0        0     2629 2022-09-07 16:16:02.407586 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/settle_fixed_income.py
--rw-r--r--   0        0        0      379 2023-01-24 18:58:48.259913 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/__init__.py
--rw-r--r--   0        0        0      899 2023-01-24 18:58:48.260123 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/account_tag.py
--rw-r--r--   0        0        0     1199 2023-01-24 18:58:48.260052 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/derivative_error.py
--rw-r--r--   0        0        0     1331 2023-01-24 18:58:48.260374 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/derivative_metadata.py
--rw-r--r--   0        0        0      879 2023-01-24 18:58:48.260308 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/expiration_status.py
--rw-r--r--   0        0        0     1029 2022-09-07 16:16:02.407732 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/fixed_income_metadata.py
--rw-r--r--   0        0        0      977 2023-01-24 18:58:48.259984 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/initialize_derivative_params.py
--rw-r--r--   0        0        0      748 2022-09-07 16:16:02.407828 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/initialize_fixed_income_params.py
--rw-r--r--   0        0        0      943 2023-01-24 18:58:48.260186 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/instrument_type.py
--rw-r--r--   0        0        0      868 2023-01-24 18:58:48.260246 dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/oracle_type.py
--rw-r--r--   0        0        0      124 2022-09-07 16:16:02.407957 dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/__init__.py
--rw-r--r--   0        0        0      138 2022-09-07 16:16:02.408030 dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/addrs.py
--rw-r--r--   0        0        0      409 2022-09-07 16:16:02.408146 dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/instructions/__init__.py
--rw-r--r--   0        0        0     3270 2022-09-07 16:16:02.408235 dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/instructions/create_risk_state_account.py
--rw-r--r--   0        0        0      437 2022-09-07 16:16:02.408323 dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/instructions/instruction_tag.py
--rw-r--r--   0        0        0     3961 2022-09-07 16:16:02.408404 dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/instructions/validate_account_health.py
--rw-r--r--   0        0        0     3991 2022-09-07 16:16:02.408481 dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/instructions/validate_account_liquidation.py
--rw-r--r--   0        0        0      296 2023-01-24 18:58:48.264281 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/__init__.py
--rw-r--r--   0        0        0     1091 2023-01-24 18:58:48.265127 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/accounts.py
--rw-r--r--   0        0        0      138 2023-01-24 18:58:48.264353 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/addrs.py
--rw-r--r--   0        0        0      180 2023-01-24 18:58:48.265063 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/constants.py
--rw-r--r--   0        0        0      784 2023-01-24 18:58:48.265194 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/__init__.py
--rw-r--r--   0        0        0     2808 2023-01-24 18:58:48.265812 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/close_mark_prices.py
--rw-r--r--   0        0        0     3302 2023-01-24 18:58:48.265606 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/create_risk_state_account.py
--rw-r--r--   0        0        0     3739 2023-01-24 18:58:48.265673 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/initialize_covariance_matrix.py
--rw-r--r--   0        0        0     3528 2023-01-25 14:46:55.408079 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/initialize_mark_prices.py
--rw-r--r--   0        0        0      654 2023-01-24 18:58:48.265951 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/instruction_tag.py
--rw-r--r--   0        0        0     2494 2023-01-25 14:46:55.408242 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/update_mark_prices.py
--rw-r--r--   0        0        0     4961 2023-01-25 14:46:55.408411 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/validate_account_health.py
--rw-r--r--   0        0        0     4991 2023-01-25 14:46:55.408595 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/validate_account_liquidation.py
--rw-r--r--   0        0        0      452 2023-01-24 18:58:48.264420 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/__init__.py
--rw-r--r--   0        0        0      665 2023-01-24 18:58:48.264805 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/correlation_matrix.py
--rw-r--r--   0        0        0      880 2023-01-24 18:58:48.264874 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/covariance_metadata.py
--rw-r--r--   0        0        0      418 2023-01-24 18:58:48.264483 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/fast_int.py
--rw-r--r--   0        0        0      634 2023-01-24 18:58:48.264619 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/initialize_mark_prices_params.py
--rw-r--r--   0        0        0      622 2023-01-24 18:58:48.264551 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/mark_price.py
--rw-r--r--   0        0        0      908 2023-01-24 18:58:48.264939 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/mark_prices_array.py
--rw-r--r--   0        0        0      930 2023-01-24 18:58:48.264742 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/risk_account_tag.py
--rw-r--r--   0        0        0     1660 2023-01-24 18:58:48.264681 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/risk_error.py
--rw-r--r--   0        0        0      891 2023-01-24 18:58:48.265003 dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/variance_cache.py
--rw-r--r--   0        0        0     2418 2022-08-24 13:49:21.985348 dexteritysdk-0.2.3/dexteritysdk/constant_fees/actions.py
--rw-r--r--   0        0        0        0 2022-08-24 13:49:21.985383 dexteritysdk-0.2.3/dexteritysdk/constant_fees/addrs.py
--rw-r--r--   0        0        0     2251 2022-08-24 13:49:21.985473 dexteritysdk-0.2.3/dexteritysdk/constant_fees/instructions.py
--rw-r--r--   0        0        0      162 2022-08-24 13:49:21.985545 dexteritysdk-0.2.3/dexteritysdk/constant_fees/state.py
--rw-r--r--   0        0        0    41508 2022-09-08 12:11:05.816702 dexteritysdk-0.2.3/dexteritysdk/dex/actions.py
--rw-r--r--   0        0        0     4443 2022-08-24 13:49:21.985778 dexteritysdk-0.2.3/dexteritysdk/dex/addrs.py
--rw-r--r--   0        0        0    47980 2023-01-25 18:12:44.039761 dexteritysdk-0.2.3/dexteritysdk/dex/sdk_context.py
--rw-r--r--   0        0        0     3046 2022-08-24 13:49:21.986089 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/actions.py
--rw-r--r--   0        0        0      410 2022-08-24 13:49:21.986210 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/__init__.py
--rw-r--r--   0        0        0      204 2022-08-24 13:49:21.986279 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/common.py
--rw-r--r--   0        0        0      825 2022-08-24 13:49:21.986349 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/initialize_clock.py
--rw-r--r--   0        0        0      956 2022-08-24 13:49:21.986427 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/initialize_oracle.py
--rw-r--r--   0        0        0     1020 2022-08-24 13:49:21.986495 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/update_clock.py
--rw-r--r--   0        0        0      962 2022-08-24 13:49:21.986563 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/update_price.py
--rw-r--r--   0        0        0      459 2022-08-24 13:49:21.986667 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/state/__init__.py
--rw-r--r--   0        0        0      168 2022-08-24 13:49:21.986739 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/state/clock.py
--rw-r--r--   0        0        0      117 2022-08-24 13:49:21.986798 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/state/common.py
--rw-r--r--   0        0        0      260 2022-08-24 13:49:21.986866 dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/state/oracle_price.py
--rw-r--r--   0        0        0     4543 2022-08-24 13:49:21.986982 dexteritysdk-0.2.3/dexteritysdk/instruments/actions.py
--rw-r--r--   0        0        0      125 2022-08-24 13:49:21.987080 dexteritysdk-0.2.3/dexteritysdk/instruments/instructions/__init__.py
--rw-r--r--   0        0        0     1163 2022-08-24 13:49:21.987149 dexteritysdk-0.2.3/dexteritysdk/instruments/instructions/initialize_derivative.py
--rw-r--r--   0        0        0      702 2022-08-24 13:49:21.987225 dexteritysdk-0.2.3/dexteritysdk/instruments/instructions/initialize_fixed_income.py
--rw-r--r--   0        0        0      121 2022-09-27 20:09:16.734330 dexteritysdk-0.2.3/dexteritysdk/mints.py
--rw-r--r--   0        0        0     2125 2022-10-27 11:50:10.627842 dexteritysdk-0.2.3/dexteritysdk/program_ids.py
--rw-r--r--   0        0        0        0 2022-09-14 12:42:20.447710 dexteritysdk-0.2.3/dexteritysdk/pyserum/__init__.py
--rw-r--r--   0        0        0      406 2022-09-14 12:42:20.448359 dexteritysdk-0.2.3/dexteritysdk/pyserum/enums.py
--rw-r--r--   0        0        0     1952 2022-10-27 11:50:10.627988 dexteritysdk-0.2.3/dexteritysdk/pyserum/event_queue.py
--rw-r--r--   0        0        0        0 2022-10-27 11:50:10.628019 dexteritysdk-0.2.3/dexteritysdk/pyserum/layouts/__init__.py
--rw-r--r--   0        0        0     1292 2022-10-27 11:50:10.628342 dexteritysdk-0.2.3/dexteritysdk/pyserum/layouts/event_queue.py
--rw-r--r--   0        0        0     1803 2022-10-27 11:50:10.628583 dexteritysdk-0.2.3/dexteritysdk/pyserum/layouts/slab.py
--rw-r--r--   0        0        0     3094 2022-10-27 11:50:10.628776 dexteritysdk-0.2.3/dexteritysdk/pyserum/orderbook.py
--rw-r--r--   0        0        0      338 2022-10-27 11:50:10.628969 dexteritysdk-0.2.3/dexteritysdk/pyserum/serum_types.py
--rw-r--r--   0        0        0        0 2022-10-27 11:50:10.629018 dexteritysdk-0.2.3/dexteritysdk/pyserum/structs/__init__.py
--rw-r--r--   0        0        0     2132 2022-10-27 11:50:10.629382 dexteritysdk-0.2.3/dexteritysdk/pyserum/structs/event_queue.py
--rw-r--r--   0        0        0     4849 2022-10-27 11:50:10.629553 dexteritysdk-0.2.3/dexteritysdk/pyserum/structs/slab.py
--rw-r--r--   0        0        0     1982 2022-08-24 13:49:21.987415 dexteritysdk-0.2.3/dexteritysdk/risk/actions.py
--rwxr-xr-x   0        0        0      644 2022-08-24 13:49:21.987521 dexteritysdk-0.2.3/dexteritysdk/scripts/build
--rw-r--r--   0        0        0      637 2022-08-24 13:49:21.987602 dexteritysdk-0.2.3/dexteritysdk/scripts/discriminant.py
--rw-r--r--   0        0        0     1001 2022-11-15 12:14:24.588496 dexteritysdk-0.2.3/dexteritysdk/scripts/extract_program_ids.py
--rw-r--r--   0        0        0     5370 2022-11-01 16:42:15.751927 dexteritysdk-0.2.3/dexteritysdk/scripts/generate_code.py
--rw-r--r--   0        0        0     1575 2022-08-24 13:49:21.987886 dexteritysdk-0.2.3/dexteritysdk/scripts/get_trader_risk_groups_key.py
--rw-r--r--   0        0        0      382 2022-08-24 13:49:21.987967 dexteritysdk-0.2.3/dexteritysdk/scripts/keypair_to_b58.py
--rw-r--r--   0        0        0      479 2022-08-24 13:49:21.988055 dexteritysdk-0.2.3/dexteritysdk/scripts/start_test_validator.py
--rw-r--r--   0        0        0     1890 2022-08-24 13:49:21.988179 dexteritysdk-0.2.3/dexteritysdk/solmate/__init__.py
--rw-r--r--   0        0        0      150 2022-08-24 13:49:21.988298 dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/__init__.py
--rw-r--r--   0        0        0    30166 2022-08-31 15:13:19.245018 dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/codegen.py
--rw-r--r--   0        0        0      398 2022-08-24 13:49:21.988565 dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/discriminant.py
--rw-r--r--   0        0        0     8605 2022-08-24 13:49:21.988670 dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/editor.py
--rw-r--r--   0        0        0     4473 2022-08-24 13:49:21.988761 dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/idl.py
--rw-r--r--   0        0        0      232 2022-08-24 13:49:21.988837 dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/sighash.py
--rw-r--r--   0        0        0     3112 2022-08-24 13:49:21.988926 dexteritysdk-0.2.3/dexteritysdk/solmate/cli.py
--rw-r--r--   0        0        0     2748 2022-08-24 13:49:21.989013 dexteritysdk-0.2.3/dexteritysdk/solmate/dtypes.py
--rw-r--r--   0        0        0      924 2022-08-24 13:49:21.989085 dexteritysdk-0.2.3/dexteritysdk/solmate/utils.py
--rw-r--r--   0        0        0      151 2022-08-24 13:49:21.989209 dexteritysdk-0.2.3/dexteritysdk/utils/__init__.py
--rw-r--r--   0        0        0       50 2022-08-24 13:49:21.989328 dexteritysdk-0.2.3/dexteritysdk/utils/aob/__init__.py
--rw-r--r--   0        0        0     1172 2022-08-24 13:49:21.989400 dexteritysdk-0.2.3/dexteritysdk/utils/aob/instructions.py
--rw-r--r--   0        0        0      570 2022-08-24 13:49:21.989506 dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/__init__.py
--rw-r--r--   0        0        0      530 2022-08-24 13:49:21.989573 dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/base.py
--rw-r--r--   0        0        0     3087 2022-08-24 13:49:21.989647 dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/event_queue.py
--rw-r--r--   0        0        0      394 2022-08-24 13:49:21.989715 dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/market_state.py
--rw-r--r--   0        0        0     6754 2022-08-24 13:49:21.989810 dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/slab.py
--rw-r--r--   0        0        0     4433 2022-08-24 13:49:21.989897 dexteritysdk-0.2.3/dexteritysdk/utils/binance_parser.py
--rw-r--r--   0        0        0      305 2022-08-24 13:49:21.989965 dexteritysdk-0.2.3/dexteritysdk/utils/random_hash.py
--rw-r--r--   0        0        0    13029 2023-01-18 19:16:53.029426 dexteritysdk-0.2.3/dexteritysdk/utils/solana.py
--rw-r--r--   0        0        0     3188 2023-01-25 18:12:44.040105 dexteritysdk-0.2.3/pyproject.toml
--rw-r--r--   0        0        0    10423 1970-01-01 00:00:00.000000 dexteritysdk-0.2.3/setup.py
--rw-r--r--   0        0        0     9492 1970-01-01 00:00:00.000000 dexteritysdk-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     4777 2023-03-17 11:59:21.422184 dexteritysdk-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2022-08-24 13:49:21.974698 dexteritysdk-0.2.8/dexteritysdk/__init__.py
+-rw-r--r--   0        0        0    18461 2022-09-08 12:11:13.318564 dexteritysdk-0.2.8/dexteritysdk/bots/bootstrap.py
+-rw-r--r--   0        0        0     8829 2022-08-24 13:49:21.975096 dexteritysdk-0.2.8/dexteritysdk/bots/consume_events_crank.py
+-rw-r--r--   0        0        0     6278 2022-08-24 13:49:21.975214 dexteritysdk-0.2.8/dexteritysdk/bots/expiration_routine.py
+-rwxr-xr-x   0        0        0     3042 2022-08-24 13:49:21.975334 dexteritysdk-0.2.8/dexteritysdk/bots/new_connect.py
+-rw-r--r--   0        0        0     7395 2022-08-24 13:49:21.975452 dexteritysdk-0.2.8/dexteritysdk/bots/oracle_price_crank.py
+-rwxr-xr-x   0        0        0     9186 2023-05-04 20:12:42.681780 dexteritysdk-0.2.8/dexteritysdk/bots/quoter_bot.py
+-rw-r--r--   0        0        0     4676 2022-08-24 13:49:21.975738 dexteritysdk-0.2.8/dexteritysdk/bots/settle_crank.py
+-rw-r--r--   0        0        0        0 2022-08-24 13:49:21.975778 dexteritysdk-0.2.8/dexteritysdk/bots/solmate_bootstrap.py
+-rw-r--r--   0        0        0     6329 2022-08-24 13:49:21.975918 dexteritysdk-0.2.8/dexteritysdk/bots/taker_bot.py
+-rw-r--r--   0        0        0       84 2022-09-07 16:16:02.404150 dexteritysdk-0.2.8/dexteritysdk/codegen/__init__.py
+-rw-r--r--   0        0        0      253 2022-09-07 16:16:02.404420 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/__init__.py
+-rw-r--r--   0        0        0      595 2022-09-07 16:16:02.404559 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/accounts.py
+-rw-r--r--   0        0        0      138 2022-09-07 16:16:02.404667 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/addrs.py
+-rw-r--r--   0        0        0      409 2022-09-07 16:16:02.404821 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/instructions/__init__.py
+-rw-r--r--   0        0        0     3269 2022-09-07 16:16:02.404965 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/instructions/create_risk_state_account.py
+-rw-r--r--   0        0        0      437 2022-09-07 16:16:02.405092 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/instructions/instruction_tag.py
+-rw-r--r--   0        0        0     3816 2022-09-07 16:16:02.405234 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/instructions/validate_account_health.py
+-rw-r--r--   0        0        0     3846 2022-09-07 16:16:02.405340 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/instructions/validate_account_liquidation.py
+-rw-r--r--   0        0        0       75 2022-09-07 16:16:02.405485 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/types/__init__.py
+-rw-r--r--   0        0        0      606 2022-09-07 16:16:02.405612 dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/types/health.py
+-rw-r--r--   0        0        0      264 2023-05-04 19:51:46.770090 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/__init__.py
+-rw-r--r--   0        0        0      264 2022-10-26 11:38:44.406419 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/__init__.py.py
+-rw-r--r--   0        0        0     1942 2023-05-04 19:51:46.778574 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/accounts.py
+-rw-r--r--   0        0        0      138 2023-05-04 19:51:46.770202 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/addrs.py
+-rw-r--r--   0        0        0      624 2023-05-04 19:51:46.778502 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/constants.py
+-rw-r--r--   0        0        0     3107 2023-05-04 19:51:46.778677 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/__init__.py
+-rw-r--r--   0        0        0     7007 2023-05-04 19:51:46.783169 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/cancel_order.py
+-rw-r--r--   0        0        0     2533 2023-05-04 19:51:46.784535 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/choose_successor.py
+-rw-r--r--   0        0        0     2206 2023-05-04 19:51:46.784608 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/claim_authority.py
+-rw-r--r--   0        0        0     4397 2023-05-04 19:51:46.784192 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/clear_expired_orderbook.py
+-rw-r--r--   0        0        0     2872 2023-05-04 19:51:46.782266 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/clear_open_orders.py
+-rw-r--r--   0        0        0     2882 2023-05-04 19:51:46.781670 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/close_trader_risk_group.py
+-rw-r--r--   0        0        0     5855 2023-05-04 19:51:46.782807 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/consume_orderbook_events.py
+-rw-r--r--   0        0        0     4451 2023-05-04 19:51:46.780150 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/deactivate_market_product.py
+-rw-r--r--   0        0        0     4369 2023-05-04 19:51:46.783405 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/deposit_funds.py
+-rw-r--r--   0        0        0     2192 2023-05-04 19:51:46.784899 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/disable_killswitch.py
+-rw-r--r--   0        0        0     2186 2023-05-04 19:51:46.785040 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/enable_killswitch.py
+-rw-r--r--   0        0        0     2754 2023-05-04 19:51:46.783974 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_combo.py
+-rw-r--r--   0        0        0     3144 2023-05-04 19:51:46.779631 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_market_product.py
+-rw-r--r--   0        0        0     7893 2023-05-04 19:51:46.779421 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_market_product_group.py
+-rw-r--r--   0        0        0     4459 2023-05-04 19:51:46.780820 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_print_trade.py
+-rw-r--r--   0        0        0     4587 2023-05-04 19:51:46.781521 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_trader_risk_group.py
+-rw-r--r--   0        0        0     2028 2023-05-04 19:51:46.785132 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/instruction_tag.py
+-rw-r--r--   0        0        0     9466 2023-05-04 19:51:46.781926 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/new_order.py
+-rw-r--r--   0        0        0     4033 2023-05-04 19:51:46.784328 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/pop_events.py
+-rw-r--r--   0        0        0     2193 2023-05-04 19:51:46.780642 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/remove_market_product.py
+-rw-r--r--   0        0        0     2242 2023-05-04 19:51:46.780732 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/remove_market_product_group.py
+-rw-r--r--   0        0        0     2829 2023-05-04 19:51:46.782379 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/set_num_risk_state_accounts.py
+-rw-r--r--   0        0        0     3019 2023-05-04 19:51:46.784686 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/setup_capital_limits.py
+-rw-r--r--   0        0        0     9361 2023-05-04 19:51:46.781242 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/sign_print_trade.py
+-rw-r--r--   0        0        0     4454 2023-05-04 19:51:46.784399 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/sweep_fees.py
+-rw-r--r--   0        0        0     5721 2023-05-04 19:51:46.783837 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/transfer_full_position.py
+-rw-r--r--   0        0        0     3270 2023-05-04 19:51:46.784755 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_capital_limits.py
+-rw-r--r--   0        0        0     2939 2023-05-04 19:51:46.779554 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_market_product_group.py
+-rw-r--r--   0        0        0     2471 2023-05-04 19:51:46.783689 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_product_funding.py
+-rw-r--r--   0        0        0     2880 2023-05-04 19:51:46.783765 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_product_mark_price_config.py
+-rw-r--r--   0        0        0     4387 2023-05-04 19:51:46.784053 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_trader_funding.py
+-rw-r--r--   0        0        0     2523 2023-05-04 19:51:46.784830 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_trader_risk_group_owner.py
+-rw-r--r--   0        0        0     2523 2023-05-04 19:19:47.538783 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_trader_risk_group_owner.py.old
+-rw-r--r--   0        0        0     5083 2023-05-04 19:51:46.782473 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_variance_cache.py
+-rw-r--r--   0        0        0     6429 2023-05-04 19:51:46.783547 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/withdraw_funds.py
+-rw-r--r--   0        0        0     2505 2023-05-04 19:51:46.770512 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-04 19:51:46.777161 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/account_tag.py
+-rw-r--r--   0        0        0      858 2023-05-04 19:51:46.777653 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/action_status.py
+-rw-r--r--   0        0        0      453 2023-05-04 19:51:46.772734 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/bitset.py
+-rw-r--r--   0        0        0      503 2023-05-04 19:51:46.770741 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/call_back_info.py
+-rw-r--r--   0        0        0      458 2023-05-04 19:51:46.775305 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/cancel_order_params.py
+-rw-r--r--   0        0        0      628 2023-05-04 19:51:46.777728 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/capital_limits.py
+-rw-r--r--   0        0        0      535 2023-05-04 19:51:46.778430 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/capital_limits_params.py
+-rw-r--r--   0        0        0      469 2023-05-04 19:51:46.776898 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/clear_expired_orderbook_params.py
+-rw-r--r--   0        0        0      670 2023-05-04 19:51:46.772282 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/combo.py
+-rw-r--r--   0        0        0      467 2023-05-04 19:51:46.774759 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/consume_orderbook_events_params.py
+-rw-r--r--   0        0        0      495 2023-05-04 19:51:46.775533 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/deposit_funds_params.py
+-rw-r--r--   0        0        0     3483 2023-05-04 19:51:46.777086 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/dex_error.py
+-rw-r--r--   0        0        0     3347 2023-05-04 19:51:46.773140 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/fractional.py
+-rw-r--r--   0        0        0      583 2023-05-04 19:51:46.772413 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/health_info.py
+-rw-r--r--   0        0        0      778 2023-05-04 19:51:46.777526 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/health_result.py
+-rw-r--r--   0        0        0      906 2023-05-04 19:51:46.777591 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/health_status.py
+-rw-r--r--   0        0        0      668 2023-05-04 19:51:46.776435 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/initialize_combo_params.py
+-rw-r--r--   0        0        0      955 2023-05-04 19:51:46.773207 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/initialize_market_product_group_params.py
+-rw-r--r--   0        0        0      647 2023-05-04 19:51:46.774079 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/initialize_market_product_params.py
+-rw-r--r--   0        0        0      767 2023-05-04 19:51:46.773940 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/initialize_print_trade_params.py
+-rw-r--r--   0        0        0      545 2023-05-04 19:51:46.772347 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/leg.py
+-rw-r--r--   0        0        0      875 2023-05-04 19:51:46.772480 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/liquidation_info.py
+-rw-r--r--   0        0        0     3458 2023-05-04 20:06:27.289397 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/market_product_group.py
+-rw-r--r--   0        0        0      824 2023-05-04 19:51:46.774147 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/new_order_params.py
+-rw-r--r--   0        0        0      786 2023-05-04 19:51:46.771138 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/open_orders.py
+-rw-r--r--   0        0        0      649 2023-05-04 19:51:46.771062 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/open_orders_metadata.py
+-rw-r--r--   0        0        0      548 2023-05-04 19:51:46.771509 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/open_orders_node.py
+-rw-r--r--   0        0        0      975 2023-05-04 19:51:46.777451 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/operation_type.py
+-rw-r--r--   0        0        0      868 2023-05-04 19:51:46.772610 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/order_info.py
+-rw-r--r--   0        0        0      901 2023-05-04 19:51:46.777297 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/order_type.py
+-rw-r--r--   0        0        0     1297 2023-05-04 19:51:46.771734 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/outright.py
+-rw-r--r--   0        0        0      473 2023-05-04 19:51:46.770614 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/params.py
+-rw-r--r--   0        0        0      444 2023-05-04 19:51:46.776773 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/pop_events_params.py
+-rw-r--r--   0        0        0      691 2023-05-04 19:51:46.770979 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/price_ewma.py
+-rw-r--r--   0        0        0      892 2023-05-04 19:51:46.778225 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/print_trade.py
+-rw-r--r--   0        0        0      555 2023-05-04 19:19:47.538949 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/print_trade_product.py
+-rw-r--r--   0        0        0      570 2023-05-04 19:19:47.539072 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/print_trade_product_index.py
+-rw-r--r--   0        0        0     1644 2023-05-04 19:51:46.777372 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/product.py
+-rw-r--r--   0        0        0      519 2023-05-04 19:51:46.778159 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/product_array.py
+-rw-r--r--   0        0        0      855 2023-05-04 19:51:46.771848 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/product_metadata.py
+-rw-r--r--   0        0        0      903 2023-05-04 19:51:46.777230 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/product_status.py
+-rw-r--r--   0        0        0      512 2023-05-04 19:51:46.778287 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/risk_output_register.py
+-rw-r--r--   0        0        0      508 2023-05-04 19:51:46.774636 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/set_num_risk_state_accounts_params.py
+-rw-r--r--   0        0        0      755 2023-05-04 19:51:46.774011 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/sign_print_trade_params.py
+-rw-r--r--   0        0        0      550 2023-05-04 19:51:46.772543 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/social_loss.py
+-rw-r--r--   0        0        0      686 2023-05-04 19:51:46.770900 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/trader_fee_params.py
+-rw-r--r--   0        0        0      538 2023-05-04 19:51:46.770825 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/trader_fees.py
+-rw-r--r--   0        0        0      837 2023-05-04 19:51:46.772674 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/trader_position.py
+-rw-r--r--   0        0        0     1352 2023-05-04 19:51:46.778362 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/trader_risk_group.py
+-rw-r--r--   0        0        0      438 2023-05-04 19:51:46.773875 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/update_market_product_group_params.py
+-rw-r--r--   0        0        0      621 2023-05-04 19:51:46.776030 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/update_product_funding_params.py
+-rw-r--r--   0        0        0      598 2023-05-04 19:51:46.776350 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/update_product_mark_price_config_params.py
+-rw-r--r--   0        0        0     1385 2023-05-04 19:51:46.776989 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/util_error.py
+-rw-r--r--   0        0        0      497 2023-05-04 19:51:46.775607 dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/withdraw_funds_params.py
+-rw-r--r--   0        0        0      234 2023-05-04 19:51:46.787964 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/__init__.py
+-rw-r--r--   0        0        0      639 2023-05-04 19:51:46.788897 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/accounts.py
+-rw-r--r--   0        0        0      138 2023-05-04 19:51:46.788057 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/addrs.py
+-rw-r--r--   0        0        0      370 2023-05-04 19:51:46.788973 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/__init__.py
+-rw-r--r--   0        0        0     2603 2023-05-04 19:51:46.789228 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/close_derivative_account.py
+-rw-r--r--   0        0        0     3613 2023-05-04 19:51:46.789056 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/initialize_derivative.py
+-rw-r--r--   0        0        0     3299 2022-09-07 16:16:02.407477 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/initialize_fixed_income.py
+-rw-r--r--   0        0        0      423 2023-05-04 19:51:46.789310 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/instruction_tag.py
+-rw-r--r--   0        0        0     2948 2023-05-04 19:51:46.789138 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/settle_derivative.py
+-rw-r--r--   0        0        0     2629 2022-09-07 16:16:02.407586 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/settle_fixed_income.py
+-rw-r--r--   0        0        0      379 2023-05-04 20:06:29.687281 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/__init__.py
+-rw-r--r--   0        0        0      899 2023-05-04 19:51:46.788492 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/account_tag.py
+-rw-r--r--   0        0        0     1199 2023-05-04 19:51:46.788379 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/derivative_error.py
+-rw-r--r--   0        0        0     1331 2023-05-04 20:06:29.687508 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/derivative_metadata.py
+-rw-r--r--   0        0        0      879 2023-05-04 19:51:46.788739 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/expiration_status.py
+-rw-r--r--   0        0        0     1029 2022-09-07 16:16:02.407732 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/fixed_income_metadata.py
+-rw-r--r--   0        0        0      440 2023-05-04 19:51:46.788231 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/fractional.py
+-rw-r--r--   0        0        0      977 2023-05-04 20:06:29.687682 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/initialize_derivative_params.py
+-rw-r--r--   0        0        0      748 2022-09-07 16:16:02.407828 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/initialize_fixed_income_params.py
+-rw-r--r--   0        0        0      943 2023-05-04 19:51:46.788596 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/instrument_type.py
+-rw-r--r--   0        0        0      868 2023-05-04 19:51:46.788667 dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/oracle_type.py
+-rw-r--r--   0        0        0      124 2022-09-07 16:16:02.407957 dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/__init__.py
+-rw-r--r--   0        0        0      138 2022-09-07 16:16:02.408030 dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/addrs.py
+-rw-r--r--   0        0        0      409 2022-09-07 16:16:02.408146 dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/instructions/__init__.py
+-rw-r--r--   0        0        0     3270 2022-09-07 16:16:02.408235 dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/instructions/create_risk_state_account.py
+-rw-r--r--   0        0        0      437 2022-09-07 16:16:02.408323 dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/instructions/instruction_tag.py
+-rw-r--r--   0        0        0     3961 2022-09-07 16:16:02.408404 dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/instructions/validate_account_health.py
+-rw-r--r--   0        0        0     3991 2022-09-07 16:16:02.408481 dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/instructions/validate_account_liquidation.py
+-rw-r--r--   0        0        0      296 2023-05-04 19:51:46.793645 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/__init__.py
+-rw-r--r--   0        0        0     1091 2023-05-04 19:51:46.794772 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/accounts.py
+-rw-r--r--   0        0        0      138 2023-05-04 19:51:46.793743 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/addrs.py
+-rw-r--r--   0        0        0      180 2023-05-04 19:51:46.794703 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/constants.py
+-rw-r--r--   0        0        0     1044 2023-05-04 19:51:46.794853 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/__init__.py
+-rw-r--r--   0        0        0     2808 2023-05-04 19:51:46.795569 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/close_mark_prices.py
+-rw-r--r--   0        0        0     3302 2023-05-04 19:51:46.795345 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/create_risk_state_account.py
+-rw-r--r--   0        0        0     3739 2023-05-04 19:51:46.795417 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/initialize_covariance_matrix.py
+-rw-r--r--   0        0        0     3528 2023-05-04 19:51:46.795489 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/initialize_mark_prices.py
+-rw-r--r--   0        0        0      788 2023-05-04 19:51:46.795782 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/instruction_tag.py
+-rw-r--r--   0        0        0     3758 2023-05-04 19:51:46.795709 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/remove_market_product_index_from_variance_cache.py
+-rw-r--r--   0        0        0     2536 2023-05-04 19:51:46.794932 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/resize_variance_cache.py
+-rw-r--r--   0        0        0     2494 2023-05-04 19:51:46.795636 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/update_mark_prices.py
+-rw-r--r--   0        0        0     5177 2023-05-04 19:51:46.795020 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/validate_account_health.py
+-rw-r--r--   0        0        0     4991 2023-05-04 19:51:46.795198 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/validate_account_liquidation.py
+-rw-r--r--   0        0        0      452 2023-05-04 19:51:46.793896 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/__init__.py
+-rw-r--r--   0        0        0      665 2023-05-04 19:51:46.794363 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/correlation_matrix.py
+-rw-r--r--   0        0        0      880 2023-05-04 19:51:46.794460 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/covariance_metadata.py
+-rw-r--r--   0        0        0      418 2023-05-04 19:51:46.793974 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/fast_int.py
+-rw-r--r--   0        0        0      634 2023-05-04 19:51:46.794122 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/initialize_mark_prices_params.py
+-rw-r--r--   0        0        0      981 2023-05-04 19:51:59.201333 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/mark_price.py
+-rw-r--r--   0        0        0      845 2023-05-04 19:52:04.919716 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/mark_prices_array.py
+-rw-r--r--   0        0        0      930 2023-05-04 19:51:46.794268 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/risk_account_tag.py
+-rw-r--r--   0        0        0     1772 2023-05-04 19:51:46.794194 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/risk_error.py
+-rw-r--r--   0        0        0      927 2023-05-04 19:51:46.794632 dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/variance_cache.py
+-rw-r--r--   0        0        0     2418 2022-08-24 13:49:21.985348 dexteritysdk-0.2.8/dexteritysdk/constant_fees/actions.py
+-rw-r--r--   0        0        0        0 2022-08-24 13:49:21.985383 dexteritysdk-0.2.8/dexteritysdk/constant_fees/addrs.py
+-rw-r--r--   0        0        0     2251 2022-08-24 13:49:21.985473 dexteritysdk-0.2.8/dexteritysdk/constant_fees/instructions.py
+-rw-r--r--   0        0        0      162 2022-08-24 13:49:21.985545 dexteritysdk-0.2.8/dexteritysdk/constant_fees/state.py
+-rw-r--r--   0        0        0    41508 2022-09-08 12:11:05.816702 dexteritysdk-0.2.8/dexteritysdk/dex/actions.py
+-rw-r--r--   0        0        0     4443 2023-03-29 18:27:50.920383 dexteritysdk-0.2.8/dexteritysdk/dex/addrs.py
+-rw-r--r--   0        0        0    49294 2023-05-04 20:07:37.624315 dexteritysdk-0.2.8/dexteritysdk/dex/sdk_context.py
+-rw-r--r--   0        0        0     3046 2022-08-24 13:49:21.986089 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/actions.py
+-rw-r--r--   0        0        0      410 2022-08-24 13:49:21.986210 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/__init__.py
+-rw-r--r--   0        0        0      204 2022-08-24 13:49:21.986279 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/common.py
+-rw-r--r--   0        0        0      825 2022-08-24 13:49:21.986349 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/initialize_clock.py
+-rw-r--r--   0        0        0      956 2022-08-24 13:49:21.986427 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/initialize_oracle.py
+-rw-r--r--   0        0        0     1020 2022-08-24 13:49:21.986495 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/update_clock.py
+-rw-r--r--   0        0        0      962 2022-08-24 13:49:21.986563 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/update_price.py
+-rw-r--r--   0        0        0      459 2022-08-24 13:49:21.986667 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/state/__init__.py
+-rw-r--r--   0        0        0      168 2022-08-24 13:49:21.986739 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/state/clock.py
+-rw-r--r--   0        0        0      117 2022-08-24 13:49:21.986798 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/state/common.py
+-rw-r--r--   0        0        0      260 2022-08-24 13:49:21.986866 dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/state/oracle_price.py
+-rw-r--r--   0        0        0     4543 2022-08-24 13:49:21.986982 dexteritysdk-0.2.8/dexteritysdk/instruments/actions.py
+-rw-r--r--   0        0        0      125 2022-08-24 13:49:21.987080 dexteritysdk-0.2.8/dexteritysdk/instruments/instructions/__init__.py
+-rw-r--r--   0        0        0     1163 2022-08-24 13:49:21.987149 dexteritysdk-0.2.8/dexteritysdk/instruments/instructions/initialize_derivative.py
+-rw-r--r--   0        0        0      702 2022-08-24 13:49:21.987225 dexteritysdk-0.2.8/dexteritysdk/instruments/instructions/initialize_fixed_income.py
+-rw-r--r--   0        0        0      121 2022-09-27 20:09:16.734330 dexteritysdk-0.2.8/dexteritysdk/mints.py
+-rw-r--r--   0        0        0     2125 2023-03-29 18:27:50.921690 dexteritysdk-0.2.8/dexteritysdk/program_ids.py
+-rw-r--r--   0        0        0        0 2022-09-14 12:42:20.447710 dexteritysdk-0.2.8/dexteritysdk/pyserum/__init__.py
+-rw-r--r--   0        0        0      406 2022-09-14 12:42:20.448359 dexteritysdk-0.2.8/dexteritysdk/pyserum/enums.py
+-rw-r--r--   0        0        0     1952 2022-10-27 11:50:10.627988 dexteritysdk-0.2.8/dexteritysdk/pyserum/event_queue.py
+-rw-r--r--   0        0        0        0 2022-10-27 11:50:10.628019 dexteritysdk-0.2.8/dexteritysdk/pyserum/layouts/__init__.py
+-rw-r--r--   0        0        0     1292 2022-10-27 11:50:10.628342 dexteritysdk-0.2.8/dexteritysdk/pyserum/layouts/event_queue.py
+-rw-r--r--   0        0        0     1803 2022-10-27 11:50:10.628583 dexteritysdk-0.2.8/dexteritysdk/pyserum/layouts/slab.py
+-rw-r--r--   0        0        0     3094 2022-10-27 11:50:10.628776 dexteritysdk-0.2.8/dexteritysdk/pyserum/orderbook.py
+-rw-r--r--   0        0        0      338 2022-10-27 11:50:10.628969 dexteritysdk-0.2.8/dexteritysdk/pyserum/serum_types.py
+-rw-r--r--   0        0        0        0 2022-10-27 11:50:10.629018 dexteritysdk-0.2.8/dexteritysdk/pyserum/structs/__init__.py
+-rw-r--r--   0        0        0     2132 2022-10-27 11:50:10.629382 dexteritysdk-0.2.8/dexteritysdk/pyserum/structs/event_queue.py
+-rw-r--r--   0        0        0     4849 2022-10-27 11:50:10.629553 dexteritysdk-0.2.8/dexteritysdk/pyserum/structs/slab.py
+-rw-r--r--   0        0        0     1982 2022-08-24 13:49:21.987415 dexteritysdk-0.2.8/dexteritysdk/risk/actions.py
+-rwxr-xr-x   0        0        0      644 2022-08-24 13:49:21.987521 dexteritysdk-0.2.8/dexteritysdk/scripts/build
+-rw-r--r--   0        0        0      637 2022-08-24 13:49:21.987602 dexteritysdk-0.2.8/dexteritysdk/scripts/discriminant.py
+-rw-r--r--   0        0        0     1001 2022-11-15 12:14:24.588496 dexteritysdk-0.2.8/dexteritysdk/scripts/extract_program_ids.py
+-rw-r--r--   0        0        0     5370 2022-11-01 16:42:15.751927 dexteritysdk-0.2.8/dexteritysdk/scripts/generate_code.py
+-rw-r--r--   0        0        0     1575 2022-08-24 13:49:21.987886 dexteritysdk-0.2.8/dexteritysdk/scripts/get_trader_risk_groups_key.py
+-rw-r--r--   0        0        0      382 2022-08-24 13:49:21.987967 dexteritysdk-0.2.8/dexteritysdk/scripts/keypair_to_b58.py
+-rw-r--r--   0        0        0      479 2022-08-24 13:49:21.988055 dexteritysdk-0.2.8/dexteritysdk/scripts/start_test_validator.py
+-rw-r--r--   0        0        0     1890 2022-08-24 13:49:21.988179 dexteritysdk-0.2.8/dexteritysdk/solmate/__init__.py
+-rw-r--r--   0        0        0      150 2022-08-24 13:49:21.988298 dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/__init__.py
+-rw-r--r--   0        0        0    30166 2022-08-31 15:13:19.245018 dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/codegen.py
+-rw-r--r--   0        0        0      398 2022-08-24 13:49:21.988565 dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/discriminant.py
+-rw-r--r--   0        0        0     8605 2022-08-24 13:49:21.988670 dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/editor.py
+-rw-r--r--   0        0        0     4473 2022-08-24 13:49:21.988761 dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/idl.py
+-rw-r--r--   0        0        0      232 2023-02-10 13:58:01.771202 dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/sighash.py
+-rw-r--r--   0        0        0     3112 2022-08-24 13:49:21.988926 dexteritysdk-0.2.8/dexteritysdk/solmate/cli.py
+-rw-r--r--   0        0        0     2748 2022-08-24 13:49:21.989013 dexteritysdk-0.2.8/dexteritysdk/solmate/dtypes.py
+-rw-r--r--   0        0        0      924 2022-08-24 13:49:21.989085 dexteritysdk-0.2.8/dexteritysdk/solmate/utils.py
+-rw-r--r--   0        0        0      151 2022-08-24 13:49:21.989209 dexteritysdk-0.2.8/dexteritysdk/utils/__init__.py
+-rw-r--r--   0        0        0       50 2022-08-24 13:49:21.989328 dexteritysdk-0.2.8/dexteritysdk/utils/aob/__init__.py
+-rw-r--r--   0        0        0     1172 2022-08-24 13:49:21.989400 dexteritysdk-0.2.8/dexteritysdk/utils/aob/instructions.py
+-rw-r--r--   0        0        0      570 2022-08-24 13:49:21.989506 dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/__init__.py
+-rw-r--r--   0        0        0      530 2022-08-24 13:49:21.989573 dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/base.py
+-rw-r--r--   0        0        0     3087 2022-08-24 13:49:21.989647 dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/event_queue.py
+-rw-r--r--   0        0        0      394 2022-08-24 13:49:21.989715 dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/market_state.py
+-rw-r--r--   0        0        0     6754 2022-08-24 13:49:21.989810 dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/slab.py
+-rw-r--r--   0        0        0     4433 2022-08-24 13:49:21.989897 dexteritysdk-0.2.8/dexteritysdk/utils/binance_parser.py
+-rw-r--r--   0        0        0      305 2022-08-24 13:49:21.989965 dexteritysdk-0.2.8/dexteritysdk/utils/random_hash.py
+-rw-r--r--   0        0        0    13029 2023-01-18 19:16:53.029426 dexteritysdk-0.2.8/dexteritysdk/utils/solana.py
+-rw-r--r--   0        0        0     3188 2023-05-04 20:18:56.886267 dexteritysdk-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    10451 1970-01-01 00:00:00.000000 dexteritysdk-0.2.8/setup.py
+-rw-r--r--   0        0        0     9518 1970-01-01 00:00:00.000000 dexteritysdk-0.2.8/PKG-INFO
```

### Comparing `dexteritysdk-0.2.3/README.md` & `dexteritysdk-0.2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 ```python
 # this will withdraw 0.1 USDC back to your wallet
 trader.withdraw(ctx, 0.1)
 ```
 
 You can check your balance at any time.
 ```python
-trader.get_trader_risk_group().cash_balance
+trg, _ = trader.get_trader_risk_group()
+trg.cash_balance
 ```
 
 ## Trading on Dexterity
 
 ### Listing trading products and order books
 The `products` field of a `SDKContext` instance, is a list of the available trading products (`SDKProduct`).
 Every `SDKProduct` has a `name` and a `get_orderbook(ctx)` function that will return its order book (`SDKOrderBook`).
@@ -139,9 +140,10 @@
 trader.cancel_all_orders(ctx, products)
 ```
 If any cancel fails, an exception will be raised.
 
 ### Positions
 Positions can also be listed, by iterating the `trader_positions` array:
 ```python
-trader.get_trader_risk_group().trader_positions
+trg, _ = trader.get_trader_risk_group()
+trg.trader_positions
 ```
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/bots/bootstrap.py` & `dexteritysdk-0.2.8/dexteritysdk/bots/bootstrap.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/bots/consume_events_crank.py` & `dexteritysdk-0.2.8/dexteritysdk/bots/consume_events_crank.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/bots/expiration_routine.py` & `dexteritysdk-0.2.8/dexteritysdk/bots/expiration_routine.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/bots/new_connect.py` & `dexteritysdk-0.2.8/dexteritysdk/bots/new_connect.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/bots/oracle_price_crank.py` & `dexteritysdk-0.2.8/dexteritysdk/bots/oracle_price_crank.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/bots/quoter_bot.py` & `dexteritysdk-0.2.8/dexteritysdk/bots/quoter_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,14 +205,15 @@
     print(f"keypair pubkey = {keypair.public_key}")
 
     sdk = SDKContext.connect(
         client,
         market_product_group_key=mpg_key,
         payer=keypair,
         **programs,
+        fee_model_program_id=PublicKey("5u8mLVnUSQNSbKdZPNGTfWHGwV5uJh9by5Fa6jb6BP6h"),
         raise_on_error=True
     )
 
     wallet = instructions.get_associated_token_address(keypair.public_key, sdk.vault_mint)
     print(f"wallet = {wallet}")
 
     if args.trader_risk_group is None:
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/bots/settle_crank.py` & `dexteritysdk-0.2.8/dexteritysdk/bots/settle_crank.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/bots/taker_bot.py` & `dexteritysdk-0.2.8/dexteritysdk/bots/taker_bot.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/accounts.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/accounts.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/instructions/create_risk_state_account.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/instructions/create_risk_state_account.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/instructions/validate_account_health.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/instructions/validate_account_health.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/instructions/validate_account_liquidation.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/instructions/validate_account_liquidation.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/alpha_risk_engine/types/health.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/alpha_risk_engine/types/health.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/accounts.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/accounts.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/constants.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/constants.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/__init__.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,26 +15,38 @@
     ClearExpiredOrderbookIx,
     clear_expired_orderbook,
 )
 from .clear_open_orders import (
     ClearOpenOrdersIx,
     clear_open_orders,
 )
+from .close_trader_risk_group import (
+    CloseTraderRiskGroupIx,
+    close_trader_risk_group,
+)
 from .consume_orderbook_events import (
     ConsumeOrderbookEventsIx,
     consume_orderbook_events,
 )
 from .deactivate_market_product import (
     DeactivateMarketProductIx,
     deactivate_market_product,
 )
 from .deposit_funds import (
     DepositFundsIx,
     deposit_funds,
 )
+from .disable_killswitch import (
+    DisableKillswitchIx,
+    disable_killswitch,
+)
+from .enable_killswitch import (
+    EnableKillswitchIx,
+    enable_killswitch,
+)
 from .initialize_combo import (
     InitializeComboIx,
     initialize_combo,
 )
 from .initialize_market_product import (
     InitializeMarketProductIx,
     initialize_market_product,
@@ -64,14 +76,18 @@
     RemoveMarketProductIx,
     remove_market_product,
 )
 from .remove_market_product_group import (
     RemoveMarketProductGroupIx,
     remove_market_product_group,
 )
+from .set_num_risk_state_accounts import (
+    SetNumRiskStateAccountsIx,
+    set_num_risk_state_accounts,
+)
 from .setup_capital_limits import (
     SetupCapitalLimitsIx,
     setup_capital_limits,
 )
 from .sign_print_trade import (
     SignPrintTradeIx,
     sign_print_trade,
@@ -92,14 +108,18 @@
     UpdateMarketProductGroupIx,
     update_market_product_group,
 )
 from .update_product_funding import (
     UpdateProductFundingIx,
     update_product_funding,
 )
+from .update_product_mark_price_config import (
+    UpdateProductMarkPriceConfigIx,
+    update_product_mark_price_config,
+)
 from .update_trader_funding import (
     UpdateTraderFundingIx,
     update_trader_funding,
 )
 from .update_trader_risk_group_owner import (
     UpdateTraderRiskGroupOwnerIx,
     update_trader_risk_group_owner,
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/cancel_order.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/cancel_order.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/choose_successor.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/choose_successor.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/claim_authority.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/claim_authority.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/clear_expired_orderbook.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/clear_expired_orderbook.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/clear_open_orders.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/clear_open_orders.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/consume_orderbook_events.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/consume_orderbook_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
             is_signer=False,
             is_writable=False,
         )
     if isinstance(fee_model_configuration_acct, (str, PublicKey)):
         fee_model_configuration_acct = to_account_meta(
             fee_model_configuration_acct,
             is_signer=False,
-            is_writable=False,
+            is_writable=True,
         )
     if isinstance(fee_output_register, (str, PublicKey)):
         fee_output_register = to_account_meta(
             fee_output_register,
             is_signer=False,
             is_writable=True,
         )
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/deactivate_market_product.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/deactivate_market_product.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/deposit_funds.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/deposit_funds.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,30 +28,28 @@
     token_program: AccountMeta
     user: AccountMeta
     user_token_account: AccountMeta
     trader_risk_group: AccountMeta
     market_product_group: AccountMeta
     market_product_group_vault: AccountMeta
     capital_limits: AccountMeta
-    whitelist_ata_acct: AccountMeta
     remaining_accounts: Optional[List[AccountMeta]]
 
     # data fields
     params: DepositFundsParams
 
     def to_instruction(self):
         keys = []
         keys.append(self.token_program)
         keys.append(self.user)
         keys.append(self.user_token_account)
         keys.append(self.trader_risk_group)
         keys.append(self.market_product_group)
         keys.append(self.market_product_group_vault)
         keys.append(self.capital_limits)
-        keys.append(self.whitelist_ata_acct)
         if self.remaining_accounts is not None:
             keys.extend(self.remaining_accounts)
 
         buffer = BytesIO()
         buffer.write(InstructionTag.to_bytes(InstructionTag.DEPOSIT_FUNDS))
         buffer.write(BYTES_CATALOG.pack(DepositFundsParams, self.params))
 
@@ -68,15 +66,14 @@
 def deposit_funds(
     user: Union[str, PublicKey, AccountMeta],
     user_token_account: Union[str, PublicKey, AccountMeta],
     trader_risk_group: Union[str, PublicKey, AccountMeta],
     market_product_group: Union[str, PublicKey, AccountMeta],
     market_product_group_vault: Union[str, PublicKey, AccountMeta],
     capital_limits: Union[str, PublicKey, AccountMeta],
-    whitelist_ata_acct: Union[str, PublicKey, AccountMeta],
     params: DepositFundsParams,
     token_program: Union[str, PublicKey, AccountMeta] = PublicKey("TokenkegQfeZyiNwAJbNbGKPFXCWuBvf9Ss623VQ5DA"),
     remaining_accounts: Optional[List[AccountMeta]] = None,
     program_id: Optional[PublicKey] = None,
 ):
     if program_id is None:
         program_id = PublicKey("FUfpR31LmcP1VSbz5zDaM7nxnH55iBHkpwusgrnhaFjL")
@@ -119,29 +116,22 @@
         )
     if isinstance(capital_limits, (str, PublicKey)):
         capital_limits = to_account_meta(
             capital_limits,
             is_signer=False,
             is_writable=False,
         )
-    if isinstance(whitelist_ata_acct, (str, PublicKey)):
-        whitelist_ata_acct = to_account_meta(
-            whitelist_ata_acct,
-            is_signer=False,
-            is_writable=False,
-        )
 
     return DepositFundsIx(
         program_id=program_id,
         token_program=token_program,
         user=user,
         user_token_account=user_token_account,
         trader_risk_group=trader_risk_group,
         market_product_group=market_product_group,
         market_product_group_vault=market_product_group_vault,
         capital_limits=capital_limits,
-        whitelist_ata_acct=whitelist_ata_acct,
         remaining_accounts=remaining_accounts,
         params=params,
     ).to_instruction()
 
 # LOCK-END
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_combo.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_combo.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_market_product.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_market_product.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 ):
     if program_id is None:
         program_id = PublicKey("FUfpR31LmcP1VSbz5zDaM7nxnH55iBHkpwusgrnhaFjL")
 
     if isinstance(authority, (str, PublicKey)):
         authority = to_account_meta(
             authority,
-            is_signer=True,
+            is_signer=False,
             is_writable=False,
         )
     if isinstance(market_product_group, (str, PublicKey)):
         market_product_group = to_account_meta(
             market_product_group,
             is_signer=False,
             is_writable=True,
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_market_product_group.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_market_product_group.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_print_trade.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_print_trade.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/initialize_trader_risk_group.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/initialize_trader_risk_group.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/instruction_tag.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/instruction_tag.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,29 +17,34 @@
     INITIALIZE_MARKET_PRODUCT = InstructionDiscriminant()
     DEACTIVATE_MARKET_PRODUCT = InstructionDiscriminant()
     REMOVE_MARKET_PRODUCT = InstructionDiscriminant()
     REMOVE_MARKET_PRODUCT_GROUP = InstructionDiscriminant()
     INITIALIZE_PRINT_TRADE = InstructionDiscriminant()
     SIGN_PRINT_TRADE = InstructionDiscriminant()
     INITIALIZE_TRADER_RISK_GROUP = InstructionDiscriminant()
+    CLOSE_TRADER_RISK_GROUP = InstructionDiscriminant()
     NEW_ORDER = InstructionDiscriminant()
     CLEAR_OPEN_ORDERS = InstructionDiscriminant()
+    SET_NUM_RISK_STATE_ACCOUNTS = InstructionDiscriminant()
     UPDATE_VARIANCE_CACHE = InstructionDiscriminant()
     CONSUME_ORDERBOOK_EVENTS = InstructionDiscriminant()
     CANCEL_ORDER = InstructionDiscriminant()
     DEPOSIT_FUNDS = InstructionDiscriminant()
     WITHDRAW_FUNDS = InstructionDiscriminant()
     UPDATE_PRODUCT_FUNDING = InstructionDiscriminant()
+    UPDATE_PRODUCT_MARK_PRICE_CONFIG = InstructionDiscriminant()
     TRANSFER_FULL_POSITION = InstructionDiscriminant()
     INITIALIZE_COMBO = InstructionDiscriminant()
     UPDATE_TRADER_FUNDING = InstructionDiscriminant()
     CLEAR_EXPIRED_ORDERBOOK = InstructionDiscriminant()
     POP_EVENTS = InstructionDiscriminant()
     SWEEP_FEES = InstructionDiscriminant()
     CHOOSE_SUCCESSOR = InstructionDiscriminant()
     CLAIM_AUTHORITY = InstructionDiscriminant()
     SETUP_CAPITAL_LIMITS = InstructionDiscriminant()
     UPDATE_CAPITAL_LIMITS = InstructionDiscriminant()
     UPDATE_TRADER_RISK_GROUP_OWNER = InstructionDiscriminant()
+    DISABLE_KILLSWITCH = InstructionDiscriminant()
+    ENABLE_KILLSWITCH = InstructionDiscriminant()
     # LOCK-END
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/new_order.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/new_order.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     trader_fee_state_acct: AccountMeta
     fee_output_register: AccountMeta
     risk_engine_program: AccountMeta
     risk_model_configuration_acct: AccountMeta
     risk_output_register: AccountMeta
     trader_risk_state_acct: AccountMeta
     risk_and_fee_signer: AccountMeta
+    referrer_trg: AccountMeta
     remaining_accounts: Optional[List[AccountMeta]]
 
     # data fields
     params: NewOrderParams
 
     def to_instruction(self):
         keys = []
@@ -68,14 +69,15 @@
         keys.append(self.trader_fee_state_acct)
         keys.append(self.fee_output_register)
         keys.append(self.risk_engine_program)
         keys.append(self.risk_model_configuration_acct)
         keys.append(self.risk_output_register)
         keys.append(self.trader_risk_state_acct)
         keys.append(self.risk_and_fee_signer)
+        keys.append(self.referrer_trg)
         if self.remaining_accounts is not None:
             keys.extend(self.remaining_accounts)
 
         buffer = BytesIO()
         buffer.write(InstructionTag.to_bytes(InstructionTag.NEW_ORDER))
         buffer.write(BYTES_CATALOG.pack(NewOrderParams, self.params))
 
@@ -105,14 +107,15 @@
     trader_fee_state_acct: Union[str, PublicKey, AccountMeta],
     fee_output_register: Union[str, PublicKey, AccountMeta],
     risk_engine_program: Union[str, PublicKey, AccountMeta],
     risk_model_configuration_acct: Union[str, PublicKey, AccountMeta],
     risk_output_register: Union[str, PublicKey, AccountMeta],
     trader_risk_state_acct: Union[str, PublicKey, AccountMeta],
     risk_and_fee_signer: Union[str, PublicKey, AccountMeta],
+    referrer_trg: Union[str, PublicKey, AccountMeta],
     params: NewOrderParams,
     system_program: Union[str, PublicKey, AccountMeta] = PublicKey("11111111111111111111111111111111"),
     remaining_accounts: Optional[List[AccountMeta]] = None,
     program_id: Optional[PublicKey] = None,
 ):
     if program_id is None:
         program_id = PublicKey("FUfpR31LmcP1VSbz5zDaM7nxnH55iBHkpwusgrnhaFjL")
@@ -189,15 +192,15 @@
             is_signer=False,
             is_writable=False,
         )
     if isinstance(fee_model_configuration_acct, (str, PublicKey)):
         fee_model_configuration_acct = to_account_meta(
             fee_model_configuration_acct,
             is_signer=False,
-            is_writable=False,
+            is_writable=True,
         )
     if isinstance(trader_fee_state_acct, (str, PublicKey)):
         trader_fee_state_acct = to_account_meta(
             trader_fee_state_acct,
             is_signer=False,
             is_writable=True,
         )
@@ -233,14 +236,20 @@
         )
     if isinstance(risk_and_fee_signer, (str, PublicKey)):
         risk_and_fee_signer = to_account_meta(
             risk_and_fee_signer,
             is_signer=False,
             is_writable=False,
         )
+    if isinstance(referrer_trg, (str, PublicKey)):
+        referrer_trg = to_account_meta(
+            referrer_trg,
+            is_signer=False,
+            is_writable=True,
+        )
 
     return NewOrderIx(
         program_id=program_id,
         user=user,
         trader_risk_group=trader_risk_group,
         market_product_group=market_product_group,
         product=product,
@@ -256,12 +265,13 @@
         trader_fee_state_acct=trader_fee_state_acct,
         fee_output_register=fee_output_register,
         risk_engine_program=risk_engine_program,
         risk_model_configuration_acct=risk_model_configuration_acct,
         risk_output_register=risk_output_register,
         trader_risk_state_acct=trader_risk_state_acct,
         risk_and_fee_signer=risk_and_fee_signer,
+        referrer_trg=referrer_trg,
         remaining_accounts=remaining_accounts,
         params=params,
     ).to_instruction()
 
 # LOCK-END
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/pop_events.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/pop_events.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/remove_market_product.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/remove_market_product.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/remove_market_product_group.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/remove_market_product_group.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/setup_capital_limits.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/setup_capital_limits.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/sign_print_trade.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/sign_print_trade.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/sweep_fees.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/sweep_fees.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/transfer_full_position.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/transfer_full_position.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_capital_limits.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_capital_limits.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_market_product_group.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/initialize_mark_prices.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # LOCK-BEGIN[imports]: DON'T MODIFY
 from .instruction_tag import InstructionTag
 from dataclasses import dataclass
-from dexteritysdk.codegen.dex.types import UpdateMarketProductGroupParams
+from dexteritysdk.codegen.risk_engine.types import InitializeMarkPricesParams
 from dexteritysdk.solmate.utils import to_account_meta
 from io import BytesIO
 from podite import BYTES_CATALOG
 from solana.publickey import PublicKey
 from solana.transaction import (
     AccountMeta,
     TransactionInstruction,
@@ -15,103 +15,103 @@
     Optional,
     Union,
 )
 
 # LOCK-END
 
 
-# LOCK-BEGIN[ix_cls(update_market_product_group)]: DON'T MODIFY
+# LOCK-BEGIN[ix_cls(initialize_mark_prices)]: DON'T MODIFY
 @dataclass
-class UpdateMarketProductGroupIx:
+class InitializeMarkPricesIx:
     program_id: PublicKey
 
     # account metas
+    payer: AccountMeta
     authority: AccountMeta
+    mark_prices: AccountMeta
     market_product_group: AccountMeta
-    fee_collector: AccountMeta
-    staking_fee_collector: AccountMeta
     system_program: AccountMeta
     remaining_accounts: Optional[List[AccountMeta]]
 
     # data fields
-    params: UpdateMarketProductGroupParams
+    params: InitializeMarkPricesParams
 
     def to_instruction(self):
         keys = []
+        keys.append(self.payer)
         keys.append(self.authority)
+        keys.append(self.mark_prices)
         keys.append(self.market_product_group)
-        keys.append(self.fee_collector)
-        keys.append(self.staking_fee_collector)
         keys.append(self.system_program)
         if self.remaining_accounts is not None:
             keys.extend(self.remaining_accounts)
 
         buffer = BytesIO()
-        buffer.write(InstructionTag.to_bytes(InstructionTag.UPDATE_MARKET_PRODUCT_GROUP))
-        buffer.write(BYTES_CATALOG.pack(UpdateMarketProductGroupParams, self.params))
+        buffer.write(InstructionTag.to_bytes(InstructionTag.INITIALIZE_MARK_PRICES))
+        buffer.write(BYTES_CATALOG.pack(InitializeMarkPricesParams, self.params))
 
         return TransactionInstruction(
             keys=keys,
             program_id=self.program_id,
             data=buffer.getvalue(),
         )
 
 # LOCK-END
 
 
-# LOCK-BEGIN[ix_fn(update_market_product_group)]: DON'T MODIFY
-def update_market_product_group(
+# LOCK-BEGIN[ix_fn(initialize_mark_prices)]: DON'T MODIFY
+def initialize_mark_prices(
+    payer: Union[str, PublicKey, AccountMeta],
     authority: Union[str, PublicKey, AccountMeta],
+    mark_prices: Union[str, PublicKey, AccountMeta],
     market_product_group: Union[str, PublicKey, AccountMeta],
-    fee_collector: Union[str, PublicKey, AccountMeta],
-    staking_fee_collector: Union[str, PublicKey, AccountMeta],
-    params: UpdateMarketProductGroupParams,
+    params: InitializeMarkPricesParams,
     system_program: Union[str, PublicKey, AccountMeta] = PublicKey("11111111111111111111111111111111"),
     remaining_accounts: Optional[List[AccountMeta]] = None,
     program_id: Optional[PublicKey] = None,
 ):
     if program_id is None:
-        program_id = PublicKey("FUfpR31LmcP1VSbz5zDaM7nxnH55iBHkpwusgrnhaFjL")
+        program_id = PublicKey("92wdgEqyiDKrcbFHoBTg8HxMj932xweRCKaciGSW3uMr")
 
+    if isinstance(payer, (str, PublicKey)):
+        payer = to_account_meta(
+            payer,
+            is_signer=True,
+            is_writable=True,
+        )
     if isinstance(authority, (str, PublicKey)):
         authority = to_account_meta(
             authority,
             is_signer=True,
+            is_writable=False,
+        )
+    if isinstance(mark_prices, (str, PublicKey)):
+        mark_prices = to_account_meta(
+            mark_prices,
+            is_signer=False,
             is_writable=True,
         )
     if isinstance(market_product_group, (str, PublicKey)):
         market_product_group = to_account_meta(
             market_product_group,
             is_signer=False,
-            is_writable=True,
-        )
-    if isinstance(fee_collector, (str, PublicKey)):
-        fee_collector = to_account_meta(
-            fee_collector,
-            is_signer=False,
-            is_writable=False,
-        )
-    if isinstance(staking_fee_collector, (str, PublicKey)):
-        staking_fee_collector = to_account_meta(
-            staking_fee_collector,
-            is_signer=False,
             is_writable=False,
         )
     if isinstance(system_program, (str, PublicKey)):
         system_program = to_account_meta(
             system_program,
             is_signer=False,
             is_writable=False,
         )
 
-    return UpdateMarketProductGroupIx(
+    return InitializeMarkPricesIx(
         program_id=program_id,
+        payer=payer,
         authority=authority,
+        mark_prices=mark_prices,
         market_product_group=market_product_group,
-        fee_collector=fee_collector,
-        staking_fee_collector=staking_fee_collector,
         system_program=system_program,
         remaining_accounts=remaining_accounts,
         params=params,
     ).to_instruction()
 
 # LOCK-END
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_product_funding.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_product_funding.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_trader_funding.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_trader_funding.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_trader_risk_group_owner.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_trader_risk_group_owner.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/update_variance_cache.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_variance_cache.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/instructions/withdraw_funds.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/withdraw_funds.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/__init__.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,21 @@
 from .price_ewma import PriceEwma
 from .print_trade import PrintTrade
 from .product import Product
 from .product_array import ProductArray
 from .product_metadata import ProductMetadata
 from .product_status import ProductStatus
 from .risk_output_register import RiskOutputRegister
+from .set_num_risk_state_accounts_params import SetNumRiskStateAccountsParams
 from .sign_print_trade_params import SignPrintTradeParams
 from .social_loss import SocialLoss
 from .trader_fee_params import TraderFeeParams
 from .trader_fees import TraderFees
 from .trader_position import TraderPosition
 from .trader_risk_group import TraderRiskGroup
 from .update_market_product_group_params import UpdateMarketProductGroupParams
 from .update_product_funding_params import UpdateProductFundingParams
+from .update_product_mark_price_config_params import UpdateProductMarkPriceConfigParams
 from .util_error import UtilError
 from .withdraw_funds_params import WithdrawFundsParams
 
 # LOCK-END
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/account_tag.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/account_tag.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/action_status.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/action_status.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/capital_limits.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/capital_limits.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/capital_limits_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/capital_limits_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/combo.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/combo.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/dex_error.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/dex_error.py`

 * *Files 17% similar despite different names*

```diff
@@ -65,17 +65,24 @@
     NEGATIVE_WITHDRAW_LIMIT = None
     DEPOSIT_DENIED_INSUFFICIENT_BALANCE_ON_WHITELIST_ATA_TOKEN = None
     DEPOSIT_DECLINED_UNFROZEN_WHITELIST_ATA_TOKEN = None
     DEPOSIT_DECLINED_NON_EXISTENT_WHITELIST_ATA_TOKEN_ON_TRADER_RISK_GROUP = None
     INVALID_PRODUCT_STATUS_IN_UPDATE_FUNDING = None
     CONTRACT_IS_NOT_EXPIRING = None
     CONTRACT_HAS_NON_ZERO_OPEN_INTEREST = None
+    CONTRACT_HAS_NON_ZERO_OPEN_INTEREST_OR_RISK_STATE_ACCOUNTS = None
     CONTRACT_IS_ACTIVE = None
     FAILED_TO_GET_ORDER_QUANTITY = None
     SELF_TRADE_BEHAVIOR_DECREMENT_TAKE_IS_DISALLOWED = None
+    PRICE_BAND_VIOLATION = None
+    UNEXPECTED_IMBALANCED_OPEN_INTEREST = None
+    MAXIMUM_OPEN_INTEREST_EXCEEDED = None
+    MARKET_PRODUCT_GROUP_KILLSWITCH_IS_ON = None
+    INVALID_FUTURE_EXPIRY = None
+    MAX_REFERRER_FEE_BPS_EXCEEDED = None
     # LOCK-END
 
     @classmethod
     def _to_bytes_partial(cls, buffer, obj, **kwargs):
         # to modify packing, change this method
         return super()._to_bytes_partial(buffer, obj, **kwargs)
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/fractional.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/fractional.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     def simplify(self):
         m = self.m
         exp = self.exp
 
         if m == 0:
             return Fractional(0, 0)
 
-        while m % 10 == 0:
+        while m % 10 == 0 and exp > 0:
             m //= 10
             exp -= 1
         return Fractional(m, exp)
 
     def __repr__(self):
         if self.m == MAX_FRACTIONAL_M and self.exp == MAX_FRACTIONAL_EXP:
             return "Inf"
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/health_info.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/health_info.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/health_result.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/health_result.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/health_status.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/health_status.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/initialize_combo_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/initialize_combo_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/initialize_market_product_group_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/initialize_market_product_group_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/initialize_market_product_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/initialize_market_product_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/initialize_print_trade_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/initialize_print_trade_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/leg.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/leg.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/liquidation_info.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/liquidation_info.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/market_product_group.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/market_product_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     min_maker_fee_bps: I16
     max_taker_fee_bps: I16
     min_taker_fee_bps: I16
     fee_output_register: PublicKey
     risk_output_register: PublicKey
     sequence_number: U128
     staking_fee_collector: PublicKey
+    is_killed: bool
     # LOCK-END
 
     @classmethod
     def to_bytes(cls, obj, **kwargs):
         return cls.pack(obj, converter="bytes", **kwargs)
 
     @classmethod
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/new_order_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/new_order_params.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 class NewOrderParams:
     side: Side
     max_base_qty: Fractional
     order_type: "OrderType"
     self_trade_behavior: SelfTradeBehavior
     match_limit: U64
     limit_price: Fractional
+    referrer_fee_bps: Fractional
     # LOCK-END
 
     @classmethod
     def to_bytes(cls, obj, **kwargs):
         return cls.pack(obj, converter="bytes", **kwargs)
 
     @classmethod
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/open_orders.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/open_orders.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/open_orders_metadata.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/open_orders_metadata.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/open_orders_node.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/open_orders_node.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/operation_type.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/operation_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 @pod
 class OperationType(Enum[AutoTagType]):
     NEW_ORDER = None
     CANCEL_ORDER = None
     CHECK_HEALTH = None
     POSITION_TRANSFER = None
     CONSUME_EVENTS = None
+    CHECK_WITHDRAWAL_HEALTH = None
     # LOCK-END
 
     @classmethod
     def _to_bytes_partial(cls, buffer, obj, **kwargs):
         # to modify packing, change this method
         return super()._to_bytes_partial(buffer, obj, **kwargs)
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/order_info.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/order_info.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/order_type.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/order_type.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/outright.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/outright.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 # LOCK-END
 
 
 # LOCK-BEGIN[class(Outright)]: DON'T MODIFY
 @pod
 class Outright:
     metadata: "ProductMetadata"
-    num_queue_events: Usize
+    num_risk_state_accounts: Usize
     product_status: "ProductStatus"
     dust: "Fractional"
     cum_funding_per_share: "Fractional"
     cum_social_loss_per_share: "Fractional"
     open_long_interest: "Fractional"
     open_short_interest: "Fractional"
-    padding: FixedLenArray[U64, 14]
+    mark_price_qualifying_cum_value: "Fractional"
+    mark_price_max_qualifying_width: "Fractional"
+    padding: FixedLenArray[U64, 10]
     # LOCK-END
 
     def is_expired(self) -> bool:
         return self.product_status == ProductStatus.EXPIRED
 
     def is_active(self) -> bool:
         return self.product_status != ProductStatus.UNINITIALIZED
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/price_ewma.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/price_ewma.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/print_trade.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/print_trade.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/product.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/product.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/product_array.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/product_array.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/product_metadata.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/product_metadata.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/product_status.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/product_status.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/risk_output_register.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/risk_output_register.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/sign_print_trade_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/sign_print_trade_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/social_loss.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/social_loss.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/trader_fee_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/trader_fee_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/trader_fees.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/trader_fees.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/trader_position.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/trader_position.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/trader_risk_group.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/trader_risk_group.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/update_product_funding_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/update_product_funding_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/dex/types/util_error.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/types/util_error.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/accounts.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/accounts.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/close_derivative_account.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/close_derivative_account.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/initialize_derivative.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/initialize_derivative.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/initialize_fixed_income.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/initialize_fixed_income.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/settle_derivative.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/settle_derivative.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/instructions/settle_fixed_income.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/instructions/settle_fixed_income.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/account_tag.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/account_tag.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/derivative_error.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/derivative_error.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/derivative_metadata.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/derivative_metadata.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/expiration_status.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/expiration_status.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/fixed_income_metadata.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/fixed_income_metadata.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/initialize_derivative_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/initialize_derivative_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/initialize_fixed_income_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/initialize_fixed_income_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/instrument_type.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/instrument_type.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/instruments/types/oracle_type.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/instruments/types/oracle_type.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/instructions/create_risk_state_account.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/instructions/create_risk_state_account.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/instructions/validate_account_health.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/instructions/validate_account_health.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/noop_risk_engine/instructions/validate_account_liquidation.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/noop_risk_engine/instructions/validate_account_liquidation.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/accounts.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/accounts.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/__init__.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,22 @@
     initialize_covariance_matrix,
 )
 from .initialize_mark_prices import (
     InitializeMarkPricesIx,
     initialize_mark_prices,
 )
 from .instruction_tag import InstructionTag
+from .remove_market_product_index_from_variance_cache import (
+    RemoveMarketProductIndexFromVarianceCacheIx,
+    remove_market_product_index_from_variance_cache,
+)
+from .resize_variance_cache import (
+    ResizeVarianceCacheIx,
+    resize_variance_cache,
+)
 from .update_mark_prices import (
     UpdateMarkPricesIx,
     update_mark_prices,
 )
 from .validate_account_health import (
     ValidateAccountHealthIx,
     validate_account_health,
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/close_mark_prices.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/close_mark_prices.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/create_risk_state_account.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/create_risk_state_account.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/initialize_covariance_matrix.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/initialize_covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/initialize_mark_prices.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/dex/instructions/update_market_product_group.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # LOCK-BEGIN[imports]: DON'T MODIFY
 from .instruction_tag import InstructionTag
 from dataclasses import dataclass
-from dexteritysdk.codegen.risk_engine.types import InitializeMarkPricesParams
+from dexteritysdk.codegen.dex.types import UpdateMarketProductGroupParams
 from dexteritysdk.solmate.utils import to_account_meta
 from io import BytesIO
 from podite import BYTES_CATALOG
 from solana.publickey import PublicKey
 from solana.transaction import (
     AccountMeta,
     TransactionInstruction,
@@ -15,103 +15,83 @@
     Optional,
     Union,
 )
 
 # LOCK-END
 
 
-# LOCK-BEGIN[ix_cls(initialize_mark_prices)]: DON'T MODIFY
+# LOCK-BEGIN[ix_cls(update_market_product_group)]: DON'T MODIFY
 @dataclass
-class InitializeMarkPricesIx:
+class UpdateMarketProductGroupIx:
     program_id: PublicKey
 
     # account metas
-    payer: AccountMeta
     authority: AccountMeta
-    mark_prices: AccountMeta
     market_product_group: AccountMeta
     system_program: AccountMeta
     remaining_accounts: Optional[List[AccountMeta]]
 
     # data fields
-    params: InitializeMarkPricesParams
+    params: UpdateMarketProductGroupParams
 
     def to_instruction(self):
         keys = []
-        keys.append(self.payer)
         keys.append(self.authority)
-        keys.append(self.mark_prices)
         keys.append(self.market_product_group)
         keys.append(self.system_program)
         if self.remaining_accounts is not None:
             keys.extend(self.remaining_accounts)
 
         buffer = BytesIO()
-        buffer.write(InstructionTag.to_bytes(InstructionTag.INITIALIZE_MARK_PRICES))
-        buffer.write(BYTES_CATALOG.pack(InitializeMarkPricesParams, self.params))
+        buffer.write(InstructionTag.to_bytes(InstructionTag.UPDATE_MARKET_PRODUCT_GROUP))
+        buffer.write(BYTES_CATALOG.pack(UpdateMarketProductGroupParams, self.params))
 
         return TransactionInstruction(
             keys=keys,
             program_id=self.program_id,
             data=buffer.getvalue(),
         )
 
 # LOCK-END
 
 
-# LOCK-BEGIN[ix_fn(initialize_mark_prices)]: DON'T MODIFY
-def initialize_mark_prices(
-    payer: Union[str, PublicKey, AccountMeta],
+# LOCK-BEGIN[ix_fn(update_market_product_group)]: DON'T MODIFY
+def update_market_product_group(
     authority: Union[str, PublicKey, AccountMeta],
-    mark_prices: Union[str, PublicKey, AccountMeta],
     market_product_group: Union[str, PublicKey, AccountMeta],
-    params: InitializeMarkPricesParams,
+    params: UpdateMarketProductGroupParams,
     system_program: Union[str, PublicKey, AccountMeta] = PublicKey("11111111111111111111111111111111"),
     remaining_accounts: Optional[List[AccountMeta]] = None,
     program_id: Optional[PublicKey] = None,
 ):
     if program_id is None:
-        program_id = PublicKey("92wdgEqyiDKrcbFHoBTg8HxMj932xweRCKaciGSW3uMr")
+        program_id = PublicKey("FUfpR31LmcP1VSbz5zDaM7nxnH55iBHkpwusgrnhaFjL")
 
-    if isinstance(payer, (str, PublicKey)):
-        payer = to_account_meta(
-            payer,
-            is_signer=True,
-            is_writable=True,
-        )
     if isinstance(authority, (str, PublicKey)):
         authority = to_account_meta(
             authority,
             is_signer=True,
-            is_writable=False,
-        )
-    if isinstance(mark_prices, (str, PublicKey)):
-        mark_prices = to_account_meta(
-            mark_prices,
-            is_signer=False,
             is_writable=True,
         )
     if isinstance(market_product_group, (str, PublicKey)):
         market_product_group = to_account_meta(
             market_product_group,
             is_signer=False,
-            is_writable=False,
+            is_writable=True,
         )
     if isinstance(system_program, (str, PublicKey)):
         system_program = to_account_meta(
             system_program,
             is_signer=False,
             is_writable=False,
         )
 
-    return InitializeMarkPricesIx(
+    return UpdateMarketProductGroupIx(
         program_id=program_id,
-        payer=payer,
         authority=authority,
-        mark_prices=mark_prices,
         market_product_group=market_product_group,
         system_program=system_program,
         remaining_accounts=remaining_accounts,
         params=params,
     ).to_instruction()
 
 # LOCK-END
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/instruction_tag.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/instruction_tag.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 
 # LOCK-END
 
 
 # LOCK-BEGIN[instruction_tag]: DON'T MODIFY
 @pod
 class InstructionTag(Enum[U64]):
+    RESIZE_VARIANCE_CACHE = InstructionDiscriminant()
     VALIDATE_ACCOUNT_HEALTH = InstructionDiscriminant()
     VALIDATE_ACCOUNT_LIQUIDATION = InstructionDiscriminant()
     CREATE_RISK_STATE_ACCOUNT = InstructionDiscriminant()
     INITIALIZE_COVARIANCE_MATRIX = InstructionDiscriminant()
     INITIALIZE_MARK_PRICES = InstructionDiscriminant()
     CLOSE_MARK_PRICES = InstructionDiscriminant()
     UPDATE_MARK_PRICES = InstructionDiscriminant()
+    REMOVE_MARKET_PRODUCT_INDEX_FROM_VARIANCE_CACHE = InstructionDiscriminant()
     # LOCK-END
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/update_mark_prices.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/update_mark_prices.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/validate_account_health.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/validate_account_liquidation.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     Optional,
     Union,
 )
 
 # LOCK-END
 
 
-# LOCK-BEGIN[ix_cls(validate_account_health)]: DON'T MODIFY
+# LOCK-BEGIN[ix_cls(validate_account_liquidation)]: DON'T MODIFY
 @dataclass
-class ValidateAccountHealthIx:
+class ValidateAccountLiquidationIx:
     program_id: PublicKey
 
     # account metas
     market_product_group: AccountMeta
     trader_risk_group: AccountMeta
     risk_output_register: AccountMeta
     variance_cache: AccountMeta
@@ -46,27 +46,27 @@
         keys.append(self.covariance_metadata)
         keys.append(self.correlation_matrix)
         keys.append(self.mark_prices)
         if self.remaining_accounts is not None:
             keys.extend(self.remaining_accounts)
 
         buffer = BytesIO()
-        buffer.write(InstructionTag.to_bytes(InstructionTag.VALIDATE_ACCOUNT_HEALTH))
+        buffer.write(InstructionTag.to_bytes(InstructionTag.VALIDATE_ACCOUNT_LIQUIDATION))
 
         return TransactionInstruction(
             keys=keys,
             program_id=self.program_id,
             data=buffer.getvalue(),
         )
 
 # LOCK-END
 
 
-# LOCK-BEGIN[ix_fn(validate_account_health)]: DON'T MODIFY
-def validate_account_health(
+# LOCK-BEGIN[ix_fn(validate_account_liquidation)]: DON'T MODIFY
+def validate_account_liquidation(
     market_product_group: Union[str, PublicKey, AccountMeta],
     trader_risk_group: Union[str, PublicKey, AccountMeta],
     risk_output_register: Union[str, PublicKey, AccountMeta],
     variance_cache: Union[str, PublicKey, AccountMeta],
     risk_model_configuration: Union[str, PublicKey, AccountMeta],
     risk_signer: Union[str, PublicKey, AccountMeta],
     covariance_metadata: Union[str, PublicKey, AccountMeta],
@@ -129,15 +129,15 @@
     if isinstance(mark_prices, (str, PublicKey)):
         mark_prices = to_account_meta(
             mark_prices,
             is_signer=False,
             is_writable=True,
         )
 
-    return ValidateAccountHealthIx(
+    return ValidateAccountLiquidationIx(
         program_id=program_id,
         market_product_group=market_product_group,
         trader_risk_group=trader_risk_group,
         risk_output_register=risk_output_register,
         variance_cache=variance_cache,
         risk_model_configuration=risk_model_configuration,
         risk_signer=risk_signer,
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/instructions/validate_account_liquidation.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/instructions/validate_account_health.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # LOCK-BEGIN[imports]: DON'T MODIFY
 from .instruction_tag import InstructionTag
 from dataclasses import dataclass
+from dexteritysdk.codegen.dex.types.order_info import OrderInfo
 from dexteritysdk.solmate.utils import to_account_meta
 from io import BytesIO
 from podite import BYTES_CATALOG
 from solana.publickey import PublicKey
 from solana.transaction import (
     AccountMeta,
     TransactionInstruction,
@@ -14,31 +15,34 @@
     Optional,
     Union,
 )
 
 # LOCK-END
 
 
-# LOCK-BEGIN[ix_cls(validate_account_liquidation)]: DON'T MODIFY
+# LOCK-BEGIN[ix_cls(validate_account_health)]: DON'T MODIFY
 @dataclass
-class ValidateAccountLiquidationIx:
+class ValidateAccountHealthIx:
     program_id: PublicKey
 
     # account metas
     market_product_group: AccountMeta
     trader_risk_group: AccountMeta
     risk_output_register: AccountMeta
     variance_cache: AccountMeta
     risk_model_configuration: AccountMeta
     risk_signer: AccountMeta
     covariance_metadata: AccountMeta
     correlation_matrix: AccountMeta
     mark_prices: AccountMeta
     remaining_accounts: Optional[List[AccountMeta]]
 
+    # data fields
+    params: OrderInfo
+
     def to_instruction(self):
         keys = []
         keys.append(self.market_product_group)
         keys.append(self.trader_risk_group)
         keys.append(self.risk_output_register)
         keys.append(self.variance_cache)
         keys.append(self.risk_model_configuration)
@@ -46,36 +50,38 @@
         keys.append(self.covariance_metadata)
         keys.append(self.correlation_matrix)
         keys.append(self.mark_prices)
         if self.remaining_accounts is not None:
             keys.extend(self.remaining_accounts)
 
         buffer = BytesIO()
-        buffer.write(InstructionTag.to_bytes(InstructionTag.VALIDATE_ACCOUNT_LIQUIDATION))
+        buffer.write(InstructionTag.to_bytes(InstructionTag.VALIDATE_ACCOUNT_HEALTH))
+        buffer.write(BYTES_CATALOG.pack(OrderInfo, self.params))
 
         return TransactionInstruction(
             keys=keys,
             program_id=self.program_id,
             data=buffer.getvalue(),
         )
 
 # LOCK-END
 
 
-# LOCK-BEGIN[ix_fn(validate_account_liquidation)]: DON'T MODIFY
-def validate_account_liquidation(
+# LOCK-BEGIN[ix_fn(validate_account_health)]: DON'T MODIFY
+def validate_account_health(
     market_product_group: Union[str, PublicKey, AccountMeta],
     trader_risk_group: Union[str, PublicKey, AccountMeta],
     risk_output_register: Union[str, PublicKey, AccountMeta],
     variance_cache: Union[str, PublicKey, AccountMeta],
     risk_model_configuration: Union[str, PublicKey, AccountMeta],
     risk_signer: Union[str, PublicKey, AccountMeta],
     covariance_metadata: Union[str, PublicKey, AccountMeta],
     correlation_matrix: Union[str, PublicKey, AccountMeta],
     mark_prices: Union[str, PublicKey, AccountMeta],
+    params: OrderInfo,
     remaining_accounts: Optional[List[AccountMeta]] = None,
     program_id: Optional[PublicKey] = None,
 ):
     if program_id is None:
         program_id = PublicKey("92wdgEqyiDKrcbFHoBTg8HxMj932xweRCKaciGSW3uMr")
 
     if isinstance(market_product_group, (str, PublicKey)):
@@ -129,22 +135,23 @@
     if isinstance(mark_prices, (str, PublicKey)):
         mark_prices = to_account_meta(
             mark_prices,
             is_signer=False,
             is_writable=True,
         )
 
-    return ValidateAccountLiquidationIx(
+    return ValidateAccountHealthIx(
         program_id=program_id,
         market_product_group=market_product_group,
         trader_risk_group=trader_risk_group,
         risk_output_register=risk_output_register,
         variance_cache=variance_cache,
         risk_model_configuration=risk_model_configuration,
         risk_signer=risk_signer,
         covariance_metadata=covariance_metadata,
         correlation_matrix=correlation_matrix,
         mark_prices=mark_prices,
         remaining_accounts=remaining_accounts,
+        params=params,
     ).to_instruction()
 
 # LOCK-END
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/correlation_matrix.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/covariance_metadata.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/covariance_metadata.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/initialize_mark_prices_params.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/initialize_mark_prices_params.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/mark_prices_array.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/mark_prices_array.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 # LOCK-BEGIN[imports]: DON'T MODIFY
 from dexteritysdk.codegen.instruments.types.oracle_type import OracleType
 from dexteritysdk.codegen.risk_engine.types.mark_price import MarkPrice
 from podite import (
     FixedLenArray,
-    U64,
     U8,
     pod,
 )
 from solana.publickey import PublicKey
 
 # LOCK-END
 
 
 # LOCK-BEGIN[class(MarkPricesArray)]: DON'T MODIFY
 @pod
 class MarkPricesArray:
     bump: U8
-    padding0: FixedLenArray[U8, 7]
-    update_slot: U64
     is_hardcoded_oracle: bool
     hardcoded_oracle: PublicKey
-    padding1: FixedLenArray[U8, 7]
+    _padding0: FixedLenArray[U8, 6]
     hardcoded_oracle_type: OracleType
-    padding2: FixedLenArray[U8, 7]
+    _padding1: FixedLenArray[U8, 7]
     array: FixedLenArray[MarkPrice, 64]
     # LOCK-END
 
     @classmethod
     def to_bytes(cls, obj, **kwargs):
         return cls.pack(obj, converter="bytes", **kwargs)
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/risk_account_tag.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/risk_account_tag.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/risk_error.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/risk_error.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     COMBO_SIZE_GREATER_THAN_COLLECTION_LEN = None
     INVALID_MARK_PRICE_ACCOUNTS_LEN = None
     MISMATCHED_ORACLE_PRICE_ACCOUNT = None
     MISSING_MARK_PRICE = None
     INCORRECT_MARK_PRICES_BUMP = None
     MARK_PRICES_ARRAY_IS_FULL = None
     MARK_PRICES_OUT_OF_DATE = None
+    FAILED_TO_FIND_MARKET_PRODUCT_INDEX_IN_VARIANCE_CACHE = None
+    BOOK_SPREAD_TOO_WIDE_FOR_MARK_PRICE = None
     # LOCK-END
 
     @classmethod
     def _to_bytes_partial(cls, buffer, obj, **kwargs):
         # to modify packing, change this method
         return super()._to_bytes_partial(buffer, obj, **kwargs)
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/codegen/risk_engine/types/variance_cache.py` & `dexteritysdk-0.2.8/dexteritysdk/codegen/risk_engine/types/variance_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     update_slot: U64
     position_value: FastInt
     total_variance: FastInt
     open_order_variance: FastInt
     product_indexes: FixedLenArray[Usize, 32]
     positions: FixedLenArray[FastInt, 32]
     sigma_p: FixedLenArray[FastInt, 32]
+    total_liquidity_buffer: FastInt
     # LOCK-END
 
     @classmethod
     def to_bytes(cls, obj, **kwargs):
         return cls.pack(obj, converter="bytes", **kwargs)
 
     @classmethod
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/constant_fees/actions.py` & `dexteritysdk-0.2.8/dexteritysdk/constant_fees/actions.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/constant_fees/instructions.py` & `dexteritysdk-0.2.8/dexteritysdk/constant_fees/instructions.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/dex/actions.py` & `dexteritysdk-0.2.8/dexteritysdk/dex/actions.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/dex/addrs.py` & `dexteritysdk-0.2.8/dexteritysdk/dex/addrs.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/dex/sdk_context.py` & `dexteritysdk-0.2.8/dexteritysdk/dex/sdk_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import base58
 
 from collections import defaultdict
 from collections.abc import Iterable
 from dataclasses import dataclass
 from enum import Enum
-from typing import List, Union, Optional, Callable, Any
+from typing import Any, Callable, List, Optional, Tuple, Union
 
 from borsh_construct import CStruct, U32, U8
 from solana.rpc import commitment, types
 from solana.rpc.commitment import Confirmed
 from solana.rpc.websocket_api import connect as solana_ws_connect
 from solders.rpc.responses import AccountNotification, SubscriptionResult, SubscriptionError
 from spl.token import instructions as spl_token_instructions
@@ -58,14 +58,16 @@
 
 @dataclass
 class SDKFill:
     product: "SDKProduct"
     side: aaob_state.Side
     order_id: int
     qty: float
+    price: float
+    is_maker: bool
 
 
 @dataclass
 class SDKPosition:
     product: "SDKProduct"
     position: float
     pending_position: float
@@ -341,36 +343,44 @@
                                         if isinstance(e, FillEvent) and fills_callback:
                                             # if we were the maker
                                             if e.maker_callback.account == self.account:
                                                 # convert taker to maker side
                                                 maker_side = aaob_state.Side.BID \
                                                     if e.taker_side == Side.ASK else aaob_state.Side.ASK
                                                 fill_size = e.base_size / (10 ** product.metadata.base_decimals)
+                                                quote_size = e.quote_size / (10 ** product.metadata.base_decimals)
+                                                fill_price = quote_size / fill_size if fill_size != 0.0 else float('NaN')
                                                 if fills_callback:
                                                     fills_callback(
                                                         SDKFill(
                                                             product,
                                                             maker_side,
                                                             e.maker_order_id,
-                                                            fill_size
+                                                            fill_size,
+                                                            fill_price,
+                                                            is_maker=True
                                                         ),
                                                         SDKEventType.NEW
                                                     )
                                             # else if we were the taker
                                             elif e.taker_callback.account == self.account:
                                                 taker_side = aaob_state.Side.ASK \
                                                     if e.taker_side == Side.ASK else aaob_state.Side.BID
-                                                size = e.base_size / (10 ** product.metadata.base_decimals)
+                                                fill_size = e.base_size / (10 ** product.metadata.base_decimals)
+                                                quote_size = e.quote_size / (10 ** product.metadata.base_decimals)
+                                                fill_price = quote_size / fill_size if fill_size != 0.0 else float('NaN')
                                                 if fills_callback:
                                                     fills_callback(
                                                         SDKFill(
                                                             product,
                                                             taker_side,
                                                             None,
-                                                            size
+                                                            fill_size,
+                                                            fill_price,
+                                                            is_maker=False
                                                         ),
                                                         SDKEventType.NEW
                                                     )
                                         elif isinstance(e, OutEvent) and orders_callback:
                                             if e.callback.account == self.account:
                                                 handled_orders.add(e.order_id)
                                                 event_type = SDKEventType.FILLED if e.base_size == 0 \
@@ -455,55 +465,56 @@
     @staticmethod
     def connect(
             sdk: "SDKContext",
             account: PublicKey,
             keypair: Keypair,
     ) -> "SDKTrader":
         wallet = spl_token_instructions.get_associated_token_address(keypair.public_key, sdk.vault_mint)
-        trader_fee_state_acct = daddrs.get_trader_fee_state_acct(account, sdk.market_product_group,
-                                                                 sdk.fee_model_program)
         trg: dtys.TraderRiskGroup = explore(account).data_obj
         assert trg.market_product_group == sdk.market_product_group
-        assert trg.fee_state_account == trader_fee_state_acct
         assert trg.owner == keypair.public_key
 
         whitelist_token_wallet = spl_token_instructions.get_associated_token_address(
             keypair.public_key,
             mints.WHITELIST_TOKEN_MINT
         )
 
         return SDKTrader(
-            keypair, account, wallet, trader_fee_state_acct, trg.risk_state_account, whitelist_token_wallet,
+            keypair, account, wallet, trg.fee_state_account, trg.risk_state_account, whitelist_token_wallet,
             _batches_lock=threading.Lock(), _batch_id=0, _pending_batches={})
 
-    def get_trader_risk_group(self) -> (dtys.TraderRiskGroup, int):
+    def get_trader_risk_group(self) -> Tuple[dtys.TraderRiskGroup, int]:
         account_details = fetch_account_details(self.account)
         return account_details.data_obj, account_details.slot
 
     def deposit(self, sdk: "SDKContext", qty: Union[float, dtys.Fractional]):
         if not isinstance(qty, dtys.Fractional):
             qty = dtys.Fractional(int(qty * (10 ** sdk.decimals)), sdk.decimals)
         ix = dixs.deposit_funds(
             user=self.keypair.public_key,
             user_token_account=self.wallet,
             trader_risk_group=self.account,
             market_product_group=sdk.market_product_group,
             market_product_group_vault=sdk.market_product_group_vault,
             capital_limits=sdk.capital_limits,
-            whitelist_ata_acct=self.whitelist_token_wallet,
             params=dtys.DepositFundsParams(
                 quantity=qty,
             ),
             program_id=sdk.dex_program,
         )
         return sdk.send_instructions(ix)
 
     def withdraw(self, sdk: "SDKContext", qty: Union[float, dtys.Fractional]):
         if not isinstance(qty, dtys.Fractional):
             qty = dtys.Fractional(int(qty * sdk.decimals), sdk.decimals)
+
+        remaining_accounts = [
+            to_account_meta(ra, is_signer=False, is_writable=True) for ra in sdk.additional_risk_accts
+        ]
+
         update_mark_prices_ix = self._update_mark_prices_ix(sdk)
         ix = dixs.withdraw_funds(
             user=self.keypair.public_key,
             user_token_account=self.wallet,
             trader_risk_group=self.account,
             market_product_group=sdk.market_product_group,
             market_product_group_vault=sdk.market_product_group_vault,
@@ -513,14 +524,15 @@
             risk_signer=sdk.risk_signer,
             capital_limits=sdk.capital_limits,
             trader_risk_state_acct=self.trader_risk_state_acct,
             params=dtys.WithdrawFundsParams(
                 quantity=qty,
             ),
             program_id=sdk.dex_program,
+            remaining_accounts=remaining_accounts,
         )
         return sdk.send_instructions(update_mark_prices_ix, ix)
 
     def init_batch(self):
         self._batches_lock.acquire()
         batch_id = self._batch_id
         self._batch_id += 1
@@ -611,17 +623,22 @@
             product: Union[SDKProduct, PublicKey],
             side: aaob_state.Side,
             size: Union[dtys.Fractional, float],
             price: Union[dtys.Fractional, float],
             self_trade_behavior: aaob_state.SelfTradeBehavior = aaob_state.SelfTradeBehavior.CANCEL_PROVIDE,
             order_type: dtys.OrderType = dtys.OrderType.LIMIT,
             risk_accounts: Optional[List[PublicKey]] = None,
+            referrer_trg: Optional[PublicKey] = None,
+            referrer_fee_bps: dtys.Fractional = dtys.Fractional(0, 0),
     ):
         remaining_accounts = [to_account_meta(ra, is_signer=False, is_writable=True) for ra in risk_accounts]
 
+        if referrer_trg is None:
+            referrer_trg = self.account
+
         ix = dixs.new_order(
             program_id=sdk.dex_program,
             user=self.keypair.public_key,
             trader_risk_group=self.account,
             market_product_group=sdk.market_product_group,
             product=product.key,
             aaob_program=sdk.aaob_program,
@@ -635,21 +652,23 @@
             trader_fee_state_acct=self.trader_fee_state_acct,
             fee_output_register=sdk.fee_output_register,
             risk_engine_program=sdk.risk_engine_program,
             risk_model_configuration_acct=sdk.risk_model_configuration_acct,
             risk_output_register=sdk.risk_output_register,
             trader_risk_state_acct=self.trader_risk_state_acct,
             risk_and_fee_signer=sdk.risk_signer,
+            referrer_trg=referrer_trg,
             params=dtys.NewOrderParams(
                 side=side,
                 max_base_qty=dtys.Fractional.into(size, product.metadata.base_decimals),
                 order_type=order_type,
                 self_trade_behavior=self_trade_behavior,
                 match_limit=10,
-                limit_price=dtys.Fractional.into(price, product.metadata.base_decimals),
+                limit_price=dtys.Fractional.into(price, 8).simplify(),
+                referrer_fee_bps=referrer_fee_bps,
             ),
             remaining_accounts=remaining_accounts,
         )
 
         return ix
 
     def cancel(
@@ -743,22 +762,25 @@
             risk_signer=sdk.risk_signer,
             params=CancelOrderParams(order_id=order_id, no_err=no_err),
             remaining_accounts=None,
             program_id=sdk.dex_program,
         )
 
         # workaround to correctly serialize no_err
+        ix_data = bytearray(ix.data)
+        if len(ix_data) < 25:
+            ix_data.append(0)
         if no_err:
-            return TransactionInstruction(
-                keys=ix.keys,
-                program_id=ix.program_id,
-                data=ix.data[:-1] + b'\x01',
-            )
+            ix_data = ix_data[:-1] + b'\x01'
 
-        return ix
+        return TransactionInstruction(
+            keys=ix.keys,
+            program_id=ix.program_id,
+            data=bytes(ix_data),
+        )
 
     def replace(
             self,
             sdk: "SDKContext",
             product: Union[SDKProduct, PublicKey],
             order_id: int,
             side: aaob_state.Side,
@@ -1032,28 +1054,33 @@
         if mark_prices.is_hardcoded_oracle:
             mark_price_accounts.append(mark_prices.hardcoded_oracle)
 
         for idx, prod in mpg.active_products():
             if mpg.is_expired(prod):
                 continue
             metadata = prod.metadata()
-            orderbook: aaob_state.MarketState = fetch_account_details(metadata.orderbook).data_obj
-            products.append(
-                SDKProduct(
-                    metadata.product_key,
-                    idx,
-                    bytes(metadata.name).decode('utf-8').strip(),
-                    orderbook=metadata.orderbook,
-                    asks=orderbook.asks,
-                    bids=orderbook.bids,
-                    event_queue=orderbook.event_queue,
-                    market_signer=daddrs.get_market_signer(metadata.product_key),
-                    metadata=metadata,
+            product_name = bytes(metadata.name).decode('utf-8').strip()
+            try:
+                orderbook: aaob_state.MarketState = fetch_account_details(metadata.orderbook).data_obj
+                products.append(
+                    SDKProduct(
+                        metadata.product_key,
+                        idx,
+                        product_name,
+                        orderbook=metadata.orderbook,
+                        asks=orderbook.asks,
+                        bids=orderbook.bids,
+                        event_queue=orderbook.event_queue,
+                        market_signer=daddrs.get_market_signer(metadata.product_key),
+                        metadata=metadata,
+                    )
                 )
-            )
+            except:
+                print(f"WARNING: Ignoring invalid product {product_name}")
+                continue
 
             if not mark_prices.is_hardcoded_oracle and prod.is_outright():
                 derivative_metadata: DerivativeMetadata = fetch_account_details(metadata.product_key).data_obj
                 mark_price_accounts.append(metadata.product_key)
                 price_oracle_accounts.append(derivative_metadata.price_oracle)
 
         self.products = products
```

### Comparing `dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/actions.py` & `dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/actions.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/initialize_clock.py` & `dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/initialize_clock.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/initialize_oracle.py` & `dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/initialize_oracle.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/update_clock.py` & `dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/update_clock.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/dummy_oracle/instructions/update_price.py` & `dexteritysdk-0.2.8/dexteritysdk/dummy_oracle/instructions/update_price.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/instruments/actions.py` & `dexteritysdk-0.2.8/dexteritysdk/instruments/actions.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/instruments/instructions/initialize_derivative.py` & `dexteritysdk-0.2.8/dexteritysdk/instruments/instructions/initialize_derivative.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/instruments/instructions/initialize_fixed_income.py` & `dexteritysdk-0.2.8/dexteritysdk/instruments/instructions/initialize_fixed_income.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/program_ids.py` & `dexteritysdk-0.2.8/dexteritysdk/program_ids.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/pyserum/event_queue.py` & `dexteritysdk-0.2.8/dexteritysdk/pyserum/event_queue.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/pyserum/layouts/event_queue.py` & `dexteritysdk-0.2.8/dexteritysdk/pyserum/layouts/event_queue.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/pyserum/layouts/slab.py` & `dexteritysdk-0.2.8/dexteritysdk/pyserum/layouts/slab.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/pyserum/orderbook.py` & `dexteritysdk-0.2.8/dexteritysdk/pyserum/orderbook.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/pyserum/structs/event_queue.py` & `dexteritysdk-0.2.8/dexteritysdk/pyserum/structs/event_queue.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/pyserum/structs/slab.py` & `dexteritysdk-0.2.8/dexteritysdk/pyserum/structs/slab.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/risk/actions.py` & `dexteritysdk-0.2.8/dexteritysdk/risk/actions.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/scripts/build` & `dexteritysdk-0.2.8/dexteritysdk/scripts/build`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/scripts/discriminant.py` & `dexteritysdk-0.2.8/dexteritysdk/scripts/discriminant.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/scripts/extract_program_ids.py` & `dexteritysdk-0.2.8/dexteritysdk/scripts/extract_program_ids.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/scripts/generate_code.py` & `dexteritysdk-0.2.8/dexteritysdk/scripts/generate_code.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/scripts/get_trader_risk_groups_key.py` & `dexteritysdk-0.2.8/dexteritysdk/scripts/get_trader_risk_groups_key.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/solmate/__init__.py` & `dexteritysdk-0.2.8/dexteritysdk/solmate/__init__.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/codegen.py` & `dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/codegen.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/editor.py` & `dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/editor.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/solmate/anchor/idl.py` & `dexteritysdk-0.2.8/dexteritysdk/solmate/anchor/idl.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/solmate/cli.py` & `dexteritysdk-0.2.8/dexteritysdk/solmate/cli.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/solmate/dtypes.py` & `dexteritysdk-0.2.8/dexteritysdk/solmate/dtypes.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/solmate/utils.py` & `dexteritysdk-0.2.8/dexteritysdk/solmate/utils.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/utils/aob/instructions.py` & `dexteritysdk-0.2.8/dexteritysdk/utils/aob/instructions.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/__init__.py` & `dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/__init__.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/base.py` & `dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/base.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/event_queue.py` & `dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/event_queue.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/utils/aob/state/slab.py` & `dexteritysdk-0.2.8/dexteritysdk/utils/aob/state/slab.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/utils/binance_parser.py` & `dexteritysdk-0.2.8/dexteritysdk/utils/binance_parser.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/dexteritysdk/utils/solana.py` & `dexteritysdk-0.2.8/dexteritysdk/utils/solana.py`

 * *Files identical despite different names*

### Comparing `dexteritysdk-0.2.3/pyproject.toml` & `dexteritysdk-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dexteritysdk"
-version = "0.2.3"
+version = "0.2.8"
 description = "Client for Dexterity - a modular derivatives decentralized exchange reference implementation"
 authors = ["Joe Howarth <josephehowarth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 generate-code = "dexteritysdk.scripts.generate_code:main"
 local-validator = "dexteritysdk.scripts.start_test_validator:main"
```

### Comparing `dexteritysdk-0.2.3/setup.py` & `dexteritysdk-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,17 +157,17 @@
                      'keypair-to-b58 = '
                      'dexteritysdk.scripts.keypair_to_b58:main',
                      'local-validator = '
                      'dexteritysdk.scripts.start_test_validator:main']}
 
 setup_kwargs = {
     'name': 'dexteritysdk',
-    'version': '0.2.3',
+    'version': '0.2.8',
     'description': 'Client for Dexterity - a modular derivatives decentralized exchange reference implementation',
-    'long_description': '# Dexterity client SDK\n**Dexterity** is a derivatives decentralized exchange running on Solana.\nThis package provides the basic blocks in order to integrate and trade on Dexterity.\n\nYou can learn more about Dexterity [here](https://docs.hxro.network/market-protocols/derivatives-protocol/dexterity).\n\n## Prerequisites\n* [Solana.py](https://pypi.org/project/solana/)\n\n## Creating the client\nFirst, an instance of a Solana client is required.\n```python\nfrom dexteritysdk.dex.sdk_context import SDKContext, SDKTrader\nfrom solana.rpc.api import Client\nfrom solana.keypair import Keypair\nfrom solana.publickey import PublicKey\n\ndef main():\n\t# use "https://api.mainnet-beta.solana.com" for mainnet\n\tnetwork = "https://api.devnet.solana.com"\n\tclient = Client(network)\n```\n\nA Keypair for the payer has to also be provided.\n```python\nkeypair = Keypair.from_secret_key(keypair_bytes)\n```\nThe SDK also requires the **Market Product Group (MPG)** that we\'re going to trade on.\n\nThe public key of the default MPG is **`HiCy6vzuN3yLXD3z35D6nV7bzNLcyrvGLf3uSKuutSLo`** for mainnet or **`HyWxreWnng9ZBDPYpuYugAfpCMkRkJ1oz93oyoybDFLB`** for devnet.\n```python\n# mainnet MPG\nmpg = PublicKey("HiCy6vzuN3yLXD3z35D6nV7bzNLcyrvGLf3uSKuutSLo")\n\n# ** OR **\n# devnet MPG\nmpg = PublicKey("HyWxreWnng9ZBDPYpuYugAfpCMkRkJ1oz93oyoybDFLB")\n```\nNow, we\'re ready to get an instance of `SDKContext` for this MPG.\n```python\nctx = SDKContext.connect(\n\tclient=client,\n\tmarket_product_group_key=mpg,\n\tpayer=keypair,\n\traise_on_error=True\n)\n```\n\n## Registering new trader / TRG\nIf you\'re a new trader, creation of a trading account is required.\n```python\ntrader = ctx.register_trader(keypair)\ntrg_key = trader.account\n```\n\nThe **Trader Risk Group (TRG)** is your trading account, that you can now use.\n\n## Using an existing TRG\nIf you already have a trader set up, you need to provide the TRG public key for it.\nThe SDK allows you to list all your registered TRGs.\n```python\n# this will return a list of your all your TRG public keys\n# for example: [HeykeQWRh6DC2Tz5X3WBuWdMHicyECDEFGMjomV6LBye, HeyZNJ9gQVAEqHeCFFQ781E53d66DATKXHeynwnCFBye]\ntrg_keys = ctx.list_trader_risk_groups()\n```\n\nAfter finding your TRG, you can initialise the `SDKTrader` instance.\n```python\nfrom dexteritysdk.codegen.dex.types import TraderRiskGroup\nfrom dexteritysdk.program_ids import *\nfrom dexteritysdk.utils.solana import explore\n\n# ...\ntrader = SDKTrader.connect(ctx, trg_pubkey, keypair)\n```\n\n## Funding the TRG\nTo start trading, you need to deposit funds.\nThe tokens deposited have to be MPG vault mint tokens (e.g. USDC).\nThe wallet you provided will be debited.\n```python\n# this will deposit 733.1 USDC\ntrader.deposit(ctx, 733.1)\n```\n\nYou can also withdraw in a similar fashion.\n```python\n# this will withdraw 0.1 USDC back to your wallet\ntrader.withdraw(ctx, 0.1)\n```\n\nYou can check your balance at any time.\n```python\ntrader.get_trader_risk_group().cash_balance\n```\n\n## Trading on Dexterity\n\n### Listing trading products and order books\nThe `products` field of a `SDKContext` instance, is a list of the available trading products (`SDKProduct`).\nEvery `SDKProduct` has a `name` and a `get_orderbook(ctx)` function that will return its order book (`SDKOrderBook`).\nThe `SDKOrderBook` contains all `SDKOrders` on each side of the book.\n\nHere\'s an example:\n```python\nfor product in ctx.products:\n\tbook = product.get_orderbook(ctx, refresh=True)\n\tprint(f"Printing the order book of {product.name}")\n\tfor order in book.bids:\n\t\tprint(f"Bid of size {order.qty} at {order.price}")\n\tfor order in book.asks:\n\t\tprint(f"Ask of size {order.qty} at {order.price}")\n```\n\n### Placing an order\n\nPlacing an order is straightforward.\n```python\nfrom dexteritysdk.utils.aob import Side\n# ...\norder_summary = trader.place_order(ctx, product, Side.ASK, size, price)\n```\nThe returned `SDKOrderSummary` contains the `order_id` of the new order, as well as the `remaining_qty` and `filled_qty` if your order has been filled. If the order is immediately fully filled, `order_id` will be `None`.\n\nIf there\'s any error, an exception will be raised.\n\n### Cancelling orders\nTo cancel a previous order you can call `trader.cancel(ctx, product, order_id)`.\nFollowing the previous example:\n```python\ntrader.cancel(ctx, product, order_summary.order_id)\n```\n\nYou can also cancel all your open orders for multiple products.\n```python\n# products is a list of SDKProduct\n# if products list is empty or None, then all your open orders will be cancelled\nproducts = [ctx.products[0], ctx.products[2]]\ntrader.cancel_all_orders(ctx, products)\n```\nIf any cancel fails, an exception will be raised.\n\n### Positions\nPositions can also be listed, by iterating the `trader_positions` array:\n```python\ntrader.get_trader_risk_group().trader_positions\n```\n',
+    'long_description': '# Dexterity client SDK\n**Dexterity** is a derivatives decentralized exchange running on Solana.\nThis package provides the basic blocks in order to integrate and trade on Dexterity.\n\nYou can learn more about Dexterity [here](https://docs.hxro.network/market-protocols/derivatives-protocol/dexterity).\n\n## Prerequisites\n* [Solana.py](https://pypi.org/project/solana/)\n\n## Creating the client\nFirst, an instance of a Solana client is required.\n```python\nfrom dexteritysdk.dex.sdk_context import SDKContext, SDKTrader\nfrom solana.rpc.api import Client\nfrom solana.keypair import Keypair\nfrom solana.publickey import PublicKey\n\ndef main():\n\t# use "https://api.mainnet-beta.solana.com" for mainnet\n\tnetwork = "https://api.devnet.solana.com"\n\tclient = Client(network)\n```\n\nA Keypair for the payer has to also be provided.\n```python\nkeypair = Keypair.from_secret_key(keypair_bytes)\n```\nThe SDK also requires the **Market Product Group (MPG)** that we\'re going to trade on.\n\nThe public key of the default MPG is **`HiCy6vzuN3yLXD3z35D6nV7bzNLcyrvGLf3uSKuutSLo`** for mainnet or **`HyWxreWnng9ZBDPYpuYugAfpCMkRkJ1oz93oyoybDFLB`** for devnet.\n```python\n# mainnet MPG\nmpg = PublicKey("HiCy6vzuN3yLXD3z35D6nV7bzNLcyrvGLf3uSKuutSLo")\n\n# ** OR **\n# devnet MPG\nmpg = PublicKey("HyWxreWnng9ZBDPYpuYugAfpCMkRkJ1oz93oyoybDFLB")\n```\nNow, we\'re ready to get an instance of `SDKContext` for this MPG.\n```python\nctx = SDKContext.connect(\n\tclient=client,\n\tmarket_product_group_key=mpg,\n\tpayer=keypair,\n\traise_on_error=True\n)\n```\n\n## Registering new trader / TRG\nIf you\'re a new trader, creation of a trading account is required.\n```python\ntrader = ctx.register_trader(keypair)\ntrg_key = trader.account\n```\n\nThe **Trader Risk Group (TRG)** is your trading account, that you can now use.\n\n## Using an existing TRG\nIf you already have a trader set up, you need to provide the TRG public key for it.\nThe SDK allows you to list all your registered TRGs.\n```python\n# this will return a list of your all your TRG public keys\n# for example: [HeykeQWRh6DC2Tz5X3WBuWdMHicyECDEFGMjomV6LBye, HeyZNJ9gQVAEqHeCFFQ781E53d66DATKXHeynwnCFBye]\ntrg_keys = ctx.list_trader_risk_groups()\n```\n\nAfter finding your TRG, you can initialise the `SDKTrader` instance.\n```python\nfrom dexteritysdk.codegen.dex.types import TraderRiskGroup\nfrom dexteritysdk.program_ids import *\nfrom dexteritysdk.utils.solana import explore\n\n# ...\ntrader = SDKTrader.connect(ctx, trg_pubkey, keypair)\n```\n\n## Funding the TRG\nTo start trading, you need to deposit funds.\nThe tokens deposited have to be MPG vault mint tokens (e.g. USDC).\nThe wallet you provided will be debited.\n```python\n# this will deposit 733.1 USDC\ntrader.deposit(ctx, 733.1)\n```\n\nYou can also withdraw in a similar fashion.\n```python\n# this will withdraw 0.1 USDC back to your wallet\ntrader.withdraw(ctx, 0.1)\n```\n\nYou can check your balance at any time.\n```python\ntrg, _ = trader.get_trader_risk_group()\ntrg.cash_balance\n```\n\n## Trading on Dexterity\n\n### Listing trading products and order books\nThe `products` field of a `SDKContext` instance, is a list of the available trading products (`SDKProduct`).\nEvery `SDKProduct` has a `name` and a `get_orderbook(ctx)` function that will return its order book (`SDKOrderBook`).\nThe `SDKOrderBook` contains all `SDKOrders` on each side of the book.\n\nHere\'s an example:\n```python\nfor product in ctx.products:\n\tbook = product.get_orderbook(ctx, refresh=True)\n\tprint(f"Printing the order book of {product.name}")\n\tfor order in book.bids:\n\t\tprint(f"Bid of size {order.qty} at {order.price}")\n\tfor order in book.asks:\n\t\tprint(f"Ask of size {order.qty} at {order.price}")\n```\n\n### Placing an order\n\nPlacing an order is straightforward.\n```python\nfrom dexteritysdk.utils.aob import Side\n# ...\norder_summary = trader.place_order(ctx, product, Side.ASK, size, price)\n```\nThe returned `SDKOrderSummary` contains the `order_id` of the new order, as well as the `remaining_qty` and `filled_qty` if your order has been filled. If the order is immediately fully filled, `order_id` will be `None`.\n\nIf there\'s any error, an exception will be raised.\n\n### Cancelling orders\nTo cancel a previous order you can call `trader.cancel(ctx, product, order_id)`.\nFollowing the previous example:\n```python\ntrader.cancel(ctx, product, order_summary.order_id)\n```\n\nYou can also cancel all your open orders for multiple products.\n```python\n# products is a list of SDKProduct\n# if products list is empty or None, then all your open orders will be cancelled\nproducts = [ctx.products[0], ctx.products[2]]\ntrader.cancel_all_orders(ctx, products)\n```\nIf any cancel fails, an exception will be raised.\n\n### Positions\nPositions can also be listed, by iterating the `trader_positions` array:\n```python\ntrg, _ = trader.get_trader_risk_group()\ntrg.trader_positions\n```\n',
     'author': 'Joe Howarth',
     'author_email': 'josephehowarth@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `dexteritysdk-0.2.3/PKG-INFO` & `dexteritysdk-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexteritysdk
-Version: 0.2.3
+Version: 0.2.8
 Summary: Client for Dexterity - a modular derivatives decentralized exchange reference implementation
 Author: Joe Howarth
 Author-email: josephehowarth@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -202,15 +202,16 @@
 ```python
 # this will withdraw 0.1 USDC back to your wallet
 trader.withdraw(ctx, 0.1)
 ```
 
 You can check your balance at any time.
 ```python
-trader.get_trader_risk_group().cash_balance
+trg, _ = trader.get_trader_risk_group()
+trg.cash_balance
 ```
 
 ## Trading on Dexterity
 
 ### Listing trading products and order books
 The `products` field of a `SDKContext` instance, is a list of the available trading products (`SDKProduct`).
 Every `SDKProduct` has a `name` and a `get_orderbook(ctx)` function that will return its order book (`SDKOrderBook`).
@@ -254,10 +255,11 @@
 trader.cancel_all_orders(ctx, products)
 ```
 If any cancel fails, an exception will be raised.
 
 ### Positions
 Positions can also be listed, by iterating the `trader_positions` array:
 ```python
-trader.get_trader_risk_group().trader_positions
+trg, _ = trader.get_trader_risk_group()
+trg.trader_positions
 ```
```

