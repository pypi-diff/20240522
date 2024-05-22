# Comparing `tmp/bookio_fetchfox-2.6.1.tar.gz` & `tmp/bookio_fetchfox-2.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bookio_fetchfox-2.6.1.tar", max compression
+gzip compressed data, was "bookio_fetchfox-2.6.2.tar", max compression
```

## Comparing `bookio_fetchfox-2.6.1.tar` & `bookio_fetchfox-2.6.2.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     3560 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/README.md
--rw-r--r--   0        0        0        0 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/algorand/__init__.py
--rw-r--r--   0        0        0     2686 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/algorand/algonodecloud.py
--rw-r--r--   0        0        0     1551 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/algorand/nfdomains.py
--rw-r--r--   0        0        0      721 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/algorand/randswapcom.py
--rw-r--r--   0        0        0      354 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/bookio.py
--rw-r--r--   0        0        0        0 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/cardano/__init__.py
--rw-r--r--   0        0        0     2489 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/cardano/dexhunterio.py
--rw-r--r--   0        0        0     7444 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/cardano/gomaestroorg.py
--rw-r--r--   0        0        0     1917 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/cardano/jpgstore.py
--rw-r--r--   0        0        0      635 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/cardano/muesliswapcom.py
--rwxr-xr-x   0        0        0     2830 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/coingeckocom.py
--rw-r--r--   0        0        0        0 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/evm/__init__.py
--rw-r--r--   0        0        0     1191 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/evm/ensideascom.py
--rw-r--r--   0        0        0     5952 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/evm/moralisio.py
--rw-r--r--   0        0        0     3268 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/evm/openseaio.py
--rw-r--r--   0        0        0      341 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/pinatacloud.py
--rw-r--r--   0        0        0      260 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/apis/price.py
--rw-r--r--   0        0        0      120 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/__init__.py
--rw-r--r--   0        0        0       33 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/algorand/__init__.py
--rw-r--r--   0        0        0     7656 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/algorand/blockchain.py
--rw-r--r--   0        0        0      689 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/algorand/exceptions.py
--rw-r--r--   0        0        0      502 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/algorand/utils.py
--rw-r--r--   0        0        0     3408 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/base.py
--rw-r--r--   0        0        0       32 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/cardano/__init__.py
--rw-r--r--   0        0        0    17633 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/cardano/blockchain.py
--rw-r--r--   0        0        0      679 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/cardano/exceptions.py
--rw-r--r--   0        0        0     1060 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/cardano/utils.py
--rw-r--r--   0        0        0       33 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/ethereum/__init__.py
--rw-r--r--   0        0        0     1696 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/ethereum/blockchain.py
--rw-r--r--   0        0        0       28 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/evm/__init__.py
--rw-r--r--   0        0        0    11880 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/evm/blockchain.py
--rw-r--r--   0        0        0      753 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/evm/exceptions.py
--rw-r--r--   0        0        0      617 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/evm/utils.py
--rw-r--r--   0        0        0      443 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/exceptions.py
--rw-r--r--   0        0        0       32 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/polygon/__init__.py
--rw-r--r--   0        0        0     1706 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/polygon/blockchain.py
--rw-r--r--   0        0        0      146 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/blockchains/utils.py
--rw-r--r--   0        0        0      322 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/checks.py
--rw-r--r--   0        0        0        0 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/constants/__init__.py
--rw-r--r--   0        0        0      299 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/constants/beard.py
--rw-r--r--   0        0        0      158 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/constants/blockchains.py
--rw-r--r--   0        0        0      399 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/constants/book.py
--rw-r--r--   0        0        0       82 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/constants/cardano.py
--rw-r--r--   0        0        0      194 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/constants/currencies.py
--rw-r--r--   0        0        0       66 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/constants/evm.py
--rw-r--r--   0        0        0      341 2024-05-12 14:21:17.243914 bookio_fetchfox-2.6.1/fetchfox/constants/marketplaces.py
--rw-r--r--   0        0        0   453386 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/constants/ranks.py
--rw-r--r--   0        0        0       95 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/constants/sales.py
--rw-r--r--   0        0        0       62 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/constants/specials.py
--rw-r--r--   0        0        0      329 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/__init__.py
--rw-r--r--   0        0        0     3719 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/asset.py
--rw-r--r--   0        0        0     3666 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/campaign.py
--rw-r--r--   0        0        0      285 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/floor.py
--rw-r--r--   0        0        0      495 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/holding.py
--rw-r--r--   0        0        0     1572 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/listing.py
--rw-r--r--   0        0        0      948 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/order.py
--rw-r--r--   0        0        0     1203 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/pair_stats.py
--rw-r--r--   0        0        0      365 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/rank.py
--rw-r--r--   0        0        0     2023 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/dtos/sale.py
--rw-r--r--   0        0        0        0 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/helpers/__init__.py
--rw-r--r--   0        0        0      150 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/helpers/formatters.py
--rw-r--r--   0        0        0        0 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/pools/__init__.py
--rw-r--r--   0        0        0     1212 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/pools/book_pool.py
--rw-r--r--   0        0        0     6138 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/rest.py
--rw-r--r--   0        0        0      106 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/tokens/__init__.py
--rw-r--r--   0        0        0     4042 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/tokens/base.py
--rw-r--r--   0        0        0      750 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/tokens/beard_token.py
--rw-r--r--   0        0        0      817 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/tokens/book_token.py
--rw-r--r--   0        0        0      808 2024-05-12 14:21:17.247914 bookio_fetchfox-2.6.1/fetchfox/tokens/hosky_token.py
--rw-r--r--   0        0        0     1170 2024-05-12 14:21:17.259914 bookio_fetchfox-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 bookio_fetchfox-2.6.1/setup.py
--rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 bookio_fetchfox-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0     3560 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/algorand/__init__.py
+-rw-r--r--   0        0        0     2686 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/algorand/algonodecloud.py
+-rw-r--r--   0        0        0     1551 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/algorand/nfdomains.py
+-rw-r--r--   0        0        0      721 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/algorand/randswapcom.py
+-rw-r--r--   0        0        0      354 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/bookio.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/cardano/__init__.py
+-rw-r--r--   0        0        0     2489 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/cardano/dexhunterio.py
+-rw-r--r--   0        0        0     7444 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/cardano/gomaestroorg.py
+-rw-r--r--   0        0        0     1917 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/cardano/jpgstore.py
+-rw-r--r--   0        0        0      635 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/cardano/muesliswapcom.py
+-rwxr-xr-x   0        0        0     3180 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/coingeckocom.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/evm/__init__.py
+-rw-r--r--   0        0        0     1191 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/evm/ensideascom.py
+-rw-r--r--   0        0        0     5952 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/evm/moralisio.py
+-rw-r--r--   0        0        0     3268 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/evm/openseaio.py
+-rw-r--r--   0        0        0      341 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/pinatacloud.py
+-rw-r--r--   0        0        0      260 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/apis/price.py
+-rw-r--r--   0        0        0      120 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/algorand/__init__.py
+-rw-r--r--   0        0        0     7656 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/algorand/blockchain.py
+-rw-r--r--   0        0        0      689 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/algorand/exceptions.py
+-rw-r--r--   0        0        0      502 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/algorand/utils.py
+-rw-r--r--   0        0        0     3408 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/base.py
+-rw-r--r--   0        0        0       32 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/cardano/__init__.py
+-rw-r--r--   0        0        0    17633 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/cardano/blockchain.py
+-rw-r--r--   0        0        0      679 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/cardano/exceptions.py
+-rw-r--r--   0        0        0     1060 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/cardano/utils.py
+-rw-r--r--   0        0        0       33 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/ethereum/__init__.py
+-rw-r--r--   0        0        0     1696 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/ethereum/blockchain.py
+-rw-r--r--   0        0        0       28 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/evm/__init__.py
+-rw-r--r--   0        0        0    11880 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/evm/blockchain.py
+-rw-r--r--   0        0        0      753 2024-05-22 19:49:17.706214 bookio_fetchfox-2.6.2/fetchfox/blockchains/evm/exceptions.py
+-rw-r--r--   0        0        0      617 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/blockchains/evm/utils.py
+-rw-r--r--   0        0        0      443 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/blockchains/exceptions.py
+-rw-r--r--   0        0        0       32 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/blockchains/polygon/__init__.py
+-rw-r--r--   0        0        0     1706 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/blockchains/polygon/blockchain.py
+-rw-r--r--   0        0        0      146 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/blockchains/utils.py
+-rw-r--r--   0        0        0      322 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/checks.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/beard.py
+-rw-r--r--   0        0        0      158 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/blockchains.py
+-rw-r--r--   0        0        0      399 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/book.py
+-rw-r--r--   0        0        0       82 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/cardano.py
+-rw-r--r--   0        0        0      194 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/currencies.py
+-rw-r--r--   0        0        0       66 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/evm.py
+-rw-r--r--   0        0        0      341 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/marketplaces.py
+-rw-r--r--   0        0        0   453386 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/ranks.py
+-rw-r--r--   0        0        0       95 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/sales.py
+-rw-r--r--   0        0        0       62 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/constants/specials.py
+-rw-r--r--   0        0        0      329 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/__init__.py
+-rw-r--r--   0        0        0     3719 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/asset.py
+-rw-r--r--   0        0        0     3666 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/campaign.py
+-rw-r--r--   0        0        0      285 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/floor.py
+-rw-r--r--   0        0        0      495 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/holding.py
+-rw-r--r--   0        0        0     1572 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/listing.py
+-rw-r--r--   0        0        0      948 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/order.py
+-rw-r--r--   0        0        0     1203 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/pair_stats.py
+-rw-r--r--   0        0        0      365 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/rank.py
+-rw-r--r--   0        0        0     2023 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/dtos/sale.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/helpers/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/helpers/formatters.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/pools/__init__.py
+-rw-r--r--   0        0        0     1212 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/pools/book_pool.py
+-rw-r--r--   0        0        0     6138 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/rest.py
+-rw-r--r--   0        0        0      106 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/tokens/__init__.py
+-rw-r--r--   0        0        0     4042 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/tokens/base.py
+-rw-r--r--   0        0        0      750 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/tokens/beard_token.py
+-rw-r--r--   0        0        0      817 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/tokens/book_token.py
+-rw-r--r--   0        0        0      808 2024-05-22 19:49:17.710214 bookio_fetchfox-2.6.2/fetchfox/tokens/hosky_token.py
+-rw-r--r--   0        0        0     1170 2024-05-22 19:49:17.722214 bookio_fetchfox-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 bookio_fetchfox-2.6.2/setup.py
+-rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 bookio_fetchfox-2.6.2/PKG-INFO
```

### Comparing `bookio_fetchfox-2.6.1/README.md` & `bookio_fetchfox-2.6.2/README.md`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/algorand/algonodecloud.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/algorand/algonodecloud.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/algorand/nfdomains.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/algorand/nfdomains.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/algorand/randswapcom.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/algorand/randswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/cardano/dexhunterio.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/cardano/dexhunterio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/cardano/gomaestroorg.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/cardano/gomaestroorg.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/cardano/jpgstore.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/cardano/jpgstore.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/cardano/muesliswapcom.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/cardano/muesliswapcom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/coingeckocom.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/coingeckocom.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,46 +53,59 @@
     MATIC: "matic-network",
 }
 
 logger = logging.getLogger(__name__)
 
 
 def get(service: str, params: dict = None, version: int = 3) -> Tuple[dict, int]:
+    logger.debug("calling %s", service)
+
     time.sleep(60 / RATE_LIMIT)
 
     return rest.get(
         url=f"{BASE_URL}/v{version}/{service}",
         headers=HEADERS,
         params=params,
     )
 
 
 @ttl_cache(ttl=60 * 60)
 def get_exchange(crypto: str, fiat: str = USD, date: datetime = None):
     crypto, fiat = crypto.strip().upper(), fiat.strip().lower()
     coin_id = IDS[crypto]
 
-    date = date or datetime.now()
-
     logger.info("fetching exchange %s/%s (%s) [%s]", crypto, fiat, coin_id, API_KEY_TYPE)
 
-    response, status_code = get(
-        service=f"coins/{coin_id}/history",
-        params={
-            "date": date.strftime("%d-%m-%Y"),
-            "localization": "false",
-        },
-    )
+    if date is None:
+        response, status_code = get(
+            service="simple/price",
+            params={
+                "ids": coin_id,
+                "vs_currencies": fiat,
+            },
+        )
+
+        return response[coin_id][fiat]
+    else:
+        date = date or datetime.now()
+
+        response, status_code = get(
+            service=f"coins/{coin_id}/history",
+            params={
+                "date": date.strftime("%d-%m-%Y"),
+                "localization": "false",
+            },
+        )
 
-    market_data = response.get("market_data")
+        market_data = response.get("market_data")
 
-    if not market_data:
-        return None
+        if not market_data:
+            return None
 
-    return market_data["current_price"][fiat]
+        return market_data["current_price"][fiat]
 
 
 @ttl_cache(ttl=60 * 60)
 def get_ath(crypto: str, fiat: str = USD):
     crypto, fiat = crypto.strip().upper(), fiat.strip().lower()
     coin_id = IDS[crypto]
```

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/evm/ensideascom.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/evm/ensideascom.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/evm/moralisio.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/evm/moralisio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/apis/evm/openseaio.py` & `bookio_fetchfox-2.6.2/fetchfox/apis/evm/openseaio.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/algorand/blockchain.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/algorand/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/algorand/exceptions.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/algorand/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/base.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/cardano/blockchain.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/cardano/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/cardano/exceptions.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/cardano/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/cardano/utils.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/cardano/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/ethereum/blockchain.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/ethereum/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/evm/blockchain.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/evm/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/evm/exceptions.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/evm/exceptions.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/evm/utils.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/evm/utils.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/blockchains/polygon/blockchain.py` & `bookio_fetchfox-2.6.2/fetchfox/blockchains/polygon/blockchain.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/constants/ranks.py` & `bookio_fetchfox-2.6.2/fetchfox/constants/ranks.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/dtos/asset.py` & `bookio_fetchfox-2.6.2/fetchfox/dtos/asset.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/dtos/campaign.py` & `bookio_fetchfox-2.6.2/fetchfox/dtos/campaign.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/dtos/listing.py` & `bookio_fetchfox-2.6.2/fetchfox/dtos/listing.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/dtos/order.py` & `bookio_fetchfox-2.6.2/fetchfox/dtos/order.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/dtos/pair_stats.py` & `bookio_fetchfox-2.6.2/fetchfox/dtos/pair_stats.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/dtos/sale.py` & `bookio_fetchfox-2.6.2/fetchfox/dtos/sale.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/pools/book_pool.py` & `bookio_fetchfox-2.6.2/fetchfox/pools/book_pool.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/rest.py` & `bookio_fetchfox-2.6.2/fetchfox/rest.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/tokens/base.py` & `bookio_fetchfox-2.6.2/fetchfox/tokens/base.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/tokens/beard_token.py` & `bookio_fetchfox-2.6.2/fetchfox/tokens/beard_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/tokens/book_token.py` & `bookio_fetchfox-2.6.2/fetchfox/tokens/book_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/fetchfox/tokens/hosky_token.py` & `bookio_fetchfox-2.6.2/fetchfox/tokens/hosky_token.py`

 * *Files identical despite different names*

### Comparing `bookio_fetchfox-2.6.1/pyproject.toml` & `bookio_fetchfox-2.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bookio-fetchfox"
-version = "2.6.1"
+version = "2.6.2"
 description = "Collection of API services to fetch information from several blockchains."
 documentation = "https://github.com/book-io/fetchfox/blob/main/README.md"
 homepage = "https://github.com/book-io/fetchfox"
 license = "MIT"
 readme = "README.md"
 
 authors = [
```

### Comparing `bookio_fetchfox-2.6.1/setup.py` & `bookio_fetchfox-2.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'backoff>=2.2.1,<3.0.0',
  'cachetools>=5.3.1,<6.0.0',
  'certifi>=2024.2.2,<2025.0.0',
  'pytz>=2023.3,<2024.0']
 
 setup_kwargs = {
     'name': 'bookio-fetchfox',
-    'version': '2.6.1',
+    'version': '2.6.2',
     'description': 'Collection of API services to fetch information from several blockchains.',
     'long_description': '# book.io / fetchfox\n\n> Collection of API services to fetch information from several blockchains.\n\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/4030.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/2010.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/1027.png)\n![](https://s2.coinmarketcap.com/static/img/coins/64x64/3890.png)\n\n\n## Supported Blockchains\n\n### Algorand\n\n```python\nimport os\nfrom fetchfox.blockchains import Algorand\n\nalgorand = Algorand()\n\n# Brave New World\ncreator_address = "6WII6ES4H6UW7G7T7RJX63CUNPKJEPEGQ3PTYVVU3JHJ652W34GCJV5OVY"\n\nfor asset in algorand.get_assets(creator_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([algonode.cloud](https://algonode.cloud))\n* get_assets ([algonode.cloud](https://algonode.cloud))\n* get_holdings ([algonode.cloud](https://algonode.cloud))\n* get_snapshot ([algonode.cloud](https://algonode.cloud))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_floor ([randgallery.com](https://randgallery.com) / [algoxnft.com](https://algoxnft.com))\n* get_sales ([nftexplorer.app¹](https://nftexplorer.app))\n\n\n### Cardano\n\n```python\nimport os\nfrom fetchfox.blockchains import Cardano\n\ncardano = Cardano(\n    gomaestroorg_api_key=os.getenv("GOMAESTROORG_API_KEY"),\n)\n\n# Gutenberg Bible\npolicy_id = "477cec772adb1466b301fb8161f505aa66ed1ee8d69d3e7984256a43"\n\nfor asset in cardano.get_collection_assets(policy_id):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([gomaestro.org²](https://gomaestro.org))\n* get_assets ([gomaestro.org²](https://gomaestro.org))\n* get_holdings ([gomaestro.org²](https://bgomaestro.org))\n* get_campaigns ([book.io](https://book.io))\n* get_snapshot ([gomaestro.org²](https://gomaestro.org))\n* get_listings ([jpg.store](https://jpg.store))\n* get_floor ([jpg.store](https://jpg.store))\n* get_sales ([jpg.store](https://jpg.store))\n\n\n### EVM (Ethereum and Polygon)\n\n```python\nimport os\nfrom fetchfox.blockchains import Ethereum, Polygon\n\nethereum = Ethereum(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\npolygon = Polygon(\n    geckodriver_path=os.getenv("GECKODRIVER_PATH"),\n    moralisio_api_key=os.getenv("MORALIS_API_KEY"),\n    openseaio_api_key=os.getenv("OPENSEA_API_KEY"),\n)\n\n\n# Alice in Wonderland\ncontract_address = "0x919da7fef646226f88f70305201de392ff365059"\n\nfor asset in ethereum.get_assets(contract_address):\n    print(asset)\n\n# Art of War\ncontract_address = "0xb56010e0500e4f163758881603b8083996ae47ec"\n\nfor asset in polygon.get_assets(contract_address):\n    print(asset)\n```\n\n#### Services\n\n* get_asset ([moralis.io³](https://moralis.io))\n* get_assets ([moralis.io³](https://moralis.io))\n* get_holdings ([moralis.io³](https://moralis.io))\n* get_snapshot ([moralis.io³](https://moralis.io))\n* get_campaigns ([book.io](https://book.io))\n* get_listings ([opensea.io⁴](https://opensea.io))\n* get_floor ([opensea.io⁴](https://opensea.io))\n* get_sales ([opensea.io⁴](https://opensea.io))\n\n\n> ¹ **nftexplorer.app** this api has been deprecated.\n> \n> ² **gomaestro.org** services require an [api key](https://www.gomaestro.org/pricing).\n> \n> ³ **moralis.io** services require an [api key](https://moralis.io/pricing).\n> \n> ⁴ **opensea.io** some services also require an [api key](https://docs.opensea.io/reference/api-keys). \n\n---\n\n![fetch, the fox](https://i.imgur.com/fm6mqzS.png)\n> fetch, the fox\n\n',
     'author': 'Fede',
     'author_email': 'fede@book.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/book-io/fetchfox',
```

### Comparing `bookio_fetchfox-2.6.1/PKG-INFO` & `bookio_fetchfox-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookio-fetchfox
-Version: 2.6.1
+Version: 2.6.2
 Summary: Collection of API services to fetch information from several blockchains.
 Home-page: https://github.com/book-io/fetchfox
 License: MIT
 Keywords: book.io,blockchain,crypto,algorand,cardano,ethereum,polygon
 Author: Fede
 Author-email: fede@book.io
 Requires-Python: >=3.8,<4.0
```

