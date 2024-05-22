# Comparing `tmp/volstreet-8.3.3.tar.gz` & `tmp/volstreet-8.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-8.3.3.tar", last modified: Tue May 21 10:20:53 2024, max compression
+gzip compressed data, was "volstreet-8.3.4.tar", last modified: Wed May 22 20:58:49 2024, max compression
```

## Comparing `volstreet-8.3.3.tar` & `volstreet-8.3.4.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.363038 volstreet-8.3.3/
--rw-rw-rw-   0        0        0     1293 2024-05-21 10:20:53.363038 volstreet-8.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.3.3/README.md
--rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.3.3/pyproject.toml
--rw-rw-rw-   0        0        0     1155 2024-05-21 10:20:53.363038 volstreet-8.3.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.252664 volstreet-8.3.3/volstreet/
--rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.3.3/volstreet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.268804 volstreet-8.3.3/volstreet/angel_interface/
--rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.3.3/volstreet/angel_interface/__init__.py
--rw-rw-rw-   0        0        0     3726 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/angel_interface/access_rate_handler.py
--rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.3.3/volstreet/angel_interface/active_session.py
--rw-rw-rw-   0        0        0     3315 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/angel_interface/async_interface.py
--rw-rw-rw-   0        0        0     7280 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/angel_interface/base_websocket.py
--rw-rw-rw-   0        0        0    18658 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/angel_interface/interface.py
--rw-rw-rw-   0        0        0     2501 2024-04-06 10:22:09.000000 volstreet-8.3.3/volstreet/angel_interface/login.py
--rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/angel_interface/order_websocket.py
--rw-rw-rw-   0        0        0    30773 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/angel_interface/price_websocket.py
--rw-rw-rw-   0        0        0     6687 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/angel_interface/smart_connect.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.300069 volstreet-8.3.3/volstreet/backtests/
--rw-rw-rw-   0        0        0      290 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/backtests/__init__.py
--rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.3.3/volstreet/backtests/analysis.py
--rw-rw-rw-   0        0        0     4181 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/backtests/data_updation.py
--rw-rw-rw-   0        0        0    11651 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/backtests/database.py
--rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.3.3/volstreet/backtests/delta_hedging.py
--rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/backtests/delta_optimizer.py
--rw-rw-rw-   0        0        0    48672 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/backtests/framework.py
--rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.3.3/volstreet/backtests/intraday_backtest_abc.py
--rw-rw-rw-   0        0        0     7375 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/backtests/proxy_functions.py
--rw-rw-rw-   0        0        0     2707 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/backtests/result_processing.py
--rw-rw-rw-   0        0        0     6184 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/backtests/runner.py
--rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.3.3/volstreet/backtests/tools.py
--rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.3.3/volstreet/backtests/trend.py
--rw-rw-rw-   0        0        0     1924 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/backtests/underlying_info.py
--rw-rw-rw-   0        0        0    20882 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     4712 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/config.py
--rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/database_connection.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.315686 volstreet-8.3.3/volstreet/datamodule/
--rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.3.3/volstreet/datamodule/__init__.py
--rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/datamodule/analysis.py
--rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/datamodule/archive.py
--rw-rw-rw-   0        0        0     9819 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/datamodule/data_handling.py
--rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/datamodule/eod_client.py
--rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/datamodule/gambling.py
--rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/datamodule/intraday_data.py
--rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.3.3/volstreet/datamodule/stockmock.py
--rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/datamodule/trading_assistance.py
--rw-rw-rw-   0        0        0    25622 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.3.3/volstreet/decorators.py
--rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.315686 volstreet-8.3.3/volstreet/historical_info/
--rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.3.3/volstreet/historical_info/__init__.py
--rw-rw-rw-   0        0        0    21283 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/historical_info/index_expiries.pkl
--rw-rw-rw-   0        0        0    17053 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/historical_info/market_days.pkl
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.315686 volstreet-8.3.3/volstreet/models/
--rw-rw-rw-   0        0        0      568 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/models/__init__.py
--rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/parallelization.py
--rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.3.3/volstreet/performance_tracking.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.315686 volstreet-8.3.3/volstreet/position_dashboard/
--rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.3.3/volstreet/position_dashboard/__init__.py
--rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.3.3/volstreet/position_dashboard/app.py
--rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.3.3/volstreet/position_dashboard/formatting.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.331316 volstreet-8.3.3/volstreet/strategies/
--rw-rw-rw-   0        0        0      183 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/strategies/__init__.py
--rw-rw-rw-   0        0        0    32518 2024-05-21 10:18:48.000000 volstreet-8.3.3/volstreet/strategies/deployment.py
--rw-rw-rw-   0        0        0     1925 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/strategies/error_handling.py
--rw-rw-rw-   0        0        0    57538 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/strategies/helpers.py
--rw-rw-rw-   0        0        0     6352 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/strategies/monitoring.py
--rw-rw-rw-   0        0        0    18537 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/strategies/optimization.py
--rw-rw-rw-   0        0        0   103760 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/strategies/strats.py
--rw-rw-rw-   0        0        0     1251 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/strategies/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.347025 volstreet-8.3.3/volstreet/trade_interface/
--rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.3.3/volstreet/trade_interface/__init__.py
--rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.3.3/volstreet/trade_interface/instruments.py
--rw-rw-rw-   0        0        0    19390 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/trade_interface/order_execution.py
--rw-rw-rw-   0        0        0    20161 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/trade_interface/underlyings.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.347025 volstreet-8.3.3/volstreet/utils/
--rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/utils/__init__.py
--rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/utils/change_config.py
--rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.3.3/volstreet/utils/communication.py
--rw-rw-rw-   0        0        0    14493 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/utils/core.py
--rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.3.3/volstreet/utils/data_io.py
--rw-rw-rw-   0        0        0     9915 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/utils/scrip_processing.py
--rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.3.3/volstreet/vectorized_blackscholes.py
--rw-rw-rw-   0        0        0       16 2024-05-21 08:12:54.000000 volstreet-8.3.3/volstreet/volstreet_mode.json
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.363038 volstreet-8.3.3/volstreet/vslogging/
--rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.3.3/volstreet/vslogging/__init__.py
--rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.3.3/volstreet/vslogging/formatters.py
--rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.3.3/volstreet/vslogging/logging_config.json
--rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.3.3/volstreet/vslogging/logging_setup.py
--rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.3.3/volstreet/vslogging/parsing.py
-drwxrwxrwx   0        0        0        0 2024-05-21 10:20:53.363038 volstreet-8.3.3/volstreet.egg-info/
--rw-rw-rw-   0        0        0     1293 2024-05-21 10:20:53.000000 volstreet-8.3.3/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2833 2024-05-21 10:20:53.000000 volstreet-8.3.3/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 10:20:53.000000 volstreet-8.3.3/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      460 2024-05-21 10:20:53.000000 volstreet-8.3.3/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 10:20:53.000000 volstreet-8.3.3/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.218704 volstreet-8.3.4/
+-rw-rw-rw-   0        0        0     1293 2024-05-22 20:58:49.218704 volstreet-8.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-03-14 04:36:05.000000 volstreet-8.3.4/README.md
+-rw-rw-rw-   0        0        0       91 2024-03-14 04:36:05.000000 volstreet-8.3.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1155 2024-05-22 20:58:49.218704 volstreet-8.3.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.061591 volstreet-8.3.4/volstreet/
+-rw-rw-rw-   0        0        0      442 2024-03-14 09:55:16.000000 volstreet-8.3.4/volstreet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.093232 volstreet-8.3.4/volstreet/angel_interface/
+-rw-rw-rw-   0        0        0      247 2024-04-26 02:47:59.000000 volstreet-8.3.4/volstreet/angel_interface/__init__.py
+-rw-rw-rw-   0        0        0     3726 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/angel_interface/access_rate_handler.py
+-rw-rw-rw-   0        0        0      274 2024-04-23 04:22:25.000000 volstreet-8.3.4/volstreet/angel_interface/active_session.py
+-rw-rw-rw-   0        0        0     3315 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/angel_interface/async_interface.py
+-rw-rw-rw-   0        0        0     7249 2024-05-22 16:21:22.000000 volstreet-8.3.4/volstreet/angel_interface/base_websocket.py
+-rw-rw-rw-   0        0        0    18658 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/angel_interface/interface.py
+-rw-rw-rw-   0        0        0     2552 2024-05-22 12:44:38.000000 volstreet-8.3.4/volstreet/angel_interface/login.py
+-rw-rw-rw-   0        0        0     1988 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/angel_interface/order_websocket.py
+-rw-rw-rw-   0        0        0    30913 2024-05-22 20:52:23.000000 volstreet-8.3.4/volstreet/angel_interface/price_websocket.py
+-rw-rw-rw-   0        0        0     6687 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/angel_interface/smart_connect.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.124490 volstreet-8.3.4/volstreet/backtests/
+-rw-rw-rw-   0        0        0      290 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/backtests/__init__.py
+-rw-rw-rw-   0        0        0     4064 2024-04-23 04:22:25.000000 volstreet-8.3.4/volstreet/backtests/analysis.py
+-rw-rw-rw-   0        0        0     4181 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/backtests/data_updation.py
+-rw-rw-rw-   0        0        0    11651 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/backtests/database.py
+-rw-rw-rw-   0        0        0    38400 2024-04-03 08:06:51.000000 volstreet-8.3.4/volstreet/backtests/delta_hedging.py
+-rw-rw-rw-   0        0        0     5695 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/backtests/delta_optimizer.py
+-rw-rw-rw-   0        0        0    48672 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/backtests/framework.py
+-rw-rw-rw-   0        0        0     5410 2024-04-13 06:57:57.000000 volstreet-8.3.4/volstreet/backtests/intraday_backtest_abc.py
+-rw-rw-rw-   0        0        0     7375 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/backtests/proxy_functions.py
+-rw-rw-rw-   0        0        0     2707 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/backtests/result_processing.py
+-rw-rw-rw-   0        0        0     6184 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/backtests/runner.py
+-rw-rw-rw-   0        0        0     6446 2024-03-26 10:23:44.000000 volstreet-8.3.4/volstreet/backtests/tools.py
+-rw-rw-rw-   0        0        0    15734 2024-04-13 06:57:57.000000 volstreet-8.3.4/volstreet/backtests/trend.py
+-rw-rw-rw-   0        0        0     1924 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/backtests/underlying_info.py
+-rw-rw-rw-   0        0        0    20882 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     4756 2024-05-22 12:43:30.000000 volstreet-8.3.4/volstreet/config.py
+-rw-rw-rw-   0        0        0     2162 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/database_connection.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.140114 volstreet-8.3.4/volstreet/datamodule/
+-rw-rw-rw-   0        0        0      163 2024-04-13 05:46:57.000000 volstreet-8.3.4/volstreet/datamodule/__init__.py
+-rw-rw-rw-   0        0        0     7358 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/datamodule/analysis.py
+-rw-rw-rw-   0        0        0    21130 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/datamodule/archive.py
+-rw-rw-rw-   0        0        0     9819 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/datamodule/data_handling.py
+-rw-rw-rw-   0        0        0     4534 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/datamodule/eod_client.py
+-rw-rw-rw-   0        0        0     5639 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/datamodule/gambling.py
+-rw-rw-rw-   0        0        0     8098 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/datamodule/intraday_data.py
+-rw-rw-rw-   0        0        0    15754 2024-03-26 10:23:44.000000 volstreet-8.3.4/volstreet/datamodule/stockmock.py
+-rw-rw-rw-   0        0        0     1219 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/datamodule/trading_assistance.py
+-rw-rw-rw-   0        0        0    25622 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     2573 2024-04-03 08:06:51.000000 volstreet-8.3.4/volstreet/decorators.py
+-rw-rw-rw-   0        0        0     1683 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0     1698 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.155740 volstreet-8.3.4/volstreet/historical_info/
+-rw-rw-rw-   0        0        0      975 2024-04-24 06:53:53.000000 volstreet-8.3.4/volstreet/historical_info/__init__.py
+-rw-rw-rw-   0        0        0    21283 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/historical_info/index_expiries.pkl
+-rw-rw-rw-   0        0        0    17079 2024-05-22 20:48:02.000000 volstreet-8.3.4/volstreet/historical_info/market_days.pkl
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.155740 volstreet-8.3.4/volstreet/models/
+-rw-rw-rw-   0        0        0      568 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/models/__init__.py
+-rw-rw-rw-   0        0        0      772 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/parallelization.py
+-rw-rw-rw-   0        0        0     1659 2024-04-06 06:31:33.000000 volstreet-8.3.4/volstreet/performance_tracking.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.155740 volstreet-8.3.4/volstreet/position_dashboard/
+-rw-rw-rw-   0        0        0        0 2024-04-17 11:41:53.000000 volstreet-8.3.4/volstreet/position_dashboard/__init__.py
+-rw-rw-rw-   0        0        0     1972 2024-04-17 11:41:53.000000 volstreet-8.3.4/volstreet/position_dashboard/app.py
+-rw-rw-rw-   0        0        0      572 2024-04-17 11:41:53.000000 volstreet-8.3.4/volstreet/position_dashboard/formatting.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.171386 volstreet-8.3.4/volstreet/strategies/
+-rw-rw-rw-   0        0        0      183 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/strategies/__init__.py
+-rw-rw-rw-   0        0        0    32536 2024-05-22 16:37:48.000000 volstreet-8.3.4/volstreet/strategies/deployment.py
+-rw-rw-rw-   0        0        0     1925 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/strategies/error_handling.py
+-rw-rw-rw-   0        0        0    57538 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/strategies/helpers.py
+-rw-rw-rw-   0        0        0     6352 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/strategies/monitoring.py
+-rw-rw-rw-   0        0        0    18537 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/strategies/optimization.py
+-rw-rw-rw-   0        0        0   103760 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/strategies/strats.py
+-rw-rw-rw-   0        0        0     1251 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/strategies/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.187422 volstreet-8.3.4/volstreet/trade_interface/
+-rw-rw-rw-   0        0        0      224 2024-04-17 11:41:53.000000 volstreet-8.3.4/volstreet/trade_interface/__init__.py
+-rw-rw-rw-   0        0        0    26799 2024-04-23 04:22:25.000000 volstreet-8.3.4/volstreet/trade_interface/instruments.py
+-rw-rw-rw-   0        0        0    19390 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/trade_interface/order_execution.py
+-rw-rw-rw-   0        0        0    20161 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/trade_interface/underlyings.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.203058 volstreet-8.3.4/volstreet/utils/
+-rw-rw-rw-   0        0        0      138 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/utils/__init__.py
+-rw-rw-rw-   0        0        0      757 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/utils/change_config.py
+-rw-rw-rw-   0        0        0     3052 2024-04-09 12:38:37.000000 volstreet-8.3.4/volstreet/utils/communication.py
+-rw-rw-rw-   0        0        0    14493 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/utils/core.py
+-rw-rw-rw-   0        0        0     4419 2024-03-14 04:36:05.000000 volstreet-8.3.4/volstreet/utils/data_io.py
+-rw-rw-rw-   0        0        0     9915 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/utils/scrip_processing.py
+-rw-rw-rw-   0        0        0     6488 2024-04-23 04:22:25.000000 volstreet-8.3.4/volstreet/vectorized_blackscholes.py
+-rw-rw-rw-   0        0        0       16 2024-05-21 08:12:54.000000 volstreet-8.3.4/volstreet/volstreet_mode.json
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.203058 volstreet-8.3.4/volstreet/vslogging/
+-rw-rw-rw-   0        0        0       81 2024-03-15 09:40:04.000000 volstreet-8.3.4/volstreet/vslogging/__init__.py
+-rw-rw-rw-   0        0        0     2023 2024-03-26 10:23:44.000000 volstreet-8.3.4/volstreet/vslogging/formatters.py
+-rw-rw-rw-   0        0        0     1492 2024-03-27 04:16:21.000000 volstreet-8.3.4/volstreet/vslogging/logging_config.json
+-rw-rw-rw-   0        0        0      842 2024-03-26 10:23:44.000000 volstreet-8.3.4/volstreet/vslogging/logging_setup.py
+-rw-rw-rw-   0        0        0     1390 2024-04-17 11:41:53.000000 volstreet-8.3.4/volstreet/vslogging/parsing.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:58:49.218704 volstreet-8.3.4/volstreet.egg-info/
+-rw-rw-rw-   0        0        0     1293 2024-05-22 20:58:48.000000 volstreet-8.3.4/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2833 2024-05-22 20:58:49.000000 volstreet-8.3.4/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:58:48.000000 volstreet-8.3.4/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      460 2024-05-22 20:58:48.000000 volstreet-8.3.4/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 20:58:48.000000 volstreet-8.3.4/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-8.3.3/PKG-INFO` & `volstreet-8.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.3.3
+Version: 8.3.4
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.3.3/setup.cfg` & `volstreet-8.3.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 382e 332e 330d 0a61  rsion = 8.3.3..a
+00000020: 7273 696f 6e20 3d20 382e 332e 340d 0a61  rsion = 8.3.4..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-8.3.3/volstreet/angel_interface/access_rate_handler.py` & `volstreet-8.3.4/volstreet/angel_interface/access_rate_handler.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/angel_interface/async_interface.py` & `volstreet-8.3.4/volstreet/angel_interface/async_interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/angel_interface/base_websocket.py` & `volstreet-8.3.4/volstreet/angel_interface/base_websocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         self.reconnecting = True
         if self.current_retry_attempt < self.MAX_RETRY_ATTEMPT:
             self.current_retry_attempt += 1
             logger.info(
                 f"{self.websocket_type} reconnecting attempt: {self.current_retry_attempt}"
             )
             time.sleep(self.RETRY_DELAY)
-            threading.Thread(target=self.connect).start()
+            self.connect()
         else:
             logger.warning(
                 f"{self.websocket_type} connection retry limit exceeded. Max attempts: {self.MAX_RETRY_ATTEMPT}"
             )
             self.connected.value = False
 
     def close_connection(self):
```

### Comparing `volstreet-8.3.3/volstreet/angel_interface/interface.py` & `volstreet-8.3.4/volstreet/angel_interface/interface.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/angel_interface/login.py` & `volstreet-8.3.4/volstreet/angel_interface/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             os.makedirs(user_dir)
 
         # Set obj and login_data in config
         ActiveSession.obj = obj
         ActiveSession.login_data = login_data
 
         set_error_notification_settings("user", obj.userId)
+        logger.extra.update({"user": obj.userId})
         notifier(
             f'Date: {current_time().strftime("%d %b %Y %H:%M:%S")}\nLogged in successfully.',
             webhook_url,
             "CRUCIAL",
         )
     else:
         notifier(
```

### Comparing `volstreet-8.3.3/volstreet/angel_interface/order_websocket.py` & `volstreet-8.3.4/volstreet/angel_interface/order_websocket.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/angel_interface/price_websocket.py` & `volstreet-8.3.4/volstreet/angel_interface/price_websocket.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import threading
 from volstreet.config import token_symbol_dict, logger, token_exchange_dict
 from volstreet.utils import (
     current_time,
     get_symbol_token,
     strike_range_different,
     log_error,
+    notifier,
 )
 from volstreet.angel_interface.base_websocket import BaseWebsocket
 
 
 class PriceWebsocket(BaseWebsocket):
     LITTLE_ENDIAN_BYTE_ORDER = "<"
 
@@ -148,22 +149,25 @@
                 if "last_traded_timestamp" in message
                 else None
             ),
             **message,
         }
 
     def on_error(self, wsapp, error):
+        notifier(
+            f"Price websocket connection has faced an error: {error}", self.webhook_url
+        )
         self.RESUBSCRIBE_FLAG = True
         if self.current_retry_attempt < self.MAX_RETRY_ATTEMPT:
             self.current_retry_attempt += 1
             sleep(self.RETRY_DELAY)
 
             try:
                 self.close_connection()
-                self.connect()
+                self.retry_connect()
             except Exception as e:
                 logger.error(f"{self.websocket_type} error in on_error: {e}")
         else:
             self.close_connection()
             logger.error(f"{self.websocket_type} error in on_error: {error}")
 
     def _create_payload(self, tokens: list):
```

### Comparing `volstreet-8.3.3/volstreet/angel_interface/smart_connect.py` & `volstreet-8.3.4/volstreet/angel_interface/smart_connect.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/analysis.py` & `volstreet-8.3.4/volstreet/backtests/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/data_updation.py` & `volstreet-8.3.4/volstreet/backtests/data_updation.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/database.py` & `volstreet-8.3.4/volstreet/backtests/database.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/delta_hedging.py` & `volstreet-8.3.4/volstreet/backtests/delta_hedging.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/delta_optimizer.py` & `volstreet-8.3.4/volstreet/backtests/delta_optimizer.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/framework.py` & `volstreet-8.3.4/volstreet/backtests/framework.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/intraday_backtest_abc.py` & `volstreet-8.3.4/volstreet/backtests/intraday_backtest_abc.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/proxy_functions.py` & `volstreet-8.3.4/volstreet/backtests/proxy_functions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/result_processing.py` & `volstreet-8.3.4/volstreet/backtests/result_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/runner.py` & `volstreet-8.3.4/volstreet/backtests/runner.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/tools.py` & `volstreet-8.3.4/volstreet/backtests/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/trend.py` & `volstreet-8.3.4/volstreet/backtests/trend.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/backtests/underlying_info.py` & `volstreet-8.3.4/volstreet/backtests/underlying_info.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/blackscholes.py` & `volstreet-8.3.4/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/config.py` & `volstreet-8.3.4/volstreet/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,15 @@
 backtest_mode = "backtest" in _mode
 backtest_state = None
 
 
 # Create loggers
 setup_logging()
 logger = logging.getLogger("volstreet")
+logger = logging.LoggerAdapter(logger, {})
 
 if backtest_mode:
     scrips = pd.DataFrame()
     token_symbol_dict = {}
     token_exchange_dict = defaultdict(lambda: "BACKTESTER")
 else:
     # Get the list of scrips
```

### Comparing `volstreet-8.3.3/volstreet/database_connection.py` & `volstreet-8.3.4/volstreet/database_connection.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/datamodule/analysis.py` & `volstreet-8.3.4/volstreet/datamodule/analysis.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/datamodule/archive.py` & `volstreet-8.3.4/volstreet/datamodule/archive.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/datamodule/data_handling.py` & `volstreet-8.3.4/volstreet/datamodule/data_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/datamodule/eod_client.py` & `volstreet-8.3.4/volstreet/datamodule/eod_client.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/datamodule/gambling.py` & `volstreet-8.3.4/volstreet/datamodule/gambling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/datamodule/intraday_data.py` & `volstreet-8.3.4/volstreet/datamodule/intraday_data.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/datamodule/stockmock.py` & `volstreet-8.3.4/volstreet/datamodule/stockmock.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/datamodule/trading_assistance.py` & `volstreet-8.3.4/volstreet/datamodule/trading_assistance.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/dealingroom.py` & `volstreet-8.3.4/volstreet/dealingroom.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/decorators.py` & `volstreet-8.3.4/volstreet/decorators.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/discord_bot.py` & `volstreet-8.3.4/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/exceptions.py` & `volstreet-8.3.4/volstreet/exceptions.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/historical_info/__init__.py` & `volstreet-8.3.4/volstreet/historical_info/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/historical_info/index_expiries.pkl` & `volstreet-8.3.4/volstreet/historical_info/index_expiries.pkl`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/historical_info/market_days.pkl` & `volstreet-8.3.4/volstreet/historical_info/market_days.pkl`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9592 4200 0000 0000 005d 9428 8c08  ....B......].(..
+00000000: 8004 95ac 4200 0000 0000 005d 9428 8c08  ....B......].(..
 00000010: 6461 7465 7469 6d65 948c 0464 6174 6594  datetime...date.
 00000020: 9394 4304 07e3 0201 9485 9452 9468 0343  ..C........R.h.C
 00000030: 0407 e302 0494 8594 5294 6803 4304 07e3  ........R.h.C...
 00000040: 0205 9485 9452 9468 0343 0407 e302 0694  .....R.h.C......
 00000050: 8594 5294 6803 4304 07e3 0207 9485 9452  ..R.h.C........R
 00000060: 9468 0343 0407 e302 0894 8594 5294 6803  .h.C........R.h.
 00000070: 4304 07e3 020b 9485 9452 9468 0343 0407  C........R.h.C..
@@ -1059,8 +1059,10 @@
 00004220: 0794 8594 5294 6803 4304 07e8 0508 9485  ....R.h.C.......
 00004230: 9452 9468 0343 0407 e805 0994 8594 5294  .R.h.C........R.
 00004240: 6803 4304 07e8 050a 9485 9452 9468 0343  h.C........R.h.C
 00004250: 0407 e805 0d94 8594 5294 6803 4304 07e8  ........R.h.C...
 00004260: 050e 9485 9452 9468 0343 0407 e805 0f94  .....R.h.C......
 00004270: 8594 5294 6803 4304 07e8 0510 9485 9452  ..R.h.C........R
 00004280: 9468 0343 0407 e805 1194 8594 5294 6803  .h.C........R.h.
-00004290: 4304 07e8 0512 9485 9452 9465 2e         C........R.e.
+00004290: 4304 07e8 0512 9485 9452 9468 0343 0407  C........R.h.C..
+000042a0: e805 1594 8594 5294 6803 4304 07e8 0516  ......R.h.C.....
+000042b0: 9485 9452 9465 2e                        ...R.e.
```

### Comparing `volstreet-8.3.3/volstreet/models/__init__.py` & `volstreet-8.3.4/volstreet/models/__init__.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/parallelization.py` & `volstreet-8.3.4/volstreet/parallelization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/performance_tracking.py` & `volstreet-8.3.4/volstreet/performance_tracking.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/position_dashboard/app.py` & `volstreet-8.3.4/volstreet/position_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/position_dashboard/formatting.py` & `volstreet-8.3.4/volstreet/position_dashboard/formatting.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/strategies/deployment.py` & `volstreet-8.3.4/volstreet/strategies/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -679,15 +679,15 @@
         f"Starting open orders handler in client {client.name} at {current_time()}..."
     )
     Thread(target=client.continuously_handle_open_orders).start()
 
     # Starting live feeds
     logger.info(f"Starting live feeds in client {client.name} at {current_time()}...")
     if websockets:
-        LiveFeeds.start_price_feed(process_manager)
+        LiveFeeds.start_price_feed(process_manager, client.error_url)
         LiveFeeds.start_order_feed(process_manager)
 
     # Starting strategies
     strategy_threads = [Thread(target=strategy.run) for strategy in client.strategies]
     logger.info(f"Starting strategies in client {client.name} at {current_time()}")
     for strategy in strategy_threads:
         strategy.start()
```

### Comparing `volstreet-8.3.3/volstreet/strategies/error_handling.py` & `volstreet-8.3.4/volstreet/strategies/error_handling.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/strategies/helpers.py` & `volstreet-8.3.4/volstreet/strategies/helpers.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/strategies/monitoring.py` & `volstreet-8.3.4/volstreet/strategies/monitoring.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/strategies/optimization.py` & `volstreet-8.3.4/volstreet/strategies/optimization.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/strategies/strats.py` & `volstreet-8.3.4/volstreet/strategies/strats.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/strategies/tools.py` & `volstreet-8.3.4/volstreet/strategies/tools.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/trade_interface/instruments.py` & `volstreet-8.3.4/volstreet/trade_interface/instruments.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/trade_interface/order_execution.py` & `volstreet-8.3.4/volstreet/trade_interface/order_execution.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/trade_interface/underlyings.py` & `volstreet-8.3.4/volstreet/trade_interface/underlyings.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/utils/change_config.py` & `volstreet-8.3.4/volstreet/utils/change_config.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/utils/communication.py` & `volstreet-8.3.4/volstreet/utils/communication.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/utils/core.py` & `volstreet-8.3.4/volstreet/utils/core.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/utils/data_io.py` & `volstreet-8.3.4/volstreet/utils/data_io.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/utils/scrip_processing.py` & `volstreet-8.3.4/volstreet/utils/scrip_processing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/vectorized_blackscholes.py` & `volstreet-8.3.4/volstreet/vectorized_blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/vslogging/formatters.py` & `volstreet-8.3.4/volstreet/vslogging/formatters.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/vslogging/logging_config.json` & `volstreet-8.3.4/volstreet/vslogging/logging_config.json`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/vslogging/logging_setup.py` & `volstreet-8.3.4/volstreet/vslogging/logging_setup.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet/vslogging/parsing.py` & `volstreet-8.3.4/volstreet/vslogging/parsing.py`

 * *Files identical despite different names*

### Comparing `volstreet-8.3.3/volstreet.egg-info/PKG-INFO` & `volstreet-8.3.4/volstreet.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volstreet
-Version: 8.3.3
+Version: 8.3.4
 Summary: VolStreet is a Python library for automated trading
 Home-page: https://github.com/rahulthakkr/volstreet
 Author: Rahul Thakkar
 Author-email: r.thakkar15@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `volstreet-8.3.3/volstreet.egg-info/SOURCES.txt` & `volstreet-8.3.4/volstreet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

