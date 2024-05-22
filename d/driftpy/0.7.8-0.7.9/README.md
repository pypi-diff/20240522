# Comparing `tmp/driftpy-0.7.8.tar.gz` & `tmp/driftpy-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driftpy-0.7.8.tar", max compression
+gzip compressed data, was "driftpy-0.7.9.tar", max compression
```

## Comparing `driftpy-0.7.8.tar` & `driftpy-0.7.9.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0     2673 2024-01-08 17:02:07.710116 driftpy-0.7.8/README.md
--rw-r--r--   0        0        0     2365 2024-01-08 17:02:07.714116 driftpy-0.7.8/pyproject.toml
--rw-r--r--   0        0        0       22 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/__init__.py
--rw-r--r--   0        0        0     4390 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/account_subscription_config.py
--rw-r--r--   0        0        0       49 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/__init__.py
--rw-r--r--   0        0        0     5554 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/bulk_account_loader.py
--rw-r--r--   0        0        0       48 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/cache/__init__.py
--rw-r--r--   0        0        0     3299 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/cache/drift_client.py
--rw-r--r--   0        0        0     1330 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/cache/user.py
--rw-r--r--   0        0        0       48 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/demo/__init__.py
--rw-r--r--   0        0        0     3709 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/demo/drift_client.py
--rw-r--r--   0        0        0     1328 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/demo/user.py
--rw-r--r--   0        0        0     3620 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/get_accounts.py
--rw-r--r--   0        0        0     3436 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/oracle.py
--rw-r--r--   0        0        0       48 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/polling/__init__.py
--rw-r--r--   0        0        0     6122 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/polling/drift_client.py
--rw-r--r--   0        0        0     2348 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/polling/user.py
--rw-r--r--   0        0        0     1982 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/types.py
--rw-r--r--   0        0        0       48 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/ws/__init__.py
--rw-r--r--   0        0        0     3267 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/ws/account_subscriber.py
--rw-r--r--   0        0        0     6104 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/ws/drift_client.py
--rw-r--r--   0        0        0     4592 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/ws/program_account_subscriber.py
--rw-r--r--   0        0        0      467 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/accounts/ws/user.py
--rw-r--r--   0        0        0      729 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/address_lookup_table.py
--rw-r--r--   0        0        0     2516 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/addresses.py
--rw-r--r--   0        0        0    18424 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/admin.py
--rw-r--r--   0        0        0     2031 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/auction_subscriber/auction_subscriber.py
--rw-r--r--   0        0        0      466 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/auction_subscriber/types.py
--rw-r--r--   0        0        0       50 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/constants/__init__.py
--rw-r--r--   0        0        0     4666 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/constants/config.py
--rw-r--r--   0        0        0     4070 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/constants/numeric_constants.py
--rw-r--r--   0        0        0     8556 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/constants/perp_markets.py
--rw-r--r--   0        0        0     4006 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/constants/spot_markets.py
--rw-r--r--   0        0        0    11659 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/decode/user.py
--rw-r--r--   0        0        0      496 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/dlob/client_types.py
--rw-r--r--   0        0        0    41092 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/dlob/dlob.py
--rw-r--r--   0        0        0     5424 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/dlob/dlob_client.py
--rw-r--r--   0        0        0     2215 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/dlob/dlob_helpers.py
--rw-r--r--   0        0        0     4493 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/dlob/dlob_node.py
--rw-r--r--   0        0        0     5444 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/dlob/dlob_subscriber.py
--rw-r--r--   0        0        0     4098 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/dlob/node_list.py
--rw-r--r--   0        0        0    10544 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/dlob/orderbook_levels.py
--rw-r--r--   0        0        0    84192 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/drift_client.py
--rw-r--r--   0        0        0    29551 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/drift_user.py
--rw-r--r--   0        0        0        0 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/__init__.py
--rw-r--r--   0        0        0     2218 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/event_list.py
--rw-r--r--   0        0        0     3329 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/event_subscriber.py
--rw-r--r--   0        0        0     2862 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/fetch_logs.py
--rw-r--r--   0        0        0     1903 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/polling_log_provider.py
--rw-r--r--   0        0        0      762 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/sort.py
--rw-r--r--   0        0        0     1724 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/tx_event_cache.py
--rw-r--r--   0        0        0     4069 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/types.py
--rw-r--r--   0        0        0     2292 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/events/websocket_log_provider.py
--rw-r--r--   0        0        0        0 2024-01-08 17:02:07.714116 driftpy-0.7.8/src/driftpy/idl/__init__.py
--rw-r--r--   0        0        0   245372 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/idl/drift.json
--rw-r--r--   0        0        0     2277 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/idl/pyth.json
--rw-r--r--   0        0        0     2776 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/idl/token_faucet.json
--rw-r--r--   0        0        0      640 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/keypair.py
--rw-r--r--   0        0        0    29573 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/amm.py
--rw-r--r--   0        0        0     2598 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/auction.py
--rw-r--r--   0        0        0      243 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/conversion.py
--rw-r--r--   0        0        0      805 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/exchange_status.py
--rw-r--r--   0        0        0     9583 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/funding.py
--rw-r--r--   0        0        0     7266 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/margin.py
--rw-r--r--   0        0        0     7150 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/market.py
--rw-r--r--   0        0        0     1572 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/oracles.py
--rw-r--r--   0        0        0     2776 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/orders.py
--rw-r--r--   0        0        0     4893 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/perp_position.py
--rw-r--r--   0        0        0    12160 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/repeg.py
--rw-r--r--   0        0        0     1155 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/spot_market.py
--rw-r--r--   0        0        0     3973 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/spot_position.py
--rw-r--r--   0        0        0    10041 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/trade.py
--rw-r--r--   0        0        0     4644 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/user.py
--rw-r--r--   0        0        0      106 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/math/utils.py
--rw-r--r--   0        0        0      466 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/memcmp.py
--rw-r--r--   0        0        0      603 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/name.py
--rw-r--r--   0        0        0        0 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/py.typed
--rw-r--r--   0        0        0     9800 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/setup/helpers.py
--rw-r--r--   0        0        0     2128 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/slot/slot_subscriber.py
--rw-r--r--   0        0        0        0 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/tx/__init__.py
--rw-r--r--   0        0        0     2722 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/tx/standard_tx_sender.py
--rw-r--r--   0        0        0     1114 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/tx/types.py
--rw-r--r--   0        0        0    28967 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/types.py
--rw-r--r--   0        0        0     1210 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/user_map/polling_sub.py
--rw-r--r--   0        0        0      977 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/user_map/types.py
--rw-r--r--   0        0        0     7356 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/user_map/user_map.py
--rw-r--r--   0        0        0     1084 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/user_map/user_map_config.py
--rw-r--r--   0        0        0     1956 2024-01-08 17:02:07.718116 driftpy-0.7.8/src/driftpy/user_map/websocket_sub.py
--rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 driftpy-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0     2673 2024-01-09 02:04:41.068108 driftpy-0.7.9/README.md
+-rw-r--r--   0        0        0     2365 2024-01-09 02:04:41.072108 driftpy-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/__init__.py
+-rw-r--r--   0        0        0     4390 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/account_subscription_config.py
+-rw-r--r--   0        0        0       49 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/__init__.py
+-rw-r--r--   0        0        0     5554 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/bulk_account_loader.py
+-rw-r--r--   0        0        0       48 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/cache/__init__.py
+-rw-r--r--   0        0        0     3299 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/cache/drift_client.py
+-rw-r--r--   0        0        0     1330 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/cache/user.py
+-rw-r--r--   0        0        0       48 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/demo/__init__.py
+-rw-r--r--   0        0        0     3709 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/demo/drift_client.py
+-rw-r--r--   0        0        0     1328 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/demo/user.py
+-rw-r--r--   0        0        0     3620 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/get_accounts.py
+-rw-r--r--   0        0        0     3436 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/oracle.py
+-rw-r--r--   0        0        0       48 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/polling/__init__.py
+-rw-r--r--   0        0        0     6122 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/polling/drift_client.py
+-rw-r--r--   0        0        0     2348 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/polling/user.py
+-rw-r--r--   0        0        0     1982 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/types.py
+-rw-r--r--   0        0        0       48 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/ws/__init__.py
+-rw-r--r--   0        0        0     3267 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/ws/account_subscriber.py
+-rw-r--r--   0        0        0     6104 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/ws/drift_client.py
+-rw-r--r--   0        0        0     4592 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/ws/program_account_subscriber.py
+-rw-r--r--   0        0        0      467 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/accounts/ws/user.py
+-rw-r--r--   0        0        0      729 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/address_lookup_table.py
+-rw-r--r--   0        0        0     2516 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/addresses.py
+-rw-r--r--   0        0        0    18424 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/admin.py
+-rw-r--r--   0        0        0     2031 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/auction_subscriber/auction_subscriber.py
+-rw-r--r--   0        0        0      466 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/auction_subscriber/types.py
+-rw-r--r--   0        0        0       50 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/constants/__init__.py
+-rw-r--r--   0        0        0     4666 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/constants/config.py
+-rw-r--r--   0        0        0     4070 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/constants/numeric_constants.py
+-rw-r--r--   0        0        0     8556 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/constants/perp_markets.py
+-rw-r--r--   0        0        0     4006 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/constants/spot_markets.py
+-rw-r--r--   0        0        0    11659 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/decode/user.py
+-rw-r--r--   0        0        0      496 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/dlob/client_types.py
+-rw-r--r--   0        0        0    41092 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/dlob/dlob.py
+-rw-r--r--   0        0        0     5424 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/dlob/dlob_client.py
+-rw-r--r--   0        0        0     2215 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/dlob/dlob_helpers.py
+-rw-r--r--   0        0        0     4493 2024-01-09 02:04:41.072108 driftpy-0.7.9/src/driftpy/dlob/dlob_node.py
+-rw-r--r--   0        0        0     5444 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/dlob/dlob_subscriber.py
+-rw-r--r--   0        0        0     4098 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/dlob/node_list.py
+-rw-r--r--   0        0        0    10544 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/dlob/orderbook_levels.py
+-rw-r--r--   0        0        0    84223 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/drift_client.py
+-rw-r--r--   0        0        0    29551 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/drift_user.py
+-rw-r--r--   0        0        0        0 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/__init__.py
+-rw-r--r--   0        0        0     2218 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/event_list.py
+-rw-r--r--   0        0        0     3329 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/event_subscriber.py
+-rw-r--r--   0        0        0     2862 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/fetch_logs.py
+-rw-r--r--   0        0        0     1903 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/polling_log_provider.py
+-rw-r--r--   0        0        0      762 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/sort.py
+-rw-r--r--   0        0        0     1724 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/tx_event_cache.py
+-rw-r--r--   0        0        0     4069 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/types.py
+-rw-r--r--   0        0        0     2292 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/events/websocket_log_provider.py
+-rw-r--r--   0        0        0        0 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/idl/__init__.py
+-rw-r--r--   0        0        0   245372 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/idl/drift.json
+-rw-r--r--   0        0        0     2277 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/idl/pyth.json
+-rw-r--r--   0        0        0     2776 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/idl/token_faucet.json
+-rw-r--r--   0        0        0      640 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/keypair.py
+-rw-r--r--   0        0        0    29573 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/amm.py
+-rw-r--r--   0        0        0     2598 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/auction.py
+-rw-r--r--   0        0        0      243 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/conversion.py
+-rw-r--r--   0        0        0      805 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/exchange_status.py
+-rw-r--r--   0        0        0     9583 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/funding.py
+-rw-r--r--   0        0        0     7266 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/margin.py
+-rw-r--r--   0        0        0     7150 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/market.py
+-rw-r--r--   0        0        0     1572 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/oracles.py
+-rw-r--r--   0        0        0     2776 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/orders.py
+-rw-r--r--   0        0        0     4893 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/perp_position.py
+-rw-r--r--   0        0        0    12160 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/repeg.py
+-rw-r--r--   0        0        0     1155 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/spot_market.py
+-rw-r--r--   0        0        0     3973 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/spot_position.py
+-rw-r--r--   0        0        0    10041 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/trade.py
+-rw-r--r--   0        0        0     4644 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/user.py
+-rw-r--r--   0        0        0      106 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/math/utils.py
+-rw-r--r--   0        0        0      466 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/memcmp.py
+-rw-r--r--   0        0        0      603 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/name.py
+-rw-r--r--   0        0        0        0 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/py.typed
+-rw-r--r--   0        0        0     9800 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/setup/helpers.py
+-rw-r--r--   0        0        0     2128 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/slot/slot_subscriber.py
+-rw-r--r--   0        0        0        0 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/tx/__init__.py
+-rw-r--r--   0        0        0     2722 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/tx/standard_tx_sender.py
+-rw-r--r--   0        0        0     1114 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/tx/types.py
+-rw-r--r--   0        0        0    28967 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/types.py
+-rw-r--r--   0        0        0     1210 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/user_map/polling_sub.py
+-rw-r--r--   0        0        0      977 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/user_map/types.py
+-rw-r--r--   0        0        0     7356 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/user_map/user_map.py
+-rw-r--r--   0        0        0     1084 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/user_map/user_map_config.py
+-rw-r--r--   0        0        0     1956 2024-01-09 02:04:41.076108 driftpy-0.7.9/src/driftpy/user_map/websocket_sub.py
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 driftpy-0.7.9/PKG-INFO
```

### Comparing `driftpy-0.7.8/README.md` & `driftpy-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/pyproject.toml` & `driftpy-0.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "driftpy"
-version = "0.7.8"
+version = "0.7.9"
 description = "A Python client for the Drift DEX"
 authors = ["x19 <https://twitter.com/0xNineteen@gmail.com>", "bigz <https://twitter.com/bigz_pubkey>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/drift-labs/driftpy"
 documentation = "https://drift-labs.github.io/driftpy/"
```

### Comparing `driftpy-0.7.8/src/driftpy/account_subscription_config.py` & `driftpy-0.7.9/src/driftpy/account_subscription_config.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/bulk_account_loader.py` & `driftpy-0.7.9/src/driftpy/accounts/bulk_account_loader.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/cache/drift_client.py` & `driftpy-0.7.9/src/driftpy/accounts/cache/drift_client.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/cache/user.py` & `driftpy-0.7.9/src/driftpy/accounts/cache/user.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/demo/drift_client.py` & `driftpy-0.7.9/src/driftpy/accounts/demo/drift_client.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/demo/user.py` & `driftpy-0.7.9/src/driftpy/accounts/demo/user.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/get_accounts.py` & `driftpy-0.7.9/src/driftpy/accounts/get_accounts.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/oracle.py` & `driftpy-0.7.9/src/driftpy/accounts/oracle.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/polling/drift_client.py` & `driftpy-0.7.9/src/driftpy/accounts/polling/drift_client.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/polling/user.py` & `driftpy-0.7.9/src/driftpy/accounts/polling/user.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/types.py` & `driftpy-0.7.9/src/driftpy/accounts/types.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/ws/account_subscriber.py` & `driftpy-0.7.9/src/driftpy/accounts/ws/account_subscriber.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/ws/drift_client.py` & `driftpy-0.7.9/src/driftpy/accounts/ws/drift_client.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/accounts/ws/program_account_subscriber.py` & `driftpy-0.7.9/src/driftpy/accounts/ws/program_account_subscriber.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/address_lookup_table.py` & `driftpy-0.7.9/src/driftpy/address_lookup_table.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/addresses.py` & `driftpy-0.7.9/src/driftpy/addresses.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/admin.py` & `driftpy-0.7.9/src/driftpy/admin.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/auction_subscriber/auction_subscriber.py` & `driftpy-0.7.9/src/driftpy/auction_subscriber/auction_subscriber.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/constants/config.py` & `driftpy-0.7.9/src/driftpy/constants/config.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/constants/numeric_constants.py` & `driftpy-0.7.9/src/driftpy/constants/numeric_constants.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/constants/perp_markets.py` & `driftpy-0.7.9/src/driftpy/constants/perp_markets.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/constants/spot_markets.py` & `driftpy-0.7.9/src/driftpy/constants/spot_markets.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/decode/user.py` & `driftpy-0.7.9/src/driftpy/decode/user.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/dlob/dlob.py` & `driftpy-0.7.9/src/driftpy/dlob/dlob.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/dlob/dlob_client.py` & `driftpy-0.7.9/src/driftpy/dlob/dlob_client.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/dlob/dlob_helpers.py` & `driftpy-0.7.9/src/driftpy/dlob/dlob_helpers.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/dlob/dlob_node.py` & `driftpy-0.7.9/src/driftpy/dlob/dlob_node.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/dlob/dlob_subscriber.py` & `driftpy-0.7.9/src/driftpy/dlob/dlob_subscriber.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/dlob/node_list.py` & `driftpy-0.7.9/src/driftpy/dlob/node_list.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/dlob/orderbook_levels.py` & `driftpy-0.7.9/src/driftpy/dlob/orderbook_levels.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/drift_client.py` & `driftpy-0.7.9/src/driftpy/drift_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2301,15 +2301,15 @@
         out_ata: Optional[Pubkey] = None,
         in_ata: Optional[Pubkey] = None,
         slippage_bps: Optional[int] = None,
         quote=None,
         reduce_only: Optional[SwapReduceOnly] = None,
         user_account_public_key: Optional[Pubkey] = None,
     ):
-        pre_instructions = []
+        pre_instructions: list[Instruction] = []
         JUPITER_URL = "https://quote-api.jup.ag/v6"
 
         out_market = self.get_spot_market_account(out_market_idx)
         in_market = self.get_spot_market_account(in_market_idx)
 
         if slippage_bps is None:
             slippage_bps = 10
@@ -2327,15 +2327,15 @@
         if out_ata is None:
             out_ata: Pubkey = self.get_associated_token_account_public_key(
                 out_market.market_index
             )
 
             ai = await self.connection.get_account_info(out_ata)
 
-            if not ai:
+            if not ai.value:
                 pre_instructions.append(
                     self.create_associated_token_account_idempotent_instruction(
                         out_ata,
                         self.wallet.public_key,
                         self.wallet.public_key,
                         out_market.mint,
                     )
@@ -2344,15 +2344,15 @@
         if in_ata is None:
             in_ata: Pubkey = self.get_associated_token_account_public_key(
                 in_market.market_index
             )
 
             ai = await self.connection.get_account_info(in_ata)
 
-            if not ai:
+            if not ai.value:
                 pre_instructions.append(
                     self.create_associated_token_account_idempotent_instruction(
                         in_ata,
                         self.wallet.public_key,
                         self.wallet.public_key,
                         in_market.mint,
                     )
```

### Comparing `driftpy-0.7.8/src/driftpy/drift_user.py` & `driftpy-0.7.9/src/driftpy/drift_user.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/events/event_list.py` & `driftpy-0.7.9/src/driftpy/events/event_list.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/events/event_subscriber.py` & `driftpy-0.7.9/src/driftpy/events/event_subscriber.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/events/fetch_logs.py` & `driftpy-0.7.9/src/driftpy/events/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/events/polling_log_provider.py` & `driftpy-0.7.9/src/driftpy/events/polling_log_provider.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/events/sort.py` & `driftpy-0.7.9/src/driftpy/events/sort.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/events/tx_event_cache.py` & `driftpy-0.7.9/src/driftpy/events/tx_event_cache.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/events/types.py` & `driftpy-0.7.9/src/driftpy/events/types.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/events/websocket_log_provider.py` & `driftpy-0.7.9/src/driftpy/events/websocket_log_provider.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/idl/drift.json` & `driftpy-0.7.9/src/driftpy/idl/drift.json`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/idl/pyth.json` & `driftpy-0.7.9/src/driftpy/idl/pyth.json`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/idl/token_faucet.json` & `driftpy-0.7.9/src/driftpy/idl/token_faucet.json`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/keypair.py` & `driftpy-0.7.9/src/driftpy/keypair.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/amm.py` & `driftpy-0.7.9/src/driftpy/math/amm.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/auction.py` & `driftpy-0.7.9/src/driftpy/math/auction.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/exchange_status.py` & `driftpy-0.7.9/src/driftpy/math/exchange_status.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/funding.py` & `driftpy-0.7.9/src/driftpy/math/funding.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/margin.py` & `driftpy-0.7.9/src/driftpy/math/margin.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/market.py` & `driftpy-0.7.9/src/driftpy/math/market.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/oracles.py` & `driftpy-0.7.9/src/driftpy/math/oracles.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/orders.py` & `driftpy-0.7.9/src/driftpy/math/orders.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/perp_position.py` & `driftpy-0.7.9/src/driftpy/math/perp_position.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/repeg.py` & `driftpy-0.7.9/src/driftpy/math/repeg.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/spot_market.py` & `driftpy-0.7.9/src/driftpy/math/spot_market.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/spot_position.py` & `driftpy-0.7.9/src/driftpy/math/spot_position.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/trade.py` & `driftpy-0.7.9/src/driftpy/math/trade.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/math/user.py` & `driftpy-0.7.9/src/driftpy/math/user.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/name.py` & `driftpy-0.7.9/src/driftpy/name.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/setup/helpers.py` & `driftpy-0.7.9/src/driftpy/setup/helpers.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/slot/slot_subscriber.py` & `driftpy-0.7.9/src/driftpy/slot/slot_subscriber.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/tx/standard_tx_sender.py` & `driftpy-0.7.9/src/driftpy/tx/standard_tx_sender.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/tx/types.py` & `driftpy-0.7.9/src/driftpy/tx/types.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/types.py` & `driftpy-0.7.9/src/driftpy/types.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/user_map/polling_sub.py` & `driftpy-0.7.9/src/driftpy/user_map/polling_sub.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/user_map/types.py` & `driftpy-0.7.9/src/driftpy/user_map/types.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/user_map/user_map.py` & `driftpy-0.7.9/src/driftpy/user_map/user_map.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/user_map/user_map_config.py` & `driftpy-0.7.9/src/driftpy/user_map/user_map_config.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/src/driftpy/user_map/websocket_sub.py` & `driftpy-0.7.9/src/driftpy/user_map/websocket_sub.py`

 * *Files identical despite different names*

### Comparing `driftpy-0.7.8/PKG-INFO` & `driftpy-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: driftpy
-Version: 0.7.8
+Version: 0.7.9
 Summary: A Python client for the Drift DEX
 Home-page: https://github.com/drift-labs/driftpy
 License: MIT
 Author: x19
 Author-email: https://twitter.com/0xNineteen@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

