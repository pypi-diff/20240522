# Comparing `tmp/bittensor-6.9.2.tar.gz` & `tmp/bittensor-6.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-6.9.2.tar", last modified: Fri Mar  8 22:10:32 2024, max compression
+gzip compressed data, was "bittensor-6.9.3.tar", last modified: Tue Mar 12 21:55:13 2024, max compression
```

## Comparing `bittensor-6.9.2.tar` & `bittensor-6.9.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.389206 bittensor-6.9.2/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1087 2023-12-07 03:49:27.000000 bittensor-6.9.2/LICENSE
--rw-rw-r--   0 phil      (1007) phil      (1008)    18529 2024-03-08 22:10:32.385206 bittensor-6.9.2/PKG-INFO
--rw-rw-r--   0 phil      (1007) phil      (1008)    17503 2024-03-01 00:22:30.000000 bittensor-6.9.2/README.md
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.377206 bittensor-6.9.2/bin/
--rwxrwxr-x   0 phil      (1007) phil      (1008)     2012 2024-01-15 16:21:51.000000 bittensor-6.9.2/bin/btcli
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.381206 bittensor-6.9.2/bittensor/
--rw-rw-r--   0 phil      (1007) phil      (1008)     7480 2024-03-08 15:59:04.000000 bittensor-6.9.2/bittensor/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    67213 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/axon.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    11584 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/btlogging.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    38473 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/chain_data.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    11194 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/cli.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.381206 bittensor-6.9.2/bittensor/commands/
--rw-rw-r--   0 phil      (1007) phil      (1008)     3913 2024-01-15 16:21:51.000000 bittensor-6.9.2/bittensor/commands/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    38241 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/commands/delegates.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    13519 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/identity.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    11154 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/inspect.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4926 2024-01-26 17:31:18.000000 bittensor-6.9.2/bittensor/commands/list.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10770 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/commands/metagraph.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5096 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/misc.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    25534 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/commands/network.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    30254 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/overview.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    25769 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/register.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    28679 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/root.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    23862 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/senate.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    23616 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/stake.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5781 2024-01-26 17:31:18.000000 bittensor-6.9.2/bittensor/commands/transfer.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    13182 2024-01-26 17:31:18.000000 bittensor-6.9.2/bittensor/commands/unstake.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     9078 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/commands/utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    41533 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/commands/wallets.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    14128 2024-03-06 20:18:48.000000 bittensor-6.9.2/bittensor/config.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    37824 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/dendrite.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     4283 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/errors.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.385206 bittensor-6.9.2/bittensor/extrinsics/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1120 2023-12-07 03:49:27.000000 bittensor-6.9.2/bittensor/extrinsics/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    14777 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/extrinsics/delegation.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8768 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/extrinsics/network.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6046 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/extrinsics/prometheus.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    20397 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/extrinsics/registration.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8992 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/extrinsics/root.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    11054 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/extrinsics/senate.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    11140 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/extrinsics/serving.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5644 2024-03-06 15:29:34.000000 bittensor-6.9.2/bittensor/extrinsics/set_weights.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    19314 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/extrinsics/staking.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6640 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/extrinsics/transfer.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    16331 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/extrinsics/unstaking.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    32032 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/keyfile.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    47097 2024-03-08 22:01:57.000000 bittensor-6.9.2/bittensor/metagraph.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.385206 bittensor-6.9.2/bittensor/mock/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1186 2023-12-07 03:49:27.000000 bittensor-6.9.2/bittensor/mock/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3216 2023-12-07 03:49:27.000000 bittensor-6.9.2/bittensor/mock/keyfile_mock.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    51533 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/mock/subtensor_mock.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5030 2023-12-07 03:49:27.000000 bittensor-6.9.2/bittensor/mock/wallet_mock.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6981 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/stream.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3283 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/subnets.py
--rw-rw-r--   0 phil      (1007) phil      (1008)   193536 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/subtensor.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    35031 2024-03-08 00:09:09.000000 bittensor-6.9.2/bittensor/synapse.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6891 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/tensor.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10401 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/threadpool.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     1510 2023-12-07 03:49:27.000000 bittensor-6.9.2/bittensor/types.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.385206 bittensor-6.9.2/bittensor/utils/
--rw-rw-r--   0 phil      (1007) phil      (1008)     7560 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/utils/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3527 2024-02-14 21:36:16.000000 bittensor-6.9.2/bittensor/utils/_register_cuda.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    10075 2024-02-14 21:36:16.000000 bittensor-6.9.2/bittensor/utils/balance.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      553 2023-12-07 03:49:27.000000 bittensor-6.9.2/bittensor/utils/formatting.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5784 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/utils/networking.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    37774 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/utils/registration.py
--rw-rw-r--   0 phil      (1007) phil      (1008)      630 2023-12-07 03:49:27.000000 bittensor-6.9.2/bittensor/utils/test_utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     6327 2024-01-09 17:50:11.000000 bittensor-6.9.2/bittensor/utils/wallet_utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    11141 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/utils/weight_utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    33414 2024-03-01 00:22:30.000000 bittensor-6.9.2/bittensor/wallet.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.381206 bittensor-6.9.2/bittensor.egg-info/
--rw-r--r--   0 phil      (1007) phil      (1008)    18529 2024-03-08 22:10:32.000000 bittensor-6.9.2/bittensor.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1007) phil      (1008)     2700 2024-03-08 22:10:32.000000 bittensor-6.9.2/bittensor.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)        1 2024-03-08 22:10:32.000000 bittensor-6.9.2/bittensor.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)      730 2024-03-08 22:10:32.000000 bittensor-6.9.2/bittensor.egg-info/requires.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)       16 2024-03-08 22:10:32.000000 bittensor-6.9.2/bittensor.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1007) phil      (1008)       38 2024-03-08 22:10:32.389206 bittensor-6.9.2/setup.cfg
--rw-rw-r--   0 phil      (1007) phil      (1008)     3705 2023-12-19 18:04:34.000000 bittensor-6.9.2/setup.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.385206 bittensor-6.9.2/tests/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1202 2023-12-07 03:49:27.000000 bittensor-6.9.2/tests/__init__.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.385206 bittensor-6.9.2/tests/helpers/
--rw-rw-r--   0 phil      (1007) phil      (1008)     1308 2023-12-07 03:49:27.000000 bittensor-6.9.2/tests/helpers/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5565 2023-12-07 03:49:27.000000 bittensor-6.9.2/tests/helpers/helpers.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.385206 bittensor-6.9.2/tests/integration_tests/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2023-12-07 03:49:27.000000 bittensor-6.9.2/tests/integration_tests/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    86929 2024-03-08 00:09:09.000000 bittensor-6.9.2/tests/integration_tests/test_cli.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    49428 2024-01-15 16:21:51.000000 bittensor-6.9.2/tests/integration_tests/test_cli_no_network.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     3450 2023-12-07 03:49:27.000000 bittensor-6.9.2/tests/integration_tests/test_metagraph_integration.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    23150 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/integration_tests/test_subtensor_integration.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.385206 bittensor-6.9.2/tests/unit_tests/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2023-12-07 03:49:27.000000 bittensor-6.9.2/tests/unit_tests/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8119 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/test_axon.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    15306 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/test_chain_data.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     8228 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/test_dendrite.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    21841 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/test_keyfile.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5969 2024-03-08 17:51:38.000000 bittensor-6.9.2/tests/unit_tests/test_metagraph.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5605 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/test_subtensor.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     7559 2024-02-15 00:33:15.000000 bittensor-6.9.2/tests/unit_tests/test_synapse.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5648 2023-12-07 03:49:27.000000 bittensor-6.9.2/tests/unit_tests/test_tensor.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    17894 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/test_wallet.py
-drwxrwxr-x   0 phil      (1007) phil      (1008)        0 2024-03-08 22:10:32.385206 bittensor-6.9.2/tests/unit_tests/utils/
--rw-rw-r--   0 phil      (1007) phil      (1008)        0 2023-12-07 03:49:27.000000 bittensor-6.9.2/tests/unit_tests/utils/__init__.py
--rw-rw-r--   0 phil      (1007) phil      (1008)    15327 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/utils/test_balance.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     5390 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/utils/test_networking.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     9661 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/utils/test_utils.py
--rw-rw-r--   0 phil      (1007) phil      (1008)     9661 2024-03-01 00:22:30.000000 bittensor-6.9.2/tests/unit_tests/utils/test_weight_utils.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.926277 bittensor-6.9.3/
+-rw-r--r--   0 alashaabana   (501) staff       (20)     1087 2022-12-14 19:12:32.000000 bittensor-6.9.3/LICENSE
+-rw-r--r--   0 alashaabana   (501) staff       (20)    18529 2024-03-12 21:55:13.926085 bittensor-6.9.3/PKG-INFO
+-rw-r--r--   0 alashaabana   (501) staff       (20)    17503 2024-02-26 16:25:46.000000 bittensor-6.9.3/README.md
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.912416 bittensor-6.9.3/bin/
+-rwxr-xr-x   0 alashaabana   (501) staff       (20)     2012 2024-01-15 19:02:35.000000 bittensor-6.9.3/bin/btcli
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.915516 bittensor-6.9.3/bittensor/
+-rw-r--r--   0 alashaabana   (501) staff       (20)     7480 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    67213 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/axon.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    11584 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/btlogging.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    38877 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/chain_data.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    11194 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/cli.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.918824 bittensor-6.9.3/bittensor/commands/
+-rw-r--r--   0 alashaabana   (501) staff       (20)     3913 2024-01-15 19:02:35.000000 bittensor-6.9.3/bittensor/commands/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    38241 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/commands/delegates.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    13519 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/identity.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    11154 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/inspect.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     4926 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/list.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    10770 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/commands/metagraph.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5096 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/misc.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    25743 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/commands/network.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    30254 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/overview.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    25769 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/register.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    28679 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/root.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    23862 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/senate.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    23616 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/stake.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5781 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/transfer.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    13182 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/unstake.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     9078 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/commands/utils.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    41540 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/commands/wallets.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    14128 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/config.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    37824 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/dendrite.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     4283 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/errors.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.920532 bittensor-6.9.3/bittensor/extrinsics/
+-rw-r--r--   0 alashaabana   (501) staff       (20)     1120 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/extrinsics/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    14777 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/delegation.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     8768 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/network.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     6046 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/prometheus.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    20397 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/registration.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     8992 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/root.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    11054 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/senate.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    11140 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/serving.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5644 2024-03-07 16:45:01.000000 bittensor-6.9.3/bittensor/extrinsics/set_weights.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    19314 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/staking.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     6640 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/extrinsics/transfer.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    16331 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/extrinsics/unstaking.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    32032 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/keyfile.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    47097 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/metagraph.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.921085 bittensor-6.9.3/bittensor/mock/
+-rw-r--r--   0 alashaabana   (501) staff       (20)     1186 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/mock/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     3216 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/mock/keyfile_mock.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    51880 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/mock/subtensor_mock.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5030 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/mock/wallet_mock.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     6981 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/stream.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     3283 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/subnets.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)   194474 2024-03-12 21:25:56.000000 bittensor-6.9.3/bittensor/subtensor.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    35031 2024-03-11 16:59:34.000000 bittensor-6.9.3/bittensor/synapse.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     6891 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/tensor.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    10401 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/threadpool.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     1510 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/types.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.922254 bittensor-6.9.3/bittensor/utils/
+-rw-r--r--   0 alashaabana   (501) staff       (20)     7560 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/utils/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     3527 2023-12-22 21:03:26.000000 bittensor-6.9.3/bittensor/utils/_register_cuda.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    10075 2023-10-02 18:12:13.000000 bittensor-6.9.3/bittensor/utils/balance.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)      553 2023-09-25 14:12:29.000000 bittensor-6.9.3/bittensor/utils/formatting.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5784 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/utils/networking.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    37774 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/utils/registration.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)      630 2023-07-04 20:47:55.000000 bittensor-6.9.3/bittensor/utils/test_utils.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     6327 2023-12-22 21:03:26.000000 bittensor-6.9.3/bittensor/utils/wallet_utils.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    11141 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/utils/weight_utils.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    33414 2024-02-26 16:25:46.000000 bittensor-6.9.3/bittensor/wallet.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.916179 bittensor-6.9.3/bittensor.egg-info/
+-rw-r--r--   0 alashaabana   (501) staff       (20)    18529 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/PKG-INFO
+-rw-r--r--   0 alashaabana   (501) staff       (20)     2700 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/SOURCES.txt
+-rw-r--r--   0 alashaabana   (501) staff       (20)        1 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/dependency_links.txt
+-rw-r--r--   0 alashaabana   (501) staff       (20)      730 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/requires.txt
+-rw-r--r--   0 alashaabana   (501) staff       (20)       16 2024-03-12 21:55:13.000000 bittensor-6.9.3/bittensor.egg-info/top_level.txt
+-rw-r--r--   0 alashaabana   (501) staff       (20)       38 2024-03-12 21:55:13.926324 bittensor-6.9.3/setup.cfg
+-rw-r--r--   0 alashaabana   (501) staff       (20)     3705 2023-10-02 18:12:13.000000 bittensor-6.9.3/setup.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.922391 bittensor-6.9.3/tests/
+-rw-r--r--   0 alashaabana   (501) staff       (20)     1202 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/__init__.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.922641 bittensor-6.9.3/tests/helpers/
+-rw-r--r--   0 alashaabana   (501) staff       (20)     1308 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/helpers/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5565 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/helpers/helpers.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.923304 bittensor-6.9.3/tests/integration_tests/
+-rw-r--r--   0 alashaabana   (501) staff       (20)        0 2023-07-20 18:02:20.000000 bittensor-6.9.3/tests/integration_tests/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    86929 2024-03-11 16:59:34.000000 bittensor-6.9.3/tests/integration_tests/test_cli.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    49428 2024-01-15 19:02:35.000000 bittensor-6.9.3/tests/integration_tests/test_cli_no_network.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     3450 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/integration_tests/test_metagraph_integration.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    23150 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/integration_tests/test_subtensor_integration.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.925187 bittensor-6.9.3/tests/unit_tests/
+-rw-r--r--   0 alashaabana   (501) staff       (20)        0 2023-07-20 18:02:20.000000 bittensor-6.9.3/tests/unit_tests/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     8119 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_axon.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    15306 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_chain_data.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     8228 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_dendrite.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    21841 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_keyfile.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5969 2024-03-11 16:59:34.000000 bittensor-6.9.3/tests/unit_tests/test_metagraph.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5605 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_subtensor.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     7559 2023-10-30 23:32:38.000000 bittensor-6.9.3/tests/unit_tests/test_synapse.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5648 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/unit_tests/test_tensor.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    17894 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/test_wallet.py
+drwxr-xr-x   0 alashaabana   (501) staff       (20)        0 2024-03-12 21:55:13.925881 bittensor-6.9.3/tests/unit_tests/utils/
+-rw-r--r--   0 alashaabana   (501) staff       (20)        0 2023-10-02 18:12:13.000000 bittensor-6.9.3/tests/unit_tests/utils/__init__.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)    15327 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/utils/test_balance.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     5390 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/utils/test_networking.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     9661 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/utils/test_utils.py
+-rw-r--r--   0 alashaabana   (501) staff       (20)     9661 2024-02-26 16:25:46.000000 bittensor-6.9.3/tests/unit_tests/utils/test_weight_utils.py
```

### Comparing `bittensor-6.9.2/LICENSE` & `bittensor-6.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/PKG-INFO` & `bittensor-6.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 6.9.2
+Version: 6.9.3
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bittensor-6.9.2/README.md` & `bittensor-6.9.3/README.md`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bin/btcli` & `bittensor-6.9.3/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/__init__.py` & `bittensor-6.9.3/bittensor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # Install and apply nest asyncio to allow the async functions
 # to run in a .ipynb
 import nest_asyncio
 
 nest_asyncio.apply()
 
 # Bittensor code and protocol version.
-__version__ = "6.9.2"
+__version__ = "6.9.3"
 
 version_split = __version__.split(".")
 __version_as_int__: int = (
     (100 * int(version_split[0]))
     + (10 * int(version_split[1]))
     + (1 * int(version_split[2]))
 )
```

### Comparing `bittensor-6.9.2/bittensor/axon.py` & `bittensor-6.9.3/bittensor/axon.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/btlogging.py` & `bittensor-6.9.3/bittensor/btlogging.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/chain_data.py` & `bittensor-6.9.3/bittensor/chain_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,14 +172,16 @@
                 ["target_regs_per_interval", "Compact<u16>"],
                 ["min_burn", "Compact<u64>"],
                 ["max_burn", "Compact<u64>"],
                 ["bonds_moving_avg", "Compact<u64>"],
                 ["max_regs_per_block", "Compact<u16>"],
                 ["serving_rate_limit", "Compact<u64>"],
                 ["max_validators", "Compact<u16>"],
+                ["adjustment_alpha", "Compact<u64>"],
+                ["difficulty", "Compact<u64>"],
             ],
         },
     }
 }
 
 
 @dataclass
@@ -878,14 +880,15 @@
     tempo: int
     modality: int
     # netuid -> topk percentile prunning score requirement (u16:MAX normalized.)
     connection_requirements: Dict[str, float]
     emission_value: float
     burn: Balance
     owner_ss58: str
+    # adjustment_alpha: int
 
     @classmethod
     def from_vec_u8(cls, vec_u8: List[int]) -> Optional["SubnetInfo"]:
         r"""Returns a SubnetInfo object from a ``vec_u8``."""
         if len(vec_u8) == 0:
             return None
 
@@ -918,14 +921,16 @@
             rho=decoded["rho"],
             kappa=decoded["kappa"],
             difficulty=decoded["difficulty"],
             immunity_period=decoded["immunity_period"],
             max_allowed_validators=decoded["max_allowed_validators"],
             min_allowed_weights=decoded["min_allowed_weights"],
             max_weight_limit=decoded["max_weights_limit"],
+            # adjustment_alpha=decoded["adjustment_alpha"],
+            # bonds_moving_avg=decoded["bonds_moving_average"],
             scaling_law_power=decoded["scaling_law_power"],
             subnetwork_n=decoded["subnetwork_n"],
             max_n=decoded["max_allowed_uids"],
             blocks_since_epoch=decoded["blocks_since_last_step"],
             tempo=decoded["tempo"],
             modality=decoded["network_modality"],
             connection_requirements={
@@ -971,14 +976,16 @@
     target_regs_per_interval: int
     min_burn: int
     max_burn: int
     bonds_moving_avg: int
     max_regs_per_block: int
     serving_rate_limit: int
     max_validators: int
+    adjustment_alpha: int
+    difficulty: int
 
     @classmethod
     def from_vec_u8(cls, vec_u8: List[int]) -> Optional["SubnetHyperparameters"]:
         r"""Returns a SubnetHyperparameters object from a ``vec_u8``."""
         if len(vec_u8) == 0:
             return None
 
@@ -1019,18 +1026,20 @@
             weights_rate_limit=decoded["weights_rate_limit"],
             adjustment_interval=decoded["adjustment_interval"],
             activity_cutoff=decoded["activity_cutoff"],
             registration_allowed=decoded["registration_allowed"],
             target_regs_per_interval=decoded["target_regs_per_interval"],
             min_burn=decoded["min_burn"],
             max_burn=decoded["max_burn"],
-            bonds_moving_avg=decoded["bonds_moving_avg"],
             max_regs_per_block=decoded["max_regs_per_block"],
             max_validators=decoded["max_validators"],
             serving_rate_limit=decoded["serving_rate_limit"],
+            bonds_moving_avg=decoded["bonds_moving_avg"],
+            adjustment_alpha=decoded["adjustment_alpha"],
+            difficulty=decoded["difficulty"],
         )
 
     def to_parameter_dict(self) -> "torch.nn.ParameterDict":
         r"""Returns a torch tensor of the subnet hyperparameters."""
         return torch.nn.ParameterDict(self.__dict__)
 
     @classmethod
```

### Comparing `bittensor-6.9.2/bittensor/cli.py` & `bittensor-6.9.3/bittensor/cli.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/__init__.py` & `bittensor-6.9.3/bittensor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/delegates.py` & `bittensor-6.9.3/bittensor/commands/delegates.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/identity.py` & `bittensor-6.9.3/bittensor/commands/identity.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/inspect.py` & `bittensor-6.9.3/bittensor/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/list.py` & `bittensor-6.9.3/bittensor/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/metagraph.py` & `bittensor-6.9.3/bittensor/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/misc.py` & `bittensor-6.9.3/bittensor/commands/misc.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/network.py` & `bittensor-6.9.3/bittensor/commands/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,19 @@
     "immunity_period": "sudo_set_immunity_period",
     "min_allowed_weights": "sudo_set_min_allowed_weights",
     "activity_cutoff": "sudo_set_activity_cutoff",
     "network_registration_allowed": "sudo_set_network_registration_allowed",
     "network_pow_registration_allowed": "sudo_set_network_pow_registration_allowed",
     "min_burn": "sudo_set_min_burn",
     "max_burn": "sudo_set_max_burn",
+    "adjustment_alpha": "sudo_set_adjustment_alpha",
+    "rho": "sudo_set_rho",
+    "kappa": "sudo_set_kappa",
+    "difficulty": "sudo_set_difficulty",
+    "bonds_moving_avg": "sudo_set_bonds_moving_average",
 }
 
 
 class SubnetSudoCommand:
     """
     Executes the ``set`` command to set hyperparameters for a specific subnet on the Bittensor network.
```

### Comparing `bittensor-6.9.2/bittensor/commands/overview.py` & `bittensor-6.9.3/bittensor/commands/overview.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/register.py` & `bittensor-6.9.3/bittensor/commands/register.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/root.py` & `bittensor-6.9.3/bittensor/commands/root.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/senate.py` & `bittensor-6.9.3/bittensor/commands/senate.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/stake.py` & `bittensor-6.9.3/bittensor/commands/stake.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/transfer.py` & `bittensor-6.9.3/bittensor/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/unstake.py` & `bittensor-6.9.3/bittensor/commands/unstake.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/utils.py` & `bittensor-6.9.3/bittensor/commands/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/commands/wallets.py` & `bittensor-6.9.3/bittensor/commands/wallets.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 import argparse
 import bittensor
 import os
 import sys
 from rich.prompt import Prompt, Confirm
 from rich.table import Table
-from typing import Optional, List
+from typing import Optional, List, Tuple
 from . import defaults
 import requests
 from ..utils import RAOPERTAO
 
 
 class RegenColdkeyCommand:
     """
@@ -688,15 +688,15 @@
         ):
             wallet_name = Prompt.ask(
                 "Enter wallet name", default=bittensor.defaults.wallet.name
             )
             config.wallet.name = str(wallet_name)
 
 
-def _get_coldkey_ss58_addresses_for_path(path: str) -> tuple[list[str], list[str]]:
+def _get_coldkey_ss58_addresses_for_path(path: str) -> Tuple[List[str], List[str]]:
     """Get all coldkey ss58 addresses from path."""
 
     def list_coldkeypub_files(dir_path):
         abspath = os.path.abspath(os.path.expanduser(dir_path))
         coldkey_files = []
         wallet_names = []
```

### Comparing `bittensor-6.9.2/bittensor/config.py` & `bittensor-6.9.3/bittensor/config.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/dendrite.py` & `bittensor-6.9.3/bittensor/dendrite.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/errors.py` & `bittensor-6.9.3/bittensor/errors.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/__init__.py` & `bittensor-6.9.3/bittensor/extrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/delegation.py` & `bittensor-6.9.3/bittensor/extrinsics/delegation.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/network.py` & `bittensor-6.9.3/bittensor/extrinsics/network.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/prometheus.py` & `bittensor-6.9.3/bittensor/extrinsics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/registration.py` & `bittensor-6.9.3/bittensor/extrinsics/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/root.py` & `bittensor-6.9.3/bittensor/extrinsics/root.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/senate.py` & `bittensor-6.9.3/bittensor/extrinsics/senate.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/serving.py` & `bittensor-6.9.3/bittensor/extrinsics/serving.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/set_weights.py` & `bittensor-6.9.3/bittensor/extrinsics/set_weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/staking.py` & `bittensor-6.9.3/bittensor/extrinsics/staking.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/transfer.py` & `bittensor-6.9.3/bittensor/extrinsics/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/extrinsics/unstaking.py` & `bittensor-6.9.3/bittensor/extrinsics/unstaking.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/keyfile.py` & `bittensor-6.9.3/bittensor/keyfile.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/metagraph.py` & `bittensor-6.9.3/bittensor/metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/mock/__init__.py` & `bittensor-6.9.3/bittensor/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/mock/keyfile_mock.py` & `bittensor-6.9.3/bittensor/mock/keyfile_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/mock/subtensor_mock.py` & `bittensor-6.9.3/bittensor/mock/subtensor_mock.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,14 +266,16 @@
                     "TotalColdkeyStake": {},
                     "TxRateLimit": {0: 0},  # No limit
                     "Delegates": {},
                     "Axons": {},
                     "Prometheus": {},
                     "SubnetOwner": {},
                     "Commits": {},
+                    "AdjustmentAlpha": {},
+                    "BondsMovingAverage": {},
                 },
             }
 
             self.block_number = 0
 
             self.network = "mock"
             self.chain_endpoint = "mock_endpoint"
@@ -324,14 +326,15 @@
             subtensor_state["MaxAllowedUids"][netuid][0] = 4096
             subtensor_state["NetworkModality"][netuid] = {}
             subtensor_state["NetworkModality"][netuid][0] = 0
             subtensor_state["BlocksSinceLastStep"][netuid] = {}
             subtensor_state["BlocksSinceLastStep"][netuid][0] = 0
             subtensor_state["Tempo"][netuid] = {}
             subtensor_state["Tempo"][netuid][0] = 99
+
             # subtensor_state['NetworkConnect'][netuid] = {}
             # subtensor_state['NetworkConnect'][netuid][0] = {}
             subtensor_state["EmissionValues"][netuid] = {}
             subtensor_state["EmissionValues"][netuid][0] = 0
             subtensor_state["Burn"][netuid] = {}
             subtensor_state["Burn"][netuid][0] = 0
             subtensor_state["Commits"][netuid] = {}
@@ -360,14 +363,19 @@
 
             subtensor_state["Axons"][netuid] = {}
             subtensor_state["Prometheus"][netuid] = {}
 
             subtensor_state["NetworksAdded"][netuid] = {}
             subtensor_state["NetworksAdded"][netuid][0] = True
 
+            subtensor_state["AdjustmentAlpha"][netuid] = {}
+            subtensor_state["AdjustmentAlpha"][netuid][0] = 1000
+
+            subtensor_state["BondsMovingAverage"][netuid] = {}
+            subtensor_state["BondsMovingAverage"][netuid][0] = 1000
         else:
             raise Exception("Subnet already exists")
 
     def set_difficulty(self, netuid: int, difficulty: int) -> None:
         subtensor_state = self.chain_state["SubtensorModule"]
         if netuid not in subtensor_state["NetworksAdded"]:
             raise Exception("Subnet does not exist")
```

### Comparing `bittensor-6.9.2/bittensor/mock/wallet_mock.py` & `bittensor-6.9.3/bittensor/mock/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/stream.py` & `bittensor-6.9.3/bittensor/stream.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/subnets.py` & `bittensor-6.9.3/bittensor/subnets.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/subtensor.py` & `bittensor-6.9.3/bittensor/subtensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 from .extrinsics.senate import (
     register_senate_extrinsic,
     leave_senate_extrinsic,
     vote_senate_extrinsic,
 )
 from .extrinsics.root import root_register_extrinsic, set_root_weights_extrinsic
 from .types import AxonServeCallParams, PrometheusServeCallParams
-from .utils import U16_NORMALIZED_FLOAT, ss58_to_vec_u8
+from .utils import U16_NORMALIZED_FLOAT, ss58_to_vec_u8, U64_NORMALIZED_FLOAT
 from .utils.balance import Balance
 from .utils.registration import POWSolution
 
 logger = logger.opt(colors=True)
 
 KEY_NONCE: Dict[str, int] = {}
 
@@ -2854,14 +2854,36 @@
         if not self.subnet_exists(netuid, block):
             return None
         _result = self.query_subtensor("MaxWeightsLimit", block, [netuid])
         if not hasattr(_result, "value") or _result is None:
             return None
         return U16_NORMALIZED_FLOAT(_result.value)
 
+    def adjustment_alpha(
+        self, netuid: int, block: Optional[int] = None
+    ) -> Optional[float]:
+        """Returns network AdjustmentAlpha hyper parameter"""
+        if not self.subnet_exists(netuid, block):
+            return None
+        _result = self.query_subtensor("AdjustmentAlpha", block, [netuid])
+        if not hasattr(_result, "value") or _result is None:
+            return None
+        return U64_NORMALIZED_FLOAT(_result.value)
+
+    def bonds_moving_avg(
+        self, netuid: int, block: Optional[int] = None
+    ) -> Optional[float]:
+        """Returns network BondsMovingAverage hyper parameter"""
+        if not self.subnet_exists(netuid, block):
+            return None
+        _result = self.query_subtensor("BondsMovingAverage", block, [netuid])
+        if not hasattr(_result, "value") or _result is None:
+            return None
+        return U64_NORMALIZED_FLOAT(_result.value)
+
     def scaling_law_power(
         self, netuid: int, block: Optional[int] = None
     ) -> Optional[float]:
         """Returns network ScalingLawPower hyper parameter"""
         if not self.subnet_exists(netuid, block):
             return None
         _result = self.query_subtensor("ScalingLawPower", block, [netuid])
```

### Comparing `bittensor-6.9.2/bittensor/synapse.py` & `bittensor-6.9.3/bittensor/synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/tensor.py` & `bittensor-6.9.3/bittensor/tensor.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/threadpool.py` & `bittensor-6.9.3/bittensor/threadpool.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/types.py` & `bittensor-6.9.3/bittensor/types.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/__init__.py` & `bittensor-6.9.3/bittensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/_register_cuda.py` & `bittensor-6.9.3/bittensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/balance.py` & `bittensor-6.9.3/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/formatting.py` & `bittensor-6.9.3/bittensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/networking.py` & `bittensor-6.9.3/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/registration.py` & `bittensor-6.9.3/bittensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/test_utils.py` & `bittensor-6.9.3/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/wallet_utils.py` & `bittensor-6.9.3/bittensor/utils/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/utils/weight_utils.py` & `bittensor-6.9.3/bittensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor/wallet.py` & `bittensor-6.9.3/bittensor/wallet.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor.egg-info/PKG-INFO` & `bittensor-6.9.3/bittensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 6.9.2
+Version: 6.9.3
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bittensor-6.9.2/bittensor.egg-info/SOURCES.txt` & `bittensor-6.9.3/bittensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/bittensor.egg-info/requires.txt` & `bittensor-6.9.3/bittensor.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/setup.py` & `bittensor-6.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/__init__.py` & `bittensor-6.9.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/helpers/__init__.py` & `bittensor-6.9.3/tests/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/helpers/helpers.py` & `bittensor-6.9.3/tests/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/integration_tests/test_cli.py` & `bittensor-6.9.3/tests/integration_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/integration_tests/test_cli_no_network.py` & `bittensor-6.9.3/tests/integration_tests/test_cli_no_network.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/integration_tests/test_metagraph_integration.py` & `bittensor-6.9.3/tests/integration_tests/test_metagraph_integration.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/integration_tests/test_subtensor_integration.py` & `bittensor-6.9.3/tests/integration_tests/test_subtensor_integration.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_axon.py` & `bittensor-6.9.3/tests/unit_tests/test_axon.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_chain_data.py` & `bittensor-6.9.3/tests/unit_tests/test_chain_data.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_dendrite.py` & `bittensor-6.9.3/tests/unit_tests/test_dendrite.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_keyfile.py` & `bittensor-6.9.3/tests/unit_tests/test_keyfile.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_metagraph.py` & `bittensor-6.9.3/tests/unit_tests/test_metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_subtensor.py` & `bittensor-6.9.3/tests/unit_tests/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_synapse.py` & `bittensor-6.9.3/tests/unit_tests/test_synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_tensor.py` & `bittensor-6.9.3/tests/unit_tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/test_wallet.py` & `bittensor-6.9.3/tests/unit_tests/test_wallet.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/utils/test_balance.py` & `bittensor-6.9.3/tests/unit_tests/utils/test_balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/utils/test_networking.py` & `bittensor-6.9.3/tests/unit_tests/utils/test_networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/utils/test_utils.py` & `bittensor-6.9.3/tests/unit_tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-6.9.2/tests/unit_tests/utils/test_weight_utils.py` & `bittensor-6.9.3/tests/unit_tests/utils/test_weight_utils.py`

 * *Files identical despite different names*

