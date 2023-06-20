# Comparing `tmp/api_master-1.3.tar.gz` & `tmp/api_master-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_master-1.3.tar", last modified: Fri Jun 16 23:28:28 2023, max compression
+gzip compressed data, was "api_master-1.4.tar", last modified: Tue Jun 20 17:50:12 2023, max compression
```

## Comparing `api_master-1.3.tar` & `api_master-1.4.tar`

### file list

```diff
@@ -1,299 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.036078 api_master-1.3/
--rw-rw-rw-   0        0        0     2484 2023-06-16 23:28:28.036078 api_master-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1929 2023-06-16 23:10:25.000000 api_master-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.897001 api_master-1.3/api_master.egg-info/
--rw-rw-rw-   0        0        0     2484 2023-06-16 23:28:27.000000 api_master-1.3/api_master.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10676 2023-06-16 23:28:27.000000 api_master-1.3/api_master.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-16 23:28:27.000000 api_master-1.3/api_master.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-16 23:28:27.000000 api_master-1.3/api_master.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.901507 api_master-1.3/polygonsdk/
--rw-rw-rw-   0        0        0      189 2023-06-16 23:22:57.000000 api_master-1.3/polygonsdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.905717 api_master-1.3/polygonsdk/_discord/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/__init__.py
--rw-rw-rw-   0        0        0     7983 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/discord_stock_example.py
--rw-rw-rw-   0        0        0    44936 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/discord_stock_market.py
--rw-rw-rw-   0        0        0    16306 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/embeddings.py
--rw-rw-rw-   0        0        0      581 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/emojis.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.908227 api_master-1.3/polygonsdk/_discord/hooks/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/hooks/__init__.py
--rw-rw-rw-   0        0        0     1594 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/hooks/channel_webhooks.py
--rw-rw-rw-   0        0        0    10521 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/hooks/hook_dicts.py
--rw-rw-rw-   0        0        0     5462 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/hooks/send_webhook.py
--rw-rw-rw-   0        0        0    33594 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/live_discord.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.908227 api_master-1.3/polygonsdk/_discord/selectmenus/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/selectmenus/__init__.py
--rw-rw-rw-   0        0        0    33209 2023-06-11 22:20:44.000000 api_master-1.3/polygonsdk/_discord/selectmenus/mainselect.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.910230 api_master-1.3/polygonsdk/_discord/views/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/views/__init__.py
--rw-rw-rw-   0        0        0     1640 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/views/mainview.py
--rw-rw-rw-   0        0        0     3792 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/views/menus.py
--rw-rw-rw-   0        0        0     7502 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/_discord/webhook_creation.py
--rw-rw-rw-   0        0        0     7264 2023-06-16 23:04:23.000000 api_master-1.3/polygonsdk/app.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.912227 api_master-1.3/polygonsdk/bot/
--rw-rw-rw-   0        0        0       72 2023-06-16 22:29:19.000000 api_master-1.3/polygonsdk/bot/__init__.py
--rw-rw-rw-   0        0        0    13384 2023-06-16 23:23:57.000000 api_master-1.3/polygonsdk/bot/autocomp.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.916227 api_master-1.3/polygonsdk/bot/cogs/
--rw-rw-rw-   0        0        0      162 2023-06-16 22:30:15.000000 api_master-1.3/polygonsdk/bot/cogs/__init__.py
--rw-rw-rw-   0        0        0     4478 2023-06-16 03:42:45.000000 api_master-1.3/polygonsdk/bot/cogs/earnings.py
--rw-rw-rw-   0        0        0     1406 2023-06-16 02:49:27.000000 api_master-1.3/polygonsdk/bot/cogs/evaluate.py
--rw-rw-rw-   0        0        0    11853 2023-06-06 22:47:55.000000 api_master-1.3/polygonsdk/bot/cogs/jasmy.py
--rw-rw-rw-   0        0        0     2219 2023-06-15 04:47:31.000000 api_master-1.3/polygonsdk/bot/cogs/navigate.py
--rw-rw-rw-   0        0        0     1794 2023-06-06 22:53:29.000000 api_master-1.3/polygonsdk/bot/cogs/scan.py
--rw-rw-rw-   0        0        0    10785 2023-06-16 03:00:26.000000 api_master-1.3/polygonsdk/bot/cogs/stream.py
--rw-rw-rw-   0        0        0    32431 2023-06-16 03:44:06.000000 api_master-1.3/polygonsdk/bot/cogs/webull.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.922100 api_master-1.3/polygonsdk/bot/cogs2/
--rw-rw-rw-   0        0        0        0 2022-10-11 19:37:24.000000 api_master-1.3/polygonsdk/bot/cogs2/__init__.py
--rw-rw-rw-   0        0        0    13678 2023-06-06 22:33:16.000000 api_master-1.3/polygonsdk/bot/cogs2/analysis.py
--rw-rw-rw-   0        0        0     4580 2023-06-16 02:58:46.000000 api_master-1.3/polygonsdk/bot/cogs2/collect.py
--rw-rw-rw-   0        0        0    14094 2023-06-16 03:47:55.000000 api_master-1.3/polygonsdk/bot/cogs2/economy.py
--rw-rw-rw-   0        0        0    13966 2023-06-16 03:00:46.000000 api_master-1.3/polygonsdk/bot/cogs2/learn.py
--rw-rw-rw-   0        0        0     3830 2023-06-16 03:47:27.000000 api_master-1.3/polygonsdk/bot/cogs2/news.py
--rw-rw-rw-   0        0        0    75051 2023-04-11 14:56:18.000000 api_master-1.3/polygonsdk/bot/cogs2/occ.py
--rw-rw-rw-   0        0        0    19227 2023-06-16 03:43:01.000000 api_master-1.3/polygonsdk/bot/cogs2/options.py
--rw-rw-rw-   0        0        0     1823 2023-06-16 02:52:02.000000 api_master-1.3/polygonsdk/bot/cogs2/prices_and_technicals.py
--rw-rw-rw-   0        0        0    50520 2023-06-16 03:47:06.000000 api_master-1.3/polygonsdk/bot/cogs2/stock.py
--rw-rw-rw-   0        0        0    17675 2023-06-16 03:02:03.000000 api_master-1.3/polygonsdk/bot/cogs2/view.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.928178 api_master-1.3/polygonsdk/bot/cogs3/
--rw-rw-rw-   0        0        0        0 2022-10-18 03:53:56.000000 api_master-1.3/polygonsdk/bot/cogs3/__init__.py
--rw-rw-rw-   0        0        0     2420 2023-06-16 03:03:50.000000 api_master-1.3/polygonsdk/bot/cogs3/allinone.py
--rw-rw-rw-   0        0        0     4646 2023-06-16 03:07:36.000000 api_master-1.3/polygonsdk/bot/cogs3/cboe.py
--rw-rw-rw-   0        0        0    13259 2023-06-16 03:11:09.000000 api_master-1.3/polygonsdk/bot/cogs3/discord.py
--rw-rw-rw-   0        0        0    15308 2023-06-16 03:45:39.000000 api_master-1.3/polygonsdk/bot/cogs3/fed.py
--rw-rw-rw-   0        0        0     4049 2023-06-16 03:15:01.000000 api_master-1.3/polygonsdk/bot/cogs3/fudstop.py
--rw-rw-rw-   0        0        0    10534 2023-06-16 03:14:52.000000 api_master-1.3/polygonsdk/bot/cogs3/iv.py
--rw-rw-rw-   0        0        0     7484 2023-06-16 03:14:29.000000 api_master-1.3/polygonsdk/bot/cogs3/reddit.py
--rw-rw-rw-   0        0        0     2604 2023-06-16 03:13:44.000000 api_master-1.3/polygonsdk/bot/cogs3/school.py
--rw-rw-rw-   0        0        0     8852 2023-06-16 03:11:56.000000 api_master-1.3/polygonsdk/bot/cogs3/social.py
--rw-rw-rw-   0        0        0     9893 2023-06-16 03:41:40.000000 api_master-1.3/polygonsdk/bot/cogs3/strat.py
--rw-rw-rw-   0        0        0     6919 2023-06-11 22:19:59.000000 api_master-1.3/polygonsdk/bot/discord_emojis.py
--rw-rw-rw-   0        0        0     1440 2023-06-16 03:51:23.000000 api_master-1.3/polygonsdk/bot/main.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.928178 api_master-1.3/polygonsdk/bot/utils/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/bot/utils/__init__.py
--rw-rw-rw-   0        0        0     1368 2023-06-16 02:40:26.000000 api_master-1.3/polygonsdk/bot/utils/crypto_coins.py
--rw-rw-rw-   0        0        0      998 2023-06-16 02:35:33.000000 api_master-1.3/polygonsdk/bot/utils/date_times.py
--rw-rw-rw-   0        0        0   224003 2023-06-16 03:10:59.000000 api_master-1.3/polygonsdk/bot/utils/lists_and_dicts.py
--rw-rw-rw-   0        0        0   199781 2023-06-16 02:46:46.000000 api_master-1.3/polygonsdk/bot/utils/webull_tickers.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.928178 api_master-1.3/polygonsdk/bot/views/
--rw-rw-rw-   0        0        0       49 2023-06-16 22:29:34.000000 api_master-1.3/polygonsdk/bot/views/__init__.py
--rw-rw-rw-   0        0        0  1503928 2023-06-16 03:50:00.000000 api_master-1.3/polygonsdk/bot/views/learnviews.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.945593 api_master-1.3/polygonsdk/bot/views/uiviews/
--rw-rw-rw-   0        0        0   320159 2023-06-16 03:04:42.000000 api_master-1.3/polygonsdk/bot/views/uiviews/MarketAnalysis.py
--rw-rw-rw-   0        0        0     5109 2023-06-16 03:43:55.000000 api_master-1.3/polygonsdk/bot/views/uiviews/TickerAnalysis.py
--rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.3/polygonsdk/bot/views/uiviews/__init__ copy.py
--rw-rw-rw-   0        0        0        0 2022-10-25 14:28:50.000000 api_master-1.3/polygonsdk/bot/views/uiviews/__init__.py
--rw-rw-rw-   0        0        0     5169 2023-06-16 03:04:01.000000 api_master-1.3/polygonsdk/bot/views/uiviews/capitalflow.py
--rw-rw-rw-   0        0        0   110984 2022-11-14 02:53:40.000000 api_master-1.3/polygonsdk/bot/views/uiviews/cmslist.py
--rw-rw-rw-   0        0        0   107414 2023-06-16 12:53:34.000000 api_master-1.3/polygonsdk/bot/views/uiviews/cmslist2.py
--rw-rw-rw-   0        0        0    18026 2023-06-16 03:04:21.000000 api_master-1.3/polygonsdk/bot/views/uiviews/directiondrop.py
--rw-rw-rw-   0        0        0     9311 2023-06-16 03:04:32.000000 api_master-1.3/polygonsdk/bot/views/uiviews/financialselects.py
--rw-rw-rw-   0        0        0    12480 2023-06-16 03:04:50.000000 api_master-1.3/polygonsdk/bot/views/uiviews/ftds.py
--rw-rw-rw-   0        0        0     4675 2023-06-16 03:04:58.000000 api_master-1.3/polygonsdk/bot/views/uiviews/leveragedropdown.py
--rw-rw-rw-   0        0        0     7693 2023-06-16 03:05:03.000000 api_master-1.3/polygonsdk/bot/views/uiviews/lowfloat.py
--rw-rw-rw-   0        0        0     4487 2023-06-16 03:51:49.000000 api_master-1.3/polygonsdk/bot/views/uiviews/masterview.py
--rw-rw-rw-   0        0        0     5619 2022-11-05 23:34:22.000000 api_master-1.3/polygonsdk/bot/views/uiviews/mostactive.py
--rw-rw-rw-   0        0        0     6579 2022-11-05 23:04:27.000000 api_master-1.3/polygonsdk/bot/views/uiviews/pressrelease.py
--rw-rw-rw-   0        0        0     3355 2023-06-16 03:17:25.000000 api_master-1.3/polygonsdk/bot/views/uiviews/quote.py
--rw-rw-rw-   0        0        0    13749 2023-06-16 03:04:42.000000 api_master-1.3/polygonsdk/bot/views/uiviews/shortinterest.py
--rw-rw-rw-   0        0        0     3551 2023-06-16 12:56:25.000000 api_master-1.3/polygonsdk/cfg.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.947593 api_master-1.3/polygonsdk/examples/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/__init__.py
--rw-rw-rw-   0        0        0     5940 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/all_attributes.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.947593 api_master-1.3/polygonsdk/examples/functions/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:36:14.000000 api_master-1.3/polygonsdk/examples/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.952194 api_master-1.3/polygonsdk/examples/functions/options/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:36:18.000000 api_master-1.3/polygonsdk/examples/functions/options/__init__.py
--rw-rw-rw-   0        0        0      706 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/options/create_option_symbol.py
--rw-rw-rw-   0        0        0      910 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/options/fetch_entire_chain.py
--rw-rw-rw-   0        0        0     1625 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/options/option_quote.py
--rw-rw-rw-   0        0        0     2408 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/options/option_trades.py
--rw-rw-rw-   0        0        0     1797 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/options/plot_option_aggs.py
--rw-rw-rw-   0        0        0     5590 2023-06-14 15:27:10.000000 api_master-1.3/polygonsdk/examples/functions/options/scanner_example.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.956194 api_master-1.3/polygonsdk/examples/functions/stocks/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:36:22.000000 api_master-1.3/polygonsdk/examples/functions/stocks/__init__.py
--rw-rw-rw-   0        0        0     1796 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/stocks/latest_news.py
--rw-rw-rw-   0        0        0     1408 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/stocks/plot_aggs.py
--rw-rw-rw-   0        0        0     8185 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/stocks/scan_candles.py
--rw-rw-rw-   0        0        0     2116 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/stocks/stock_aggregates.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.964310 api_master-1.3/polygonsdk/examples/functions/technical_analysis/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:36:27.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/__init__.py
--rw-rw-rw-   0        0        0      533 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/bollinger_bands.py
--rw-rw-rw-   0        0        0     4375 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/candle_patterns.py
--rw-rw-rw-   0        0        0     1376 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/ema.py
--rw-rw-rw-   0        0        0      693 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/find_gaps.py
--rw-rw-rw-   0        0        0     2399 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/get_ema.py
--rw-rw-rw-   0        0        0      644 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/get_logo.py
--rw-rw-rw-   0        0        0     3195 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/get_macd.py
--rw-rw-rw-   0        0        0      665 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/get_pivot_points.py
--rw-rw-rw-   0        0        0     2051 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/get_rsi.py
--rw-rw-rw-   0        0        0     1935 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/get_sma.py
--rw-rw-rw-   0        0        0      930 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/macd_sma_rsi.py
--rw-rw-rw-   0        0        0      487 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/rate_of_change.py
--rw-rw-rw-   0        0        0      627 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/rsi.py
--rw-rw-rw-   0        0        0     1189 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/functions/technical_analysis/support_resistance.py
--rw-rw-rw-   0        0        0      703 2023-06-14 15:26:12.000000 api_master-1.3/polygonsdk/examples/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.968310 api_master-1.3/polygonsdk/examples/realtime_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/realtime_markets/__init__.py
--rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/realtime_markets/crypto_market.py
--rw-rw-rw-   0        0        0    44945 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/realtime_markets/discord_market.py
--rw-rw-rw-   0        0        0      922 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/realtime_markets/forex_market.py
--rw-rw-rw-   0        0        0      776 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/realtime_markets/indices_market.py
--rw-rw-rw-   0        0        0      989 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/realtime_markets/options_market.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.970818 api_master-1.3/polygonsdk/examples/simulated_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/simulated_markets/__init__.py
--rw-rw-rw-   0        0        0      688 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/examples/simulated_markets/helpers.py
--rw-rw-rw-   0        0        0     5115 2023-06-11 22:19:16.000000 api_master-1.3/polygonsdk/examples/simulated_markets/mock_discord.py
--rw-rw-rw-   0        0        0     1951 2023-06-12 01:17:16.000000 api_master-1.3/polygonsdk/examples/simulated_markets/mock_market.py
--rw-rw-rw-   0        0        0     1551 2023-06-12 01:18:49.000000 api_master-1.3/polygonsdk/examples/simulated_markets/mock_options_market.py
--rw-rw-rw-   0        0        0    14776 2023-06-16 14:39:01.000000 api_master-1.3/polygonsdk/examples/webull_data.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.976817 api_master-1.3/polygonsdk/funcs/
--rw-rw-rw-   0        0        0        0 2023-06-11 22:29:36.000000 api_master-1.3/polygonsdk/funcs/__init__.py
--rw-rw-rw-   0        0        0    36181 2023-06-11 22:44:36.000000 api_master-1.3/polygonsdk/funcs/get_data.py
--rw-rw-rw-   0        0        0      619 2023-06-13 22:33:48.000000 api_master-1.3/polygonsdk/funcs/get_latest_crypto_data.py
--rw-rw-rw-   0        0        0      585 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/funcs/get_latest_forex_data.py
--rw-rw-rw-   0        0        0      446 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/funcs/get_latest_indices_data.py
--rw-rw-rw-   0        0        0      762 2023-06-11 21:54:23.000000 api_master-1.3/polygonsdk/funcs/get_latest_options_data.py
--rw-rw-rw-   0        0        0      598 2023-06-12 00:39:12.000000 api_master-1.3/polygonsdk/funcs/get_latest_ticker_data.py
--rw-rw-rw-   0        0        0      335 2023-06-16 14:21:39.000000 api_master-1.3/polygonsdk/funcs/get_webull_data.py
--rw-rw-rw-   0        0        0     1052 2023-06-12 01:22:03.000000 api_master-1.3/polygonsdk/funcs/sec_filings.py
--rw-rw-rw-   0        0        0     2264 2023-06-12 01:16:14.000000 api_master-1.3/polygonsdk/funcs/webull_examples.py
--rw-rw-rw-   0        0        0     1252 2023-06-16 14:28:50.000000 api_master-1.3/polygonsdk/myconfig.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.976817 api_master-1.3/polygonsdk/sdks/
--rw-rw-rw-   0        0        0      275 2023-06-16 23:26:41.000000 api_master-1.3/polygonsdk/sdks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.978818 api_master-1.3/polygonsdk/sdks/discord_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/discord_sdk/__init__.py
--rw-rw-rw-   0        0        0       53 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/discord_sdk/channel_ids.py
--rw-rw-rw-   0        0        0     4497 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/discord_sdk/discord_sdk.py
--rw-rw-rw-   0        0        0     2157 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/discord_sdk/searching.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.993049 api_master-1.3/polygonsdk/sdks/examples/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/__init__.py
--rw-rw-rw-   0        0        0     6184 2023-06-12 00:26:46.000000 api_master-1.3/polygonsdk/sdks/examples/all_attributes.py
--rw-rw-rw-   0        0        0      517 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/bollinger_bands.py
--rw-rw-rw-   0        0        0      706 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/create_option_symbol.py
--rw-rw-rw-   0        0        0     1664 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/ema.py
--rw-rw-rw-   0        0        0      910 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/fetch_entire_chain.py
--rw-rw-rw-   0        0        0      649 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/find_gaps.py
--rw-rw-rw-   0        0        0      823 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_all_options_data.py
--rw-rw-rw-   0        0        0     2399 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_ema.py
--rw-rw-rw-   0        0        0      600 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_latest_crypto_data.py
--rw-rw-rw-   0        0        0      585 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_latest_forex_data.py
--rw-rw-rw-   0        0        0      446 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_latest_indices_data.py
--rw-rw-rw-   0        0        0      644 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_latest_ticker_data.py
--rw-rw-rw-   0        0        0     3161 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_macd.py
--rw-rw-rw-   0        0        0      582 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_pivot_points.py
--rw-rw-rw-   0        0        0     2051 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_rsi.py
--rw-rw-rw-   0        0        0     2172 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/get_sma.py
--rw-rw-rw-   0        0        0     1796 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/latest_news.py
--rw-rw-rw-   0        0        0     1625 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/option_quote.py
--rw-rw-rw-   0        0        0     2408 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/option_trades.py
--rw-rw-rw-   0        0        0     1408 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/plot_aggs.py
--rw-rw-rw-   0        0        0      796 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/plot_macd.py
--rw-rw-rw-   0        0        0     1797 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/plot_option_aggs.py
--rw-rw-rw-   0        0        0      487 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/rate_of_change.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.995049 api_master-1.3/polygonsdk/sdks/examples/realtime_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/realtime_markets/__init__.py
--rw-rw-rw-   0        0        0     2479 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/realtime_markets/crypto_market.py
--rw-rw-rw-   0        0        0      922 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/realtime_markets/forex_market.py
--rw-rw-rw-   0        0        0      776 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/realtime_markets/indices_market.py
--rw-rw-rw-   0        0        0      989 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/realtime_markets/options_market.py
--rw-rw-rw-   0        0        0     4837 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/scanner_example.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.997049 api_master-1.3/polygonsdk/sdks/examples/simulated_markets/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/simulated_markets/__init__.py
--rw-rw-rw-   0        0        0      688 2023-06-14 15:26:03.000000 api_master-1.3/polygonsdk/sdks/examples/simulated_markets/helpers.py
--rw-rw-rw-   0        0        0     2606 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/simulated_markets/mock_market.py
--rw-rw-rw-   0        0        0     1806 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/simulated_markets/mock_options_market.py
--rw-rw-rw-   0        0        0     2116 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/stock_aggregates.py
--rw-rw-rw-   0        0        0     1189 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/examples/support_resistance.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:27.999049 api_master-1.3/polygonsdk/sdks/fudstop_sdk/
--rw-rw-rw-   0        0        0        1 2023-06-12 00:06:40.000000 api_master-1.3/polygonsdk/sdks/fudstop_sdk/__init__.py
--rw-rw-rw-   0        0        0     3095 2023-06-16 23:24:04.000000 api_master-1.3/polygonsdk/sdks/fudstop_sdk/fudstop_sdk.py
--rw-rw-rw-   0        0        0     1847 2023-06-16 23:24:08.000000 api_master-1.3/polygonsdk/sdks/fudstop_sdk/gaps.py
--rw-rw-rw-   0        0        0      613 2023-06-16 23:24:13.000000 api_master-1.3/polygonsdk/sdks/fudstop_sdk/option_vol_totals.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.001559 api_master-1.3/polygonsdk/sdks/helpers/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/helpers/__init__.py
--rw-rw-rw-   0        0        0     2001 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/helpers/conditions.py
--rw-rw-rw-   0        0        0        2 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/helpers/get_cik.py
--rw-rw-rw-   0        0        0     5442 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/helpers/helpers.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.003559 api_master-1.3/polygonsdk/sdks/models/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/models/__init__.py
--rw-rw-rw-   0        0        0      488 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/models/common.py
--rw-rw-rw-   0        0        0     5097 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/models/maps.py
--rw-rw-rw-   0        0        0    13078 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/models/test_events.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.016067 api_master-1.3/polygonsdk/sdks/polygon_sdk/
--rw-rw-rw-   0        0        0      543 2023-06-16 22:28:47.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/__init__.py
--rw-rw-rw-   0        0        0     1265 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/aggregates.py
--rw-rw-rw-   0        0        0    29379 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/async_options_sdk.py
--rw-rw-rw-   0        0        0    52775 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/async_polygon_sdk.py
--rw-rw-rw-   0        0        0     1135 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/company_info.py
--rw-rw-rw-   0        0        0      703 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/daily_open_close.py
--rw-rw-rw-   0        0        0    15043 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/financials.py
--rw-rw-rw-   0        0        0     6644 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/forex_crypto.py
--rw-rw-rw-   0        0        0     8957 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/get_all_options.py
--rw-rw-rw-   0        0        0     1131 2023-06-11 21:54:24.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/indices_snapshot.py
--rw-rw-rw-   0        0        0      823 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/logo.py
--rw-rw-rw-   0        0        0    27900 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/mapping_dicts.py
--rw-rw-rw-   0        0        0      782 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/models.py
--rw-rw-rw-   0        0        0      819 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/news.py
--rw-rw-rw-   0        0        0      820 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/option_aggs.py
--rw-rw-rw-   0        0        0     1493 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/option_quote.py
--rw-rw-rw-   0        0        0     3079 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/option_snapshot.py
--rw-rw-rw-   0        0        0      873 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/option_trades.py
--rw-rw-rw-   0        0        0      538 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/pivot_points.py
--rw-rw-rw-   0        0        0      690 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/quote.py
--rw-rw-rw-   0        0        0      151 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/sec.py
--rw-rw-rw-   0        0        0     4192 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/snapshot.py
--rw-rw-rw-   0        0        0     1313 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/technical_conditions.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.018066 api_master-1.3/polygonsdk/sdks/polygon_sdk/technicals/
--rw-rw-rw-   0        0        0        1 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/technicals/__init__.py
--rw-rw-rw-   0        0        0      248 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/technicals/ema.py
--rw-rw-rw-   0        0        0      229 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/technicals/macd.py
--rw-rw-rw-   0        0        0      233 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/technicals/rsi.py
--rw-rw-rw-   0        0        0      244 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/technicals/sma.py
--rw-rw-rw-   0        0        0     3361 2023-06-13 21:44:27.000000 api_master-1.3/polygonsdk/sdks/polygon_sdk/tickernews.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.021657 api_master-1.3/polygonsdk/sdks/stocksera_sdk/
--rw-rw-rw-   0        0        0      103 2023-06-16 22:27:26.000000 api_master-1.3/polygonsdk/sdks/stocksera_sdk/__init__.py
--rw-rw-rw-   0        0        0      757 2023-06-14 23:11:39.000000 api_master-1.3/polygonsdk/sdks/stocksera_sdk/borrowed.py
--rw-rw-rw-   0        0        0      956 2023-06-14 23:30:32.000000 api_master-1.3/polygonsdk/sdks/stocksera_sdk/earnings.py
--rw-rw-rw-   0        0        0     1309 2023-06-16 14:28:24.000000 api_master-1.3/polygonsdk/sdks/stocksera_sdk/stocksera_sdk.py
--rw-rw-rw-   0        0        0      580 2023-06-14 23:22:44.000000 api_master-1.3/polygonsdk/sdks/stocksera_sdk/treasury.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.021657 api_master-1.3/polygonsdk/sdks/terminals/
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/terminals/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.021657 api_master-1.3/polygonsdk/sdks/terminals/crypto/
--rw-rw-rw-   0        0        0        0 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/terminals/crypto/__init__.py
--rw-rw-rw-   0        0        0     1672 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/terminals/crypto/menu.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.031724 api_master-1.3/polygonsdk/sdks/webull_sdk/
--rw-rw-rw-   0        0        0      440 2023-06-16 22:31:19.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/__init__.py
--rw-rw-rw-   0        0        0      882 2023-06-11 22:15:21.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/calendar.py
--rw-rw-rw-   0        0        0     9144 2023-06-16 14:33:32.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/capitalflow.py
--rw-rw-rw-   0        0        0     1152 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/cost_distribution.py
--rw-rw-rw-   0        0        0     2282 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/derivative_query.py
--rw-rw-rw-   0        0        0     2426 2023-06-11 22:15:21.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/etf_finder.py
--rw-rw-rw-   0        0        0      486 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/etf_holdings.py
--rw-rw-rw-   0        0        0     1100 2023-06-16 14:24:58.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/events.py
--rw-rw-rw-   0        0        0     7818 2023-06-11 22:15:21.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/financial_statement.py
--rw-rw-rw-   0        0        0     3780 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/forecast.py
--rw-rw-rw-   0        0        0     1033 2023-06-11 22:15:21.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/institutional_holdings.py
--rw-rw-rw-   0        0        0     1235 2023-06-16 22:35:10.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/manage.py
--rw-rw-rw-   0        0        0      617 2023-06-11 22:15:21.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/news.py
--rw-rw-rw-   0        0        0      307 2023-06-11 22:15:21.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/shortinterest.py
--rw-rw-rw-   0        0        0     2730 2023-06-11 21:54:25.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/top_gainers.py
--rw-rw-rw-   0        0        0    16723 2023-06-11 22:15:21.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/top_options.py
--rw-rw-rw-   0        0        0     5556 2023-06-11 22:15:21.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/webull_data.py
--rw-rw-rw-   0        0        0    42510 2023-06-16 23:24:24.000000 api_master-1.3/polygonsdk/sdks/webull_sdk/webull_sdk.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.031724 api_master-1.3/polygonsdk/static/
--rw-rw-rw-   0        0        0      101 2023-06-14 14:26:46.000000 api_master-1.3/polygonsdk/static/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.031724 api_master-1.3/polygonsdk/static/css/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:37:24.000000 api_master-1.3/polygonsdk/static/css/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.031724 api_master-1.3/polygonsdk/static/images/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:37:29.000000 api_master-1.3/polygonsdk/static/images/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.031724 api_master-1.3/polygonsdk/static/js/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:37:34.000000 api_master-1.3/polygonsdk/static/js/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.031724 api_master-1.3/polygonsdk/static/py/
--rw-rw-rw-   0        0        0        0 2023-06-13 22:37:38.000000 api_master-1.3/polygonsdk/static/py/__init__.py
--rw-rw-rw-   0        0        0      573 2023-06-15 22:05:01.000000 api_master-1.3/polygonsdk/static/py/commands.py
--rw-rw-rw-   0        0        0      796 2023-06-12 21:29:16.000000 api_master-1.3/polygonsdk/static/py/snippets.py
--rw-rw-rw-   0        0        0      312 2023-06-12 21:41:31.000000 api_master-1.3/polygonsdk/static/py/website_components.py
-drwxrwxrwx   0        0        0        0 2023-06-16 23:28:28.035729 api_master-1.3/polygonsdk/templates/
--rw-rw-rw-   0        0        0        0 2023-06-16 22:25:34.000000 api_master-1.3/polygonsdk/templates/__init__.py
--rw-rw-rw-   0        0        0     4315 2023-06-15 21:34:52.000000 api_master-1.3/polygonsdk/test.py
--rw-rw-rw-   0        0        0       42 2023-06-16 23:28:28.036078 api_master-1.3/setup.cfg
--rw-rw-rw-   0        0        0      755 2023-06-16 23:28:22.000000 api_master-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:50:12.928197 api_master-1.4/
+-rw-rw-rw-   0        0        0     2484 2023-06-20 17:50:12.928197 api_master-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1929 2023-06-12 00:29:12.000000 api_master-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 17:50:12.928197 api_master-1.4/api_master.egg-info/
+-rw-rw-rw-   0        0        0     2484 2023-06-20 17:50:12.000000 api_master-1.4/api_master.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2023-06-20 17:50:12.000000 api_master-1.4/api_master.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 17:50:12.000000 api_master-1.4/api_master.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 17:50:12.000000 api_master-1.4/api_master.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 17:50:12.928197 api_master-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      755 2023-06-20 17:50:06.000000 api_master-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:50:12.928197 api_master-1.4/static/
+-rw-rw-rw-   0        0        0      101 2023-06-14 14:26:46.000000 api_master-1.4/static/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:50:12.928197 api_master-1.4/static/css/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:37:24.000000 api_master-1.4/static/css/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:50:12.928197 api_master-1.4/static/images/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:37:29.000000 api_master-1.4/static/images/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:50:12.928197 api_master-1.4/static/js/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:37:34.000000 api_master-1.4/static/js/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:50:12.928197 api_master-1.4/static/py/
+-rw-rw-rw-   0        0        0        0 2023-06-13 22:37:38.000000 api_master-1.4/static/py/__init__.py
+-rw-rw-rw-   0        0        0    43484 2023-06-19 20:44:14.000000 api_master-1.4/static/py/api_functions.py
+-rw-rw-rw-   0        0        0      573 2023-06-15 22:05:01.000000 api_master-1.4/static/py/commands.py
+-rw-rw-rw-   0        0        0      796 2023-06-12 21:29:16.000000 api_master-1.4/static/py/snippets.py
+-rw-rw-rw-   0        0        0      312 2023-06-12 21:41:31.000000 api_master-1.4/static/py/website_components.py
+drwxrwxrwx   0        0        0        0 2023-06-20 17:50:12.928197 api_master-1.4/templates/
+-rw-rw-rw-   0        0        0        0 2023-06-16 22:25:34.000000 api_master-1.4/templates/__init__.py
```

### Comparing `api_master-1.3/PKG-INFO` & `api_master-1.4/api_master.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: api_master
-Version: 1.3
+Name: api-master
+Version: 1.4
 Summary: Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.
 Home-page: https://github.com/your-username/your-package-repo
 Author: Chuck Dustin
 Author-email: chuckdustin12@gmail.com
 Keywords: trading,stocks,options,crypto,forex,indices,discord
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `api_master-1.3/README.md` & `api_master-1.4/README.md`

 * *Files identical despite different names*

### Comparing `api_master-1.3/api_master.egg-info/PKG-INFO` & `api_master-1.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: api-master
-Version: 1.3
+Name: api_master
+Version: 1.4
 Summary: Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.
 Home-page: https://github.com/your-username/your-package-repo
 Author: Chuck Dustin
 Author-email: chuckdustin12@gmail.com
 Keywords: trading,stocks,options,crypto,forex,indices,discord
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `api_master-1.3/polygonsdk/sdks/webull_sdk/webull_sdk.py` & `api_master-1.4/static/py/api_functions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,824 +1,744 @@
-from pathlib import Path
-import sys
-
-# Get the absolute path of the current file
-current_file_path = Path(__file__).resolve()
-
-# Get the absolute path of the 'cfg' module
-cfg_module_path = current_file_path.parent.parent / 'cfg'
+import requests
+from api_master.sdks.webull_sdk.webull_sdk import AsyncWebullSDK
+from api_master.examples.webull_webull_data import Webull
+from api_master.cfg import thirty_days_from_now_str
+import aiohttp
+webull = AsyncWebullSDK()
 
-# Add the module path to sys.path
-sys.path.append(str(cfg_module_path))
 
 
+async def fetch(session, url):
+    async with session.get(url) as response:
+        return await response.json()
 
-import aiohttp
-from .derivative_query import QueryDerivatives
-from typing import List, Optional
-from aiohttp.client_exceptions import ContentTypeError
-from .capitalflow import CapitalFlow
-import aiohttp
-from dateutil import parser
-from .etf_holdings import ETFHoldings
-from .calendar import EarningsCalendar
-from .cost_distribution import CostDistribution
-from .events import Event
-import pandas as pd
-from .webull_data import Analysis, WebullStockData, WebullVolAnalysis
-from .top_gainers import GainersData
-from .etf_finder import ETFCommodity
-from .top_options import BelongTicker, Values, Derivative, TickerValues
-from typing import Dict,Union
-from datetime import datetime, timedelta, timezone
-from .financial_statement import FinancialStatement, CashFlow, BalanceSheet
-from .news import NewsItem
-from .shortinterest import ShortInterest
-from ...cfg import today_str, thirty_days_ago_str
-from .institutional_holdings import InstitutionHolding
-now = datetime.now()
-ninety_days_from_now = now + timedelta(days=90)
-ninety_days = ninety_days_from_now.strftime("%Y-%m-%d")
-seen_article_urls = set()
-thresholds = {
-    'current_ratio': 1.5,
-    'quick_ratio': 1,
-    'debt_to_equity_ratio': 2,
-    'return_on_assets': 0.05,
-    'return_on_equity': 0.15,
-    'gross_profit_margin': 0.4,
-    'operating_margin': 0.1,
-    'net_profit_margin': 0.05,
-    'dividend_payout_ratio': (0.3, 0.8),
-    'revenue_growth': 0.1,
-    'total_asset_turnover': 0.5,
-    'inventory_turnover': 5,
-    'days_sales_outstanding': 45,
-    'debt_ratio': 0.6,
-    'interest_coverage': 3,
-    'price_to_earnings_ratio': 15,
-    'price_to_sales_ratio': 2.5,
-    'price_to_book_value': 3,
-    'eps_growth': 0.1,
-    'free_cash_flow_margin': 0.05,
-    'score': 14,
-}
-class AsyncWebullSDK:
-    def __init__(self, tickerId=None, symbol=None):
-        self.tickerId = tickerId
-        self._ticker = None
-        self._values = None
-        self._earning_release_id = None
-        self._ticker_id = None
-        self._region_id = None
-        self._qualifier = None
-        self._eps = None
-        self._eps_estimate = None
-        self._year = None
-        self._quarter = None
-        self._release_date = None
-        self._is_live = None
-        self._last_release_date = None
-        self._publish_status = None
-        self.tickerId = tickerId
-        self.symbol = symbol
-        self.base_url = "https://quotes-gw.webullfintech.com/api/"
-
-    async def get_top_gainers_data(self, type: str):
+async def get_price_data(api_key,tickers: str):
+    if tickers.startswith('SPX'):
+        ticker = "I:SPX"
+        type = "v3/snapshot/indices/I:SPX"
+        url = f"https://api.polygon.io/v3/snapshot/indices?ticker.any_of=I:SPX&apiKey={api_key}"
         async with aiohttp.ClientSession() as session:
-            async with session.get(f"https://quotes-gw.webullfintech.com/api/bgw/market/topGainers?regionId=6&rankType={type}&pageIndex=1&pageSize=350") as response:
-                data = await response.json()
-                print(data)
-                datas = data['data']
-                top_gainers = [d['ticker'] for d in datas]
-                results = GainersData(top_gainers)
-                
-            return results    
-            
-    async def top_options_chains(self, rank_type):
-        url = f"https://quotes-gw.webullfintech.com/api/wlas/option/rank/list?regionId=6&rankType={rank_type}&pageIndex=1&pageSize=350"
+            return await fetch(session, url)
+    else:
+        type = "v2/snapshot/locale/us/markets/stocks/tickers"
+        url = f"https://api.polygon.io/v3/snapshot?ticker.any_of={tickers}&apiKey={api_key}"
+        print(url)
         async with aiohttp.ClientSession() as session:
-            async with session.get(url) as response:
-                response = await response.json()
-                data = response.get('data', None)
-                derivatives = [Derivative.from_dict(data.get("derivative", {})) for data in data]
-                values = [Values.from_dict(data.get("values", {})) for data in data]
-                belongticker = [BelongTicker.from_dict(data.get("belongTicker", {})) for data in data]
-
-                self.change = [i.change for i in belongticker]
-                self.changeRatio = [i.changeRatio for i in belongticker]
-                self.close = [i.close for i in belongticker]
-                self.symbol = [i.symbol for i in derivatives]
-                self.fiftyTwoWkHigh = [i.fiftyTwoWkHigh for i in belongticker]
-                self.fiftyTwoWkLow = [i.fiftyTwoWkLow for i in belongticker]
-                self.high = [i.high for i in belongticker]
-                self.low = [i.low for i in belongticker]
-                self.name = [i.name for i in belongticker]
-                self.marketValue = [i.marketValue for i in belongticker]
-                self.vibrateRatio = [i.vibrateRatio for i in belongticker]
-                self.volume = [i.volume for i in belongticker]
-                self.turnoverRate = [i.turnoverRate for i in belongticker]
-                self.disSymbol = [i.disSymbol for i in belongticker]
-                self.option_change = [i.change for i in derivatives]
-                self.option_change_ratio = [i.changeRatio for i in derivatives]
-                self.option_close = [i.close for i in derivatives]
-                self.strike = [i.strikePrice for i in derivatives]
-                self.direction = [i.direction for i in derivatives]
-                self.option_symbol = [i.symbol for i in derivatives]
-                self.underlying_symbol = [i.unSymbol for i in derivatives]
-                self.cycle = [i.cycle for i in derivatives]
-                self.expiry = [i.expireDate for i in derivatives]
-                self.belong_ticker_id = [i.belongTickerId for i in derivatives]
-                self.attributes_dict = {
-                    "change": self.change,
-                    "changeRatio": self.changeRatio,
-                    "close": self.close,
-                    "symbol": self.symbol,
-                    "fiftyTwoWkHigh": self.fiftyTwoWkHigh,
-                    "fiftyTwoWkLow": self.fiftyTwoWkLow,
-                    "high": self.high,
-                    "low": self.low,
-                    "name": self.name,
-                    "marketValue": self.marketValue,
-                    "vibrateRatio": self.vibrateRatio,
-                    "volume": self.volume,
-                    "turnoverRate": self.turnoverRate,
-                    "disSymbol": self.disSymbol,
-                    "option_change": self.option_change,
-                    "option_change_ratio": self.option_change_ratio,
-                    "option_close": self.option_close,
-                    "strike": self.strike,
-                    "direction": self.direction,
-                    "option_symbol": self.option_symbol,
-                    "underlying_symbol": self.underlying_symbol,
-                    "cycle": self.cycle,
-                    "expiry": self.expiry,
-                    "belong_ticker_id": self.belong_ticker_id}
-
-                self.df = pd.DataFrame(self.attributes_dict)
-
-                return self.df, derivatives
-            
-
-    async def top_options_tickers(self, rank_type):
-        """Rank Types: totalVolume / totalPosition / """
-        url = f"https://quotes-gw.webullfintech.com/api/wlas/option/rank/list?regionId=6&rankType={rank_type}&pageIndex=1&pageSize=350"
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as response:
-                response = await response.json()
-                data = response.get('data', None)
-                values = [TickerValues.from_dict(data.get("values", {})) for data in data]
-                belongticker = [BelongTicker.from_dict(data.get("ticker", {})) for data in data]
-
-
-                
+            return await fetch(session, url)
 
-                return values, belongticker, values
+async def get_near_the_money_symbols(ticker,api_key, lower_strike, upper_strike, today_str):
 
-    async def fetch_ticker_id(self, keyword):
-        url = f"{self.base_url}search/pc/tickers?keyword={keyword}&regionId=6&pageIndex=1&pageSize=1"
+    url = f"https://api.polygon.io/v3/snapshot/options/{ticker}?strike_price.gte={lower_strike}&strike_price.lte={upper_strike}&expiration_date.gte={today_str}&expiration_date.lte={today_str}&limit=250&apiKey={api_key}"
+    async with aiohttp.ClientSession() as session:
+        return await fetch(session, url)
 
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as response:
-                r = await response.json()
-                data = r.get('data', None)
-                if data is not None:
-                    try:
-                        self.tickerId = data[0]['tickerId']
-                        self.symbol = data[0]['symbol']
-                    except IndexError:
-                        pass
-                else:
-                    pass
-                return self.tickerId, self.symbol
-            
+async def get_filtered_contracts(api_key, output):
+    url = f"https://api.polygon.io/v3/snapshot?ticker.any_of={output}&apiKey={api_key}"
+    async with aiohttp.ClientSession() as session:
+        return await fetch(session, url)
 
-    async def cost_distribution(self, ticker, start_date=thirty_days_ago_str, end_date=today_str):
-        async with aiohttp.ClientSession() as session:
-            tickerid, _ = await self.fetch_ticker_id(ticker)
-            url = f"https://quotes-gw.webullfintech.com/api/quotes/chip/query?tickerId={tickerid}&startDate={start_date}&endDate={end_date}"
-            headers = {'Content-Type': 'application/json'}
-            async with session.get(url,headers=headers) as response:
-                try:
-                    response_data = await response.json()
-                    print(await response.text())
-                    data = response_data['data']
-                    cost_distribution = [CostDistribution(item) for item in data]
-                    return cost_distribution
-                except ContentTypeError as e:
-                    print(f"Error: {e}\nResponse text: {await response.text()}")
-                    return None
 
+async def earnings_calendar_endpoint(ticker):
+    earnings_calendar = await webull.get_earnings_calendar(date_str=thirty_days_from_now_str)
+    
+    earnings_data = {
+        "earning_release_id": earnings_calendar[0].earning_release_id,
+        "eps": earnings_calendar[0].eps,
+        "eps_estimate": earnings_calendar[0].eps_estimate,
+        "is_live": earnings_calendar[0].is_live,
+        "last_release_date": earnings_calendar[0].last_release_date,
+        "publish_status": earnings_calendar[0].publish_status,
+        "qualifier": earnings_calendar[0].qualifier,
+        "quarter": earnings_calendar[0].quarter,
+        "release_date": earnings_calendar[0].release_date,
+        "region_id": earnings_calendar[0].region_id,
+        "year": earnings_calendar[0].year,
+        "ticker": earnings_calendar[0].ticker,
+        "ticker_id": earnings_calendar[0].ticker_id
+    }
+    
+    return earnings_data
 
+async def stock_data_endpoint(ticker):
+    stock_data = await webull.get_webull_stock_data(ticker)
+    if stock_data:
+        avg_10d_vol = stock_data.avg_10d_vol
+        avg_vol3m = stock_data.avg_vol3m
+        estimated_earnings = stock_data.estimated_earnings
+        fifty_high = stock_data.fifty_high
+        fifty_low = stock_data.fifty_low
+        last_earnings = stock_data.last_earnings
+        outstanding_shares = stock_data.outstanding_shares
+        web_change_ratio = round(float(stock_data.web_change_ratio)*100,2)
+        total_shares = stock_data.total_shares
+        web_exchange = stock_data.web_exchange
+        web_name = stock_data.web_name
+        web_stock_close = stock_data.web_stock_close
+        web_stock_high = stock_data.web_stock_high
+        web_stock_low = stock_data.web_stock_low
+        web_stock_open = stock_data.web_stock_open
+        web_stock_vol = float(stock_data.web_stock_vol)
+        web_symb = stock_data.web_symb
+        web_vibrate_ratio = stock_data.web_vibrate_ratio
+
+        data_dict = {
+            "Average 10 Day Volume": stock_data.avg_10d_vol,
+            "Average Volume 3 Months": stock_data.avg_vol3m,
+            "Estimated Earnings Data": stock_data.estimated_earnings,
+            "Fifty Two Week High": stock_data.fifty_high,
+            "Fifty Two Week Low": stock_data.fifty_low,
+            "Next Earnings": stock_data.last_earnings,
+            "Outstanding Shares": stock_data.outstanding_shares,
+            "Web Change Ratio": round(float(stock_data.web_change_ratio) * 100, 2),
+            "Total Shares": stock_data.total_shares,
+            "Exchange": stock_data.web_exchange,
+            "Company Name": stock_data.web_name,
+            "Stock Close": stock_data.web_stock_close,
+            "Stock High": stock_data.web_stock_high,
+            "Stock Low": stock_data.web_stock_low,
+            "Stock Open": stock_data.web_stock_open,
+            "Stock Volume": float(stock_data.web_stock_vol),
+            "Symbol": stock_data.web_symb,
+            "Vibrate Ratio": stock_data.web_vibrate_ratio
+        }
 
-    async def economic_events(self,from_date=today_str, to_date=ninety_days_from_now):
-        url = f"https://chartevents-reuters.tradingview.com/events?minImportance=1&from={from_date}&to={ninety_days}"
+        return data_dict
 
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as response:
-                response_data = await response.json()
-                events_data = response_data['result']
-
-                events = [Event(item) for item in events_data]
-
-                data = {
-                    "Actual": [event.actual if event.actual is not None else None for event in events],
-                    "Comment": [event.comment for event in events],
-                    "Country": [event.country for event in events],
-                    "Currency": [event.currency for event in events],
-                    "Date": [event.date for event in events],
-                    "Time": [event.time for event in events],
-                    "Forecast": [event.forecast if event.forecast is not None else None for event in events],
-                    "ID": [event.id for event in events],
-                    "Importance": [event.importance for event in events],
-                    "Indicator": [event.indicator for event in events],
-                    "Link": [event.link for event in events],
-                    "Period": [event.period for event in events],
-                    "Previous": [event.previous if event.previous is not None else None for event in events],
-                    "Scale": [event.scale for event in events],
-                    "Source": [event.source for event in events],
-                    "Title": [event.title for event in events],
-                    "Unit": [event.unit for event in events],
-                }
-                df = pd.DataFrame(data)
-                return df
 
 
-    async def get_etf_categories(self, type: str) -> Optional[List[ETFCommodity]]:
-            """
-            Retrieves a list of ETFs from the following types:
-            >>> commodity
-            >>> industry
-            >>> index
-            >>> other
-
-            Args:
-                type (str): The category type of ETFCommodity instances to retrieve. Must be one of "index", "industry", "commodity", or "other".
-
-            Returns:
-                Optional[List[ETFCommodity]]: A list of ETFCommodity instances containing ETF or commodity data. Returns None if an error occurs while fetching the data.
-            """
-            url = f"https://quotes-gw.webullfintech.com/api/wlas/etfinder/pcFinder?topNum=5&finderId=wlas.etfinder.{type}&nbboLevel=false"
-            async with aiohttp.ClientSession() as session:
-                async with session.get(url) as response:
-                    if response.status == 200:
-                        data = await response.json()
-
-                        tabs = data.get('tabs')
-                        ticker_tuples = [t.get('tickerTupleList') for t in tabs]
-                        if data:
-                            etfs = []
-                            for i, ticker_list in enumerate(ticker_tuples):
-                                for ticker_data in ticker_list:
-                                    etf = ETFCommodity(tabs[i], ticker_data)
-                                    etfs.append(etf)      
-                            return etfs
-                    else:
-                        print(f"Error fetching data: {response.status}")
-                        return None
+async def analyst_ratings_endpoint(ticker):
+    analysis_data = await webull.get_analysis_data(ticker)
+    if analysis_data is None:
+        return
+
+    buy = analysis_data.buy if analysis_data.buy is not None else "N/A"
+    hold = analysis_data.hold if analysis_data.hold is not None else "N/A"
+    overall_rating = analysis_data.rating if analysis_data.rating is not None else "N/A"
+    suggestion = analysis_data.rating_suggestion if analysis_data.rating_suggestion is not None else "N/A"
+    rating_totals = analysis_data.rating_totals if analysis_data.rating_totals is not None else "N/A"
+    sell = analysis_data.sell if analysis_data.sell is not None else "N/A"
+    strongbuy = analysis_data.strongbuy if analysis_data.strongbuy is not None else "N/A"
+    underperform = analysis_data.underperform if analysis_data.underperform is not None else "N/A"
+
+    data_dict = { 
+        'Strong Buy Ratings': strongbuy,
+        'Buy Ratings': buy,
+        'Hold Ratings': hold,
+        'Underperform Rating': underperform,
+        'Sell Rating': sell,
+        'Analyst Count': rating_totals,
+        'Suggestion': suggestion,
+        'Overall Rating': overall_rating
+    }
+
+    return data_dict
+async def institutional_holdings_endpoint(ticker):
+    institutionHoldings = await webull.get_institutional_holdings(ticker)
+    if institutionHoldings is None:
+        return
+
+    decreaseChange = float(institutionHoldings.institution_holding.decrease.holding_count_change) if institutionHoldings.institution_holding.decrease.holding_count_change is not None else "N/A"
+    decreasedShares = float(institutionHoldings.institution_holding.decrease.institutional_count) if institutionHoldings.institution_holding.decrease.institutional_count is not None else "N/A"
+    increaseChange = float(institutionHoldings.institution_holding.increase.holding_count_change) if institutionHoldings.institution_holding.increase.holding_count_change is not None else "N/A"
+    increasedShares = float(institutionHoldings.institution_holding.increase.institutional_count) if institutionHoldings.institution_holding.increase.institutional_count is not None else "N/A"
+    newChange = float(institutionHoldings.institution_holding.new_position.holding_count_change) if institutionHoldings.institution_holding.new_position.holding_count_change is not None else "N/A"
+    newShares = float(institutionHoldings.institution_holding.new_position.institutional_count) if institutionHoldings.institution_holding.new_position.institutional_count is not None else "N/A"
+    soldOutChange = float(institutionHoldings.institution_holding.sold_out.holding_count_change) if institutionHoldings.institution_holding.sold_out.holding_count_change is not None else "N/A"
+    soldOutShares = float(institutionHoldings.institution_holding.sold_out.institutional_count) if institutionHoldings.institution_holding.sold_out.institutional_count is not None else "N/A"
+    net_shares_changed = soldOutChange + newChange + increaseChange + decreaseChange
+    net_institution_change = newShares + soldOutShares + increasedShares + decreasedShares
+
+    stats = institutionHoldings.institution_holding.stat
+    totalHeldShares = stats.holding_count if stats.holding_count is not None else "N/A"
+    totalHeldSharesChange = stats.holding_count_change if stats.holding_count_change is not None else "N/A"
+    totalOwnershipRatioOfFloat = stats.holding_ratio if stats.holding_ratio is not None else "N/A"
+    totalOwnershipRatioOfFloatChange = stats.holding_ratio_change if stats.holding_ratio_change is not None else "N/A"
+    totalNumberOfInstitutions = float(stats.institutional_count) if stats.institutional_count is not None else "N/A"
+
+    data_dict = {
+        'decreaseChange': float(institutionHoldings.institution_holding.decrease.holding_count_change) if institutionHoldings.institution_holding.decrease.holding_count_change is not None else "N/A",
+        'decreasedShares': float(institutionHoldings.institution_holding.decrease.institutional_count) if institutionHoldings.institution_holding.decrease.institutional_count is not None else "N/A",
+        'increaseChange': float(institutionHoldings.institution_holding.increase.holding_count_change) if institutionHoldings.institution_holding.increase.holding_count_change is not None else "N/A",
+        'increasedShares': float(institutionHoldings.institution_holding.increase.institutional_count) if institutionHoldings.institution_holding.increase.institutional_count is not None else "N/A",
+        'newChange': float(institutionHoldings.institution_holding.new_position.holding_count_change) if institutionHoldings.institution_holding.new_position.holding_count_change is not None else "N/A",
+        'newShares': float(institutionHoldings.institution_holding.new_position.institutional_count) if institutionHoldings.institution_holding.new_position.institutional_count is not None else "N/A",
+        'soldOutChange': float(institutionHoldings.institution_holding.sold_out.holding_count_change) if institutionHoldings.institution_holding.sold_out.holding_count_change is not None else "N/A",
+        'soldOutShares': float(institutionHoldings.institution_holding.sold_out.institutional_count) if institutionHoldings.institution_holding.sold_out.institutional_count is not None else "N/A"
+    }
+
+    data_dict['net_shares_changed'] = data_dict['soldOutChange'] + data_dict['newChange'] + data_dict['increaseChange'] + data_dict['decreaseChange']
+    data_dict['net_institution_change'] = data_dict['newShares'] + data_dict['soldOutShares'] + data_dict['increasedShares'] + data_dict['decreasedShares']
+
+    stats = institutionHoldings.institution_holding.stat
+    data_dict['totalHeldShares'] = stats.holding_count if stats.holding_count is not None else "N/A"
+    data_dict['totalHeldSharesChange'] = stats.holding_count_change if stats.holding_count_change is not None else "N/A"
+    data_dict['totalOwnershipRatioOfFloat'] = stats.holding_ratio if stats.holding_ratio is not None else "N/A"
+    data_dict['totalOwnershipRatioOfFloatChange'] = stats.holding_ratio_change if stats.holding_ratio_change is not None else "N/A"
+    data_dict['totalNumberOfInstitutions'] = float(stats.institutional_count) if stats.institutional_count is not None else "N/A"
+
+
+    return data_dict
+
+
+async def short_interest_endpoint(ticker):
+    short_interest = await webull.get_short_interest(ticker)
+    if short_interest is None:
+        return
+
+    short_int = f"{float(short_interest.short_int[0]):,}" if short_interest.short_int[0] is not None else "N/A"
+    avg_vol = f"{float(short_interest.avg_volume[0]):,}" if short_interest.avg_volume[0] is not None else "N/A"
+    days_to_cover = short_interest.days_to_cover[0] if short_interest.days_to_cover[0] is not None else "N/A"
+    settlement = short_interest.settlement[0] if short_interest.settlement[0] is not None else "N/A"
+
+
+    data_dict = { 
+        'Short Interest': short_int,
+        'Average Volume': avg_vol,
+        'Days to Cover': days_to_cover,
+        'Settlement Date': settlement
+    }
+
+    return data_dict
+
+async def capital_flow_endpoint(ticker):
+    capitalFlow = await webull.capital_flow(ticker)
+    largeNet = capitalFlow.largenet if capitalFlow.largenet is not None else "N/A"
+    largeIn = capitalFlow.largein if capitalFlow.largein is not None else "N/A"
+    largeOut = capitalFlow.largeout if capitalFlow.largeout is not None else "N/A"
+
+    majorNet = capitalFlow.majornet if capitalFlow.majornet is not None else "N/A"
+    majorIn = capitalFlow.majorin if capitalFlow.majorin is not None else "N/A"
+    majorOut = capitalFlow.majorout if capitalFlow.majorout is not None else "N/A"
+    majorInRatio = capitalFlow.majorinratio if capitalFlow.majorinratio is not None else "N/A"
+    majorOutRatio = capitalFlow.majoroutratio if capitalFlow.majoroutratio is not None else "N/A"
+
+    smallNet = capitalFlow.smallnet if capitalFlow.smallnet is not None else "N/A"
+    smallIn = capitalFlow.smallin if capitalFlow.smallin is not None else "N/A"
+    smallOut = capitalFlow.smallout if capitalFlow.smallout is not None else "N/A"
+    smallInRatio = capitalFlow.smallinratio if capitalFlow.smallinratio is not None else "N/A"
+    smallOutRatio = capitalFlow.smalloutratio if capitalFlow.smalloutratio is not None else "N/A"
+
+    retailIn = capitalFlow.retailin if capitalFlow.retailin is not None else "N/A"
+    retailOutRatio = capitalFlow.retailoutratio if capitalFlow.retailoutratio is not None else "N/A"
+    retailInRatio = capitalFlow.retailinratio if capitalFlow.retailinratio is not None else "N/A"
+    retailOut = capitalFlow.retailout if capitalFlow.retailout is not None else "N/A"
+
+    mediumIn = capitalFlow.mediumin if capitalFlow.mediumin is not None else "N/A"
+    mediumOut = capitalFlow.mediumout if capitalFlow.mediumout is not None else "N/A"
+    mediumNet = capitalFlow.mediumnet if capitalFlow.mediumnet is not None else "N/A"
+    mediumInRatio = capitalFlow.mediuminratio if capitalFlow.mediuminratio is not None else "N/A"
+    mediumOutRatio = capitalFlow.mediumoutratio if capitalFlow.mediumoutratio is not None else "N/A"
+
+    superIn = capitalFlow.superin if capitalFlow.superin is not None else "N/A"
+    superOut = capitalFlow.superout if capitalFlow.superout is not None else "N/A"
+    superNet = capitalFlow.supernet if capitalFlow.supernet is not None else "N/A"
+
+    newLargeIn = capitalFlow.newlargein if capitalFlow.newlargein is not None else "N/A"
+    newLargeOut = capitalFlow.newlargeout if capitalFlow.newlargeout is not None else "N/A"
+    newLargeNet = capitalFlow.newlargenet if capitalFlow.newlargenet is not None else "N/A"
+    newLargeInRatio = capitalFlow.newlargeinratio if capitalFlow.newlargeinratio is not None else "N/A"
+    newLargeOutRatio = capitalFlow.newlargeoutratio if capitalFlow.newlargeoutratio is not None else "N/A"
+    capital_flow_dict = {
+        'largeNet': largeNet,
+        'largeIn': largeIn,
+        'largeOut': largeOut,
+        'majorNet': majorNet,
+        'majorIn': majorIn,
+        'majorOut': majorOut,
+        'majorInRatio': majorInRatio,
+        'majorOutRatio': majorOutRatio,
+        'smallNet': smallNet,
+        'smallIn': smallIn,
+        'smallOut': smallOut,
+        'smallInRatio': smallInRatio,
+        'smallOutRatio': smallOutRatio,
+        'retailIn': retailIn,
+        'retailOutRatio': retailOutRatio,
+        'retailInRatio': retailInRatio,
+        'retailOut': retailOut,
+        'mediumIn': mediumIn,
+        'mediumOut': mediumOut,
+        'mediumNet': mediumNet,
+        'mediumInRatio': mediumInRatio,
+        'mediumOutRatio': mediumOutRatio,
+        'superIn': superIn,
+        'superOut': superOut,
+        'superNet': superNet,
+        'newLargeIn': newLargeIn,
+        'newLargeOut': newLargeOut,
+        'newLargeNet': newLargeNet,
+        'newLargeInRatio': newLargeInRatio,
+        'newLargeOutRatio': newLargeOutRatio
+    }
+
+    return capital_flow_dict
+
+async def financial_ratios_endpoint(ticker):
+    balance_sheet = await webull.get_balancesheet(ticker)
+    fin_statement = await webull.get_financial_statement(ticker)
+    cash_flow = await webull.get_cash_flow(ticker)
+    
+    market_data = await webull.get_webull_stock_data(ticker)
+    price = market_data.web_stock_close
+    print(market_data.avg_10d_vol)
+
+    financial_ratios=    await webull.calculate_ratios(balance_sheet, 
+                                                    fin_statement, 
+                                                    cash_flow, price)
+    
+    return financial_ratios
 
-    async def get_earnings_calendar(self, date_str):
-        url = f"{self.base_url}bgw/explore/calendar/earnings?regionId=6&pageIndex=1&pageSize=50&startDate={date_str}"
-        async with aiohttp.ClientSession() as session:
-           
-            async with session.get(url) as response:
-                data = await response.json()
-                results = data['data']
-
-                earnings_calendars = [EarningsCalendar(result) for result in results]
-                return earnings_calendars
-            
-
-    async def get_balancesheet(self, ticker: str) -> List[BalanceSheet]:
-        """
-        Retrieves a list of BalanceSheet instances for a given stock ticker.
-
-        Args:
-            ticker (str): The ticker symbol of the stock to retrieve balance sheet statements for.
-
-        Returns:
-            List[BalanceSheet]: A list of BalanceSheet instances containing balance sheet statement data.
-        """
-        async with aiohttp.ClientSession() as session:
-            tickerid, _ = await self.fetch_ticker_id(ticker)
-            
-            async with session.get(f"https://quotes-gw.webullfintech.com/api/information/financial/balancesheet?tickerId={tickerid}&type=102&fiscalPeriod=1,2,3,4&limit=50") as response:
-                
-                if response.status == 200:
-                    r = await response.json()
-                    try:
-                        data = r['data']
-                        balance_sheets = [BalanceSheet(statement) for statement in data]
-                        return balance_sheets
-                    except KeyError:
-                        pass
 
+async def balance_sheet_endpoint(ticker):
+    balance_sheet = await webull.get_balancesheet(ticker)
+    if balance_sheet is None:
+        return None
 
+    try:
+        accounts_payable = [i.accountsPayable if i.accountsPayable is not None else "N/A" for i in balance_sheet]
+        accounts_receivable = [i.accountsReceTradeNet if i.accountsReceTradeNet is not None else "N/A" for i in balance_sheet]
+        accrued_expenses = [i.accruedExpenses if i.accruedExpenses is not None else "N/A" for i in balance_sheet]
+        accumulated_depreciation = [i.accumulatedDepreciationTotal if i.accumulatedDepreciationTotal is not None else "N/A" for i in balance_sheet]
+        additional_paid_in_capital = [i.additionalPaidInCapital if i.additionalPaidInCapital is not None else "N/A" for i in balance_sheet]
+        cash_and_short_term_investments = [i.cashAndShortTermInvest if i.cashAndShortTermInvest is not None else "N/A" for i in balance_sheet]
+        cash_equivalents = [i.cashEquivalents if i.cashEquivalents is not None else "N/A" for i in balance_sheet]
+        common_stock = [i.commonStock if i.commonStock is not None else "N/A" for i in balance_sheet]
+        current_port_of_long_term_debt = [i.currentPortofLTDebtCapitalLeases if i.currentPortofLTDebtCapitalLeases is not None else "N/A" for i in balance_sheet]
+        balance_sheet_end_date = [i.endDate if i.endDate is not None else "N/A" for i in balance_sheet]
+        balance_sheet_fiscal_period = [i.fiscalPeriod if i.fiscalPeriod is not None else "N/A" for i in balance_sheet]
+        balance_sheet_fiscal_year = [i.fiscalYear if i.fiscalYear is not None else "N/A" for i in balance_sheet]
+        long_term_debt = [i.longTermDebt if i.longTermDebt is not None else "N/A" for i in balance_sheet]
+        notes_payable_short_term_debt = [i.notesPayableShortTermDebt if i.notesPayableShortTermDebt is not None else "N/A" for i in balance_sheet]
+        other_current_assets = [i.otherCurrentAssetsTotal if i.otherCurrentAssetsTotal is not None else "N/A" for i in balance_sheet]
+        other_equity = [i.otherEquityTotal if i.otherEquityTotal is not None else "N/A" for i in balance_sheet]
+        other_liabilities = [i.otherLiabilitiesTotal if i.otherLiabilitiesTotal is not None else "N/A" for i in balance_sheet]
+        other_long_term_assets = [i.otherLongTermAssetsTotal if i.otherLongTermAssetsTotal is not None else "N/A" for i in balance_sheet]
+        ppe_total_gross = [i.ppeTotalGross if i.ppeTotalGross is not None else "N/A" for i in balance_sheet]
+        ppe_total_net = [i.ppeTotalNet if i.ppeTotalNet is not None else "N/A" for i in balance_sheet]
+        prepaid_expenses = [i.prepaidExpenses if i.prepaidExpenses is not None else "N/A" for i in balance_sheet]
+        balance_sheet_publish_date = [i.publishDate if i.publishDate is not None else "N/A" for i in balance_sheet]
+        retained_earnings = [i.retainedEarnings if i.retainedEarnings is not None else "N/A" for i in balance_sheet]
+        short_term_investments = [i.shortTermInvestments if i.shortTermInvestments is not None else "N/A" for i in balance_sheet]
+        total_assets = [i.totalAssets if i.totalAssets is not None else "N/A" for i in balance_sheet]
+        total_common_shares_outstanding = [i.totalCommonSharesOutstanding if i.totalCommonSharesOutstanding is not None else "N/A" for i in balance_sheet]
+        total_current_assets = [i.totalCurrentAssets if i.totalCurrentAssets is not None else "N/A" for i in balance_sheet]
+        total_current_liabilities = [i.totalCurrentLiabilities if i.totalCurrentLiabilities is not None else "N/A" for i in balance_sheet]
+        total_debt = [i.totalDebt if i.totalDebt is not None else "N/A" for i in balance_sheet]
+        total_equity = [i.totalEquity if i.totalEquity is not None else "N/A" for i in balance_sheet]
+        total_inventory = [i.totalInventory if i.totalInventory is not None else "N/A" for i in balance_sheet]
+        total_liabilities = [i.totalLiabilities if i.totalLiabilities is not None else "N/A" for i in balance_sheet]
+        total_liabilities_shareholders_equity = [i.totalLiabilitiesShareholdersEquity if i.totalLiabilitiesShareholdersEquity is not None else "N/A" for i in balance_sheet]
+        total_long_term_debt = [i.totalLongTermDebt if i.totalLongTermDebt is not None else "N/A" for i in balance_sheet]
+        total_non_current_assets = [i.totalNonCurrentAssets if i.totalNonCurrentAssets is not None else "N/A" for i in balance_sheet]
+        total_non_current_liabilities = [i.totalNonCurrentLiabilities if i.totalNonCurrentLiabilities is not None else "N/A" for i in balance_sheet]
+        total_receivables_net = [i.totalReceivablesNet if i.totalReceivablesNet is not None else "N/A" for i in balance_sheet]
+        total_stockholders_equity = [i.totalStockhodersEquity if i.totalStockhodersEquity is not None else "N/A" for i in balance_sheet]
+        balance_sheet_type = [i.type if i.type is not None else "N/A" for i in balance_sheet]
+    except Exception as e:
+        print(f"Failed to get balance sheet data for {ticker}: {e}")
+        return None
 
-    async def get_financial_statement(self, ticker: str) -> List[FinancialStatement]:
 
-        """
-        Retrieves a list of FinancialStatement instances for a given stock ticker.
 
-        Args:
-            ticker (str): The ticker symbol of the stock to retrieve financial statements for.
+    balance_sheet_data = {}
 
-        Returns:
-            List[FinancialStatement]: A list of FinancialStatement instances containing financial statement data.
-        """
-        async with aiohttp.ClientSession() as session:
-            tickerid, _ = await self.fetch_ticker_id(ticker)
-            async with session.get(f"https://quotes-gw.webullfintech.com/api/information/financial/incomestatement?tickerId={tickerid}&type=102&fiscalPeriod=1,2,3,4&limit=11") as resp:
-                if resp.status == 200:
-                    r = await resp.json()
-                    try:
-                        data = r['data']
-                        financial_statements = [FinancialStatement(statement) for statement in data]
-                        return financial_statements
-                    except KeyError:
-                        pass
-
-    async def get_cash_flow(self, ticker):
-        """
-        Retrieves a list of CashFlow instances for a given stock ticker.
-
-        Args:
-            ticker (str): The ticker symbol of the stock to retrieve cash flow statements for.
-
-        Returns:
-            List[CashFlow]: A list of CashFlow instances containing cash flow statement data.
-        """
-        async with aiohttp.ClientSession() as session:
-            tickerid, _ = await self.fetch_ticker_id(ticker)
-            async with session.get(f"https://quotes-gw.webullfintech.com/api/information/financial/cashflow?tickerId={tickerid}&type=102&fiscalPeriod=1,2,3,4&limit=11") as resp:
-                if resp.status == 200:
-                    r = await resp.json()
-                    try:
-                        data = r['data']
-                        financial_statements = [CashFlow(statement) for statement in data]
-                        return financial_statements
-                    except KeyError:
-                        pass
-
-
-    async def get_short_interest(self, ticker):
-        """
-        Get the short interest data for a given ticker ID.
-
-        Args:
-            ticker_id (int): The unique identifier for the stock ticker.
-
-        Returns:
-            ShortInterest: An instance of the ShortInterest class containing short interest data in the form of a List, or None if an error occurs.
-        """
-        async with aiohttp.ClientSession() as session:
-            tickerid, _ = await self.fetch_ticker_id(ticker)
-            async with session.get(f"https://quotes-gw.webullfintech.com/api/information/brief/shortInterest?tickerId={tickerid}") as resp:
-                if resp.status != 200:
-                    return None
-                data = await resp.json()
-                short_interest = ShortInterest(data)
-                return short_interest
-
-
-    async def get_institutional_holdings(self, ticker):
-        """
-        Retrieves institutional holdings for a given ticker.
-
-        Args:
-            ticker (str): The ticker symbol to retrieve holdings for.
-
-        Returns:
-            InstitutionHolding: An object representing the institutional holdings for the given ticker.
-        """
-        async with aiohttp.ClientSession() as session:
-            tickerid, symbol = await self.fetch_ticker_id(ticker)
-            async with session.get(f"https://quotes-gw.webullfintech.com/api/information/stock/getInstitutionalHolding?tickerId={tickerid}") as resp:
-                if resp.status == 200:
-                    r = await resp.json()
-                    try:
-                        holdings = InstitutionHolding(r)
-                        return holdings
-                    except KeyError:
-                        print("Error parsing response")
-                        return None
-                    
+    for i in range(len(balance_sheet)):
+        publish_date = balance_sheet_publish_date[i]
+        year = balance_sheet_fiscal_year[i]
+        sheet_data = {
+            'Year': year,
+            'Accounts Payable': accounts_payable[i],
+            'Accounts Receivable': accounts_receivable[i],
+            'Accrued Expenses': accrued_expenses[i],
+            'Accumulated Depreciation': accumulated_depreciation[i],
+            'Additional Paid-in Capital': additional_paid_in_capital[i],
+            'Cash and Short-Term Investments': cash_and_short_term_investments[i],
+            'Cash Equivalents': cash_equivalents[i],
+            'Common Stock': common_stock[i],
+            'Current Portion of Long-Term Debt': current_port_of_long_term_debt[i],
+            'Balance Sheet End Date': balance_sheet_end_date[i],
+            'Long-Term Debt': long_term_debt[i],
+            'Notes Payable/Short-Term Debt': notes_payable_short_term_debt[i],
+            'Other Current Assets': other_current_assets[i],
+            'Other Equity': other_equity[i],
+            'Other Liabilities': other_liabilities[i],
+            'Other Long-Term Assets': other_long_term_assets[i],
+            'PPE Total Gross': ppe_total_gross[i],
+            'PPE Total Net': ppe_total_net[i],
+            'Prepaid Expenses': prepaid_expenses[i],
+            'Retained Earnings': retained_earnings[i],
+            'Short-Term Investments': short_term_investments[i],
+            'Total Assets': total_assets[i],
+            'Total Common Shares Outstanding': total_common_shares_outstanding[i],
+            'Total Current Assets': total_current_assets[i],
+            'Total Current Liabilities': total_current_liabilities[i],
+            'Total Debt': total_debt[i],
+            'Total Equity': total_equity[i],
+            'Total Inventory': total_inventory[i],
+            'Total Liabilities': total_liabilities[i],
+            'Total Liabilities & Shareholders Equity': total_liabilities_shareholders_equity[i],
+            'Total Long-Term Debt': total_long_term_debt[i],
+            'Total Non-Current Assets': total_non_current_assets[i],
+            'Total Non-Current Liabilities': total_non_current_liabilities[i],
+            'Total Receivables Net': total_receivables_net[i],
+            'Total Stockholders Equity': total_stockholders_equity[i],
+            'Balance Sheet Type': balance_sheet_type[i]
+        }
 
+        if publish_date not in balance_sheet_data:
+            balance_sheet_data[publish_date] = []
         
-
-    async def capital_flow(self, ticker):
-        async with aiohttp.ClientSession() as session:
-            tickerid, _ = await self.fetch_ticker_id(ticker)
-            async with session.get(f"https://quotes-gw.webullfintech.com/api/stock/capitalflow/ticker?tickerId={tickerid}&showHis=true") as response:
-                r = await response.json()
-                latest = r['latest']
-                if latest is not None:
-                    item = item = latest['item']
-                    if item is not None:
-                        return CapitalFlow(item)
-
+        balance_sheet_data[publish_date].append(sheet_data)
 
 
+        return balance_sheet_data
 
+async def cash_flow_endpoint(ticker):
+    cash_flow = await webull.get_cash_flow(ticker)
+    if cash_flow is None:
+        return
+
+    capital_expenditures = [i.capital_expenditures if i.capital_expenditures is not None else "N/A" for i in cash_flow]
+    cash_from_financing_activities = [i.cash_from_financing_activities if i.cash_from_financing_activities is not None else "N/A" for i in cash_flow]
+    cash_from_investing_activities = [i.cash_from_investing_activities if i.cash_from_investing_activities is not None else "N/A" for i in cash_flow]
+    cash_from_operating_activities = [i.cash_from_operating_activities if i.cash_from_operating_activities is not None else "N/A" for i in cash_flow]
+    changes_in_working_capital = [i.changes_in_working_capital if i.changes_in_working_capital is not None else "N/A" for i in cash_flow]
+    deferred_taxes = [i.deferred_taxes if i.deferred_taxes is not None else "N/A" for i in cash_flow]
+    depreciation_and_amortization = [i.depreciation_and_amortization if i.depreciation_and_amortization is not None else "N/A" for i in cash_flow]
+    cashflow_end_date = [i.end_date if i.end_date is not None else "N/A" for i in cash_flow]
+    financing_cashflow_items = [i.financing_cashflow_items if i.financing_cashflow_items is not None else "N/A" for i in cash_flow]
+    cashflow_fiscal_period = [i.fiscal_period if i.fiscal_period is not None else "N/A" for i in cash_flow]
+    cashflow_fiscal_year = [i.fiscal_year if i.fiscal_year is not None else "N/A" for i in cash_flow]
+    foreign_exchange_effects = [i.foreign_exchange_effects if i.foreign_exchange_effects is not None else "N/A" for i in cash_flow]
+    issuance_retirement_of_debt_net = [i.issuance_retirement_of_debt_net if i.issuance_retirement_of_debt_net is not None else "N/A" for i in cash_flow]
+    issuance_retirement_of_stock_net = [i.issuance_retirement_of_stock_net if i.issuance_retirement_of_stock_net is not None else "N/A" for i in cash_flow]
+    net_change_in_cash = [i.net_change_in_cash if i.net_change_in_cash is not None else "N/A" for i in cash_flow]
+    net_income = [i.net_income if i.net_income is not None else "N/A" for i in cash_flow]
+    non_cash_items = [i.non_cash_items if i.non_cash_items is not None else "N/A" for i in cash_flow]
+    other_investing_cashflow_items_total = [i.other_investing_cashflow_items_total if i.other_investing_cashflow_items_total is not None else "N/A" for i in cash_flow]
+    cashflow_publish_date = [i.publish_date if i.publish_date is not None else "N/A" for i in cash_flow]
+    total_cash_dividends_paid = [i.total_cash_dividends_paid if i.total_cash_dividends_paid is not None else "N/A" for i in cash_flow]
+    cashflow_type = [i.type if i.type is not None else "N/A" for i in cash_flow]
+
+    cash_flow_data = {}
+
+    for i in range(len(cash_flow)):
+        publish_date = cashflow_publish_date[i]
+        year = cashflow_fiscal_year[i]
+        statement_data = {
+            'Year': year,
+            'Capital Expenditures': capital_expenditures[i],
+            'Cash from Financing Activities': cash_from_financing_activities[i],
+            'Cash from Investing Activities': cash_from_investing_activities[i],
+            'Cash from Operating Activities': cash_from_operating_activities[i],
+            'Changes in Working Capital': changes_in_working_capital[i],
+            'Deferred Taxes': deferred_taxes[i],
+            'Depreciation and Amortization': depreciation_and_amortization[i],
+            'Cash Flow End Date': cashflow_end_date[i],
+            'Financing Cash Flow Items': financing_cashflow_items[i],
+            'Foreign Exchange Effects': foreign_exchange_effects[i],
+            'Issuance/Retirement of Debt (Net)': issuance_retirement_of_debt_net[i],
+            'Issuance/Retirement of Stock (Net)': issuance_retirement_of_stock_net[i],
+            'Net Change in Cash': net_change_in_cash[i],
+            'Net Income': net_income[i],
+            'Non-Cash Items': non_cash_items[i],
+            'Other Investing Cash Flow Items (Total)': other_investing_cashflow_items_total[i],
+            'Cash Flow Publish Date': cashflow_publish_date[i],
+            'Total Cash Dividends Paid': total_cash_dividends_paid[i],
+            'Cash Flow Type': cashflow_type[i]
+        }
 
-    async def get_webull_stock_data(self, ticker):
-        """Fetches and returns a `WebullStockData` object containing stock data for the specified ticker symbol.
-
-        Args:
-            ticker (str): The ticker symbol of the stock to fetch data for.
-
-        Returns:
-            A `WebullStockData` object containing the following attributes:
-            >>> web_name (str): The name of the stock.
-            >>> web_symb (str): The ticker symbol of the stock.
-            >>> web_exchange (str): The stock exchange the stock is traded on.
-            >>> web_stock_close (float): The most recent closing price of the stock.
-            >>> last_earnings (str): The date of the company's last earnings report.
-            >>> web_stock_vol (float): The current volume of shares traded.
-            >>> web_change_ratio (float): The change in price of the stock as a percentage.
-            >>> web_stock_open (float): The opening price of the stock for the current trading day.
-            >>> web_stock_high (float): The highest price the stock has reached during the current trading day.
-            >>> web_stock_low (float): The lowest price the stock has reached during the current trading day.
-            >>> fifty_high (float): The highest price the stock has reached in the past 52 weeks.
-            >>> avg_vol3m (float): The average volume of shares traded over the past 3 months.
-            >>> fifty_low (float): The lowest price the stock has reached in the past 52 weeks.
-            >>> avg_10d_vol (float): The average volume of shares traded over the past 10 days.
-            >>> outstanding_shares (float): The number of outstanding shares of the stock.
-            >>> total_shares (float): The total number of shares of the stock.
-            >>> estimated_earnings (str): The date of the company's next earnings report (if available).
-            >>> web_vibrate_ratio (float): The volatility of the stock.
-        """
-
-        tickerid, _ = await self.fetch_ticker_id(ticker)
-        webull_stock_data = WebullStockData(tickerid)
-
-
-        return webull_stock_data
-
-
-
-    async def get_analysis_data(self, ticker):
-        try:
-            async with aiohttp.ClientSession() as session:
-                tickerid, _ = await self.fetch_ticker_id(ticker)
-                async with session.get(f"https://quotes-gw.webullfintech.com/api/information/securities/analysis?tickerId={tickerid}") as resp:
-                    if resp.status == 200:
-                        r = await resp.json()
-                    else:
-                        return None
-
-                    # Store the fetched analysis data in the cache
-                    analysis_data = Analysis(tickerid)
-
-                    return analysis_data
-
-        except Exception as e:
-            print(f"Error getting analysis data for ticker {ticker}: {e}")
-            return None
         
-
-    async def get_webull_vol_analysis_data(self, ticker):
-            tickerid, _ = await self.fetch_ticker_id(ticker)
-            # If the ticker WebullVolAnalysis data is not in the cache or has expired, fetch it
-            webull_vol_analysis_data = WebullVolAnalysis(tickerid)
-            
-        # Store the fetched WebullVolAnalysis data in the cache
-
-
-            return webull_vol_analysis_data
-
-
-    async def calculate_score(self,
-        capital_expenditures,
-        cash_from_financing_activities,
-        cash_from_investing_activities,
-        cash_from_operating_activities,
-        net_change_in_cash,
-        net_income,
-        total_cash_dividends_paid
-    ):
-        score = 0
+        if publish_date not in cash_flow_data:
+            cash_flow_data[publish_date] = []
         
-        if cash_from_operating_activities is not None and float(cash_from_operating_activities) > 0:
-            score += 2
+        cash_flow_data[publish_date].append(statement_data)
 
-        if net_income is not None and cash_from_operating_activities is not None and float(cash_from_operating_activities) / float(net_income) > 1.2:
-            score += 1
+        return cash_flow_data
 
-        if capital_expenditures is not None and cash_from_operating_activities is not None and float(cash_from_operating_activities) > 0 and float(capital_expenditures) / float(cash_from_operating_activities) < 0.5:
-            score += 1
+async def financial_statement_endpoint(ticker):
+    financial_statement = await webull.get_financial_statement(ticker)
+    if financial_statement is None:
+        return None
 
-        if net_change_in_cash is not None and float(net_change_in_cash) > 0:
-            score += 1
-
-        if total_cash_dividends_paid is not None and net_income is not None and float(total_cash_dividends_paid) / float(net_income) < 0.5:
-            score += 1
-
-        if cash_from_financing_activities is not None and net_income is not None and float(net_income) != 0 and float(cash_from_financing_activities) / float(net_income) < 0:
-            score += 1
-
-        return {
-            "capital_expenditures": capital_expenditures,
-            "cash_from_financing_activities": cash_from_financing_activities,
-            "cash_from_investing_activities": cash_from_investing_activities,
-            "cash_from_operating_activities": cash_from_operating_activities,
-            "net_change_in_cash": net_change_in_cash,
-            "net_income": net_income,
-            "total_cash_dividends_paid": total_cash_dividends_paid,
-            "score": score
+    cost_of_revenue_total = [i.cost_of_revenue_total if i.cost_of_revenue_total is not None else "N/A" for i in financial_statement]
+    depreciation_and_amortization = [i.depreciation_and_amortization if i.depreciation_and_amortization is not None else "N/A" for i in financial_statement]
+    diluted_eps_excl_extra_items = [i.diluted_eps_excl_extra_items if i.diluted_eps_excl_extra_items is not None else "N/A" for i in financial_statement]
+    diluted_eps_incl_extra_items = [i.diluted_eps_incl_extra_items if i.diluted_eps_incl_extra_items is not None else "N/A" for i in financial_statement]
+    diluted_net_income = [i.diluted_net_income if i.diluted_net_income is not None else "N/A" for i in financial_statement]
+    diluted_normalized_eps = [i.diluted_normalized_eps if i.diluted_normalized_eps is not None else "N/A" for i in financial_statement]
+    diluted_weighted_average_shares = [i.diluted_weighted_average_shares if i.diluted_weighted_average_shares is not None else "N/A" for i in financial_statement]
+    earning_after_tax = [i.earning_after_tax if i.earning_after_tax is not None else "N/A" for i in financial_statement]
+    earning_before_tax = [i.earning_before_tax if i.earning_before_tax is not None else "N/A" for i in financial_statement]
+    end_date = [i.end_date if i.end_date is not None else "N/A" for i in financial_statement]
+    fiscal_period = [i.fiscal_period if i.fiscal_period is not None else "N/A" for i in financial_statement]
+    fiscal_year = [i.fiscal_year if i.fiscal_year is not None else "N/A" for i in financial_statement]
+    gross_profit = [i.gross_profit if i.gross_profit is not None else "N/A" for i in financial_statement]
+    income_avaito_com_excl_extra_ord = [i.income_avaito_com_excl_extra_ord if i.income_avaito_com_excl_extra_ord is not None else "N/A" for i in financial_statement]
+    income_avaito_com_incl_extra_ord = [i.income_avaito_com_incl_extra_ord if i.income_avaito_com_incl_extra_ord is not None else "N/A" for i in financial_statement]
+    income_tax = [i.income_tax if i.income_tax is not None else "N/A" for i in financial_statement]
+    inter_expse_inc_net_oper = [i.inter_expse_inc_net_oper if i.inter_expse_inc_net_oper is not None else "N/A" for i in financial_statement]
+    inter_inc_expse_net_non_oper = [i.inter_inc_expse_net_non_oper if i.inter_inc_expse_net_non_oper is not None else "N/A" for i in financial_statement]
+    net_income = [i.net_income if i.net_income is not None else "N/A" for i in financial_statement]
+    net_income_after_tax = [i.net_income_after_tax if i.net_income_after_tax is not None else "N/A" for i in financial_statement]
+    net_income_before_extra = [i.net_income_before_extra if i.net_income_before_extra is not None else "N/A" for i in financial_statement]
+    net_income_before_tax = [i.net_income_before_tax if i.net_income_before_tax is not None else "N/A" for i in financial_statement]
+    operating_expense = [i.operating_expense if i.operating_expense is not None else "N/A" for i in financial_statement]
+    operating_income = [i.operating_income if i.operating_income is not None else "N/A" for i in financial_statement]
+    operating_profit = [i.operating_profit if i.operating_profit is not None else "N/A" for i in financial_statement]
+    publish_date = [i.publish_date if i.publish_date is not None else "N/A" for i in financial_statement]
+    revenue = [i.revenue if i.revenue is not None else "N/A" for i in financial_statement]
+    sell_gen_admin_expenses = [i.sell_gen_admin_expenses if i.sell_gen_admin_expenses is not None else "N/A" for i in financial_statement]
+    total_extraordinary_items = [i.total_extraordinary_items if i.total_extraordinary_items is not None else "N/A" for i in financial_statement]
+    total_revenue = [i.total_revenue if i.total_revenue is not None else "N/A" for i in financial_statement]
+    type = [i.type if i.type is not None else "N/A" for i in financial_statement]
+    unusual_expense_income = [i.unusual_expense_income if i.unusual_expense_income is not None else "N/A" for i in financial_statement]
+
+    financial_statement_data = {}
+
+    for i in range(len(financial_statement)):
+        fin_publish_date = publish_date[i]
+        year = fiscal_year[i]
+        statement_data = {
+            'Year': year,
+            'Cost of Revenue Total': cost_of_revenue_total[i],
+            'Depreciation and Amortization': depreciation_and_amortization[i],
+            'Diluted EPS (Excl. Extra Items)': diluted_eps_excl_extra_items[i],
+            'Diluted EPS (Incl. Extra Items)': diluted_eps_incl_extra_items[i],
+            'Diluted Net Income': diluted_net_income[i],
+            'Diluted Normalized EPS': diluted_normalized_eps[i],
+            'Diluted Weighted Average Shares': diluted_weighted_average_shares[i],
+            'Earnings (After Tax)': earning_after_tax[i],
+            'Earnings (Before Tax)': earning_before_tax[i],
+            'Gross Profit': gross_profit[i],
+            'Income Avail. to Common (Excl. Extraordinary Items)': income_avaito_com_excl_extra_ord[i],
+            'Income Avail. to Common (Incl. Extraordinary Items)': income_avaito_com_incl_extra_ord[i],
+            'Income Tax': income_tax[i],
+            'Interest Expense/Income (Net) - Operating': inter_expse_inc_net_oper[i],
+            'Interest Income/Expense (Net) - Non-operating': inter_inc_expse_net_non_oper[i],
+            'Net Income': net_income[i],
+            'Net Income (After Tax)': net_income_after_tax[i],
+            'Net Income (Before Extraordinary Items)': net_income_before_extra[i],
+            'Net Income (Before Tax)': net_income_before_tax[i],
+            'Operating Expense': operating_expense[i],
+            'Operating Income': operating_income[i],
+            'Operating Profit': operating_profit[i],
+            'Revenue': revenue[i],
+            'Selling, General, and Admin. Expenses': sell_gen_admin_expenses[i],
+            'Total Extraordinary Items': total_extraordinary_items[i],
+            'Total Revenue': total_revenue[i],
+            'Type': type[i],
+            'Unusual Expense/Income': unusual_expense_income[i]
         }
-    async def financial_score(self, ticker):
-        score = 0
-        ticker_id, _ = await self.fetch_ticker_id(ticker)
-
-        marketprice = await self.get_webull_stock_data(ticker_id)
-        market_price = marketprice.web_stock_close
-        balance_sheet = await self.get_balancesheet(ticker_id)
-        cashflow = await self.get_cash_flow(ticker_id)
-        fin_statement = await self.get_financial_statement(ticker_id)
-
-        # Calculate financial ratios and metrics
-        ratios = await self.calculate_ratios(balance_sheet, fin_statement, cashflow, market_price)
-        if ratios is not None:
-        # Scoring based on the calculated ratios and metrics
-            if ratios['current_ratio'] is not None and ratios['current_ratio'] > 2:
-                score += 1
-            if ratios['quick_ratio'] is not None and ratios['quick_ratio'] > 1:
-                score += 1
-            if ratios['debt_to_equity_ratio'] is not None and ratios['debt_to_equity_ratio'] < 0.5:
-                score += 2
-            if ratios['return_on_assets'] is not None and ratios['return_on_assets'] > 0.05:
-                score += 2
-            if ratios['return_on_equity'] is not None and ratios['return_on_equity'] > 0.15:
-                score += 3
-            if ratios['gross_profit_margin'] is not None and ratios['gross_profit_margin'] > 0.4:
-                score += 2
-            if ratios['operating_margin'] is not None and ratios['operating_margin'] > 0.1:
-                score += 2
-            if ratios['net_profit_margin'] is not None and ratios['net_profit_margin'] > 0.05:
-                score += 3
-            if ratios['dividend_payout_ratio'] is not None and 0.3 <= ratios['dividend_payout_ratio'] <= 0.6:
-                score += 1
-            if ratios['revenue_growth'] is not None and ratios['revenue_growth'] > 0.1:
-                score += 2
-            if ratios['total_asset_turnover'] is not None and ratios['total_asset_turnover'] > 0.7:
-                score += 1
-            if ratios['inventory_turnover'] is not None and ratios['inventory_turnover'] > 6:
-                score += 1
-            if ratios['days_sales_outstanding'] is not None and ratios['days_sales_outstanding'] < 45:
-                score += 1
-            if ratios['debt_ratio'] is not None and ratios['debt_ratio'] < 0.5:
-                score += 2
-            if ratios['interest_coverage'] is not None and ratios['interest_coverage'] > 3:
-                score += 1
-            for k, v in ratios.items():
-                score_threshold = thresholds.get('score')
-                if k == 'score':
-                    if score_threshold is None:
-                        check = ":white_check_mark:"
-                    elif isinstance(score_threshold, tuple) and isinstance(v, float) and score_threshold[0] <= v <= score_threshold[1]:
-                        check = ":white_check_mark:"
-                    elif isinstance(score_threshold, (int, float)) and isinstance(v, float) and float(v) >= score_threshold:
-                        check = ":white_check_mark:"
-                    else:
-                        check = ":x:"
-                else:
-                    check = ":white_check_mark:" if isinstance(v, float) and thresholds.get(k) and isinstance(thresholds[k], tuple) and thresholds[k][0] <= v <= thresholds[k][1] or isinstance(thresholds.get(k), (int, float)) and (isinstance(v, float) and thresholds.get(k) is not None and float(v) >= thresholds[k] or not isinstance(v, float) and thresholds.get(k, 0) == 0) else ":x:"
-
-                return {**ratios, 'score': score}
-
-    async def calculate_ratios(self, balance_sheet, fin_statement, cashflow, market_price):
-        ratios = {}
+        if fin_publish_date not in financial_statement_data:
+            financial_statement_data[fin_publish_date] = []
         
-        # Check if fin_statement and balance_sheet are not empty
-        if fin_statement and balance_sheet:
-            if balance_sheet and balance_sheet[0].totalCurrentAssets is not None and balance_sheet[0].totalCurrentLiabilities is not None and float(balance_sheet[0].totalCurrentLiabilities) > 0 and float(balance_sheet[0].totalCurrentAssets) > 0:
-                current_ratio = float(balance_sheet[0].totalCurrentAssets) / float(balance_sheet[0].totalCurrentLiabilities)
-            else:
-                current_ratio = None
-
-            if balance_sheet[0].totalCurrentAssets is not None and balance_sheet[0].totalInventory is not None and balance_sheet[0].totalCurrentLiabilities is not None:
-                quick_ratio = (float(balance_sheet[0].totalCurrentAssets) - float(balance_sheet[0].totalInventory)) / float(balance_sheet[0].totalCurrentLiabilities)
-            else:
-                quick_ratio = None
-
-            if balance_sheet[0].totalDebt is not None and balance_sheet[0].totalEquity is not None:
-                debt_to_equity_ratio = float(balance_sheet[0].totalDebt) / float(balance_sheet[0].totalEquity)
-            else:
-                debt_to_equity_ratio = None
-
-            if fin_statement[0].net_income is not None and balance_sheet[0].totalAssets is not None:
-                if float(balance_sheet[0].totalAssets) != 0:
-                    return_on_assets = float(fin_statement[0].net_income) / float(balance_sheet[0].totalAssets)
-                else:
-                    return_on_assets = None  # or any appropriate value to represent the case when total assets are zero
-            else:
-                return_on_assets = None
-
-            if fin_statement[0].net_income is not None and balance_sheet[0].totalEquity is not None:
-                return_on_equity = float(fin_statement[0].net_income) / float(balance_sheet[0].totalEquity)
-            else:
-                return_on_equity = None
-
-            if fin_statement[0].total_revenue is not None and fin_statement[0].cost_of_revenue_total is not None and float(fin_statement[0].total_revenue) > 0:
-                gross_profit_margin = (float(fin_statement[0].total_revenue) - float(fin_statement[0].cost_of_revenue_total)) / float(fin_statement[0].total_revenue)
-            else:
-                gross_profit_margin = None
-
-            if fin_statement[0].total_revenue is not None and float(fin_statement[0].total_revenue) > 0:
-                if fin_statement[0].operating_income is not None:
-                    operating_margin = float(fin_statement[0].operating_income) / float(fin_statement[0].total_revenue)
-                else:
-                    operating_margin = None
-            else:
-                operating_margin = None
-
-            if fin_statement[0].total_revenue is not None and fin_statement[0].net_income is not None and float(fin_statement[0].total_revenue) > 0:
-                net_profit_margin = float(fin_statement[0].net_income) / float(fin_statement[0].total_revenue)
-            else:
-                net_profit_margin = None
-
-            if cashflow and cashflow[0].total_cash_dividends_paid is not None and fin_statement[0].net_income is not None and float(fin_statement[0].net_income) > 0:
-                dividend_payout_ratio = float(cashflow[0].total_cash_dividends_paid) / float(fin_statement[0].net_income)
-            else:
-                dividend_payout_ratio = None
-
-
-            try:
-                if cashflow is not None and cashflow[0].total_cash_dividends_paid is not None and fin_statement[0].net_income is not None and float(fin_statement[0].net_income) > 0:
-                    dividend_payout_ratio = float(cashflow[0].total_cash_dividends_paid) / float(fin_statement[0].net_income)
-                else:
-                    dividend_payout_ratio = None
-            except IndexError:
-                # Handle the index error here
-                dividend_payout_ratio = None
-
-            # Revenue Growth - You will need data from the previous year's financial statement
-
-            if len(fin_statement) > 1 and fin_statement[1].total_revenue is not None and float(fin_statement[1].total_revenue) > 0:
-                revenue_growth = (float(fin_statement[0].total_revenue) - float(fin_statement[1].total_revenue)) / float(fin_statement[1].total_revenue)
-            else:
-                revenue_growth = None
-                            
-            if fin_statement[0].total_revenue is not None and balance_sheet[0].totalAssets is not None and float(balance_sheet[0].totalAssets) > 0 and float(fin_statement[0].total_revenue) > 0:
-                total_asset_turnover = float(fin_statement[0].total_revenue) / float(balance_sheet[0].totalAssets)
-            else:
-                total_asset_turnover = None
-
-            # Inventory Turnover
-            try:
-                if fin_statement[0].cost_of_revenue_total is not None and fin_statement[0].cost_of_revenue_total != 0 and balance_sheet[0].totalInventory is not None and balance_sheet[0].totalInventory != 0:
-                    inventory_turnover = float(fin_statement[0].cost_of_revenue_total) / float(balance_sheet[0].totalInventory)
-                else:
-                    inventory_turnover = None
-            except ZeroDivisionError:
-                inventory_turnover = None
-
-                        # Days Sales Outstanding (DSO)
-            if fin_statement[0].total_revenue is not None and fin_statement[0].total_revenue != 0 and balance_sheet[0].totalReceivablesNet is not None and balance_sheet[0].totalReceivablesNet != 0 and float(fin_statement[0].total_revenue) != 0:
-                days_sales_outstanding = (float(balance_sheet[0].totalReceivablesNet) / float(fin_statement[0].total_revenue)) * 365
-            else:
-                days_sales_outstanding = None
-            # Debt Ratio
-            if balance_sheet[0].totalDebt is not None and balance_sheet[0].totalAssets is not None and float(balance_sheet[0].totalDebt) > 0 and float(balance_sheet[0].totalAssets) > 0:
-                debt_ratio = float(balance_sheet[0].totalDebt) / float(balance_sheet[0].totalAssets)
-            else:
-                debt_ratio = None
-
-            # Interest Coverage Ratio
-            if fin_statement[0].operating_income is not None and fin_statement[0].inter_expse_inc_net_oper is not None and float(fin_statement[0].inter_expse_inc_net_oper) > 0 and float(fin_statement[0].operating_income) > 0:
-                interest_coverage = float(fin_statement[0].operating_income) / float(fin_statement[0].inter_expse_inc_net_oper)
-            else:
-                interest_coverage = None
-
-            if fin_statement[0].diluted_eps_excl_extra_items is not None and market_price is not None and float(fin_statement[0].diluted_eps_excl_extra_items) > 0:
-                price_to_earnings_ratio = float(market_price) / float(fin_statement[0].diluted_eps_excl_extra_items)
-            else:
-                price_to_earnings_ratio = None
-
-            if (fin_statement[0].total_revenue is not None and 
-                balance_sheet[0].totalCommonSharesOutstanding is not None and 
-                market_price is not None and 
-                float(balance_sheet[0].totalCommonSharesOutstanding) > 0 and
-                float(fin_statement[0].total_revenue) != 0):
-                price_to_sales_ratio = float(market_price) * float(balance_sheet[0].totalCommonSharesOutstanding) / float(fin_statement[0].total_revenue)
-            else:
-                price_to_sales_ratio = None
-
-            if balance_sheet[0].totalEquity is not None and balance_sheet[0].totalCommonSharesOutstanding is not None and market_price is not None and float(balance_sheet[0].totalCommonSharesOutstanding) > 0:
-                price_to_book_value = float(market_price) * float(balance_sheet[0].totalCommonSharesOutstanding) / float(balance_sheet[0].totalEquity)
-            else:
-                price_to_book_value = None
-
-            if balance_sheet[0].totalReceivablesNet is not None and balance_sheet[0].totalInventory is not None and balance_sheet[0].accountsPayable is not None and fin_statement[0].cost_of_revenue_total is not None and fin_statement[0].total_revenue is not None and float(fin_statement[0].total_revenue) > 0:
-                days_sales_outstanding = 365 * float(balance_sheet[0].totalReceivablesNet) / float(fin_statement[0].total_revenue)
-                days_inventory_outstanding = 365 * float(balance_sheet[0].totalInventory) / float(fin_statement[0].cost_of_revenue_total)
-                days_payable_outstanding = 365 * float(balance_sheet[0].accountsPayable) / float(fin_statement[0].cost_of_revenue_total)
-                cash_conversion_cycle = days_sales_outstanding + float(days_inventory_outstanding) - float(days_payable_outstanding)
-            else:
-                cash_conversion_cycle = None
-            if fin_statement[0].total_revenue is not None and balance_sheet[0].ppeTotalNet is not None and float(balance_sheet[0].ppeTotalNet) > 0:
-                fixed_asset_turnover = float(fin_statement[0].total_revenue) / float(balance_sheet[0].ppeTotalNet)
-            else:
-                fixed_asset_turnover = None
-
-            if fin_statement[0].total_revenue is not None and balance_sheet[0].totalAssets is not None and float(balance_sheet[0].totalAssets) > 0:
-                asset_turnover = float(fin_statement[0].total_revenue) / float(balance_sheet[0].totalAssets)
-            else:
-                asset_turnover = None
-
-            if fin_statement[0].operating_profit is not None and balance_sheet[0].totalDebt is not None and float(fin_statement[0].operating_profit) > 0:
-                total_debt_to_ebitda = float(balance_sheet[0].totalDebt) / float(fin_statement[0].operating_profit)
-            else:
-                total_debt_to_ebitda = None
-
-            return {
-                'current_ratio': current_ratio,
-                'quick_ratio': quick_ratio,
-                'debt_to_equity_ratio': debt_to_equity_ratio,
-                'return_on_assets': return_on_assets,
-                'return_on_equity': return_on_equity,
-                'gross_profit_margin': gross_profit_margin,
-                'operating_margin': operating_margin,
-                'net_profit_margin': net_profit_margin,
-                'dividend_payout_ratio': dividend_payout_ratio,
-                'revenue_growth': revenue_growth,
-                'total_debt_to_ebitda': total_debt_to_ebitda,
-                'interest_coverage': interest_coverage,
-                'price_to_earnings_ratio': price_to_earnings_ratio,
-                'price_to_sales_ratio': price_to_sales_ratio,
-                'price_to_book_value': price_to_book_value,
-                'cash_conversion_cycle': cash_conversion_cycle,
-                'inventory_turnover': inventory_turnover,
-                'fixed_asset_turnover': fixed_asset_turnover,
-                'asset_turnover': asset_turnover,
-                'debt_ratio': debt_ratio,
-                'total_asset_turnover': total_asset_turnover,
-                'days_sales_outstanding': days_sales_outstanding
+        financial_statement_data[fin_publish_date].append(statement_data)
 
-            }
+        return financial_statement_data
+async def volume_analysis_endpoint(ticker):
+    vol_analysis_data = await webull.get_webull_vol_analysis_data(ticker)
+
+    buyvol = float(vol_analysis_data.buyVolume) if vol_analysis_data.buyVolume is not None else None
+    sellvol = float(vol_analysis_data.sellVolume) if vol_analysis_data.sellVolume is not None else None
+    nvol = float(vol_analysis_data.nVolume) if vol_analysis_data.nVolume is not None else None
+    tvol = float(vol_analysis_data.totalVolume) if vol_analysis_data.totalVolume is not None else None
+    average_traded_price = vol_analysis_data.avePrice
+    vol_analysis_results = { 
+        'Buy Volume': f"{buyvol:,}",
+        'Neutral Volume': f"{nvol:,}",
+        'Sell Volume': f"{sellvol:,}",
+        'Total Volume': f"{tvol:,}",
+        'Average Traded Price': f"{average_traded_price}"
+    }
 
-    async def get_etfs_for_ticker(self, ticker):
-        async with aiohttp.ClientSession() as session:
-            ticker_id, _ = await self.fetch_ticker_id(ticker)
-            url = f"https://quotes-gw.webullfintech.com/api/information/company/queryEtfList?tickerId={ticker_id}&pageIndex=1&pageSize=350"
-            async with session.get(url) as response:
-                r = await response.json()
-                datalist = r['dataList']
-                etf_holdings = [ETFHoldings(i) for i in datalist]
-                return etf_holdings
 
-                
 
+    return vol_analysis_results
+async def get_top_gainers_data():
+    types = ['1d','preMarket','afterMarket','5m','1m', '3m', '52w']
+    
 
 
-    async def get_webull_news(self, ticker, current_news_id: int = 0, page_size: int = 50, headers: dict = None) -> List[NewsItem]:
-        async with aiohttp.ClientSession(headers="YOUR_WEBULL_HEADERS") as session:
-            ticker_id, _ = await self.fetch_ticker_id(ticker)
-            url = f"https://quotes-gw.webullfintech.com/api/information/news/tickerNews?tickerId={ticker_id}&currentNewsId={current_news_id}&pageSize={page_size}"
-            async with session.get(url) as response:
-                news_data = await response.json()
-                return [NewsItem(news) for news in news_data]
-    async def check_recent_news(self, ticker, webull_headers):
-
-        ticker_id, _ = await self.fetch_ticker_id(ticker)
-        news = await self.get_webull_news(ticker_id, headers=webull_headers)
-
-        if not news:
-            return None
-
-        latest_news = news[0]
-        news_time = parser.parse(latest_news.news_time)
-        time_threshold = datetime.now(timezone.utc) - timedelta(minutes=90)
-
-        if news_time >= time_threshold:
-            return {
-                'news_url': latest_news.news_url,
-                'source_name': latest_news.source_name,
-                'title': latest_news.title,
-                'news_time': news_time
-            }
+    data_dict = {}
 
-        return None
-    
-    async def get_recent_news_for_tickers(self,ticker, webull_headers):
-        ticker_id, _ = await self.fetch_ticker_id(ticker)
-        recent_news_list = []
-        recent_news = await self.check_recent_news(ticker_id, webull_headers)
-        if recent_news is not None and recent_news['news_url'] not in seen_article_urls:
-            seen_article_urls.add(recent_news['news_url'])
-            recent_news_list.append(recent_news)
+    for i in types:
+        r = requests.get(f"https://quotes-gw.webullfintech.com/api/bgw/market/topGainers?regionId=6&rankType={i}&pageIndex=1&pageSize=350").json()
+        if 'data' in r:
+            data = r['data']
+            tickers = [d['ticker'] for d in data]
+
+            ticker_data = []
+            for ticker in tickers:
+                exchangeId = ticker.get('exchangeId')
+                type_val = ticker.get('type')
+                secType = ticker.get('secType')
+                regionId = ticker.get('regionId')
+                currencyId = ticker.get('currencyId')
+                currencyCode = ticker.get('currencyCode')
+                name = ticker.get('name')
+                symbol = ticker.get('symbol')
+                disSymbol = ticker.get('disSymbol')
+                disExchangeCode = ticker.get('disExchangeCode')
+                exchangeCode = ticker.get('exchangeCode')
+                listStatus = ticker.get('listStatus')
+                template = ticker.get('template')
+                derivativeSupport = ticker.get('derivativeSupport')
+                isPTP = ticker.get('isPTP')
+                tradeTime = ticker.get('tradeTime')
+                faTradeTime = ticker.get('faTradeTime')
+                status = ticker.get('status')
+                close = ticker.get('close')
+                change = ticker.get('change')
+                changeRatio = ticker.get('changeRatio')
+                marketValue = ticker.get('marketValue')
+                volume = ticker.get('volume')
+                turnoverRate = ticker.get('turnoverRate')
+                regionName = ticker.get('regionName')
+                regionIsoCode = ticker.get('regionIsoCode')
+                peTtm = ticker.get('peTtm')
+                preClose = ticker.get('preClose')
+                fiftyTwoWkHigh = ticker.get('fiftyTwoWkHigh')
+                fiftyTwoWkLow = ticker.get('fiftyTwoWkLow')
+                open_val = ticker.get('open')
+                high = ticker.get('high')
+                low = ticker.get('low')
+                
+                ticker_dict = {
+                    'Exchange ID': exchangeId,
+                    'Type': type_val,
+                    'Security Type': secType,
+                    'Region ID': regionId,
+                    'Currency ID': currencyId,
+                    'Currency Code': currencyCode,
+                    'Name': name,
+                    'Symbol': symbol,
+                    'Display Symbol': disSymbol,
+                    'Display Exchange Code': disExchangeCode,
+                    'Exchange Code': exchangeCode,
+                    'List Status': listStatus,
+                    'Template': template,
+                    'Derivative Support': derivativeSupport,
+                    'Is PTP': isPTP,
+                    'Trade Time': tradeTime,
+                    'FA Trade Time': faTradeTime,
+                    'Status': status,
+                    'Close Price': close,
+                    'Change': change,
+                    'Change Ratio': changeRatio,
+                    'Market Value': marketValue,
+                    'Volume': volume,
+                    'Turnover Rate': turnoverRate,
+                    'Region Name': regionName,
+                    'Region ISO Code': regionIsoCode,
+                    'PE Ratio TTM': peTtm,
+                    'Previous Close': preClose,
+                    '52-Week High': fiftyTwoWkHigh,
+                    '52-Week Low': fiftyTwoWkLow,
+                    'Open Price': open_val,
+                    'High Price': high,
+                    'Low Price': low
+                }
 
-        return recent_news_list
-    
+                ticker_data.append(ticker_dict)
 
+            data_dict[i] = ticker_data
 
-    async def get_option_data(self, symbol):
-        option_data_dict = {}
-        url = f"https://quotes-gw.webullfintech.com/api/quote/option/quotes/queryBatch?derivativeIds={symbol}"
-        async with aiohttp.ClientSession() as session:
-            async with session.get(url) as response:
-                data = await response.json()
-                print(data)
-                opt_data = [QueryDerivatives(i) for i in data]
 
-        return opt_data
+            return data_dict
+        
+async def get_fifty_twos_endpoint():
+    data = await webull.fifty_two_high_and_lows()
+
+    data_dict = {
+        'tickerId': data.tickerId,
+        'exchangeId': data.exchangeId,
+        'type': data.type,
+        'secType': data.secType,
+        'regionId': data.regionId,
+        'currencyId': data.currencyId,
+        'currencyCode': data.currencyCode,
+        'name': data.name,
+        'symbol': data.symbol,
+        'disSymbol': data.disSymbol,
+        'disExchangeCode': data.disExchangeCode,
+        'exchangeCode': data.exchangeCode,
+        'listStatus': data.listStatus,
+        'template': data.template,
+        'derivativeSupport': data.derivativeSupport,
+        'isPTP': data.isPTP,
+        'tradeTime': data.tradeTime,
+        'faTradeTime': data.faTradeTime,
+        'status': data.status,
+        'close': data.close,
+        'change': data.change,
+        'changeRatio': data.changeRatio,
+        'marketValue': data.marketValue,
+        'volume': data.volume,
+        'regionName': data.regionName,
+        'regionIsoCode': data.regionIsoCode,
+        'peTtm': data.peTtm,
+        'preClose': data.preClose,
+        'fiftyTwoWkHigh': data.fiftyTwoWkHigh,
+        'fiftyTwoWkLow': data.fiftyTwoWkLow,
+        'open': data.open,
+        'high': data.high,
+        'low': data.low,
+        'vibrateRatio': data.vibrateRatio,
+        'pchange': data.pchange,
+        'pchRatio': data.pchRatio,
+        'pprice': data.pprice
+    }
+
+    return data_dict
+
+async def top_active():
+    data = await webull.top_active_stocks()
+
+    data_dict = {
+        'tickerId': data.tickerId,
+        'exchangeId': data.exchangeId,
+        'type': data.type,
+        'secType': data.secType,
+        'regionId': data.regionId,
+        'currencyId': data.currencyId,
+        'currencyCode': data.currencyCode,
+        'name': data.name,
+        'symbol': data.symbol,
+        'disSymbol': data.disSymbol,
+        'disExchangeCode': data.disExchangeCode,
+        'exchangeCode': data.exchangeCode,
+        'listStatus': data.listStatus,
+        'template': data.template,
+        'derivativeSupport': data.derivativeSupport,
+        'isPTP': data.isPTP,
+        'tradeTime': data.tradeTime,
+        'faTradeTime': data.faTradeTime,
+        'status': data.status,
+        'close': data.close,
+        'change': data.change,
+        'changeRatio': data.changeRatio,
+        'marketValue': data.marketValue,
+        'volume': data.volume,
+        'regionName': data.regionName,
+        'regionIsoCode': data.regionIsoCode,
+        'peTtm': data.peTtm,
+        'preClose': data.preClose,
+        'fiftyTwoWkHigh': data.fiftyTwoWkHigh,
+        'fiftyTwoWkLow': data.fiftyTwoWkLow,
+        'open': data.open,
+        'high': data.high,
+        'low': data.low,
+        'vibrateRatio': data.vibrateRatio,
+        'pchange': data.pchange,
+        'pchRatio': data.pchRatio,
+        'pprice': data.pprice
+    }
+
+    return data_dict
+
+
+
+async def process_data():
+    webull = Webull()
+    await webull.fetch_data('AAPL')
+    return webull.__dict__
```

### Comparing `api_master-1.3/polygonsdk/static/py/commands.py` & `api_master-1.4/static/py/commands.py`

 * *Files identical despite different names*

### Comparing `api_master-1.3/polygonsdk/static/py/snippets.py` & `api_master-1.4/static/py/snippets.py`

 * *Files identical despite different names*

### Comparing `api_master-1.3/setup.py` & `api_master-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='api_master',
-    version='1.3',
+    version='1.4',
     author='Chuck Dustin',
     author_email='chuckdustin12@gmail.com',
     description='Utilize several market-data APIs in production-ready format for real-time and simulated market analysis.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/your-username/your-package-repo',
     packages=find_packages(),
```

