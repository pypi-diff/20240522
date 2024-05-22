# Comparing `tmp/aiotx-1.2.5.tar.gz` & `tmp/aiotx-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotx-1.2.5.tar", last modified: Tue May 21 05:52:59 2024, max compression
+gzip compressed data, was "aiotx-1.3.0.tar", last modified: Wed May 22 20:04:49 2024, max compression
```

## Comparing `aiotx-1.2.5.tar` & `aiotx-1.3.0.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.485382 aiotx-1.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.413382 aiotx-1.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.421382 aiotx-1.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-21 05:52:53.000000 aiotx-1.2.5/.github/workflows/lint-check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-21 05:52:53.000000 aiotx-1.2.5/.github/workflows/mysql_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-21 05:52:53.000000 aiotx-1.2.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-21 05:52:53.000000 aiotx-1.2.5/.github/workflows/static.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-21 05:52:53.000000 aiotx-1.2.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-21 05:52:53.000000 aiotx-1.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-21 05:52:53.000000 aiotx-1.2.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-21 05:52:53.000000 aiotx-1.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-21 05:52:53.000000 aiotx-1.2.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-21 05:52:53.000000 aiotx-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-21 05:52:59.485382 aiotx-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-21 05:52:53.000000 aiotx-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.421382 aiotx-1.2.5/aiotx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.421382 aiotx-1.2.5/aiotx/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/clients/_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13173 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/clients/_evm_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18874 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/clients/_utxo_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.421382 aiotx-1.2.5/aiotx/types/
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.425382 aiotx-1.2.5/aiotx/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/utils/bep20_abi.json
--rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-21 05:52:53.000000 aiotx-1.2.5/aiotx/utils/erc20_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.481382 aiotx-1.2.5/aiotx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-21 05:52:59.000000 aiotx-1.2.5/aiotx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-21 05:52:59.000000 aiotx-1.2.5/aiotx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 05:52:59.000000 aiotx-1.2.5/aiotx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-21 05:52:59.000000 aiotx-1.2.5/aiotx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 05:52:59.000000 aiotx-1.2.5/aiotx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.425382 aiotx-1.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.417382 aiotx-1.2.5/docs/clients/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.429382 aiotx-1.2.5/docs/clients/evm_client/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_contract_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_contract_decimals.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_gas_price.rst
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_last_block.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_transaction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/get_transaction_count.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/send_token.rst
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/evm_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.429382 aiotx-1.2.5/docs/clients/tron_client/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/tron_client/from_wei.rst
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/tron_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/tron_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/tron_client/to_wei.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.429382 aiotx-1.2.5/docs/clients/utxo_client/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/estimate_smart_fee.rst
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/from_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/generate_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/get_address_from_private_key.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/get_balance.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/get_block_by_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/get_last_block_number.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/import_address.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/send.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/send_bulk.rst
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/clients/utxo_client/to_satoshi.rst
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/monitoring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-21 05:52:53.000000 aiotx-1.2.5/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.433382 aiotx-1.2.5/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-21 05:52:53.000000 aiotx-1.2.5/examples/aiogram_notificator_bot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-21 05:52:53.000000 aiotx-1.2.5/examples/aiogram_notificator_bot.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-21 05:52:53.000000 aiotx-1.2.5/examples/block_and_transactions_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-21 05:52:53.000000 aiotx-1.2.5/examples/two_block_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-21 05:52:53.000000 aiotx-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 05:52:53.000000 aiotx-1.2.5/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.433382 aiotx-1.2.5/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-21 05:52:53.000000 aiotx-1.2.5/scripts/build_and_test.sh
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-21 05:52:59.485382 aiotx-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-21 05:52:53.000000 aiotx-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.433382 aiotx-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.433382 aiotx-1.2.5/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.417382 aiotx-1.2.5/tests/fixtures/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.433382 aiotx-1.2.5/tests/fixtures/cassettes/bsc/
--rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9513 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.449382 aiotx-1.2.5/tests/fixtures/cassettes/btc/
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/btc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
--rw-r--r--   0 runner    (1001) docker     (127) 10849634 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127) 21956267 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.477382 aiotx-1.2.5/tests/fixtures/cassettes/eth/
--rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/get_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/get_gas_price.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/get_token_balance.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/get_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/get_transaction_count.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/send_token_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.481382 aiotx-1.2.5/tests/fixtures/cassettes/ltc/
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/get_last_block.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    40578 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_bulk.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_transaction.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    28458 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/fixtures/networks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.417382 aiotx-1.2.5/tests/test_evm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.481382 aiotx-1.2.5/tests/test_evm/test_bsc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_evm/test_bsc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_evm/test_bsc/test_bsc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_evm/test_bsc/test_bsc_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_evm/test_bsc/test_bsc_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.481382 aiotx-1.2.5/tests/test_evm/test_eth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_evm/test_eth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_evm/test_eth/test_eth_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_evm/test_eth/test_eth_input_decoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_evm/test_eth/test_eth_monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.417382 aiotx-1.2.5/tests/test_utxo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.481382 aiotx-1.2.5/tests/test_utxo/test_btc/
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_utxo/test_btc/test_btc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_utxo/test_btc/test_btc_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:59.481382 aiotx-1.2.5/tests/test_utxo/test_ltc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_utxo/test_ltc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_utxo/test_ltc/test_ltc_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-21 05:52:53.000000 aiotx-1.2.5/tests/test_utxo/test_ltc/test_ltc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.662374 aiotx-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/lint-check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/mysql_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/static.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-22 20:04:43.000000 aiotx-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-22 20:04:43.000000 aiotx-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-22 20:04:43.000000 aiotx-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-22 20:04:43.000000 aiotx-1.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-22 20:04:43.000000 aiotx-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-22 20:04:43.000000 aiotx-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-22 20:04:49.662374 aiotx-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6835 2024-05-22 20:04:43.000000 aiotx-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/aiotx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/aiotx/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/clients/_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/clients/_evm_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19072 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/clients/_utxo_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/aiotx/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.602374 aiotx-1.3.0/aiotx/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/utils/bep20_abi.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4840 2024-05-22 20:04:43.000000 aiotx-1.3.0/aiotx/utils/erc20_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.662374 aiotx-1.3.0/aiotx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8695 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 20:04:49.000000 aiotx-1.3.0/aiotx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.606374 aiotx-1.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/docs/clients/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.606374 aiotx-1.3.0/docs/clients/evm_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_contract_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_contract_decimals.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_gas_price.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_last_block.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3617 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_transaction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/get_transaction_count.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/send_token.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/evm_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.606374 aiotx-1.3.0/docs/clients/tron_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/tron_client/from_wei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/tron_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/tron_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/tron_client/to_wei.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/docs/clients/utxo_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/estimate_smart_fee.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/from_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/generate_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/get_address_from_private_key.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/get_balance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/get_block_by_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/get_last_block_number.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/import_address.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7798 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/send.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/send_bulk.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/clients/utxo_client/to_satoshi.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/monitoring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3991 2024-05-22 20:04:43.000000 aiotx-1.3.0/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   168560 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/aiogram_notificator_bot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/aiogram_notificator_bot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/block_and_transactions_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/eth_block_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/ltc_block_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-22 20:04:43.000000 aiotx-1.3.0/examples/two_block_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-22 20:04:43.000000 aiotx-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 20:04:43.000000 aiotx-1.3.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-05-22 20:04:43.000000 aiotx-1.3.0/scripts/build_and_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 20:04:49.662374 aiotx-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-05-22 20:04:43.000000 aiotx-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.610374 aiotx-1.3.0/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/tests/fixtures/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.614374 aiotx-1.3.0/tests/fixtures/cassettes/bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)    15929 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    19581 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    26713 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13929 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.626374 aiotx-1.3.0/tests/fixtures/cassettes/btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 10852371 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127) 21958019 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.654374 aiotx-1.3.0/tests/fixtures/cassettes/eth/
+-rw-r--r--   0 runner    (1001) docker     (127)     8418 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_gas_price.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     9588 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_token_balance.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17729 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8340 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11559 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/fixtures/cassettes/ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/get_last_block.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    42576 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_bulk.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12161 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_transaction.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    34448 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/fixtures/networks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/tests/test_evm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/test_evm/test_bsc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_bsc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14213 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/test_evm/test_eth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_eth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_eth/test_eth_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_eth/test_eth_input_decoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_evm/test_eth/test_eth_monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.598374 aiotx-1.3.0/tests/test_utxo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/test_utxo/test_btc/
+-rw-r--r--   0 runner    (1001) docker     (127)     5982 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_btc/test_btc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_btc/test_btc_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:49.658374 aiotx-1.3.0/tests/test_utxo/test_ltc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_ltc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_ltc/test_ltc_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-05-22 20:04:43.000000 aiotx-1.3.0/tests/test_utxo/test_ltc/test_ltc_monitor.py
```

### Comparing `aiotx-1.2.5/.github/workflows/lint-check.yml` & `aiotx-1.3.0/.github/workflows/lint-check.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/.github/workflows/mysql_test.yml` & `aiotx-1.3.0/.github/workflows/mysql_test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/.github/workflows/python-publish.yml` & `aiotx-1.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/.github/workflows/static.yml` & `aiotx-1.3.0/.github/workflows/static.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/.github/workflows/test.yml` & `aiotx-1.3.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/.gitignore` & `aiotx-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/CHANGELOG.md` & `aiotx-1.3.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
+## [1.3.0]
+- Pulling block only if they are in network to stop printing a lot of errors
+
 ## [1.2.5]
 - Pin the version of main packages and code changes for new eth_account 
 
 ## [1.2.4]
 - Add setuptoools to support python 3.12
 
 ## [1.2.3]
```

### Comparing `aiotx-1.2.5/CODE_OF_CONDUCT.md` & `aiotx-1.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/CONTRIBUTING.md` & `aiotx-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/LICENSE` & `aiotx-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/PKG-INFO` & `aiotx-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 1.2.5
+Version: 1.3.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Project-URL: Documentation, https://grommash9.github.io/aiotx/
 Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
```

### Comparing `aiotx-1.2.5/README.md` & `aiotx-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/aiotx/clients/__init__.py` & `aiotx-1.3.0/aiotx/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/aiotx/clients/_base_client.py` & `aiotx-1.3.0/aiotx/clients/_base_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/aiotx/clients/_evm_base_client.py` & `aiotx-1.3.0/aiotx/clients/_evm_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,19 +295,21 @@
         self.transaction_handlers = []
         self.running = False
         self._latest_block = None
 
     async def poll_blocks(
         self,
     ):
-        if self._latest_block is None:
-            self._latest_block = await self.client.get_last_block_number()
-        block = await self.client.get_block_by_number(self._latest_block)
+        network_latest_block = await self.client.get_last_block_number()
+        target_block = network_latest_block if self._latest_block is None else self._latest_block
+        if target_block > network_latest_block:
+            return
+        block = await self.client.get_block_by_number(target_block)
         await self.process_block(block["result"])
-        self._latest_block = self._latest_block + 1
+        self._latest_block = target_block + 1
 
     async def process_block(self, block):
         for handler in self.block_handlers:
             if asyncio.iscoroutinefunction(handler):
                 await handler(int(block["number"], 16))
             else:
                 handler(int(block["number"], 16))
```

### Comparing `aiotx-1.2.5/aiotx/clients/_utxo_base_client.py` & `aiotx-1.3.0/aiotx/clients/_utxo_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,18 +288,22 @@
         self._engine = create_async_engine(db_url, poolclass=NullPool)
         self._session = sessionmaker(self._engine, class_=AsyncSession, expire_on_commit=False)
         self.Address = create_address_model(self.client._network.name)
         self.UTXO = create_utxo_model(self.client._network.name)
         self.LastBlock = create_last_block_model(self.client._network.name)
 
     async def poll_blocks(self):
-        latest_block = await self._get_last_block()
-        block_data = await self.client.get_block_by_number(latest_block)
-        await self.process_block(latest_block, block_data)
-        await self._update_last_block(latest_block + 1)
+        network_last_block = await self.client.get_last_block_number()
+        local_latest_block = await self._get_last_block()
+        if network_last_block < local_latest_block:
+            return
+        block_data = await self.client.get_block_by_number(local_latest_block)
+        await self.process_block(local_latest_block, block_data)
+        next_block = local_latest_block + 1
+        await self._update_last_block(next_block)
 
     async def process_block(self, block_number, block_data):
         await self._update_last_block(block_number)
         for handler in self.block_handlers:
             await handler(block_number)
 
         addresses = await self._get_addresses()
```

### Comparing `aiotx-1.2.5/aiotx/exceptions.py` & `aiotx-1.3.0/aiotx/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/aiotx/utils/bep20_abi.json` & `aiotx-1.3.0/aiotx/utils/bep20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/aiotx/utils/erc20_abi.json` & `aiotx-1.3.0/aiotx/utils/erc20_abi.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/aiotx.egg-info/PKG-INFO` & `aiotx-1.3.0/aiotx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotx
-Version: 1.2.5
+Version: 1.3.0
 Summary: An asynchronous library for interacting with various cryptocurrencies and blockchains
 Home-page: https://github.com/Grommash9/aiotx
 Author: Oleksandr Prudnikov
 Author-email: prudnikov21@icloud.com
 Project-URL: Documentation, https://grommash9.github.io/aiotx/
 Project-URL: Source, https://github.com/Grommash9/aiotx
 Keywords: cryptocurrency,blockchain,bitcoin,ethereum,asyncio,aiohttp,json-rpc,payment,wallet,transaction
```

### Comparing `aiotx-1.2.5/aiotx.egg-info/SOURCES.txt` & `aiotx-1.3.0/aiotx.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,16 @@
 docs/clients/utxo_client/index.rst
 docs/clients/utxo_client/send.rst
 docs/clients/utxo_client/send_bulk.rst
 docs/clients/utxo_client/to_satoshi.rst
 examples/aiogram_notificator_bot.png
 examples/aiogram_notificator_bot.py
 examples/block_and_transactions_parser.py
+examples/eth_block_monitoring.py
+examples/ltc_block_monitoring.py
 examples/two_block_parsers.py
 scripts/build_and_test.sh
 tests/conftest.py
 tests/fixtures/networks.json
 tests/fixtures/cassettes/bsc/get_balance.yaml
 tests/fixtures/cassettes/bsc/get_contract_decimals.yaml
 tests/fixtures/cassettes/bsc/get_gas_price.yaml
@@ -79,15 +81,14 @@
 tests/fixtures/cassettes/bsc/get_token_balance.yaml
 tests/fixtures/cassettes/bsc/get_transaction.yaml
 tests/fixtures/cassettes/bsc/get_transaction_count.yaml
 tests/fixtures/cassettes/bsc/send_token_transaction.yaml
 tests/fixtures/cassettes/bsc/send_transaction.yaml
 tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml
 tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml
-tests/fixtures/cassettes/bsc/test_async_monitoring.yaml
 tests/fixtures/cassettes/btc/send_to_all_address_types.yaml
 tests/fixtures/cassettes/btc/send_transaction.yaml
 tests/fixtures/cassettes/btc/send_with_auto_fee.yaml
 tests/fixtures/cassettes/btc/test_async_monitoring.yaml
 tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml
 tests/fixtures/cassettes/eth/get_balance.yaml
 tests/fixtures/cassettes/eth/get_contract_decimals.yaml
```

### Comparing `aiotx-1.2.5/docs/Makefile` & `aiotx-1.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/get_balance.rst` & `aiotx-1.3.0/docs/clients/evm_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/get_block_by_number.rst` & `aiotx-1.3.0/docs/clients/evm_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/get_contract_balance.rst` & `aiotx-1.3.0/docs/clients/evm_client/get_contract_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/get_contract_decimals.rst` & `aiotx-1.3.0/docs/clients/evm_client/get_contract_decimals.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/get_transaction.rst` & `aiotx-1.3.0/docs/clients/evm_client/get_transaction.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/get_transaction_count.rst` & `aiotx-1.3.0/docs/clients/evm_client/get_transaction_count.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/index.rst` & `aiotx-1.3.0/docs/clients/evm_client/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/send.rst` & `aiotx-1.3.0/docs/clients/evm_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/evm_client/send_token.rst` & `aiotx-1.3.0/docs/clients/evm_client/send_token.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/estimate_smart_fee.rst` & `aiotx-1.3.0/docs/clients/utxo_client/estimate_smart_fee.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/generate_address.rst` & `aiotx-1.3.0/docs/clients/utxo_client/generate_address.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/get_address_from_private_key.rst` & `aiotx-1.3.0/docs/clients/utxo_client/get_address_from_private_key.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/get_balance.rst` & `aiotx-1.3.0/docs/clients/utxo_client/get_balance.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/get_block_by_number.rst` & `aiotx-1.3.0/docs/clients/utxo_client/get_block_by_number.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/import_address.rst` & `aiotx-1.3.0/docs/clients/utxo_client/import_address.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/index.rst` & `aiotx-1.3.0/docs/clients/utxo_client/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/send.rst` & `aiotx-1.3.0/docs/clients/utxo_client/send.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/clients/utxo_client/send_bulk.rst` & `aiotx-1.3.0/docs/clients/utxo_client/send_bulk.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/conf.py` & `aiotx-1.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/index.rst` & `aiotx-1.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/make.bat` & `aiotx-1.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/monitoring.rst` & `aiotx-1.3.0/docs/monitoring.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/docs/testing.rst` & `aiotx-1.3.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/examples/aiogram_notificator_bot.png` & `aiotx-1.3.0/examples/aiogram_notificator_bot.png`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/examples/aiogram_notificator_bot.py` & `aiotx-1.3.0/examples/aiogram_notificator_bot.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/examples/block_and_transactions_parser.py` & `aiotx-1.3.0/examples/block_and_transactions_parser.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/examples/two_block_parsers.py` & `aiotx-1.3.0/examples/two_block_parsers.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/setup.py` & `aiotx-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/conftest.py` & `aiotx-1.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_balance.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_gas_price.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_last_block.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_token_balance.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_transaction.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/get_transaction_count.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/send_token_transaction.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/send_transaction.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/bsc/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/btc/send_to_all_address_types.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/btc/send_transaction.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/btc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/btc/send_with_auto_fee.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/btc/test_async_monitoring.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/btc/test_async_monitoring.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":2812422,"error":null,"id":"curltest"}
+      string: '{"result":2817099,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -19,15 +19,15 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:10 GMT
+      - Wed, 22 May 2024 19:33:16 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
@@ -36,15 +36,15 @@
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":2812422,"error":null,"id":"curltest"}
+      string: '{"result":2817099,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -53,32 +53,32 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:11 GMT
+      - Wed, 22 May 2024 19:33:17 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":2812422,"error":null,"id":"curltest"}
+      string: '{"result":2817099,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -87,32 +87,32 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:11 GMT
+      - Wed, 22 May 2024 19:33:17 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":2812422,"error":null,"id":"curltest"}
+      string: '{"result":2817099,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -121,19 +121,53 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:11 GMT
+      - Wed, 22 May 2024 19:33:17 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
+      - f1b546936d23e3b5-a12d19355fbb795
+      X-Node-Id:
+      - bitcoin_btc-testnet_iad
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
+  response:
+    body:
+      string: '{"result":2817099,"error":null,"id":"curltest"}
+
+        '
+    headers:
+      Access-Control-Allow-Credentials:
+      - 'true'
+      Access-Control-Allow-Headers:
+      - Content-Type,Authorization,User-Agent
+      Access-Control-Allow-Methods:
+      - GET, POST, OPTIONS
+      Access-Control-Allow-Origin:
+      - ''
+      Content-Length:
+      - '48'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:33:18 GMT
+      Vary:
+      - Accept-Encoding
+      X-Host-Id:
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
     body: '{"method": "getblockhash", "params": [2811502], "jsonrpc": "2.0", "id":
@@ -156,33 +190,33 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '107'
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:12 GMT
+      - Wed, 22 May 2024 19:33:18 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
     body: '{"method": "getblock", "params": ["000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":{"hash":"000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e","confirmations":921,"height":2811502,"version":545259520,"versionHex":"20800000","merkleroot":"374d216ab61fbbefd1f7de856bd2f9c5da748081d86cf17e5c4065f262ba035e","time":1714874483,"mediantime":1714872643,"nonce":1471140407,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ecd696e56d3df7375","nTx":81,"previousblockhash":"0000000000000003d2dbf4baece500010f9ae76733912d2479a85b585483450a","nextblockhash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","strippedsize":955703,"size":965837,"weight":3832946,"tx":[{"txid":"613d2285bf6b309949df357ccdedb06946c07e152aa1e6a8c8f5bf89a9cd2508","hash":"d879e00266f70cd02c6c2e4a68edef20c360beaabc9f33950427be75f9786bd8","version":2,"size":243,"vsize":216,"weight":864,"locktime":0,"vin":[{"coinbase":"036ee62a0473e836664d65726d61696465722046545721010001da82620c0000000000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00000546,"n":0,"scriptPubKey":{"asm":"1
+      string: '{"result":{"hash":"000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e","confirmations":5598,"height":2811502,"version":545259520,"versionHex":"20800000","merkleroot":"374d216ab61fbbefd1f7de856bd2f9c5da748081d86cf17e5c4065f262ba035e","time":1714874483,"mediantime":1714872643,"nonce":1471140407,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ecd696e56d3df7375","nTx":81,"previousblockhash":"0000000000000003d2dbf4baece500010f9ae76733912d2479a85b585483450a","nextblockhash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","strippedsize":955703,"size":965837,"weight":3832946,"tx":[{"txid":"613d2285bf6b309949df357ccdedb06946c07e152aa1e6a8c8f5bf89a9cd2508","hash":"d879e00266f70cd02c6c2e4a68edef20c360beaabc9f33950427be75f9786bd8","version":2,"size":243,"vsize":216,"weight":864,"locktime":0,"vin":[{"coinbase":"036ee62a0473e836664d65726d61696465722046545721010001da82620c0000000000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00000546,"n":0,"scriptPubKey":{"asm":"1
         acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2","desc":"rawtr(acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2)#esyrrkhh","hex":"5120acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2","address":"tb1p4nel7wkc34raczk8c4jwk5cf9d47u2284rxn98rsjrs4w3p2sheqvjmfdh","type":"witness_v1_taproot"}},{"value":0.45263027,"n":1,"scriptPubKey":{"asm":"0
         c035e789d9efffa10aa92e93f48f29b8cfb224c2","desc":"addr(tb1qcq670zweall6zz4f96flfrefhr8myfxz9ll9l2)#whefl5al","hex":"0014c035e789d9efffa10aa92e93f48f29b8cfb224c2","address":"tb1qcq670zweall6zz4f96flfrefhr8myfxz9ll9l2","type":"witness_v0_keyhash"}},{"value":0.00000000,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9ed45869d21f2112abd840f9ff42cc09085dd5888d713d3a86e745afd0085c197d9","desc":"raw(6a24aa21a9ed45869d21f2112abd840f9ff42cc09085dd5888d713d3a86e745afd0085c197d9)#7uynvvu7","hex":"6a24aa21a9ed45869d21f2112abd840f9ff42cc09085dd5888d713d3a86e745afd0085c197d9","type":"nulldata"}}],"hex":"020000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff23036ee62a0473e836664d65726d61696465722046545721010001da82620c0000000000ffffffff032202000000000000225120acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2b3a8b20200000000160014c035e789d9efffa10aa92e93f48f29b8cfb224c20000000000000000266a24aa21a9ed45869d21f2112abd840f9ff42cc09085dd5888d713d3a86e745afd0085c197d90120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"6b3658a9ca6f355f818fdc9c7d8bdad1613c7f676dd5ef6055b6f213677c409d","hash":"b9918b439f45d785117c2355e626e69249490582543179c87571a50ef6d27727","version":1,"size":1009,"vsize":927,"weight":3706,"locktime":0,"vin":[{"txid":"a2a07086dae3ebea3d33c2ee59f331c43bd99814de2a836303e5bcd3b0a53e57","vout":13,"scriptSig":{"asm":"","hex":""},"txinwitness":["3045022100e006cc7f6314456ea7de328d85c3387de95ce8477680cdef1f9a6c98538bb1d00220282516f7bb578217602e675547a16e1d2e685799774363ad3c1c817ec2c4063701","03a41e8fc42e154ce9bf87c29f4062e4bf9d1cbb5131fad462ea858cec5e664e8c"],"sequence":4294967295}],"vout":[{"value":0.00050000,"n":0,"scriptPubKey":{"asm":"1
         bc46efddac6ff291a7e69180a6480bdc0887430edc5f11de3ec0e42bf65a327b","desc":"rawtr(bc46efddac6ff291a7e69180a6480bdc0887430edc5f11de3ec0e42bf65a327b)#g8gaszr8","hex":"5120bc46efddac6ff291a7e69180a6480bdc0887430edc5f11de3ec0e42bf65a327b","address":"tb1ph3rwlhdvdlefrflxjxq2vjqtmsygwscwm303rh37crjzhaj6xfaszjkl6y","type":"witness_v1_taproot"}},{"value":0.00010000,"n":1,"scriptPubKey":{"asm":"1
         a1c8f0e5d238a0d4be1d9da14601977d3512d272916e7f5a0188c137652168b2","desc":"rawtr(a1c8f0e5d238a0d4be1d9da14601977d3512d272916e7f5a0188c137652168b2)#v8rewpsx","hex":"5120a1c8f0e5d238a0d4be1d9da14601977d3512d272916e7f5a0188c137652168b2","address":"tb1p58y0pewj8zsdf0sanks5vqvh056395njj9h87ksp3rqnwefpdzeqa6vqfn","type":"witness_v1_taproot"}},{"value":0.00050000,"n":2,"scriptPubKey":{"asm":"1
         de7bb5e5d919289632d93ea2e873ae2cd7db0bf2fcf4b882f6ac7cee37178857","desc":"rawtr(de7bb5e5d919289632d93ea2e873ae2cd7db0bf2fcf4b882f6ac7cee37178857)#adzxhsu3","hex":"5120de7bb5e5d919289632d93ea2e873ae2cd7db0bf2fcf4b882f6ac7cee37178857","address":"tb1pmeamtewery5fvvke863wsuaw9ntakzljln6t3qhk437wudch3ptsauvz8k","type":"witness_v1_taproot"}},{"value":0.00050000,"n":3,"scriptPubKey":{"asm":"1
         282172d030beaf31620ef10f37e453fda223e7520a6e9cbaaecd4b1d118999cc","desc":"rawtr(282172d030beaf31620ef10f37e453fda223e7520a6e9cbaaecd4b1d118999cc)#llmqsk99","hex":"5120282172d030beaf31620ef10f37e453fda223e7520a6e9cbaaecd4b1d118999cc","address":"tb1p9qsh95psh6hnzcsw7y8n0eznlk3z8e6jpfhfew4we4936yvfn8xqee8v5u","type":"witness_v1_taproot"}},{"value":0.00050000,"n":4,"scriptPubKey":{"asm":"1
@@ -22321,27 +22355,61 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:12 GMT
+      - Wed, 22 May 2024 19:33:19 GMT
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
+  response:
+    body:
+      string: '{"result":2817099,"error":null,"id":"curltest"}
+
+        '
+    headers:
+      Access-Control-Allow-Credentials:
+      - 'true'
+      Access-Control-Allow-Headers:
+      - Content-Type,Authorization,User-Agent
+      Access-Control-Allow-Methods:
+      - GET, POST, OPTIONS
+      Access-Control-Allow-Origin:
+      - ''
+      Content-Length:
+      - '48'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:33:32 GMT
+      Vary:
+      - Accept-Encoding
+      X-Host-Id:
+      - f1b546936d23e3b5-a12d19355fbb795
+      X-Node-Id:
+      - bitcoin_btc-testnet_iad
+    status:
+      code: 200
+      message: OK
+- request:
     body: '{"method": "getblockhash", "params": [2811503], "jsonrpc": "2.0", "id":
       "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
@@ -22358,33 +22426,33 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '107'
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:14 GMT
+      - Wed, 22 May 2024 19:33:33 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-a12d19355fbb795
+      - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
     body: '{"method": "getblock", "params": ["00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":{"hash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","confirmations":920,"height":2811503,"version":536920064,"versionHex":"2000c000","merkleroot":"85b6362d300146d7d9bbcc2d23c6575712b1f1ede44dca5d20b80c0d7dfefbd4","time":1714874968,"mediantime":1714873844,"nonce":2216499726,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ece696f56d4df7475","nTx":16,"previousblockhash":"000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e","nextblockhash":"000000000000009869617263f855e273751e58fa51cfe110c6d26e6295b22d06","strippedsize":2081,"size":4241,"weight":10484,"tx":[{"txid":"11c1ac2c3d3769bec127725a5a7ec7fdcb565fbbdd70e8188421afcae4031633","hash":"2ca2712ceb637cc6304d8f3c503f8a8211da6ecd7df9575a6c97469b355f2a22","version":2,"size":220,"vsize":193,"weight":772,"locktime":0,"vin":[{"coinbase":"036fe62a564b4249542e434f4db0dd8f04ab010000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00037429,"n":0,"scriptPubKey":{"asm":"0
+      string: '{"result":{"hash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","confirmations":5597,"height":2811503,"version":536920064,"versionHex":"2000c000","merkleroot":"85b6362d300146d7d9bbcc2d23c6575712b1f1ede44dca5d20b80c0d7dfefbd4","time":1714874968,"mediantime":1714873844,"nonce":2216499726,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ece696f56d4df7475","nTx":16,"previousblockhash":"000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e","nextblockhash":"000000000000009869617263f855e273751e58fa51cfe110c6d26e6295b22d06","strippedsize":2081,"size":4241,"weight":10484,"tx":[{"txid":"11c1ac2c3d3769bec127725a5a7ec7fdcb565fbbdd70e8188421afcae4031633","hash":"2ca2712ceb637cc6304d8f3c503f8a8211da6ecd7df9575a6c97469b355f2a22","version":2,"size":220,"vsize":193,"weight":772,"locktime":0,"vin":[{"coinbase":"036fe62a564b4249542e434f4db0dd8f04ab010000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00037429,"n":0,"scriptPubKey":{"asm":"0
         ba40aa29a40a415ce244e0ca05b0f0813e048a74","desc":"addr(tb1qhfq252dypfq4ecjyur9qtv8ssylqfzn5chtrwq)#t8j7y469","hex":"0014ba40aa29a40a415ce244e0ca05b0f0813e048a74","address":"tb1qhfq252dypfq4ecjyur9qtv8ssylqfzn5chtrwq","type":"witness_v0_keyhash"}},{"value":0.00711138,"n":1,"scriptPubKey":{"asm":"OP_DUP
         OP_HASH160 5ef5a3849430c6224c94a39a35339df2bcf684f8 OP_EQUALVERIFY OP_CHECKSIG","desc":"addr(mpB45N8LULome7r9SVV8akkJRX8UnXx4hq)#6ew3ha9n","hex":"76a9145ef5a3849430c6224c94a39a35339df2bcf684f888ac","address":"mpB45N8LULome7r9SVV8akkJRX8UnXx4hq","type":"pubkeyhash"}},{"value":0.00000000,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9edf78b4082702442ac0f839ef286115667f5ecfae1a93761514f69635c96b0f98c","desc":"raw(6a24aa21a9edf78b4082702442ac0f839ef286115667f5ecfae1a93761514f69635c96b0f98c)#m4xyxg3v","hex":"6a24aa21a9edf78b4082702442ac0f839ef286115667f5ecfae1a93761514f69635c96b0f98c","type":"nulldata"}}],"hex":"020000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff15036fe62a564b4249542e434f4db0dd8f04ab010000ffffffff033592000000000000160014ba40aa29a40a415ce244e0ca05b0f0813e048a74e2d90a00000000001976a9145ef5a3849430c6224c94a39a35339df2bcf684f888ac0000000000000000266a24aa21a9edf78b4082702442ac0f839ef286115667f5ecfae1a93761514f69635c96b0f98c0120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"e6f0d3d35b256ddf11d9b93091ca0f92c79c30c780529bf7e83fde5d826f259c","hash":"9bfbab2a087abeea47d65f66e640c879735bcc3d9e695e5a808210c26f9513f0","version":2,"size":370,"vsize":154,"weight":616,"locktime":0,"vin":[{"txid":"013e8643b5e3a859a51a6d86176af374389e621f272c942ed2b395c15e9700ac","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["e027c7a206886fe16ad083c2ce9a51468eb54ba306c63efe358575481263b50a268e89ae923c069026a10f7f524a2bfbfaaacf191e147e0cf9316a31feeeacbb","20ed137d1fac3aed96faf94329050ffa20d05d18e2dffc2db9c8624f947da56e7dac0063036f726401010a746578742f706c61696e01073f406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f42494b452d4d4f544f26613d302e3030303126623d302e3030353536323937003f406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f42494b452d4d4f544f26613d302e3030303126623d302e303035353632393768","c1ed137d1fac3aed96faf94329050ffa20d05d18e2dffc2db9c8624f947da56e7d"],"sequence":4294967293}],"vout":[{"value":0.00000333,"n":0,"scriptPubKey":{"asm":"0
         49700b8cf15a7f061f10150964d1d511b0145346","desc":"addr(tb1qf9cqhr83tflsv8csz5ykf5w4zxcpg56xkd25ra)#jlcy6mwz","hex":"001449700b8cf15a7f061f10150964d1d511b0145346","address":"tb1qf9cqhr83tflsv8csz5ykf5w4zxcpg56xkd25ra","type":"witness_v0_keyhash"}}],"fee":0.00012960,"hex":"02000000000101ac00975ec195b3d22e942c271f629e3874f36a17866d1aa559a8e3b543863e010000000000fdffffff014d0100000000000016001449700b8cf15a7f061f10150964d1d511b01453460340e027c7a206886fe16ad083c2ce9a51468eb54ba306c63efe358575481263b50a268e89ae923c069026a10f7f524a2bfbfaaacf191e147e0cf9316a31feeeacbbb920ed137d1fac3aed96faf94329050ffa20d05d18e2dffc2db9c8624f947da56e7dac0063036f726401010a746578742f706c61696e01073f406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f42494b452d4d4f544f26613d302e3030303126623d302e3030353536323937003f406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f42494b452d4d4f544f26613d302e3030303126623d302e30303535363239376821c1ed137d1fac3aed96faf94329050ffa20d05d18e2dffc2db9c8624f947da56e7d00000000"},{"txid":"adcf563115a9ff9c87136310e38d77ab9ec6741fd471bc7aece25de3ee364ada","hash":"990c752ce2a15ae0764fe9ba653938a05ac8b34378c8e1c9e57b374345844c01","version":2,"size":372,"vsize":164,"weight":654,"locktime":0,"vin":[{"txid":"0888c3d31e365704e8b63fa979e2892252098654884874d5884a6fbf12267c02","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["42da84fe20142d68c20d8ece9b802c31b459ec626cce97f6a29db37f80ebf5b9b8801679ce7465603877a7460eba2f60ef05f2e77f32863d1187825d701b59ba","20b5d875d6f1540c4f97f4814bfbcc893c1d50f1c0f08dcd1fe24686fb9786f36bac0063036f726401010a746578742f706c61696e01073a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e3639373534313333003a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e363937353431333368","c0b5d875d6f1540c4f97f4814bfbcc893c1d50f1c0f08dcd1fe24686fb9786f36b"],"sequence":4294967293}],"vout":[{"value":0.00000333,"n":0,"scriptPubKey":{"asm":"1
         a40a60a85db90df3e878cb099c0848bf7120cc16b27cdfc9be7caa8a930ddabc","desc":"rawtr(a40a60a85db90df3e878cb099c0848bf7120cc16b27cdfc9be7caa8a930ddabc)#vyy7me0e","hex":"5120a40a60a85db90df3e878cb099c0848bf7120cc16b27cdfc9be7caa8a930ddabc","address":"tb1p5s9xp2zahyxl86rcevyeczzghacjpnqkkf7dljd70j4g4ycdm27qkdug9r","type":"witness_v1_taproot"}}],"fee":0.00011232,"hex":"02000000000101027c2612bf6f4a88d5744888548609522289e279a93fb6e80457361ed3c388080000000000fdffffff014d01000000000000225120a40a60a85db90df3e878cb099c0848bf7120cc16b27cdfc9be7caa8a930ddabc034042da84fe20142d68c20d8ece9b802c31b459ec626cce97f6a29db37f80ebf5b9b8801679ce7465603877a7460eba2f60ef05f2e77f32863d1187825d701b59baaf20b5d875d6f1540c4f97f4814bfbcc893c1d50f1c0f08dcd1fe24686fb9786f36bac0063036f726401010a746578742f706c61696e01073a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e3639373534313333003a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e36393735343133336821c0b5d875d6f1540c4f97f4814bfbcc893c1d50f1c0f08dcd1fe24686fb9786f36b00000000"},{"txid":"a5f8ce0c995950698d5a0fbc31952fd3fc535afafe2b3aa2098f4b5611a66e95","hash":"4d260831dc119f8870694c254b01cef13990a14218c0b8cae91080d0f96de86f","version":2,"size":205,"vsize":154,"weight":616,"locktime":0,"vin":[{"txid":"4845fc1ab542102504e2e3a7ee037965c73972eea0e665fc3ea1c28c76c9badc","vout":1,"scriptSig":{"asm":"","hex":""},"txinwitness":["18bcbc2a4c4a7f1ff6aa2e4c25f41acf746ad60826373dc880aa5b7a8fedbc427474d2f70bbb68b13d0a106e9e5c0f8a89a8ee3c2b3518a264d7c5a4aaf1f024"],"sequence":4294967295}],"vout":[{"value":0.00011781,"n":0,"scriptPubKey":{"asm":"1
         5c3fa8ae8b5a666a1d869e5b26ced73b5c14be8817a4952fc7abdf9f43a16ed5","desc":"rawtr(5c3fa8ae8b5a666a1d869e5b26ced73b5c14be8817a4952fc7abdf9f43a16ed5)#a9szlj0y","hex":"51205c3fa8ae8b5a666a1d869e5b26ced73b5c14be8817a4952fc7abdf9f43a16ed5","address":"tb1ptsl63t5ttfnx58vxnedjdnkh8dwpf05gz7jf2t78400e7sapdm2szfxszz","type":"witness_v1_taproot"}},{"value":4.79967830,"n":1,"scriptPubKey":{"asm":"1
         5e3d85c0093c513a9a7f8230c0a9ae36f46685d9c9852b3bb6ef18a35ac2e460","desc":"rawtr(5e3d85c0093c513a9a7f8230c0a9ae36f46685d9c9852b3bb6ef18a35ac2e460)#r77m003z","hex":"51205e3d85c0093c513a9a7f8230c0a9ae36f46685d9c9852b3bb6ef18a35ac2e460","address":"tb1ptc7ctsqf83gn4xnlsgcvp2dwxm6xdpweexzjkwakauv2xkkzu3sqdc4uay","type":"witness_v1_taproot"}}],"fee":0.00008162,"hex":"02000000000101dcbac9768cc2a13efc65e6a0ee7239c7657903eea7e3e204251042b51afc45480100000000ffffffff02052e0000000000002251205c3fa8ae8b5a666a1d869e5b26ced73b5c14be8817a4952fc7abdf9f43a16ed556ba9b1c000000002251205e3d85c0093c513a9a7f8230c0a9ae36f46685d9c9852b3bb6ef18a35ac2e460014018bcbc2a4c4a7f1ff6aa2e4c25f41acf746ad60826373dc880aa5b7a8fedbc427474d2f70bbb68b13d0a106e9e5c0f8a89a8ee3c2b3518a264d7c5a4aaf1f02400000000"},{"txid":"9b7c5d60b3d942efb8425e6b8cd1cc2246e9831ad0224ed877881e12d9a80612","hash":"2c7dbd241382b2d6030b3fe19538ab13e67c4a06ad41b7e00596be40e8b89158","version":2,"size":372,"vsize":164,"weight":654,"locktime":0,"vin":[{"txid":"a5f8ce0c995950698d5a0fbc31952fd3fc535afafe2b3aa2098f4b5611a66e95","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["3756a285108d160ded70348fe296fe7823cc9d80a3ccac37a4b33d81f4e5c649ddfeb9695c9b7565de60eb7784a14a3e8ab0cfbcaef756b8100d74d9b0787f0e","205b1e06c75905d5a09cbc559256fc90478798f4ffbe5351095d0b1395b5611cc7ac0063036f726401010a746578742f706c61696e01073a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e3639373534313333003a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e363937353431333368","c05b1e06c75905d5a09cbc559256fc90478798f4ffbe5351095d0b1395b5611cc7"],"sequence":4294967293}],"vout":[{"value":0.00000333,"n":0,"scriptPubKey":{"asm":"1
@@ -22421,21 +22489,55 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:19 GMT
+      - Wed, 22 May 2024 19:33:33 GMT
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
+      - f1b546936d23e3b5-a12d19355fbb795
+      X-Node-Id:
+      - bitcoin_btc-testnet_iad
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
+  response:
+    body:
+      string: '{"result":2817099,"error":null,"id":"curltest"}
+
+        '
+    headers:
+      Access-Control-Allow-Credentials:
+      - 'true'
+      Access-Control-Allow-Headers:
+      - Content-Type,Authorization,User-Agent
+      Access-Control-Allow-Methods:
+      - GET, POST, OPTIONS
+      Access-Control-Allow-Origin:
+      - ''
+      Content-Length:
+      - '48'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:34:06 GMT
+      Vary:
+      - Accept-Encoding
+      X-Host-Id:
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
     body: '{"method": "getblockhash", "params": [2811504], "jsonrpc": "2.0", "id":
@@ -22458,15 +22560,15 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '107'
       Content-Type:
       - application/json
       Date:
-      - Mon, 06 May 2024 22:19:20 GMT
+      - Wed, 22 May 2024 19:34:06 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
```

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/btc/test_async_monitoring_mysql.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":2816335,"error":null,"id":"curltest"}
+      string: '{"result":2817099,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -19,15 +19,49 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:07:53 GMT
+      - Wed, 22 May 2024 19:33:10 GMT
+      Vary:
+      - Accept-Encoding
+      X-Host-Id:
+      - f1b546936d23e3b5-d46e6ad25adfe563
+      X-Node-Id:
+      - bitcoin_btc-testnet_iad
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
+  response:
+    body:
+      string: '{"result":2817099,"error":null,"id":"curltest"}
+
+        '
+    headers:
+      Access-Control-Allow-Credentials:
+      - 'true'
+      Access-Control-Allow-Headers:
+      - Content-Type,Authorization,User-Agent
+      Access-Control-Allow-Methods:
+      - GET, POST, OPTIONS
+      Access-Control-Allow-Origin:
+      - ''
+      Content-Length:
+      - '48'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:33:10 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
@@ -36,15 +70,15 @@
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":2816335,"error":null,"id":"curltest"}
+      string: '{"result":2817099,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -53,32 +87,32 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:07:53 GMT
+      - Wed, 22 May 2024 19:33:11 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":2816335,"error":null,"id":"curltest"}
+      string: '{"result":2817099,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -87,15 +121,15 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:07:54 GMT
+      - Wed, 22 May 2024 19:33:11 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
@@ -104,15 +138,15 @@
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":2816335,"error":null,"id":"curltest"}
+      string: '{"result":2817099,"error":null,"id":"curltest"}
 
         '
     headers:
       Access-Control-Allow-Credentials:
       - 'true'
       Access-Control-Allow-Headers:
       - Content-Type,Authorization,User-Agent
@@ -121,15 +155,15 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '48'
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:07:54 GMT
+      - Wed, 22 May 2024 19:33:11 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
@@ -156,33 +190,33 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '107'
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:07:54 GMT
+      - Wed, 22 May 2024 19:33:12 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
     body: '{"method": "getblock", "params": ["000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":{"hash":"000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e","confirmations":4834,"height":2811502,"version":545259520,"versionHex":"20800000","merkleroot":"374d216ab61fbbefd1f7de856bd2f9c5da748081d86cf17e5c4065f262ba035e","time":1714874483,"mediantime":1714872643,"nonce":1471140407,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ecd696e56d3df7375","nTx":81,"previousblockhash":"0000000000000003d2dbf4baece500010f9ae76733912d2479a85b585483450a","nextblockhash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","strippedsize":955703,"size":965837,"weight":3832946,"tx":[{"txid":"613d2285bf6b309949df357ccdedb06946c07e152aa1e6a8c8f5bf89a9cd2508","hash":"d879e00266f70cd02c6c2e4a68edef20c360beaabc9f33950427be75f9786bd8","version":2,"size":243,"vsize":216,"weight":864,"locktime":0,"vin":[{"coinbase":"036ee62a0473e836664d65726d61696465722046545721010001da82620c0000000000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00000546,"n":0,"scriptPubKey":{"asm":"1
+      string: '{"result":{"hash":"000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e","confirmations":5598,"height":2811502,"version":545259520,"versionHex":"20800000","merkleroot":"374d216ab61fbbefd1f7de856bd2f9c5da748081d86cf17e5c4065f262ba035e","time":1714874483,"mediantime":1714872643,"nonce":1471140407,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ecd696e56d3df7375","nTx":81,"previousblockhash":"0000000000000003d2dbf4baece500010f9ae76733912d2479a85b585483450a","nextblockhash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","strippedsize":955703,"size":965837,"weight":3832946,"tx":[{"txid":"613d2285bf6b309949df357ccdedb06946c07e152aa1e6a8c8f5bf89a9cd2508","hash":"d879e00266f70cd02c6c2e4a68edef20c360beaabc9f33950427be75f9786bd8","version":2,"size":243,"vsize":216,"weight":864,"locktime":0,"vin":[{"coinbase":"036ee62a0473e836664d65726d61696465722046545721010001da82620c0000000000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00000546,"n":0,"scriptPubKey":{"asm":"1
         acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2","desc":"rawtr(acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2)#esyrrkhh","hex":"5120acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2","address":"tb1p4nel7wkc34raczk8c4jwk5cf9d47u2284rxn98rsjrs4w3p2sheqvjmfdh","type":"witness_v1_taproot"}},{"value":0.45263027,"n":1,"scriptPubKey":{"asm":"0
         c035e789d9efffa10aa92e93f48f29b8cfb224c2","desc":"addr(tb1qcq670zweall6zz4f96flfrefhr8myfxz9ll9l2)#whefl5al","hex":"0014c035e789d9efffa10aa92e93f48f29b8cfb224c2","address":"tb1qcq670zweall6zz4f96flfrefhr8myfxz9ll9l2","type":"witness_v0_keyhash"}},{"value":0.00000000,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9ed45869d21f2112abd840f9ff42cc09085dd5888d713d3a86e745afd0085c197d9","desc":"raw(6a24aa21a9ed45869d21f2112abd840f9ff42cc09085dd5888d713d3a86e745afd0085c197d9)#7uynvvu7","hex":"6a24aa21a9ed45869d21f2112abd840f9ff42cc09085dd5888d713d3a86e745afd0085c197d9","type":"nulldata"}}],"hex":"020000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff23036ee62a0473e836664d65726d61696465722046545721010001da82620c0000000000ffffffff032202000000000000225120acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2b3a8b20200000000160014c035e789d9efffa10aa92e93f48f29b8cfb224c20000000000000000266a24aa21a9ed45869d21f2112abd840f9ff42cc09085dd5888d713d3a86e745afd0085c197d90120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"6b3658a9ca6f355f818fdc9c7d8bdad1613c7f676dd5ef6055b6f213677c409d","hash":"b9918b439f45d785117c2355e626e69249490582543179c87571a50ef6d27727","version":1,"size":1009,"vsize":927,"weight":3706,"locktime":0,"vin":[{"txid":"a2a07086dae3ebea3d33c2ee59f331c43bd99814de2a836303e5bcd3b0a53e57","vout":13,"scriptSig":{"asm":"","hex":""},"txinwitness":["3045022100e006cc7f6314456ea7de328d85c3387de95ce8477680cdef1f9a6c98538bb1d00220282516f7bb578217602e675547a16e1d2e685799774363ad3c1c817ec2c4063701","03a41e8fc42e154ce9bf87c29f4062e4bf9d1cbb5131fad462ea858cec5e664e8c"],"sequence":4294967295}],"vout":[{"value":0.00050000,"n":0,"scriptPubKey":{"asm":"1
         bc46efddac6ff291a7e69180a6480bdc0887430edc5f11de3ec0e42bf65a327b","desc":"rawtr(bc46efddac6ff291a7e69180a6480bdc0887430edc5f11de3ec0e42bf65a327b)#g8gaszr8","hex":"5120bc46efddac6ff291a7e69180a6480bdc0887430edc5f11de3ec0e42bf65a327b","address":"tb1ph3rwlhdvdlefrflxjxq2vjqtmsygwscwm303rh37crjzhaj6xfaszjkl6y","type":"witness_v1_taproot"}},{"value":0.00010000,"n":1,"scriptPubKey":{"asm":"1
         a1c8f0e5d238a0d4be1d9da14601977d3512d272916e7f5a0188c137652168b2","desc":"rawtr(a1c8f0e5d238a0d4be1d9da14601977d3512d272916e7f5a0188c137652168b2)#v8rewpsx","hex":"5120a1c8f0e5d238a0d4be1d9da14601977d3512d272916e7f5a0188c137652168b2","address":"tb1p58y0pewj8zsdf0sanks5vqvh056395njj9h87ksp3rqnwefpdzeqa6vqfn","type":"witness_v1_taproot"}},{"value":0.00050000,"n":2,"scriptPubKey":{"asm":"1
         de7bb5e5d919289632d93ea2e873ae2cd7db0bf2fcf4b882f6ac7cee37178857","desc":"rawtr(de7bb5e5d919289632d93ea2e873ae2cd7db0bf2fcf4b882f6ac7cee37178857)#adzxhsu3","hex":"5120de7bb5e5d919289632d93ea2e873ae2cd7db0bf2fcf4b882f6ac7cee37178857","address":"tb1pmeamtewery5fvvke863wsuaw9ntakzljln6t3qhk437wudch3ptsauvz8k","type":"witness_v1_taproot"}},{"value":0.00050000,"n":3,"scriptPubKey":{"asm":"1
         282172d030beaf31620ef10f37e453fda223e7520a6e9cbaaecd4b1d118999cc","desc":"rawtr(282172d030beaf31620ef10f37e453fda223e7520a6e9cbaaecd4b1d118999cc)#llmqsk99","hex":"5120282172d030beaf31620ef10f37e453fda223e7520a6e9cbaaecd4b1d118999cc","address":"tb1p9qsh95psh6hnzcsw7y8n0eznlk3z8e6jpfhfew4we4936yvfn8xqee8v5u","type":"witness_v1_taproot"}},{"value":0.00050000,"n":4,"scriptPubKey":{"asm":"1
@@ -22321,27 +22355,61 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:07:55 GMT
+      - Wed, 22 May 2024 19:33:12 GMT
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
+  response:
+    body:
+      string: '{"result":2817099,"error":null,"id":"curltest"}
+
+        '
+    headers:
+      Access-Control-Allow-Credentials:
+      - 'true'
+      Access-Control-Allow-Headers:
+      - Content-Type,Authorization,User-Agent
+      Access-Control-Allow-Methods:
+      - GET, POST, OPTIONS
+      Access-Control-Allow-Origin:
+      - ''
+      Content-Length:
+      - '48'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:33:14 GMT
+      Vary:
+      - Accept-Encoding
+      X-Host-Id:
+      - f1b546936d23e3b5-d46e6ad25adfe563
+      X-Node-Id:
+      - bitcoin_btc-testnet_iad
+    status:
+      code: 200
+      message: OK
+- request:
     body: '{"method": "getblockhash", "params": [2811503], "jsonrpc": "2.0", "id":
       "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
@@ -22358,15 +22426,15 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '107'
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:07:57 GMT
+      - Wed, 22 May 2024 19:33:15 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
@@ -22376,15 +22444,15 @@
     body: '{"method": "getblock", "params": ["00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":{"hash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","confirmations":4833,"height":2811503,"version":536920064,"versionHex":"2000c000","merkleroot":"85b6362d300146d7d9bbcc2d23c6575712b1f1ede44dca5d20b80c0d7dfefbd4","time":1714874968,"mediantime":1714873844,"nonce":2216499726,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ece696f56d4df7475","nTx":16,"previousblockhash":"000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e","nextblockhash":"000000000000009869617263f855e273751e58fa51cfe110c6d26e6295b22d06","strippedsize":2081,"size":4241,"weight":10484,"tx":[{"txid":"11c1ac2c3d3769bec127725a5a7ec7fdcb565fbbdd70e8188421afcae4031633","hash":"2ca2712ceb637cc6304d8f3c503f8a8211da6ecd7df9575a6c97469b355f2a22","version":2,"size":220,"vsize":193,"weight":772,"locktime":0,"vin":[{"coinbase":"036fe62a564b4249542e434f4db0dd8f04ab010000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00037429,"n":0,"scriptPubKey":{"asm":"0
+      string: '{"result":{"hash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","confirmations":5597,"height":2811503,"version":536920064,"versionHex":"2000c000","merkleroot":"85b6362d300146d7d9bbcc2d23c6575712b1f1ede44dca5d20b80c0d7dfefbd4","time":1714874968,"mediantime":1714873844,"nonce":2216499726,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ece696f56d4df7475","nTx":16,"previousblockhash":"000000000000003c168f0705cbce2bea7c0790c24ecc53d24ffb797b7348042e","nextblockhash":"000000000000009869617263f855e273751e58fa51cfe110c6d26e6295b22d06","strippedsize":2081,"size":4241,"weight":10484,"tx":[{"txid":"11c1ac2c3d3769bec127725a5a7ec7fdcb565fbbdd70e8188421afcae4031633","hash":"2ca2712ceb637cc6304d8f3c503f8a8211da6ecd7df9575a6c97469b355f2a22","version":2,"size":220,"vsize":193,"weight":772,"locktime":0,"vin":[{"coinbase":"036fe62a564b4249542e434f4db0dd8f04ab010000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00037429,"n":0,"scriptPubKey":{"asm":"0
         ba40aa29a40a415ce244e0ca05b0f0813e048a74","desc":"addr(tb1qhfq252dypfq4ecjyur9qtv8ssylqfzn5chtrwq)#t8j7y469","hex":"0014ba40aa29a40a415ce244e0ca05b0f0813e048a74","address":"tb1qhfq252dypfq4ecjyur9qtv8ssylqfzn5chtrwq","type":"witness_v0_keyhash"}},{"value":0.00711138,"n":1,"scriptPubKey":{"asm":"OP_DUP
         OP_HASH160 5ef5a3849430c6224c94a39a35339df2bcf684f8 OP_EQUALVERIFY OP_CHECKSIG","desc":"addr(mpB45N8LULome7r9SVV8akkJRX8UnXx4hq)#6ew3ha9n","hex":"76a9145ef5a3849430c6224c94a39a35339df2bcf684f888ac","address":"mpB45N8LULome7r9SVV8akkJRX8UnXx4hq","type":"pubkeyhash"}},{"value":0.00000000,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9edf78b4082702442ac0f839ef286115667f5ecfae1a93761514f69635c96b0f98c","desc":"raw(6a24aa21a9edf78b4082702442ac0f839ef286115667f5ecfae1a93761514f69635c96b0f98c)#m4xyxg3v","hex":"6a24aa21a9edf78b4082702442ac0f839ef286115667f5ecfae1a93761514f69635c96b0f98c","type":"nulldata"}}],"hex":"020000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff15036fe62a564b4249542e434f4db0dd8f04ab010000ffffffff033592000000000000160014ba40aa29a40a415ce244e0ca05b0f0813e048a74e2d90a00000000001976a9145ef5a3849430c6224c94a39a35339df2bcf684f888ac0000000000000000266a24aa21a9edf78b4082702442ac0f839ef286115667f5ecfae1a93761514f69635c96b0f98c0120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"e6f0d3d35b256ddf11d9b93091ca0f92c79c30c780529bf7e83fde5d826f259c","hash":"9bfbab2a087abeea47d65f66e640c879735bcc3d9e695e5a808210c26f9513f0","version":2,"size":370,"vsize":154,"weight":616,"locktime":0,"vin":[{"txid":"013e8643b5e3a859a51a6d86176af374389e621f272c942ed2b395c15e9700ac","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["e027c7a206886fe16ad083c2ce9a51468eb54ba306c63efe358575481263b50a268e89ae923c069026a10f7f524a2bfbfaaacf191e147e0cf9316a31feeeacbb","20ed137d1fac3aed96faf94329050ffa20d05d18e2dffc2db9c8624f947da56e7dac0063036f726401010a746578742f706c61696e01073f406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f42494b452d4d4f544f26613d302e3030303126623d302e3030353536323937003f406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f42494b452d4d4f544f26613d302e3030303126623d302e303035353632393768","c1ed137d1fac3aed96faf94329050ffa20d05d18e2dffc2db9c8624f947da56e7d"],"sequence":4294967293}],"vout":[{"value":0.00000333,"n":0,"scriptPubKey":{"asm":"0
         49700b8cf15a7f061f10150964d1d511b0145346","desc":"addr(tb1qf9cqhr83tflsv8csz5ykf5w4zxcpg56xkd25ra)#jlcy6mwz","hex":"001449700b8cf15a7f061f10150964d1d511b0145346","address":"tb1qf9cqhr83tflsv8csz5ykf5w4zxcpg56xkd25ra","type":"witness_v0_keyhash"}}],"fee":0.00012960,"hex":"02000000000101ac00975ec195b3d22e942c271f629e3874f36a17866d1aa559a8e3b543863e010000000000fdffffff014d0100000000000016001449700b8cf15a7f061f10150964d1d511b01453460340e027c7a206886fe16ad083c2ce9a51468eb54ba306c63efe358575481263b50a268e89ae923c069026a10f7f524a2bfbfaaacf191e147e0cf9316a31feeeacbbb920ed137d1fac3aed96faf94329050ffa20d05d18e2dffc2db9c8624f947da56e7dac0063036f726401010a746578742f706c61696e01073f406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f42494b452d4d4f544f26613d302e3030303126623d302e3030353536323937003f406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f42494b452d4d4f544f26613d302e3030303126623d302e30303535363239376821c1ed137d1fac3aed96faf94329050ffa20d05d18e2dffc2db9c8624f947da56e7d00000000"},{"txid":"adcf563115a9ff9c87136310e38d77ab9ec6741fd471bc7aece25de3ee364ada","hash":"990c752ce2a15ae0764fe9ba653938a05ac8b34378c8e1c9e57b374345844c01","version":2,"size":372,"vsize":164,"weight":654,"locktime":0,"vin":[{"txid":"0888c3d31e365704e8b63fa979e2892252098654884874d5884a6fbf12267c02","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["42da84fe20142d68c20d8ece9b802c31b459ec626cce97f6a29db37f80ebf5b9b8801679ce7465603877a7460eba2f60ef05f2e77f32863d1187825d701b59ba","20b5d875d6f1540c4f97f4814bfbcc893c1d50f1c0f08dcd1fe24686fb9786f36bac0063036f726401010a746578742f706c61696e01073a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e3639373534313333003a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e363937353431333368","c0b5d875d6f1540c4f97f4814bfbcc893c1d50f1c0f08dcd1fe24686fb9786f36b"],"sequence":4294967293}],"vout":[{"value":0.00000333,"n":0,"scriptPubKey":{"asm":"1
         a40a60a85db90df3e878cb099c0848bf7120cc16b27cdfc9be7caa8a930ddabc","desc":"rawtr(a40a60a85db90df3e878cb099c0848bf7120cc16b27cdfc9be7caa8a930ddabc)#vyy7me0e","hex":"5120a40a60a85db90df3e878cb099c0848bf7120cc16b27cdfc9be7caa8a930ddabc","address":"tb1p5s9xp2zahyxl86rcevyeczzghacjpnqkkf7dljd70j4g4ycdm27qkdug9r","type":"witness_v1_taproot"}}],"fee":0.00011232,"hex":"02000000000101027c2612bf6f4a88d5744888548609522289e279a93fb6e80457361ed3c388080000000000fdffffff014d01000000000000225120a40a60a85db90df3e878cb099c0848bf7120cc16b27cdfc9be7caa8a930ddabc034042da84fe20142d68c20d8ece9b802c31b459ec626cce97f6a29db37f80ebf5b9b8801679ce7465603877a7460eba2f60ef05f2e77f32863d1187825d701b59baaf20b5d875d6f1540c4f97f4814bfbcc893c1d50f1c0f08dcd1fe24686fb9786f36bac0063036f726401010a746578742f706c61696e01073a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e3639373534313333003a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e36393735343133336821c0b5d875d6f1540c4f97f4814bfbcc893c1d50f1c0f08dcd1fe24686fb9786f36b00000000"},{"txid":"a5f8ce0c995950698d5a0fbc31952fd3fc535afafe2b3aa2098f4b5611a66e95","hash":"4d260831dc119f8870694c254b01cef13990a14218c0b8cae91080d0f96de86f","version":2,"size":205,"vsize":154,"weight":616,"locktime":0,"vin":[{"txid":"4845fc1ab542102504e2e3a7ee037965c73972eea0e665fc3ea1c28c76c9badc","vout":1,"scriptSig":{"asm":"","hex":""},"txinwitness":["18bcbc2a4c4a7f1ff6aa2e4c25f41acf746ad60826373dc880aa5b7a8fedbc427474d2f70bbb68b13d0a106e9e5c0f8a89a8ee3c2b3518a264d7c5a4aaf1f024"],"sequence":4294967295}],"vout":[{"value":0.00011781,"n":0,"scriptPubKey":{"asm":"1
         5c3fa8ae8b5a666a1d869e5b26ced73b5c14be8817a4952fc7abdf9f43a16ed5","desc":"rawtr(5c3fa8ae8b5a666a1d869e5b26ced73b5c14be8817a4952fc7abdf9f43a16ed5)#a9szlj0y","hex":"51205c3fa8ae8b5a666a1d869e5b26ced73b5c14be8817a4952fc7abdf9f43a16ed5","address":"tb1ptsl63t5ttfnx58vxnedjdnkh8dwpf05gz7jf2t78400e7sapdm2szfxszz","type":"witness_v1_taproot"}},{"value":4.79967830,"n":1,"scriptPubKey":{"asm":"1
         5e3d85c0093c513a9a7f8230c0a9ae36f46685d9c9852b3bb6ef18a35ac2e460","desc":"rawtr(5e3d85c0093c513a9a7f8230c0a9ae36f46685d9c9852b3bb6ef18a35ac2e460)#r77m003z","hex":"51205e3d85c0093c513a9a7f8230c0a9ae36f46685d9c9852b3bb6ef18a35ac2e460","address":"tb1ptc7ctsqf83gn4xnlsgcvp2dwxm6xdpweexzjkwakauv2xkkzu3sqdc4uay","type":"witness_v1_taproot"}}],"fee":0.00008162,"hex":"02000000000101dcbac9768cc2a13efc65e6a0ee7239c7657903eea7e3e204251042b51afc45480100000000ffffffff02052e0000000000002251205c3fa8ae8b5a666a1d869e5b26ced73b5c14be8817a4952fc7abdf9f43a16ed556ba9b1c000000002251205e3d85c0093c513a9a7f8230c0a9ae36f46685d9c9852b3bb6ef18a35ac2e460014018bcbc2a4c4a7f1ff6aa2e4c25f41acf746ad60826373dc880aa5b7a8fedbc427474d2f70bbb68b13d0a106e9e5c0f8a89a8ee3c2b3518a264d7c5a4aaf1f02400000000"},{"txid":"9b7c5d60b3d942efb8425e6b8cd1cc2246e9831ad0224ed877881e12d9a80612","hash":"2c7dbd241382b2d6030b3fe19538ab13e67c4a06ad41b7e00596be40e8b89158","version":2,"size":372,"vsize":164,"weight":654,"locktime":0,"vin":[{"txid":"a5f8ce0c995950698d5a0fbc31952fd3fc535afafe2b3aa2098f4b5611a66e95","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["3756a285108d160ded70348fe296fe7823cc9d80a3ccac37a4b33d81f4e5c649ddfeb9695c9b7565de60eb7784a14a3e8ab0cfbcaef756b8100d74d9b0787f0e","205b1e06c75905d5a09cbc559256fc90478798f4ffbe5351095d0b1395b5611cc7ac0063036f726401010a746578742f706c61696e01073a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e3639373534313333003a406d6f746f3a737761703a3a636272632d32303a737761703f61623d4d4f544f2d50495a5a4126613d31652d3826623d342e363937353431333368","c05b1e06c75905d5a09cbc559256fc90478798f4ffbe5351095d0b1395b5611cc7"],"sequence":4294967293}],"vout":[{"value":0.00000333,"n":0,"scriptPubKey":{"asm":"1
@@ -22421,20 +22489,54 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:08:11 GMT
+      - Wed, 22 May 2024 19:33:15 GMT
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Host-Id:
+      - f1b546936d23e3b5-a12d19355fbb795
+      X-Node-Id:
+      - bitcoin_btc-testnet_iad
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
+  response:
+    body:
+      string: '{"result":2817099,"error":null,"id":"curltest"}
+
+        '
+    headers:
+      Access-Control-Allow-Credentials:
+      - 'true'
+      Access-Control-Allow-Headers:
+      - Content-Type,Authorization,User-Agent
+      Access-Control-Allow-Methods:
+      - GET, POST, OPTIONS
+      Access-Control-Allow-Origin:
+      - ''
+      Content-Length:
+      - '48'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:33:29 GMT
+      Vary:
+      - Accept-Encoding
+      X-Host-Id:
       - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 - request:
@@ -22458,15 +22560,15 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Length:
       - '107'
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:08:13 GMT
+      - Wed, 22 May 2024 19:33:29 GMT
       Vary:
       - Accept-Encoding
       X-Host-Id:
       - f1b546936d23e3b5-d46e6ad25adfe563
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
@@ -22476,15 +22578,15 @@
     body: '{"method": "getblock", "params": ["000000000000009869617263f855e273751e58fa51cfe110c6d26e6295b22d06",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
   response:
     body:
-      string: '{"result":{"hash":"000000000000009869617263f855e273751e58fa51cfe110c6d26e6295b22d06","confirmations":4833,"height":2811504,"version":538968064,"versionHex":"20200000","merkleroot":"024b7920e5b19475a8783f1b85f286d6441118e12993b22213878a3574ff7702","time":1714875426,"mediantime":1714873875,"nonce":369187849,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ecf697056d5df7575","nTx":1975,"previousblockhash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","nextblockhash":"000000000000005b9147d9b1afe33b6e26b3131184c440e7d23a7870a7635fe2","strippedsize":889212,"size":1188556,"weight":3856192,"tx":[{"txid":"af9a4c02abb02abd304fc7d4b41a95ca381dc6a9c5e53061a30cdc61c458444f","hash":"4694b2c407771e3154b32ea4dcbb25cdea4d665c43be04cdb74a7a41060c9dd9","version":2,"size":243,"vsize":216,"weight":864,"locktime":0,"vin":[{"coinbase":"0370e62a0423ec36664d65726d61696465722046545721010001daf333300000000000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00000546,"n":0,"scriptPubKey":{"asm":"1
+      string: '{"result":{"hash":"000000000000009869617263f855e273751e58fa51cfe110c6d26e6295b22d06","confirmations":5596,"height":2811504,"version":538968064,"versionHex":"20200000","merkleroot":"024b7920e5b19475a8783f1b85f286d6441118e12993b22213878a3574ff7702","time":1714875426,"mediantime":1714873875,"nonce":369187849,"bits":"1a00ffff","difficulty":16777216,"chainwork":"000000000000000000000000000000000000000000000d9ecf697056d5df7575","nTx":1975,"previousblockhash":"00000000000000a47376dfff18873be53d512543fc5dff7c6e19c7766f63216e","nextblockhash":"000000000000005b9147d9b1afe33b6e26b3131184c440e7d23a7870a7635fe2","strippedsize":889212,"size":1188556,"weight":3856192,"tx":[{"txid":"af9a4c02abb02abd304fc7d4b41a95ca381dc6a9c5e53061a30cdc61c458444f","hash":"4694b2c407771e3154b32ea4dcbb25cdea4d665c43be04cdb74a7a41060c9dd9","version":2,"size":243,"vsize":216,"weight":864,"locktime":0,"vin":[{"coinbase":"0370e62a0423ec36664d65726d61696465722046545721010001daf333300000000000","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"value":0.00000546,"n":0,"scriptPubKey":{"asm":"1
         acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2","desc":"rawtr(acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2)#esyrrkhh","hex":"5120acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2","address":"tb1p4nel7wkc34raczk8c4jwk5cf9d47u2284rxn98rsjrs4w3p2sheqvjmfdh","type":"witness_v1_taproot"}},{"value":0.48753076,"n":1,"scriptPubKey":{"asm":"0
         c035e789d9efffa10aa92e93f48f29b8cfb224c2","desc":"addr(tb1qcq670zweall6zz4f96flfrefhr8myfxz9ll9l2)#whefl5al","hex":"0014c035e789d9efffa10aa92e93f48f29b8cfb224c2","address":"tb1qcq670zweall6zz4f96flfrefhr8myfxz9ll9l2","type":"witness_v0_keyhash"}},{"value":0.00000000,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9ed20a7a43cd5fb65025056bc1722c3ce64d0dfa0f483c915119dd521ab49ed6101","desc":"raw(6a24aa21a9ed20a7a43cd5fb65025056bc1722c3ce64d0dfa0f483c915119dd521ab49ed6101)#hy4sqjuq","hex":"6a24aa21a9ed20a7a43cd5fb65025056bc1722c3ce64d0dfa0f483c915119dd521ab49ed6101","type":"nulldata"}}],"hex":"020000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff230370e62a0423ec36664d65726d61696465722046545721010001daf333300000000000ffffffff032202000000000000225120acf3ff3ad88d47dc0ac7c564eb53092b6bee2947a8cd329c7090e157442a85f2b4e9e70200000000160014c035e789d9efffa10aa92e93f48f29b8cfb224c20000000000000000266a24aa21a9ed20a7a43cd5fb65025056bc1722c3ce64d0dfa0f483c915119dd521ab49ed61010120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"7b5e6b0cd7a1e2f0ea212ab91ecf0612dcad14930d15684562a45d5611e6ca38","hash":"0b432f9a174af3aa19f641dfa4d66cf2be605d2cf9586b88b4c06b8d8884eda9","version":2,"size":234,"vsize":153,"weight":609,"locktime":0,"vin":[{"txid":"43313cb0f90716da5374c688376cd3f81a18171d620262f847d6115fe21f19d5","vout":1,"scriptSig":{"asm":"","hex":""},"txinwitness":["304402206d342fb728914b709bc6ecc566a03f472218e4906aea629e5cf994c2f458d80a022049e357b86cbd6259dac03cfe871854b310b411435c013a010ab5ab85ec5addeb01","02a458c918ee9f27bb1e83b3f7c13fcef250c3ab59e0eebc2de38969803f524f92"],"sequence":4294967295}],"vout":[{"value":0.00019000,"n":0,"scriptPubKey":{"asm":"1
         341434c64f3bedbb704f36d6d02bc277f5027f4634cc9259dfb21d37d555cb30","desc":"rawtr(341434c64f3bedbb704f36d6d02bc277f5027f4634cc9259dfb21d37d555cb30)#rwf7xpfu","hex":"5120341434c64f3bedbb704f36d6d02bc277f5027f4634cc9259dfb21d37d555cb30","address":"tb1pxs2rf3j080kmkuz0xmtdq27zwl6syl6xxnxfykwlkgwn0424evcqfuht0u","type":"witness_v1_taproot"}},{"value":2.93753860,"n":1,"scriptPubKey":{"asm":"0
         70e6089fb7ccbfbcfd049cf971b5d0c2cf9c9c4b","desc":"addr(tb1qwrnq38ahejlmelgynnuhrdwsct8ee8ztk3eygz)#ttzy0tsy","hex":"001470e6089fb7ccbfbcfd049cf971b5d0c2cf9c9c4b","address":"tb1qwrnq38ahejlmelgynnuhrdwsct8ee8ztk3eygz","type":"witness_v0_keyhash"}}],"fee":0.00015300,"hex":"02000000000101d5191fe25f11d647f86202621d17181af8d36c3788c67453da1607f9b03c31430100000000ffffffff02384a000000000000225120341434c64f3bedbb704f36d6d02bc277f5027f4634cc9259dfb21d37d555cb30045482110000000016001470e6089fb7ccbfbcfd049cf971b5d0c2cf9c9c4b0247304402206d342fb728914b709bc6ecc566a03f472218e4906aea629e5cf994c2f458d80a022049e357b86cbd6259dac03cfe871854b310b411435c013a010ab5ab85ec5addeb012102a458c918ee9f27bb1e83b3f7c13fcef250c3ab59e0eebc2de38969803f524f9200000000"},{"txid":"a959ce8f6b3b1c4e4e9f98cce3ca9758c01bf65002a10bcd6f08da5f9212a426","hash":"d25a4a54941695716f815a37ae5382e501c04cc013deac38d6312998f3f65400","version":2,"size":342,"vsize":171,"weight":681,"locktime":0,"vin":[{"txid":"7b5e6b0cd7a1e2f0ea212ab91ecf0612dcad14930d15684562a45d5611e6ca38","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["ec9538cc5687226576550ec96adbd838b09c0f551c16b3dea2ddafbf4afc73a4645c82c037f1bbc8a7d3f0994a3f1b1d2c3cb0ec1040465fa33418f8c9b1c93f","20c7404f01c8507b6a2494250bf52b6654c0e7a2effd94856f4c05b1c1f0bd40deac0063036f7264010118746578742f706c61696e3b636861727365743d7574662d3800387b2270223a226272632d3230222c226f70223a227472616e73666572222c227469636b223a2273617473222c22616d74223a22302e31227d68","c07626552661640d29c076d946b975beadbd14a5bd478acf8c3d1a53bdf96eed05"],"sequence":4294967293}],"vout":[{"value":0.00000546,"n":0,"scriptPubKey":{"asm":"0
         70e6089fb7ccbfbcfd049cf971b5d0c2cf9c9c4b","desc":"addr(tb1qwrnq38ahejlmelgynnuhrdwsct8ee8ztk3eygz)#ttzy0tsy","hex":"001470e6089fb7ccbfbcfd049cf971b5d0c2cf9c9c4b","address":"tb1qwrnq38ahejlmelgynnuhrdwsct8ee8ztk3eygz","type":"witness_v0_keyhash"}},{"value":0.00001354,"n":1,"scriptPubKey":{"asm":"0
         f8f387c2fd764d02fa293f22219db981a6075c2b","desc":"addr(tb1qlrec0shawexs973f8u3zr8desxnqwhptprucdl)#4g4fw228","hex":"0014f8f387c2fd764d02fa293f22219db981a6075c2b","address":"tb1qlrec0shawexs973f8u3zr8desxnqwhptprucdl","type":"witness_v0_keyhash"}}],"fee":0.00017100,"hex":"0200000000010138cae611565da4624568150d9314addc1206cf1eb92a21eaf0e2a1d70c6b5e7b0000000000fdffffff02220200000000000016001470e6089fb7ccbfbcfd049cf971b5d0c2cf9c9c4b4a05000000000000160014f8f387c2fd764d02fa293f22219db981a6075c2b0340ec9538cc5687226576550ec96adbd838b09c0f551c16b3dea2ddafbf4afc73a4645c82c037f1bbc8a7d3f0994a3f1b1d2c3cb0ec1040465fa33418f8c9b1c93f7e20c7404f01c8507b6a2494250bf52b6654c0e7a2effd94856f4c05b1c1f0bd40deac0063036f7264010118746578742f706c61696e3b636861727365743d7574662d3800387b2270223a226272632d3230222c226f70223a227472616e73666572222c227469636b223a2273617473222c22616d74223a22302e31227d6821c07626552661640d29c076d946b975beadbd14a5bd478acf8c3d1a53bdf96eed0500000000"},{"txid":"f288cce13942735be99d247dc1f61c5f073a582d25d5e04631407e6cec986e39","hash":"23e898e24abf54f7670f10495b5cb0e6719f4493ce27f3d0020b94c0bef0d733","version":1,"size":2341,"vsize":2260,"weight":9037,"locktime":0,"vin":[{"txid":"86baae547a6f7fdf2785e618d5854ef4d776059ea9580a7a4e085780c5da91aa","vout":5,"scriptSig":{"asm":"","hex":""},"txinwitness":["3044022060db649f272b45f9696bf52b58324ff5059f42b532178984583d23bed69439ae02206436f48186f01e67c9b93c3958da1d3b6bf4796d435693be9ab3b3aacdec91b301","03a41e8fc42e154ce9bf87c29f4062e4bf9d1cbb5131fad462ea858cec5e664e8c"],"sequence":4294967295}],"vout":[{"value":0.00010000,"n":0,"scriptPubKey":{"asm":"1
@@ -41197,55 +41299,20 @@
       Access-Control-Allow-Origin:
       - ''
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json
       Date:
-      - Sun, 19 May 2024 07:09:09 GMT
+      - Wed, 22 May 2024 19:33:43 GMT
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
-      X-Node-Id:
-      - bitcoin_btc-testnet_iad
-    status:
-      code: 200
-      message: OK
-- request:
-    body: '{"method": "getblockhash", "params": [2811505], "jsonrpc": "2.0", "id":
-      "curltest"}'
-    headers: {}
-    method: POST
-    uri: https://dry-compatible-cloud.btc-testnet.quiknode.pro/268755801856724a0c520053c0bc3b0a7b1a2d3e/
-  response:
-    body:
-      string: '{"result":"000000000000005b9147d9b1afe33b6e26b3131184c440e7d23a7870a7635fe2","error":null,"id":"curltest"}
-
-        '
-    headers:
-      Access-Control-Allow-Credentials:
-      - 'true'
-      Access-Control-Allow-Headers:
-      - Content-Type,Authorization,User-Agent
-      Access-Control-Allow-Methods:
-      - GET, POST, OPTIONS
-      Access-Control-Allow-Origin:
-      - ''
-      Content-Length:
-      - '107'
-      Content-Type:
-      - application/json
-      Date:
-      - Sun, 19 May 2024 07:10:34 GMT
-      Vary:
-      - Accept-Encoding
-      X-Host-Id:
-      - f1b546936d23e3b5-d46e6ad25adfe563
+      - f1b546936d23e3b5-a12d19355fbb795
       X-Node-Id:
       - bitcoin_btc-testnet_iad
     status:
       code: 200
       message: OK
 version: 1
```

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/get_balance.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/get_contract_decimals.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_contract_decimals.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/get_gas_price.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_gas_price.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/get_last_block.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/get_token_balance.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_token_balance.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/get_transaction.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/get_transaction_count.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/get_transaction_count.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/send_token_transaction.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_token_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_token_transaction_with_auto_params.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/send_transaction.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction_with_auto_gas.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/send_transaction_with_custom_nonce.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/eth/test_async_monitoring.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/eth/test_async_monitoring.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -124,8 +124,128 @@
       strict-transport-security:
       - max-age=31536000; includeSubDomains; preload
       x-envoy-upstream-service-time:
       - '8'
     status:
       code: 200
       message: OK
+- request:
+    body: '{"method": "eth_blockNumber", "params": [], "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://ethereum-sepolia-rpc.publicnode.com
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","result":"0x5ae44a","id":1}
+
+        '
+    headers:
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 887f4f980f660639-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:46:11 GMT
+      Server:
+      - cloudflare
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '2'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"method": "eth_blockNumber", "params": [], "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://ethereum-sepolia-rpc.publicnode.com
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","result":"0x5ae44b","id":1}
+
+        '
+    headers:
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 887f4fa55b05946f-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:46:14 GMT
+      Server:
+      - cloudflare
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '2'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"method": "eth_blockNumber", "params": [], "jsonrpc": "2.0", "id": 1}'
+    headers: {}
+    method: POST
+    uri: https://ethereum-sepolia-rpc.publicnode.com
+  response:
+    body:
+      string: '{"jsonrpc":"2.0","result":"0x5ae458","id":1}
+
+        '
+    headers:
+      Access-Control-Max-Age:
+      - '1728000'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 887f53b7298063a0-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '45'
+      Content-Type:
+      - application/json
+      Date:
+      - Wed, 22 May 2024 19:49:00 GMT
+      Server:
+      - cloudflare
+      Vary:
+      - Origin, accept-encoding
+      X-Content-Type-Options:
+      - nosniff
+      alt-svc:
+      - h3=":443"; ma=86400
+      strict-transport-security:
+      - max-age=31536000; includeSubDomains; preload
+      x-envoy-upstream-service-time:
+      - '1'
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/bulk_send_with_auto_fee_and_deduct_commission.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/get_block_by_number.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/get_block_by_number.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/get_last_block.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/get_last_block.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/monitoring_balance_send_mark_as_used.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -496,8 +496,72 @@
       x-ratelimit-persec:
       - '3'
       x-xss-protection:
       - '0'
     status:
       code: 200
       message: OK
+- request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
+  response:
+    body:
+      string: '{"result":3275882,"error":null,"id":"curltest"}'
+    headers:
+      Access-Control-Allow-Origin:
+      - '*'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 887f47e6f818657b-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '47'
+      Content-Type:
+      - application/json; charset=utf-8
+      Date:
+      - Wed, 22 May 2024 19:40:56 GMT
+      Etag:
+      - W/"2f-WtEmcbTmAxiuQk/j+obrNT0AmRg"
+      NEL:
+      - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
+      Report-To:
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=E%2BxzUVu%2B9KY%2BeNzbqujSU63%2FxR8CGVrFs%2FYPhYfauhJP8q7pjrGhdYQNFRfgXVcmfDXG9QVz9iQdsz6T0GeHlvwI4HdObhNeUuCjEM8VWU6XZFKw4hwBl3qKKp16SBU%3D"}],"group":"cf-nel","max_age":604800}'
+      Server:
+      - cloudflare
+      Via:
+      - 1.1 google
+      alt-svc:
+      - h3=":443"; ma=86400
+      content-security-policy:
+      - 'default-src ''self'';base-uri ''self'';block-all-mixed-content;font-src ''self''
+        https: data:;frame-ancestors ''self'';img-src ''self'' data:;object-src ''none'';script-src
+        ''self'';script-src-attr ''none'';style-src ''self'' https: ''unsafe-inline'';upgrade-insecure-requests'
+      expect-ct:
+      - max-age=0
+      referrer-policy:
+      - no-referrer
+      strict-transport-security:
+      - max-age=15552000; includeSubDomains
+      x-content-type-options:
+      - nosniff
+      x-dns-prefetch-control:
+      - 'off'
+      x-download-options:
+      - noopen
+      x-frame-options:
+      - SAMEORIGIN
+      x-lgroup:
+      - v3:::4
+      x-permitted-cross-domain-policies:
+      - none
+      x-ratelimit-persec:
+      - '3'
+      x-xss-protection:
+      - '0'
+    status:
+      code: 200
+      message: OK
 version: 1
```

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_bulk.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_bulk.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_few_single_transactions.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_from_two_utxo.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_to_legacy_address.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_to_legacy_and_segwit_addresses.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_transaction.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_transaction.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_auto_fee.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_auto_fee_and_deduct_commission.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/send_with_fee_per_byte2.yaml`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml` & `aiotx-1.3.0/tests/fixtures/cassettes/ltc/test_async_monitoring.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -2,36 +2,100 @@
 - request:
     body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":3248792,"error":null,"id":"curltest"}'
+      string: '{"result":3275881,"error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87f6ea286fb49584-LHR
+      - 887f3f33ebc279bd-LHR
       Connection:
       - keep-alive
       Content-Length:
       - '47'
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Mon, 06 May 2024 06:29:13 GMT
+      - Wed, 22 May 2024 19:35:00 GMT
       Etag:
-      - W/"2f-VGszqwZqefFJmjtjv2jYlBzuGQ4"
+      - W/"2f-Mex06FydWLd57h5fnKbgHAWLb00"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=3mKegiq2qgcHOYTxb5KA7FTjeROz6mf2XnvIERoT1BqRNgZJdtldiO6KooG5PSkAT1DJ9ELgooU8OMM51KrtEO7%2BBkDMBO3i9E%2FDVVQ9XtuolbGnPV1Rs19hqjosHD4%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=yjh1a1hNN4AWyt8VZJHrTe3t6oC1OEo%2F5dFxS5QIXk8FS14YuH9t1M6gRGqKgLL7mXewrHkt7O2AZnvzXv3QSG22AILlH35%2BJbmSofokng8UyFNFwTVokrHjq33VPgA%3D"}],"group":"cf-nel","max_age":604800}'
+      Server:
+      - cloudflare
+      Via:
+      - 1.1 google
+      alt-svc:
+      - h3=":443"; ma=86400
+      content-security-policy:
+      - 'default-src ''self'';base-uri ''self'';block-all-mixed-content;font-src ''self''
+        https: data:;frame-ancestors ''self'';img-src ''self'' data:;object-src ''none'';script-src
+        ''self'';script-src-attr ''none'';style-src ''self'' https: ''unsafe-inline'';upgrade-insecure-requests'
+      expect-ct:
+      - max-age=0
+      referrer-policy:
+      - no-referrer
+      strict-transport-security:
+      - max-age=15552000; includeSubDomains
+      x-content-type-options:
+      - nosniff
+      x-dns-prefetch-control:
+      - 'off'
+      x-download-options:
+      - noopen
+      x-frame-options:
+      - SAMEORIGIN
+      x-lgroup:
+      - v3:::4
+      x-permitted-cross-domain-policies:
+      - none
+      x-ratelimit-persec:
+      - '3'
+      x-xss-protection:
+      - '0'
+    status:
+      code: 200
+      message: OK
+- request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
+  response:
+    body:
+      string: '{"result":3275881,"error":null,"id":"curltest"}'
+    headers:
+      Access-Control-Allow-Origin:
+      - '*'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 887f3f351d369451-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '47'
+      Content-Type:
+      - application/json; charset=utf-8
+      Date:
+      - Wed, 22 May 2024 19:35:00 GMT
+      Etag:
+      - W/"2f-Mex06FydWLd57h5fnKbgHAWLb00"
+      NEL:
+      - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
+      Report-To:
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=lRI%2FbKACeiEzps7cMJq9S%2Fcs2uh6HIfZR7%2B5X5uGi8kZdReiyd6vpWyYFOQwBaW3h1Kbs89Xuu%2FTwfezs3OENbhTCT2rAsjdV6Uxd8pA1OtZ8FdPS4MVmOafssBPSd4%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Via:
       - 1.1 google
       alt-svc:
       - h3=":443"; ma=86400
       content-security-policy:
@@ -74,29 +138,29 @@
       string: '{"result":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87f6ea2a9c4c48b6-LHR
+      - 887f3f35fc5963f8-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Mon, 06 May 2024 06:29:14 GMT
+      - Wed, 22 May 2024 19:35:00 GMT
       Etag:
       - W/"6a-LkLLyOVV1TG/alYlITH3LlU0UyM"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=FlILk8NoWcZgWdQHshepcJ7TNqS1znvPL%2BilXeDW9AGiQWMZmtn5DbgSHHMR0VkA%2BD58oSgHOyz%2FV88lbjCl7%2FfK3%2FDGIDNe3Cx%2BnBdaI6wSh3bwmvJlmwBPtGVV6ck%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=SfsAHjUYCj6Pj9nms81Iu7Er%2FNBZvlvm%2FxL8k%2FMeSk22BlSSbZMk8pUIInUCa7HlkQKwnydfpbaouuDQc6A%2FacgFEGbmYbWkMAZ%2BmG38Nsk41ocXiNVp5G3JPC8ok0k%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Via:
       - 1.1 google
       alt-svc:
@@ -134,41 +198,41 @@
     body: '{"method": "getblock", "params": ["b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":{"hash":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","confirmations":940,"strippedsize":464,"size":890,"weight":2108,"height":3247853,"version":536870912,"versionHex":"20000000","merkleroot":"983577cb9a5f6d9e0cf17c04a5c330e2a9cd5e54e365b4ecb567e33dee075604","tx":[{"txid":"7604930759225ab74868969da6b19b399d8b189bd9506f39e15019f8e08a1d44","hash":"80a7072798f45aa72450e348c719e169ce72a49995105b927971eae7b4c58732","version":2,"size":171,"vsize":144,"weight":576,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ed8e310101","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"ismweb":false,"value":6.25002728,"n":0,"scriptPubKey":{"asm":"0
+      string: '{"result":{"hash":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","confirmations":28029,"strippedsize":464,"size":890,"weight":2108,"height":3247853,"version":536870912,"versionHex":"20000000","merkleroot":"983577cb9a5f6d9e0cf17c04a5c330e2a9cd5e54e365b4ecb567e33dee075604","tx":[{"txid":"7604930759225ab74868969da6b19b399d8b189bd9506f39e15019f8e08a1d44","hash":"80a7072798f45aa72450e348c719e169ce72a49995105b927971eae7b4c58732","version":2,"size":171,"vsize":144,"weight":576,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ed8e310101","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":4294967295}],"vout":[{"ismweb":false,"value":6.25002728,"n":0,"scriptPubKey":{"asm":"0
         7bd19b7434e4d9c93c534621c23c5eba8a35c187","hex":"00147bd19b7434e4d9c93c534621c23c5eba8a35c187","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q00gekap5unvuj0zngcsuy0z7h29rtsv8d6xwsj"]}},{"ismweb":false,"value":0,"n":1,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d","hex":"6a24aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d","type":"nulldata"}}],"hex":"020000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff0603ed8e310101ffffffff02e8c84025000000001600147bd19b7434e4d9c93c534621c23c5eba8a35c1870000000000000000266a24aa21a9ed30da500691dea788d56838d1733f3dcaeb7cfe3c28e7bb7aac6d41d0ad66886d0120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"51d57f58f3ede964f0105e6a01795cc0df6f275ba4e5d408bc3ba7b57448f74b","hash":"a62d6fb8666b94654acbcf5a541c1848e712af9f96fed8197c0a7b482b3c9802","version":1,"size":370,"vsize":208,"weight":832,"locktime":0,"vin":[{"ismweb":false,"txid":"6b0f1847a67c6d4d40bd557324db7f0258a1d555d3176e666d2420730078c635","vout":0,"scriptSig":{"asm":"","hex":""},"txinwitness":["304402206debc508ebab4d24441cb85fd818c442eb3b803fd5af5fc2c4f5d8ddfae84b64022061b01a7345e8ae0e7558c446e5b9e80afd2f22250aa02f8f70f7c0af29f4ff0d01","035bc96345ad6257836f8c0267a067ac6bd3c9f7dd413f23330cc4f64248977e34"],"sequence":4294967295},{"ismweb":false,"txid":"6b0f1847a67c6d4d40bd557324db7f0258a1d555d3176e666d2420730078c635","vout":1,"scriptSig":{"asm":"","hex":""},"txinwitness":["3044022044c1e352b24403724f97b1d129bbc926a9b5b80fb743b3eeac6f119ee3ca4e5102204abcbc25491be3c6724720dd54cf6ec1e40831fb45fb554f809b92c57fc44fb701","02a1559f3b65652e92b529a5acc64cd9000a6eaa24531f61a7f928028fa3a87ac6"],"sequence":4294967295}],"vout":[{"ismweb":false,"value":6.69379664,"n":0,"scriptPubKey":{"asm":"0
         3efcd669a05d842fb1b05ec45b3b946b8f55774d","hex":"00143efcd669a05d842fb1b05ec45b3b946b8f55774d","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q8m7dv6dqtkzzlvdstmz9kwu5dw842a6d7hd5fr"]}},{"ismweb":false,"value":0.00407272,"n":1,"scriptPubKey":{"asm":"0
         abd50c308b9563c615aeb0eb00752925ab2ff279","hex":"0014abd50c308b9563c615aeb0eb00752925ab2ff279","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1q402scvytj43uv9dwkr4sqaffyk4jlunet2cwyg"]}}],"hex":"0100000000010235c678007320246d666e17d355d5a158027fdb247355bd404d6d7ca647180f6b0000000000ffffffff35c678007320246d666e17d355d5a158027fdb247355bd404d6d7ca647180f6b0100000000ffffffff0250ece527000000001600143efcd669a05d842fb1b05ec45b3b946b8f55774de836060000000000160014abd50c308b9563c615aeb0eb00752925ab2ff2790247304402206debc508ebab4d24441cb85fd818c442eb3b803fd5af5fc2c4f5d8ddfae84b64022061b01a7345e8ae0e7558c446e5b9e80afd2f22250aa02f8f70f7c0af29f4ff0d0121035bc96345ad6257836f8c0267a067ac6bd3c9f7dd413f23330cc4f64248977e3402473044022044c1e352b24403724f97b1d129bbc926a9b5b80fb743b3eeac6f119ee3ca4e5102204abcbc25491be3c6724720dd54cf6ec1e40831fb45fb554f809b92c57fc44fb7012102a1559f3b65652e92b529a5acc64cd9000a6eaa24531f61a7f928028fa3a87ac600000000"},{"txid":"155b9bd93528a805975d549b8891c1de468cdcbf3c41b7cb22042cb6c58417fe","hash":"155b9bd93528a805975d549b8891c1de468cdcbf3c41b7cb22042cb6c58417fe","version":2,"size":97,"vsize":94,"weight":376,"locktime":0,"vin":[{"ismweb":false,"txid":"acee20a3c85c660599447e1f6c298f5009b47622303db4bc6cd3b79e4fea96d3","vout":0,"scriptSig":{"asm":"","hex":""},"sequence":4294967295}],"vout":[{"ismweb":false,"value":1791337.37993343,"n":0,"scriptPubKey":{"asm":"8
         a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","hex":"5820a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","type":"witness_mweb_hogaddr"}}],"hex":"02000000000801d396ea4f9eb7d36cbcb43d302276b409508f296c1f7e449905665cc8a320eeac0000000000ffffffff017f04d2d2eba20000225820a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d570000000000"}],"time":1714833888,"mediantime":1714833364,"nonce":44487,"bits":"1e044362","difficulty":0.000916254800568373,"chainwork":"00000000000000000000000000000000000000000000000000c3adb1cb5e171c","nTx":3,"mweb":{"hash":"a479f8d5e155979028166fc94cdbe0636ba721c75466713b5233f0bf08660d57","height":3247853,"kernel_offset":"9a966bcbe6fcf6b94d7428142a0027b004b1af6a28f2f1999e3d21a565ddb187","stealth_offset":"0000000000000000000000000000000000000000000000000000000000000000","num_kernels":0,"num_txos":4722,"kernel_root":"0000000000000000000000000000000000000000000000000000000000000000","output_root":"69f9f4774c9afd3dab444bbad6df6ae0dcb2c5d6051b5054d7b306a0d348f3c4","leaf_root":"2551128703060a6d3002845179551621ff1d77ce9055933276092f9e7ba97382","inputs":[],"outputs":[],"kernels":[]},"previousblockhash":"c6f01ca05384915909b49a16cfd4a5ea6ec986b1b376c0d31a2fbdc0967d5cb8","nextblockhash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06"},"error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87f6ea2b5db9547b-LHR
+      - 887f3f370818dc57-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Mon, 06 May 2024 06:29:14 GMT
+      - Wed, 22 May 2024 19:35:01 GMT
       Etag:
-      - W/"15e8-Y8Jmn48qDfT1hdy5kmmKkqtbpw0"
+      - W/"15ea-OGS2/PUt10PcgLUlfrGcJ2iVcco"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=w97rJhafQV1sjGEuzKiHBJwLDqoYDNlsYQCUrqlj1r32L9Wr3HBSn3NGR6Ii98y6xJDrWGi2APMOEix9Wyme%2F%2FQOZL%2BzWqbt2PPJAAa3xI86Rycf6QHYddhvBM9nP6U%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=MugukFly0Ov8ab3bWaUgeowEKwDWGuHBlH0yksUdX1GRSijwWNTLFxRgCDs06HcNZo3iFsIwE8tN05bfbbqX3vc%2FA42ol08Xok6EIVgwmUH%2BMHeQwzA8yk9aMSmnaOc%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       Via:
@@ -201,43 +265,107 @@
       - '3'
       x-xss-protection:
       - '0'
     status:
       code: 200
       message: OK
 - request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
+  response:
+    body:
+      string: '{"result":3275881,"error":null,"id":"curltest"}'
+    headers:
+      Access-Control-Allow-Origin:
+      - '*'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 887f3f3e7f6c3865-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '47'
+      Content-Type:
+      - application/json; charset=utf-8
+      Date:
+      - Wed, 22 May 2024 19:35:02 GMT
+      Etag:
+      - W/"2f-Mex06FydWLd57h5fnKbgHAWLb00"
+      NEL:
+      - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
+      Report-To:
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=uwasWBwNEnrPXCg4D555jRJBEb%2BqLuuZZL8OgkLD3vT%2FzQJoBsTKh%2B01J%2F7ZcVYEvNeIeb6LtTWc%2Bkx65ljFdS24f17YyB0dC6%2FbszGdtLW0SydGaUeaXg63IwpmZEg%3D"}],"group":"cf-nel","max_age":604800}'
+      Server:
+      - cloudflare
+      Via:
+      - 1.1 google
+      alt-svc:
+      - h3=":443"; ma=86400
+      content-security-policy:
+      - 'default-src ''self'';base-uri ''self'';block-all-mixed-content;font-src ''self''
+        https: data:;frame-ancestors ''self'';img-src ''self'' data:;object-src ''none'';script-src
+        ''self'';script-src-attr ''none'';style-src ''self'' https: ''unsafe-inline'';upgrade-insecure-requests'
+      expect-ct:
+      - max-age=0
+      referrer-policy:
+      - no-referrer
+      strict-transport-security:
+      - max-age=15552000; includeSubDomains
+      x-content-type-options:
+      - nosniff
+      x-dns-prefetch-control:
+      - 'off'
+      x-download-options:
+      - noopen
+      x-frame-options:
+      - SAMEORIGIN
+      x-lgroup:
+      - v3:::4
+      x-permitted-cross-domain-policies:
+      - none
+      x-ratelimit-persec:
+      - '3'
+      x-xss-protection:
+      - '0'
+    status:
+      code: 200
+      message: OK
+- request:
     body: '{"method": "getblockhash", "params": [3247854], "jsonrpc": "2.0", "id":
       "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
       string: '{"result":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06","error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87f6ea326ac160f6-LHR
+      - 887f3f3f7bcc632b-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Mon, 06 May 2024 06:29:15 GMT
+      - Wed, 22 May 2024 19:35:02 GMT
       Etag:
       - W/"6a-AlT1INyeQ1FXH50qhJDUOe3VEos"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=F2K6fwjENosOf%2F0nAJ4EZY3Hd7IOhsFLzZi2K8oEXaFtR%2FI1hUDbBf0CpPVO6CuAh6SVzcJpTZ%2B9aqyxWrbE7d8rgnicLXf9TLjE%2FvojR4x5o88objfa9gEr0PKauxk%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=i8T1dTg0W6S2ClXFfkYj8nngF2mS3cge4nmA4E9UAPnffv2PfdgFG8AJfuYlBJI7p7xc6OAdFPhUi7DLxfprfmxjEI7Rp5QmUuPOnajQMJly5DqEL8Bvq2ep7ZrOzq0%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Via:
       - 1.1 google
       alt-svc:
@@ -275,40 +403,40 @@
     body: '{"method": "getblock", "params": ["6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":{"hash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06","confirmations":939,"strippedsize":435,"size":645,"weight":1776,"height":3247854,"version":536870912,"versionHex":"20000000","merkleroot":"9e036e586c8202e96cfbd92437e113ed23359a1e071cfc040dd3432e6fdce386","tx":[{"txid":"40d43cdee20338c0002597d00d52daadc66fb4e8a6af9a002c1da84ca7cfb170","hash":"ec1d51a86c4111648da61cb2a7755c46e999ce012d381eae0000fe393255ab8d","version":1,"size":296,"vsize":269,"weight":1076,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ee8e3104e94936660861803ced00000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":0}],"vout":[{"ismweb":false,"value":6.249375,"n":0,"scriptPubKey":{"asm":"0
+      string: '{"result":{"hash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06","confirmations":28028,"strippedsize":435,"size":645,"weight":1776,"height":3247854,"version":536870912,"versionHex":"20000000","merkleroot":"9e036e586c8202e96cfbd92437e113ed23359a1e071cfc040dd3432e6fdce386","tx":[{"txid":"40d43cdee20338c0002597d00d52daadc66fb4e8a6af9a002c1da84ca7cfb170","hash":"ec1d51a86c4111648da61cb2a7755c46e999ce012d381eae0000fe393255ab8d","version":1,"size":296,"vsize":269,"weight":1076,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ee8e3104e94936660861803ced00000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":0}],"vout":[{"ismweb":false,"value":6.249375,"n":0,"scriptPubKey":{"asm":"0
         94a1914d5e14ba06b02bb9d2b0b672f2fd125415","hex":"001494a1914d5e14ba06b02bb9d2b0b672f2fd125415","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1qjjsezn27zjaqdvpth8ftpdnj7t73y4q4vja4dq"]}},{"ismweb":false,"value":0.000625,"n":1,"scriptPubKey":{"asm":"OP_DUP
         OP_HASH160 684a4a9d1c027eddb12029e40ccd86215360790a OP_EQUALVERIFY OP_CHECKSIG","hex":"76a914684a4a9d1c027eddb12029e40ccd86215360790a88ac","reqSigs":1,"type":"pubkeyhash","addresses":["mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX"]}},{"ismweb":false,"value":0,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9ede746e1e45c418a43d974963c15c7d4ecd9e02232cf06849f9d091b841f001746","hex":"6a24aa21a9ede746e1e45c418a43d974963c15c7d4ecd9e02232cf06849f9d091b841f001746","type":"nulldata"}}],"hex":"010000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff6103ee8e3104e94936660861803ced00000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f00000000031cca3f250000000016001494a1914d5e14ba06b02bb9d2b0b672f2fd12541524f40000000000001976a914684a4a9d1c027eddb12029e40ccd86215360790a88ac0000000000000000266a24aa21a9ede746e1e45c418a43d974963c15c7d4ecd9e02232cf06849f9d091b841f0017460120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"992b887a10aa924430e905174535fd92733136b76d39e835c109e3ff2719bd69","hash":"992b887a10aa924430e905174535fd92733136b76d39e835c109e3ff2719bd69","version":2,"size":97,"vsize":94,"weight":376,"locktime":0,"vin":[{"ismweb":false,"txid":"155b9bd93528a805975d549b8891c1de468cdcbf3c41b7cb22042cb6c58417fe","vout":0,"scriptSig":{"asm":"","hex":""},"sequence":4294967295}],"vout":[{"ismweb":false,"value":1791337.37993343,"n":0,"scriptPubKey":{"asm":"8
         086024bcc947aadc5053e0a51bcaabf1f7b4c264904fb72fa3f05c47dfb7575e","hex":"5820086024bcc947aadc5053e0a51bcaabf1f7b4c264904fb72fa3f05c47dfb7575e","type":"witness_mweb_hogaddr"}}],"hex":"02000000000801fe1784c5b62c0422cbb7413cbfdc8c46dec191889b545d9705a82835d99b5b150000000000ffffffff017f04d2d2eba20000225820086024bcc947aadc5053e0a51bcaabf1f7b4c264904fb72fa3f05c47dfb7575e0000000000"}],"time":1714833897,"mediantime":1714833369,"nonce":945226240,"bits":"1e044362","difficulty":0.000916254800568373,"chainwork":"00000000000000000000000000000000000000000000000000c3adb1cb9a238c","nTx":2,"mweb":{"hash":"086024bcc947aadc5053e0a51bcaabf1f7b4c264904fb72fa3f05c47dfb7575e","height":3247854,"kernel_offset":"9a966bcbe6fcf6b94d7428142a0027b004b1af6a28f2f1999e3d21a565ddb187","stealth_offset":"0000000000000000000000000000000000000000000000000000000000000000","num_kernels":0,"num_txos":4722,"kernel_root":"0000000000000000000000000000000000000000000000000000000000000000","output_root":"69f9f4774c9afd3dab444bbad6df6ae0dcb2c5d6051b5054d7b306a0d348f3c4","leaf_root":"2551128703060a6d3002845179551621ff1d77ce9055933276092f9e7ba97382","inputs":[],"outputs":[],"kernels":[]},"previousblockhash":"b76c047e07af580555082792b2007dc969a6036391cd5aba915ec3c73755b80b","nextblockhash":"2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9"},"error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87f6ea33a90c48cd-LHR
+      - 887f3f405a7994b1-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Mon, 06 May 2024 06:29:15 GMT
+      - Wed, 22 May 2024 19:35:02 GMT
       Etag:
-      - W/"fd6-Vp1fkFZYOYkVcldYilDUrhCFXAk"
+      - W/"fd8-L3m7sczC/tWMcqT7Gz0MygeT6hk"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=BeP6quUsHMcNjjfd3xE1Ea1dB6CQVsmxrHGY5yo1c8y%2BJf2os4XRxxMmj0ssv2vprnjmATTvuznbwqSsIwUajFQpEqOAK0EqmVbXc1Rkcokuund3TRcKHmTB9lYzSEo%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=rYP3Fbu3el%2BFfnIoI2VhZ%2FKBQyVarsh4GpA9jQBZATUgLZmmmBCviTX2uw4tderAgO%2Bg2rmacRqF17jZsNruVPq%2BBZ%2BWTwaImQ1HiKblZHP%2FAGBtggF9RHLglwwQcNw%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       Via:
@@ -341,43 +469,107 @@
       - '3'
       x-xss-protection:
       - '0'
     status:
       code: 200
       message: OK
 - request:
+    body: '{"method": "getblockcount", "params": [], "jsonrpc": "2.0", "id": "curltest"}'
+    headers: {}
+    method: POST
+    uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
+  response:
+    body:
+      string: '{"result":3275882,"error":null,"id":"curltest"}'
+    headers:
+      Access-Control-Allow-Origin:
+      - '*'
+      CF-Cache-Status:
+      - DYNAMIC
+      CF-RAY:
+      - 887f4802ee7f732a-LHR
+      Connection:
+      - keep-alive
+      Content-Length:
+      - '47'
+      Content-Type:
+      - application/json; charset=utf-8
+      Date:
+      - Wed, 22 May 2024 19:41:01 GMT
+      Etag:
+      - W/"2f-WtEmcbTmAxiuQk/j+obrNT0AmRg"
+      NEL:
+      - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
+      Report-To:
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=9l%2F8HsBt69aBEhwjU6R0KozvcpZFMH84sZz0Cjvxc1slbtIi6DqCG92lON5O0V7Y98FuoZ7%2BykQraEriNuknHZk8wQInrZtdXewc0rckwwO5Dw8ILMKy1Hr1h1KPfJA%3D"}],"group":"cf-nel","max_age":604800}'
+      Server:
+      - cloudflare
+      Via:
+      - 1.1 google
+      alt-svc:
+      - h3=":443"; ma=86400
+      content-security-policy:
+      - 'default-src ''self'';base-uri ''self'';block-all-mixed-content;font-src ''self''
+        https: data:;frame-ancestors ''self'';img-src ''self'' data:;object-src ''none'';script-src
+        ''self'';script-src-attr ''none'';style-src ''self'' https: ''unsafe-inline'';upgrade-insecure-requests'
+      expect-ct:
+      - max-age=0
+      referrer-policy:
+      - no-referrer
+      strict-transport-security:
+      - max-age=15552000; includeSubDomains
+      x-content-type-options:
+      - nosniff
+      x-dns-prefetch-control:
+      - 'off'
+      x-download-options:
+      - noopen
+      x-frame-options:
+      - SAMEORIGIN
+      x-lgroup:
+      - v3:::4
+      x-permitted-cross-domain-policies:
+      - none
+      x-ratelimit-persec:
+      - '3'
+      x-xss-protection:
+      - '0'
+    status:
+      code: 200
+      message: OK
+- request:
     body: '{"method": "getblockhash", "params": [3247855], "jsonrpc": "2.0", "id":
       "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
       string: '{"result":"2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9","error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87f6ea3b0ac56557-LHR
+      - 887f48039a8a52a6-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Mon, 06 May 2024 06:29:16 GMT
+      - Wed, 22 May 2024 19:41:01 GMT
       Etag:
       - W/"6a-NIsU6VTx+O5+ZiMXacgz3yRGZ4w"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=511x3CeuFllDPCSQ56A1hNKAQah3HSi7C2xtvpv6oHkJZ5Cu9FStumH2Cu6So2uBU5rKDY1vCkhemogLSX2DtRiP9oHLEn2jHXnXjZcjZ1s%2FyGduC2nwa6LVImPW%2BcM%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=yFLKFTQunYOoUHPrWXL48Bj8YZ%2BjvuvhFrUOiLfXwm39NVQFgNC9zz4NHZQoamAtsJQK6jFY6F%2BgD5EHSP5gvnYppD3VJpT3PgBdABSIlPsHqL2HSliSuWmrJZVh0BA%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Via:
       - 1.1 google
       alt-svc:
@@ -415,40 +607,40 @@
     body: '{"method": "getblock", "params": ["2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9",
       2], "jsonrpc": "2.0", "id": "curltest"}'
     headers: {}
     method: POST
     uri: https://api.tatum.io/v3/blockchain/node/litecoin-core-testnet
   response:
     body:
-      string: '{"result":{"hash":"2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9","confirmations":938,"strippedsize":435,"size":645,"weight":1776,"height":3247855,"version":536870912,"versionHex":"20000000","merkleroot":"ea7d884bbc471d6c6ca1373c718fa8e24c0a57d280e5a4c2b633b1743d1712cd","tx":[{"txid":"cc2f6dcf37ee8cf019145c2a3eaabf70f14a42dd9aa5f31ed1baa549716fe7b9","hash":"26cd1fbff30b0fadb066f00de9f86ff29f3a54360dbfc528d9b02f489f1704b4","version":1,"size":296,"vsize":269,"weight":1076,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ef8e3104ff49366608bf4bc2d500000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":0}],"vout":[{"ismweb":false,"value":6.249375,"n":0,"scriptPubKey":{"asm":"0
+      string: '{"result":{"hash":"2466170a397703ccbeb3a3402b201deafd47503a08b3538adafc42308260a4e9","confirmations":28028,"strippedsize":435,"size":645,"weight":1776,"height":3247855,"version":536870912,"versionHex":"20000000","merkleroot":"ea7d884bbc471d6c6ca1373c718fa8e24c0a57d280e5a4c2b633b1743d1712cd","tx":[{"txid":"cc2f6dcf37ee8cf019145c2a3eaabf70f14a42dd9aa5f31ed1baa549716fe7b9","hash":"26cd1fbff30b0fadb066f00de9f86ff29f3a54360dbfc528d9b02f489f1704b4","version":1,"size":296,"vsize":269,"weight":1076,"locktime":0,"vin":[{"ismweb":false,"coinbase":"03ef8e3104ff49366608bf4bc2d500000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f","txinwitness":["0000000000000000000000000000000000000000000000000000000000000000"],"sequence":0}],"vout":[{"ismweb":false,"value":6.249375,"n":0,"scriptPubKey":{"asm":"0
         94a1914d5e14ba06b02bb9d2b0b672f2fd125415","hex":"001494a1914d5e14ba06b02bb9d2b0b672f2fd125415","reqSigs":1,"type":"witness_v0_keyhash","addresses":["tltc1qjjsezn27zjaqdvpth8ftpdnj7t73y4q4vja4dq"]}},{"ismweb":false,"value":0.000625,"n":1,"scriptPubKey":{"asm":"OP_DUP
         OP_HASH160 684a4a9d1c027eddb12029e40ccd86215360790a OP_EQUALVERIFY OP_CHECKSIG","hex":"76a914684a4a9d1c027eddb12029e40ccd86215360790a88ac","reqSigs":1,"type":"pubkeyhash","addresses":["mq2PZs9p5ZNLbu23KLKb1tdQt1mrBJM7CX"]}},{"ismweb":false,"value":0,"n":2,"scriptPubKey":{"asm":"OP_RETURN
         aa21a9edb2b3b4be9f62e0f20409d7bddecca7547ef5254dc0c6978a3985ffb60215ad8e","hex":"6a24aa21a9edb2b3b4be9f62e0f20409d7bddecca7547ef5254dc0c6978a3985ffb60215ad8e","type":"nulldata"}}],"hex":"010000000001010000000000000000000000000000000000000000000000000000000000000000ffffffff6103ef8e3104ff49366608bf4bc2d500000000482f6a61616a506f6f6ce29b8fefb88f2068747470733a2f2f6a61616a2e70616765732e64657620f09f918841736b20666f72206672656520744c54432c206f72206d696e652077697468206d652f00000000031cca3f250000000016001494a1914d5e14ba06b02bb9d2b0b672f2fd12541524f40000000000001976a914684a4a9d1c027eddb12029e40ccd86215360790a88ac0000000000000000266a24aa21a9edb2b3b4be9f62e0f20409d7bddecca7547ef5254dc0c6978a3985ffb60215ad8e0120000000000000000000000000000000000000000000000000000000000000000000000000"},{"txid":"39aea883ba364db920f2f8e36e326491749b2a576306ed253223860efcda1e0c","hash":"39aea883ba364db920f2f8e36e326491749b2a576306ed253223860efcda1e0c","version":2,"size":97,"vsize":94,"weight":376,"locktime":0,"vin":[{"ismweb":false,"txid":"992b887a10aa924430e905174535fd92733136b76d39e835c109e3ff2719bd69","vout":0,"scriptSig":{"asm":"","hex":""},"sequence":4294967295}],"vout":[{"ismweb":false,"value":1791337.37993343,"n":0,"scriptPubKey":{"asm":"8
         fc6a93f9d465d93d5f82974181c905e1ddf4c4705439109f7f38403ee8f771bb","hex":"5820fc6a93f9d465d93d5f82974181c905e1ddf4c4705439109f7f38403ee8f771bb","type":"witness_mweb_hogaddr"}}],"hex":"0200000000080169bd1927ffe309c135e8396db736317392fd35451705e9304492aa107a882b990000000000ffffffff017f04d2d2eba20000225820fc6a93f9d465d93d5f82974181c905e1ddf4c4705439109f7f38403ee8f771bb0000000000"}],"time":1714833919,"mediantime":1714833495,"nonce":4096197120,"bits":"1e044362","difficulty":0.000916254800568373,"chainwork":"00000000000000000000000000000000000000000000000000c3adb1cbd62ffc","nTx":2,"mweb":{"hash":"fc6a93f9d465d93d5f82974181c905e1ddf4c4705439109f7f38403ee8f771bb","height":3247855,"kernel_offset":"9a966bcbe6fcf6b94d7428142a0027b004b1af6a28f2f1999e3d21a565ddb187","stealth_offset":"0000000000000000000000000000000000000000000000000000000000000000","num_kernels":0,"num_txos":4722,"kernel_root":"0000000000000000000000000000000000000000000000000000000000000000","output_root":"69f9f4774c9afd3dab444bbad6df6ae0dcb2c5d6051b5054d7b306a0d348f3c4","leaf_root":"2551128703060a6d3002845179551621ff1d77ce9055933276092f9e7ba97382","inputs":[],"outputs":[],"kernels":[]},"previousblockhash":"6d91b4b01d3e22c0ac7d7deefcba7427004b02a7184f1eb6f528590177302b06","nextblockhash":"5105e7d547d990af00aeb27bf86187c2ff0a0274899e14723745e1403a931bc1"},"error":null,"id":"curltest"}'
     headers:
       Access-Control-Allow-Origin:
       - '*'
       CF-Cache-Status:
       - DYNAMIC
       CF-RAY:
-      - 87f6ea3bace563d7-LHR
+      - 887f4804398e7755-LHR
       Connection:
       - keep-alive
       Content-Encoding:
       - gzip
       Content-Type:
       - application/json; charset=utf-8
       Date:
-      - Mon, 06 May 2024 06:29:16 GMT
+      - Wed, 22 May 2024 19:41:01 GMT
       Etag:
-      - W/"fd7-946Hn+hqC84SMNRjTSfXcVVNXto"
+      - W/"fd9-rep8mOK12o4vPxzg0POAXkZ0nqw"
       NEL:
       - '{"success_fraction":0,"report_to":"cf-nel","max_age":604800}'
       Report-To:
-      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=xugW16nHfuqbkym1kU3aa6ykNnvv7RUbjbItscCj5%2BPoopPPD4FjMzg9AjV%2FwPz7UPGwIDpW9xr4QsFxVxrSReQaDbPNfm%2BmogLgdGF0Ac9SR0XW%2FAI1GBpqbAiqN6Q%3D"}],"group":"cf-nel","max_age":604800}'
+      - '{"endpoints":[{"url":"https:\/\/a.nel.cloudflare.com\/report\/v4?s=byHQLow2dNJrMpwPeE6eWOicupskebvn%2FTqr5Nk4FeHTSXv%2BXrZmTiJ6L9IMv41pmt28ckURvf3I8cghQV2d7xE%2BhRiuPYE7deN5lVgtImex1j3bLRmGbOmICW1EBJE%3D"}],"group":"cf-nel","max_age":604800}'
       Server:
       - cloudflare
       Transfer-Encoding:
       - chunked
       Vary:
       - Accept-Encoding
       Via:
```

### Comparing `aiotx-1.2.5/tests/fixtures/networks.json` & `aiotx-1.3.0/tests/fixtures/networks.json`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/test_evm/test_bsc/test_bsc_client.py` & `aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/test_evm/test_bsc/test_bsc_input_decoding.py` & `aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/test_evm/test_bsc/test_bsc_monitoring.py` & `aiotx-1.3.0/tests/test_evm/test_bsc/test_bsc_monitoring.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-import asyncio
+# import asyncio
 
-from conftest import vcr_c
+# from conftest import vcr_c
 
-from aiotx.clients import AioTxBSCClient
+# from aiotx.clients import AioTxBSCClient
 
 
-@vcr_c.use_cassette("tests/fixtures/cassettes/bsc/test_async_monitoring.yaml")
-async def test_async_monitoring(bsc_client: AioTxBSCClient):
-    blocks = []
-    transactions = []
+# @vcr_c.use_cassette("tests/fixtures/cassettes/bsc/test_async_monitoring.yaml")
+# async def test_async_monitoring(bsc_client: AioTxBSCClient):
+#     blocks = []
+#     transactions = []
 
-    @bsc_client.monitor.on_block
-    async def handle_block(block):
-        blocks.append(block)
+#     @bsc_client.monitor.on_block
+#     async def handle_block(block):
+#         blocks.append(block)
 
-    @bsc_client.monitor.on_transaction
-    async def handle_transaction(transaction):
-        transactions.append(transaction)
+#     @bsc_client.monitor.on_transaction
+#     async def handle_transaction(transaction):
+#         transactions.append(transaction)
 
-    await bsc_client.start_monitoring(584)
-    try:
-        await asyncio.sleep(3)
-    except KeyboardInterrupt:
-        bsc_client.stop_monitoring()
+#     await bsc_client.start_monitoring(584)
+#     try:
+#         await asyncio.sleep(3)
+#     except KeyboardInterrupt:
+#         bsc_client.stop_monitoring()
 
-    assert len(blocks) > 0
-    assert len(transactions) > 0
+#     assert len(blocks) > 0
+#     assert len(transactions) > 0
 
-    assert 584 in blocks
-    assert 585 in blocks
-    assert "0x2a9d5aea2c8e4759e4e664f48e0dac79e76cb024e670251ddb2788144cee6f43" in [tx["hash"] for tx in transactions]
-    assert "0xa45ccbf3c820f7bec2809461a8b7f1856246ed3b650ec2840bfbc303f118b76c" in [tx["hash"] for tx in transactions]
+#     assert 584 in blocks
+#     assert 585 in blocks
+#     assert "0x2a9d5aea2c8e4759e4e664f48e0dac79e76cb024e670251ddb2788144cee6f43" in [tx["hash"] for tx in transactions]
+#     assert "0xa45ccbf3c820f7bec2809461a8b7f1856246ed3b650ec2840bfbc303f118b76c" in [tx["hash"] for tx in transactions]
 
-    for tx in transactions:
-        assert "aiotx_decoded_input" in tx.keys()
+#     for tx in transactions:
+#         assert "aiotx_decoded_input" in tx.keys()
```

### Comparing `aiotx-1.2.5/tests/test_evm/test_eth/test_eth_client.py` & `aiotx-1.3.0/tests/test_evm/test_eth/test_eth_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/test_evm/test_eth/test_eth_input_decoding.py` & `aiotx-1.3.0/tests/test_evm/test_eth/test_eth_input_decoding.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/test_evm/test_eth/test_eth_monitoring.py` & `aiotx-1.3.0/tests/test_evm/test_eth/test_eth_monitoring.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/test_utxo/test_btc/test_btc_client.py` & `aiotx-1.3.0/tests/test_utxo/test_btc/test_btc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,14 @@
         conf_target=1,
         estimate_mode=FeeEstimate.CONSERVATIVE,
     )
     
     assert tx_id == "77cb20c4b0325242b9e5f45f4850e5387dc585d6b72bb36ba65a126534436973"
 
     utxo_list = await btc_client.monitor._get_utxo_data(TEST_BTC_ADDRESS)
-    print("utxo_list", utxo_list)
     assert len(utxo_list) == 0
 
 
 
 
 async def test_get_balance(btc_client: AioTxBTCClient):
     await btc_client.monitor._add_new_address(TEST_BTC_ADDRESS)
```

### Comparing `aiotx-1.2.5/tests/test_utxo/test_btc/test_btc_monitor.py` & `aiotx-1.3.0/tests/test_utxo/test_btc/test_btc_monitor.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/test_utxo/test_ltc/test_ltc_client.py` & `aiotx-1.3.0/tests/test_utxo/test_ltc/test_ltc_client.py`

 * *Files identical despite different names*

### Comparing `aiotx-1.2.5/tests/test_utxo/test_ltc/test_ltc_monitor.py` & `aiotx-1.3.0/tests/test_utxo/test_ltc/test_ltc_monitor.py`

 * *Files identical despite different names*

