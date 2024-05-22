# Comparing `tmp/nonebot_plugin_tetris_stats-1.2.8.tar.gz` & `tmp/nonebot_plugin_tetris_stats-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_tetris_stats-1.2.8.tar", max compression
+gzip compressed data, was "nonebot_plugin_tetris_stats-1.2.9.tar", max compression
```

## Comparing `nonebot_plugin_tetris_stats-1.2.8.tar` & `nonebot_plugin_tetris_stats-1.2.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0    34523 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/LICENSE
--rw-r--r--   0        0        0     2242 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/README.md
--rw-r--r--   0        0        0      791 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/__init__.py
--rw-r--r--   0        0        0      331 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/config.py
--rw-r--r--   0        0        0     1730 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
--rw-r--r--   0        0        0     1367 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
--rw-r--r--   0        0        0    14144 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py
--rw-r--r--   0        0        0     2052 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
--rw-r--r--   0        0        0     3026 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
--rw-r--r--   0        0        0     6279 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
--rw-r--r--   0        0        0     3256 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
--rw-r--r--   0        0        0     5458 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
--rw-r--r--   0        0        0        0 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/__init__.py
--rw-r--r--   0        0        0     3908 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
--rw-r--r--   0        0        0     1005 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
--rw-r--r--   0        0        0     4010 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/db/__init__.py
--rw-r--r--   0        0        0     3009 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/db/models.py
--rw-r--r--   0        0        0     1435 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/__init__.py
--rw-r--r--   0        0        0      208 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/constant.py
--rw-r--r--   0        0        0     2641 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py
--rw-r--r--   0        0        0      323 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/__init__.py
--rw-r--r--   0        0        0     1294 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py
--rw-r--r--   0        0        0      771 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py
--rw-r--r--   0        0        0     4122 2024-05-15 06:57:11.689524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py
--rw-r--r--   0        0        0      334 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/base.py
--rw-r--r--   0        0        0     1028 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py
--rw-r--r--   0        0        0      318 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0     3062 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py
--rw-r--r--   0        0        0     2233 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py
--rw-r--r--   0        0        0     1079 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py
--rw-r--r--   0        0        0      231 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/typing.py
--rw-r--r--   0        0        0     2917 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py
--rw-r--r--   0        0        0      536 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py
--rw-r--r--   0        0        0     1122 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py
--rw-r--r--   0        0        0    16379 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py
--rw-r--r--   0        0        0     7818 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py
--rw-r--r--   0        0        0      496 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/schemas.py
--rw-r--r--   0        0        0     2111 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py
--rw-r--r--   0        0        0       49 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/__init__.py
--rw-r--r--   0        0        0      742 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py
--rw-r--r--   0        0        0     2824 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py
--rw-r--r--   0        0        0      319 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0      189 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/schemas/user_profile.py
--rw-r--r--   0        0        0     2635 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py
--rw-r--r--   0        0        0      173 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/constant.py
--rw-r--r--   0        0        0     2939 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py
--rw-r--r--   0        0        0     2548 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py
--rw-r--r--   0        0        0       49 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/__init__.py
--rw-r--r--   0        0        0      851 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py
--rw-r--r--   0        0        0     5090 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py
--rw-r--r--   0        0        0      325 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user.py
--rw-r--r--   0        0        0     3436 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py
--rw-r--r--   0        0        0      603 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py
--rw-r--r--   0        0        0     2712 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py
--rw-r--r--   0        0        0      463 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/constant.py
--rw-r--r--   0        0        0     6463 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py
--rw-r--r--   0        0        0     1769 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/avatar.py
--rw-r--r--   0        0        0     3006 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/browser.py
--rw-r--r--   0        0        0      945 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/exception.py
--rw-r--r--   0        0        0     2097 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/host.py
--rw-r--r--   0        0        0     7337 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/metrics.py
--rw-r--r--   0        0        0      440 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/platform.py
--rw-r--r--   0        0        0      935 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/render/__init__.py
--rw-r--r--   0        0        0      197 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/render/schemas/base.py
--rw-r--r--   0        0        0      282 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/render/schemas/bind.py
--rw-r--r--   0        0        0     1521 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py
--rw-r--r--   0        0        0     6263 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/request.py
--rw-r--r--   0        0        0     1412 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/retry.py
--rw-r--r--   0        0        0      394 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/screenshot.py
--rw-r--r--   0        0        0     2594 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/templates.py
--rw-r--r--   0        0        0      922 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/typing.py
--rw-r--r--   0        0        0       93 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/version.py
--rw-r--r--   0        0        0     3643 2024-05-15 06:57:11.693524 nonebot_plugin_tetris_stats-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-16 10:05:39.625724 nonebot_plugin_tetris_stats-1.2.9/LICENSE
+-rw-r--r--   0        0        0     2242 2024-05-16 10:05:39.625724 nonebot_plugin_tetris_stats-1.2.9/README.md
+-rw-r--r--   0        0        0      733 2024-05-16 10:05:39.625724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/__init__.py
+-rw-r--r--   0        0        0      331 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/config.py
+-rw-r--r--   0        0        0     1730 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py
+-rw-r--r--   0        0        0     1367 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py
+-rw-r--r--   0        0        0    14144 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py
+-rw-r--r--   0        0        0     2052 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py
+-rw-r--r--   0        0        0     3026 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py
+-rw-r--r--   0        0        0     6279 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py
+-rw-r--r--   0        0        0     3256 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py
+-rw-r--r--   0        0        0     5458 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py
+-rw-r--r--   0        0        0        0 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/__init__.py
+-rw-r--r--   0        0        0     3908 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py
+-rw-r--r--   0        0        0     1005 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py
+-rw-r--r--   0        0        0     3927 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/db/__init__.py
+-rw-r--r--   0        0        0     3009 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/db/models.py
+-rw-r--r--   0        0        0     1377 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/__init__.py
+-rw-r--r--   0        0        0      208 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/constant.py
+-rw-r--r--   0        0        0      496 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/schemas.py
+-rw-r--r--   0        0        0     2641 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/__init__.py
+-rw-r--r--   0        0        0     1294 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/cache.py
+-rw-r--r--   0        0        0      771 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/models.py
+-rw-r--r--   0        0        0     4122 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/player.py
+-rw-r--r--   0        0        0      334 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/schemas/base.py
+-rw-r--r--   0        0        0     1028 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/schemas/tetra_league.py
+-rw-r--r--   0        0        0      318 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/schemas/user.py
+-rw-r--r--   0        0        0     3062 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/schemas/user_info.py
+-rw-r--r--   0        0        0     2247 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/schemas/user_records.py
+-rw-r--r--   0        0        0     1079 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/tetra_league.py
+-rw-r--r--   0        0        0      231 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/typing.py
+-rw-r--r--   0        0        0     2917 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/bind.py
+-rw-r--r--   0        0        0      536 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/constant.py
+-rw-r--r--   0        0        0     1122 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/model.py
+-rw-r--r--   0        0        0    16385 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/query.py
+-rw-r--r--   0        0        0     7818 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/rank.py
+-rw-r--r--   0        0        0     2111 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/api/__init__.py
+-rw-r--r--   0        0        0      742 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/api/models.py
+-rw-r--r--   0        0        0     2824 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/api/player.py
+-rw-r--r--   0        0        0      319 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/api/schemas/user.py
+-rw-r--r--   0        0        0      189 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/api/schemas/user_profile.py
+-rw-r--r--   0        0        0     2635 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/bind.py
+-rw-r--r--   0        0        0      173 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/constant.py
+-rw-r--r--   0        0        0     2939 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/query.py
+-rw-r--r--   0        0        0     2548 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/__init__.py
+-rw-r--r--   0        0        0       49 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/__init__.py
+-rw-r--r--   0        0        0      851 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/models.py
+-rw-r--r--   0        0        0     5090 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/player.py
+-rw-r--r--   0        0        0      325 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/schemas/user.py
+-rw-r--r--   0        0        0     3436 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/schemas/user_info.py
+-rw-r--r--   0        0        0      603 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/schemas/user_profile.py
+-rw-r--r--   0        0        0     2712 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/bind.py
+-rw-r--r--   0        0        0      463 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/constant.py
+-rw-r--r--   0        0        0     6463 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/query.py
+-rw-r--r--   0        0        0     1769 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/avatar.py
+-rw-r--r--   0        0        0     3006 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/browser.py
+-rw-r--r--   0        0        0      945 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/exception.py
+-rw-r--r--   0        0        0     2097 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/host.py
+-rw-r--r--   0        0        0     7337 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/metrics.py
+-rw-r--r--   0        0        0      440 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/platform.py
+-rw-r--r--   0        0        0      935 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/render/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/render/schemas/base.py
+-rw-r--r--   0        0        0      282 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/render/schemas/bind.py
+-rw-r--r--   0        0        0     1496 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py
+-rw-r--r--   0        0        0     6263 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/request.py
+-rw-r--r--   0        0        0     1412 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/retry.py
+-rw-r--r--   0        0        0      394 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/screenshot.py
+-rw-r--r--   0        0        0     2594 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/templates.py
+-rw-r--r--   0        0        0      922 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/typing.py
+-rw-r--r--   0        0        0       93 2024-05-16 10:05:39.629724 nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/version.py
+-rw-r--r--   0        0        0     3643 2024-05-16 10:05:39.633724 nonebot_plugin_tetris_stats-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     3852 1970-01-01 00:00:00.000000 nonebot_plugin_tetris_stats-1.2.9/PKG-INFO
```

### Comparing `nonebot_plugin_tetris_stats-1.2.8/LICENSE` & `nonebot_plugin_tetris_stats-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/README.md` & `nonebot_plugin_tetris_stats-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/__init__.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,9 +17,8 @@
     type='application',
     homepage='https://github.com/A-minos/nonebot-plugin-tetris-stats',
     extra={
         'orm_version_location': migrations,
     },
 )
 
-from . import game_data_processor  # noqa: F401, E402
-from .utils import host  # noqa: F401, E402
+from . import games  # noqa: F401, E402
```

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/09d4bb60160d_rename_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/0d50142b780f_add_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/3c25a5a8c050_refactor_historical.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/6c3206f90cc3_add_field.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/8a91210ce14d_correct_the_data_in_historicaldata.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/9866f53ce44f_init_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/9cd1647db502_merge_old_db.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/9f6582279ce2_recreate_historical_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/b7fbdafc339a_add_user_unique_identifier_field_to_.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/config/migrations/b9d65badc713_del_old_tos_bind_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/db/__init__.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/db/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 from ..utils.typing import CommandType, GameType
 from .models import Bind, TriggerHistoricalData
 
 UTC = timezone.utc
 
 if TYPE_CHECKING:
-    from ..game_data_processor.io_data_processor.api.models import TETRIOHistoricalData
-    from ..game_data_processor.top_data_processor.api.models import TOPHistoricalData
-    from ..game_data_processor.tos_data_processor.api.models import TOSHistoricalData
+    from ..games.tetrio.api.models import TETRIOHistoricalData
+    from ..games.top.api.models import TOPHistoricalData
+    from ..games.tos.api.models import TOSHistoricalData
 
 
 class BindStatus(Enum):
     SUCCESS = auto()
     UPDATE = auto()
```

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/db/models.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/db/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,17 +28,13 @@
             )
 
     @matcher.handle()
     def _(other: Any):  # noqa: ANN401, ARG001
         raise FinishedException
 
 
-from . import (  # noqa: F401, E402
-    io_data_processor,
-    top_data_processor,
-    tos_data_processor,
-)
+from . import tetrio, top, tos  # noqa: F401, E402
 
 
 @run_postprocessor
 async def _(matcher: Matcher, exception: NeedCatchError):
     await matcher.send(str(exception))
```

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/cache.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/tetra_league.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/schemas/tetra_league.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/schemas/user_records.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/schemas/user_records.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
 
 class MultiRecord(_Record):
     endcontext: list[EndContext]
 
 
 class SoloModeRecord(BaseModel):
-    record: SoloRecord
+    record: SoloRecord | None = None
     rank: int | None = None
 
 
 class Records(BaseModel):
     sprint: SoloModeRecord = Field(..., alias='40l')
     blitz: SoloModeRecord
```

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/api/tetra_league.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/api/tetra_league.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/constant.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/constant.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/model.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,17 +65,17 @@
         if bind is None:
             await matcher.finish('未查询到绑定信息')
         message = UniMessage(CANT_VERIFY_MESSAGE)
         player = Player(user_id=bind.game_account, trust=True)
         user, user_info, user_records = await gather(player.user, player.get_info(), player.get_records())
         sprint = user_records.data.records.sprint
         blitz = user_records.data.records.blitz
-        # with contextlib.suppress(TypeError):
-        message += UniMessage.image(raw=await make_query_image(user, user_info, sprint.record, blitz.record))
-        await message.finish()
+        with contextlib.suppress(TypeError):
+            message += UniMessage.image(raw=await make_query_image(user, user_info, sprint.record, blitz.record))
+            await message.finish()
         message += make_query_text(user_info, sprint, blitz)
         await message.finish()
 
 
 @alc.assign('query')
 async def _(account: Player, event_session: EventSession):
     async with trigger(
```

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/io_data_processor/rank.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tetrio/rank.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/top_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/top/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/__init__.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/models.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/models.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/player.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/player.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_info.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/schemas/user_info.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/api/schemas/user_profile.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/api/schemas/user_profile.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/bind.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/bind.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/game_data_processor/tos_data_processor/query.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/games/tos/query.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/avatar.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/avatar.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/browser.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/exception.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/host.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/host.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/metrics.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/render/__init__.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/render/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/render/schemas/tetrio_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from datetime import datetime
 from typing import Annotated, ClassVar
 
 from nonebot.compat import PYDANTIC_V2
 from pydantic import BaseModel
 
-from ....game_data_processor.io_data_processor.api.typing import Rank
+from ....games.tetrio.api.typing import Rank
 from ...typing import Number
 from .base import People
 
 if PYDANTIC_V2:
     from pydantic import PlainSerializer
```

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/request.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/request.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/retry.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/retry.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/templates.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/templates.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/nonebot_plugin_tetris_stats/utils/typing.py` & `nonebot_plugin_tetris_stats-1.2.9/nonebot_plugin_tetris_stats/utils/typing.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_tetris_stats-1.2.8/pyproject.toml` & `nonebot_plugin_tetris_stats-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'nonebot-plugin-tetris-stats'
-version = '1.2.8'
+version = '1.2.9'
 description = '一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件'
 authors = ['scdhh <wallfjjd@gmail.com>']
 readme = 'README.md'
 homepage = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 repository = 'https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats'
 license = 'AGPL-3.0'
```

### Comparing `nonebot_plugin_tetris_stats-1.2.8/PKG-INFO` & `nonebot_plugin_tetris_stats-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-tetris-stats
-Version: 1.2.8
+Version: 1.2.9
 Summary: 一款基于 NoneBot2 的用于查询 Tetris 相关游戏数据的插件
 Home-page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats
 License: AGPL-3.0
 Author: scdhh
 Author-email: wallfjjd@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.2.8 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-tetris-stats Version: 1.2.9 Summary:
 ä¸æ¬¾åºäº NoneBot2 çç¨äºæ¥è¯¢ Tetris ç¸å³æ¸¸ææ°æ®çæä»¶ Home-
 page: https://github.com/shoucandanghehe/nonebot-plugin-tetris-stats License:
 AGPL-3.0 Author: scdhh Author-email: wallfjjd@gmail.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: GNU Affero General Public
 License v3 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
```

