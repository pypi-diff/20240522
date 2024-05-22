# Comparing `tmp/ffun-1.5.2.tar.gz` & `tmp/ffun-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffun-1.5.2.tar", max compression
+gzip compressed data, was "ffun-1.5.3.tar", max compression
```

## Comparing `ffun-1.5.2.tar` & `ffun-1.5.3.tar`

### file list

```diff
@@ -1,231 +1,231 @@
--rw-r--r--   0        0        0      344 2024-05-19 16:42:13.929798 ffun-1.5.2/README.md
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/api/__init__.py
--rw-r--r--   0        0        0    10249 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/api/entities.py
--rw-r--r--   0        0        0    13637 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/api/http_handlers.py
--rw-r--r--   0        0        0      245 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/api/settings.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.929798 ffun-1.5.2/ffun/application/__init__.py
--rw-r--r--   0        0        0     4314 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/application.py
--rw-r--r--   0        0        0      115 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/errors.py
--rw-r--r--   0        0        0       68 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/resources.py
--rw-r--r--   0        0        0     1635 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/settings.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/tests/__init__.py
--rw-r--r--   0        0        0      422 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/tests/test_settings.py
--rw-r--r--   0        0        0     3724 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/user_settings.py
--rw-r--r--   0        0        0      281 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/utils.py
--rw-r--r--   0        0        0     1252 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/application/workers.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/auth/__init__.py
--rw-r--r--   0        0        0      984 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/auth/dependencies.py
--rw-r--r--   0        0        0      828 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/auth/settings.py
--rw-r--r--   0        0        0     2800 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/auth/supertokens.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/__init__.py
--rw-r--r--   0        0        0      174 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/application.py
--rw-r--r--   0        0        0      439 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/cli.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/__init__.py
--rw-r--r--   0        0        0      732 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/configs.py
--rw-r--r--   0        0        0     1050 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/entries.py
--rw-r--r--   0        0        0     1393 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/failed_entries.py
--rw-r--r--   0        0        0      538 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/meta.py
--rw-r--r--   0        0        0     1001 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/supertokens.py
--rw-r--r--   0        0        0      884 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/workers.py
--rw-r--r--   0        0        0      209 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/cli/commands/yoyo.py
--rw-r--r--   0        0        0     1333 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/conftest.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/__init__.py
--rw-r--r--   0        0        0      631 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/api.py
--rw-r--r--   0        0        0     3139 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/background_tasks.py
--rw-r--r--   0        0        0      493 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/entities.py
--rw-r--r--   0        0        0      552 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/errors.py
--rw-r--r--   0        0        0     2773 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/json.py
--rw-r--r--   0        0        0     5440 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/logging.py
--rw-r--r--   0        0        0     1516 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/middlewares.py
--rw-r--r--   0        0        0      882 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/migrations.py
--rw-r--r--   0        0        0     4019 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/postgresql.py
--rw-r--r--   0        0        0      695 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/register.py
--rw-r--r--   0        0        0     1442 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/sentry.py
--rw-r--r--   0        0        0      347 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/settings.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/tests/__init__.py
--rw-r--r--   0        0        0     4551 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/tests/helpers.py
--rw-r--r--   0        0        0       82 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/tests/make.py
--rw-r--r--   0        0        0      486 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/text.py
--rw-r--r--   0        0        0     1088 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/core/utils.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/domain/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/domain/tests/__init__.py
--rw-r--r--   0        0        0     6590 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/domain/tests/test_urls.py
--rw-r--r--   0        0        0     3811 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/domain/urls.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/__init__.py
--rw-r--r--   0        0        0      826 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/domain.py
--rw-r--r--   0        0        0     1905 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/entities.py
--rw-r--r--   0        0        0      131 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/errors.py
--rw-r--r--   0        0        0     1027 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
--rw-r--r--   0        0        0      641 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
--rw-r--r--   0        0        0      561 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
--rw-r--r--   0        0        0      531 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
--rw-r--r--   0        0        0      725 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
--rw-r--r--   0        0        0     4062 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/__init__.py
--rw-r--r--   0        0        0     1512 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/fixtures.py
--rw-r--r--   0        0        0     1178 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/make.py
--rw-r--r--   0        0        0      445 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/test_domain.py
--rw-r--r--   0        0        0     7782 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/__init__.py
--rw-r--r--   0        0        0      495 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/collections/artificial_intelligence.py
--rw-r--r--   0        0        0     1357 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/collections/gamedev.py
--rw-r--r--   0        0        0      777 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/domain.py
--rw-r--r--   0        0        0      128 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/entities.py
--rw-r--r--   0        0        0      573 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/predefines.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/tests/__init__.py
--rw-r--r--   0        0        0      684 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_collections/tests/fixtures.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_discoverer/__init__.py
--rw-r--r--   0        0        0     3974 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_discoverer/domain.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/__init__.py
--rw-r--r--   0        0        0      553 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/domain.py
--rw-r--r--   0        0        0      163 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/entities.py
--rw-r--r--   0        0        0      810 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
--rw-r--r--   0        0        0     2326 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/tests/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/feeds_links/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/__init__.py
--rw-r--r--   0        0        0     4734 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/background_processors.py
--rw-r--r--   0        0        0     3512 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/domain.py
--rw-r--r--   0        0        0      205 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/entities.py
--rw-r--r--   0        0        0      217 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/errors.py
--rw-r--r--   0        0        0     2101 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
--rw-r--r--   0        0        0     3035 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
--rw-r--r--   0        0        0     5112 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/__init__.py
--rw-r--r--   0        0        0     1255 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/base.py
--rw-r--r--   0        0        0     1548 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/domain.py
--rw-r--r--   0        0        0      468 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/native_tags.py
--rw-r--r--   0        0        0     3295 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/openai_chat_3_5.py
--rw-r--r--   0        0        0     4421 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/openai_chat_3_5_functions.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/tests/__init__.py
--rw-r--r--   0        0        0     1139 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/tests/test_upper_case_title.py
--rw-r--r--   0        0        0      434 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/processors/upper_case_title.py
--rw-r--r--   0        0        0     1089 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/settings.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/tests/__init__.py
--rw-r--r--   0        0        0      845 2024-05-19 16:42:13.933798 ffun-1.5.2/ffun/librarian/tests/fixtures.py
--rw-r--r--   0        0        0      487 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/helpers.py
--rw-r--r--   0        0        0      553 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/make.py
--rw-r--r--   0        0        0     2737 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/test_background_processors.py
--rw-r--r--   0        0        0    13605 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/test_domain.py
--rw-r--r--   0        0        0    14031 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/librarian/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/__init__.py
--rw-r--r--   0        0        0     1476 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/domain.py
--rw-r--r--   0        0        0     1168 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/entities.py
--rw-r--r--   0        0        0      149 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/errors.py
--rw-r--r--   0        0        0     1498 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
--rw-r--r--   0        0        0     1288 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
--rw-r--r--   0        0        0      710 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
--rw-r--r--   0        0        0     1125 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
--rw-r--r--   0        0        0     1003 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
--rw-r--r--   0        0        0     1194 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
--rw-r--r--   0        0        0      784 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
--rw-r--r--   0        0        0     5926 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/__init__.py
--rw-r--r--   0        0        0      799 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/fixtures.py
--rw-r--r--   0        0        0     1663 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/make.py
--rw-r--r--   0        0        0     1414 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/test_domain.py
--rw-r--r--   0        0        0    15331 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/library/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/__init__.py
--rw-r--r--   0        0        0      882 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/background_loader.py
--rw-r--r--   0        0        0    11775 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/domain.py
--rw-r--r--   0        0        0      181 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/errors.py
--rw-r--r--   0        0        0      477 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/settings.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/tests/__init__.py
--rw-r--r--   0        0        0     8583 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/loader/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/__init__.py
--rw-r--r--   0        0        0      504 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/domain.py
--rw-r--r--   0        0        0       57 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/entities.py
--rw-r--r--   0        0        0      855 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
--rw-r--r--   0        0        0     2447 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/tests/__init__.py
--rw-r--r--   0        0        0     4835 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/markers/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/__init__.py
--rw-r--r--   0        0        0     3557 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/domain.py
--rw-r--r--   0        0        0      345 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
--rw-r--r--   0        0        0      246 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/settings.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/tests/__init__.py
--rw-r--r--   0        0        0    15939 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/meta/tests/test_domain.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/__init__.py
--rw-r--r--   0        0        0     3840 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/domain.py
--rw-r--r--   0        0        0     1683 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/entities.py
--rw-r--r--   0        0        0     1092 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
--rw-r--r--   0        0        0      520 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
--rw-r--r--   0        0        0      799 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
--rw-r--r--   0        0        0     1008 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
--rw-r--r--   0        0        0     6307 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/tests/__init__.py
--rw-r--r--   0        0        0      834 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/tests/fixtures.py
--rw-r--r--   0        0        0      408 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/tests/helpers.py
--rw-r--r--   0        0        0     9964 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/ontology/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/__init__.py
--rw-r--r--   0        0        0     5962 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/client.py
--rw-r--r--   0        0        0      612 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/entities.py
--rw-r--r--   0        0        0      150 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/errors.py
--rw-r--r--   0        0        0     7597 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/keys_rotator.py
--rw-r--r--   0        0        0     1919 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/keys_statuses.py
--rw-r--r--   0        0        0      372 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/settings.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/__init__.py
--rw-r--r--   0        0        0      130 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/conftest.py
--rw-r--r--   0        0        0     2518 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/fixtures.py
--rw-r--r--   0        0        0    19734 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/test_keys_rotator.py
--rw-r--r--   0        0        0     2833 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/openai/tests/test_keys_statuses.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/__init__.py
--rw-r--r--   0        0        0      228 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/domain.py
--rw-r--r--   0        0        0      560 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/entities.py
--rw-r--r--   0        0        0     2355 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/feed.py
--rw-r--r--   0        0        0     1325 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/feedly.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/__init__.py
--rw-r--r--   0        0        0     1219 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
--rw-r--r--   0        0        0      639 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
--rw-r--r--   0        0        0     4745 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
--rw-r--r--   0        0        0     1072 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
--rw-r--r--   0        0        0      966 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/make.py
--rw-r--r--   0        0        0     1205 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/parsers/tests/test_feed.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/__init__.py
--rw-r--r--   0        0        0      769 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/domain.py
--rw-r--r--   0        0        0      280 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/entities.py
--rw-r--r--   0        0        0      120 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/errors.py
--rw-r--r--   0        0        0      865 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
--rw-r--r--   0        0        0     3984 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/tests/__init__.py
--rw-r--r--   0        0        0     1945 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/tests/test_domain.py
--rw-r--r--   0        0        0     9480 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/resources/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/scores/__init__.py
--rw-r--r--   0        0        0      884 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/scores/domain.py
--rw-r--r--   0        0        0      250 2024-05-19 16:42:13.937798 ffun-1.5.2/ffun/scores/entities.py
--rw-r--r--   0        0        0      104 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/errors.py
--rw-r--r--   0        0        0      851 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
--rw-r--r--   0        0        0      603 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
--rw-r--r--   0        0        0     2603 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/tests/__init__.py
--rw-r--r--   0        0        0     1239 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/tests/test_domain.py
--rw-r--r--   0        0        0     6810 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/scores/tests/test_operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/tags/__init__.py
--rw-r--r--   0        0        0     1578 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/tags/converters.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/tags/tests/__init__.py
--rw-r--r--   0        0        0     1352 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/tags/tests/test_converters.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/__init__.py
--rw-r--r--   0        0        0     1842 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/domain.py
--rw-r--r--   0        0        0       54 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/entities.py
--rw-r--r--   0        0        0      137 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/errors.py
--rw-r--r--   0        0        0      732 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
--rw-r--r--   0        0        0      534 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
--rw-r--r--   0        0        0     1748 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/operations.py
--rw-r--r--   0        0        0      581 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/settings.py
--rw-r--r--   0        0        0      508 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/tests/asserts.py
--rw-r--r--   0        0        0     6956 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/tests/test_domain.py
--rw-r--r--   0        0        0     5492 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/tests/test_operations.py
--rw-r--r--   0        0        0     2297 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/types.py
--rw-r--r--   0        0        0      489 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/user_settings/values.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/__init__.py
--rw-r--r--   0        0        0      586 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/domain.py
--rw-r--r--   0        0        0      161 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/entities.py
--rw-r--r--   0        0        0      111 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/errors.py
--rw-r--r--   0        0        0      718 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
--rw-r--r--   0        0        0     1232 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/operations.py
--rw-r--r--   0        0        0        0 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/tests/__init__.py
--rw-r--r--   0        0        0     1101 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/tests/fixtures.py
--rw-r--r--   0        0        0      348 2024-05-19 16:42:13.941798 ffun-1.5.2/ffun/users/tests/make.py
--rw-r--r--   0        0        0     4263 2024-05-19 16:42:23.089859 ffun-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0      344 2024-05-22 13:04:51.379570 ffun-1.5.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/api/__init__.py
+-rw-r--r--   0        0        0    10249 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/api/entities.py
+-rw-r--r--   0        0        0    13637 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/api/http_handlers.py
+-rw-r--r--   0        0        0      245 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/api/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/__init__.py
+-rw-r--r--   0        0        0     4314 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/application.py
+-rw-r--r--   0        0        0      115 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/errors.py
+-rw-r--r--   0        0        0       68 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/resources.py
+-rw-r--r--   0        0        0     1635 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/tests/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/tests/test_settings.py
+-rw-r--r--   0        0        0     3724 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/user_settings.py
+-rw-r--r--   0        0        0      281 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/utils.py
+-rw-r--r--   0        0        0     1252 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/application/workers.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/auth/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/auth/dependencies.py
+-rw-r--r--   0        0        0      828 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/auth/settings.py
+-rw-r--r--   0        0        0     2800 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/auth/supertokens.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/__init__.py
+-rw-r--r--   0        0        0      174 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/application.py
+-rw-r--r--   0        0        0      439 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/__init__.py
+-rw-r--r--   0        0        0      732 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/configs.py
+-rw-r--r--   0        0        0     1050 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/entries.py
+-rw-r--r--   0        0        0     1393 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/failed_entries.py
+-rw-r--r--   0        0        0      538 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/meta.py
+-rw-r--r--   0        0        0     1001 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/supertokens.py
+-rw-r--r--   0        0        0      884 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/workers.py
+-rw-r--r--   0        0        0      209 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/cli/commands/yoyo.py
+-rw-r--r--   0        0        0     1333 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/api.py
+-rw-r--r--   0        0        0     3139 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/background_tasks.py
+-rw-r--r--   0        0        0      493 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/entities.py
+-rw-r--r--   0        0        0      552 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/errors.py
+-rw-r--r--   0        0        0     2773 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/json.py
+-rw-r--r--   0        0        0     5440 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/logging.py
+-rw-r--r--   0        0        0     1516 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/middlewares.py
+-rw-r--r--   0        0        0      882 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/migrations.py
+-rw-r--r--   0        0        0     4019 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/postgresql.py
+-rw-r--r--   0        0        0      695 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/register.py
+-rw-r--r--   0        0        0     1442 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/sentry.py
+-rw-r--r--   0        0        0      347 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/tests/__init__.py
+-rw-r--r--   0        0        0     4551 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/tests/helpers.py
+-rw-r--r--   0        0        0       82 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/tests/make.py
+-rw-r--r--   0        0        0      486 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/text.py
+-rw-r--r--   0        0        0     1088 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/core/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/domain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/domain/tests/__init__.py
+-rw-r--r--   0        0        0     6590 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/domain/tests/test_urls.py
+-rw-r--r--   0        0        0     3811 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/domain/urls.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/__init__.py
+-rw-r--r--   0        0        0      826 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/domain.py
+-rw-r--r--   0        0        0     1905 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/entities.py
+-rw-r--r--   0        0        0      131 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/errors.py
+-rw-r--r--   0        0        0     1027 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py
+-rw-r--r--   0        0        0      641 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py
+-rw-r--r--   0        0        0      561 2024-05-22 13:04:51.379570 ffun-1.5.3/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py
+-rw-r--r--   0        0        0      531 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py
+-rw-r--r--   0        0        0      725 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py
+-rw-r--r--   0        0        0     4062 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/__init__.py
+-rw-r--r--   0        0        0     1512 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/fixtures.py
+-rw-r--r--   0        0        0     1178 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/make.py
+-rw-r--r--   0        0        0      445 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/test_domain.py
+-rw-r--r--   0        0        0     7782 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/collections/artificial_intelligence.py
+-rw-r--r--   0        0        0     1357 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/collections/gamedev.py
+-rw-r--r--   0        0        0      777 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/domain.py
+-rw-r--r--   0        0        0      128 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/entities.py
+-rw-r--r--   0        0        0      573 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/predefines.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/tests/__init__.py
+-rw-r--r--   0        0        0      684 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_collections/tests/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_discoverer/__init__.py
+-rw-r--r--   0        0        0     3974 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_discoverer/domain.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/__init__.py
+-rw-r--r--   0        0        0      553 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/domain.py
+-rw-r--r--   0        0        0      163 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/entities.py
+-rw-r--r--   0        0        0      810 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py
+-rw-r--r--   0        0        0     2326 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/tests/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/feeds_links/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/__init__.py
+-rw-r--r--   0        0        0     5182 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/background_processors.py
+-rw-r--r--   0        0        0     3759 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/domain.py
+-rw-r--r--   0        0        0      205 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/entities.py
+-rw-r--r--   0        0        0      217 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/errors.py
+-rw-r--r--   0        0        0     2101 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py
+-rw-r--r--   0        0        0     3035 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py
+-rw-r--r--   0        0        0     5112 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/__init__.py
+-rw-r--r--   0        0        0     1255 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/base.py
+-rw-r--r--   0        0        0     1548 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/domain.py
+-rw-r--r--   0        0        0      468 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/native_tags.py
+-rw-r--r--   0        0        0     3295 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/openai_chat_3_5.py
+-rw-r--r--   0        0        0     4421 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/openai_chat_3_5_functions.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/tests/__init__.py
+-rw-r--r--   0        0        0     1139 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/tests/test_upper_case_title.py
+-rw-r--r--   0        0        0      434 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/processors/upper_case_title.py
+-rw-r--r--   0        0        0     1089 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/fixtures.py
+-rw-r--r--   0        0        0      487 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/helpers.py
+-rw-r--r--   0        0        0      553 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/make.py
+-rw-r--r--   0        0        0     4104 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/test_background_processors.py
+-rw-r--r--   0        0        0    13605 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/test_domain.py
+-rw-r--r--   0        0        0    14031 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/librarian/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/__init__.py
+-rw-r--r--   0        0        0     1476 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/domain.py
+-rw-r--r--   0        0        0     1168 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/entities.py
+-rw-r--r--   0        0        0      149 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/errors.py
+-rw-r--r--   0        0        0     1498 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20230331_01_UsHwp-entries-table.py
+-rw-r--r--   0        0        0     1288 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py
+-rw-r--r--   0        0        0      710 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20230514_01_Bwb35-processed-state.py
+-rw-r--r--   0        0        0     1125 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py
+-rw-r--r--   0        0        0     1003 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py
+-rw-r--r--   0        0        0     1194 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py
+-rw-r--r--   0        0        0      784 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py
+-rw-r--r--   0        0        0     5926 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/__init__.py
+-rw-r--r--   0        0        0      799 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/fixtures.py
+-rw-r--r--   0        0        0     1663 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/make.py
+-rw-r--r--   0        0        0     1414 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/test_domain.py
+-rw-r--r--   0        0        0    15331 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/library/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/__init__.py
+-rw-r--r--   0        0        0      882 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/background_loader.py
+-rw-r--r--   0        0        0    11775 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/domain.py
+-rw-r--r--   0        0        0      181 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/errors.py
+-rw-r--r--   0        0        0      477 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/tests/__init__.py
+-rw-r--r--   0        0        0     8583 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/loader/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/__init__.py
+-rw-r--r--   0        0        0      504 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/domain.py
+-rw-r--r--   0        0        0       57 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/entities.py
+-rw-r--r--   0        0        0      855 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py
+-rw-r--r--   0        0        0     2447 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/tests/__init__.py
+-rw-r--r--   0        0        0     4835 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/markers/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/__init__.py
+-rw-r--r--   0        0        0     3557 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/domain.py
+-rw-r--r--   0        0        0      345 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/migrations/20240512_01_0F799-unity-duplicated-feeds.py
+-rw-r--r--   0        0        0      246 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/tests/__init__.py
+-rw-r--r--   0        0        0    15939 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/meta/tests/test_domain.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/ontology/__init__.py
+-rw-r--r--   0        0        0     3840 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/ontology/domain.py
+-rw-r--r--   0        0        0     1683 2024-05-22 13:04:51.383570 ffun-1.5.3/ffun/ontology/entities.py
+-rw-r--r--   0        0        0     1092 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py
+-rw-r--r--   0        0        0      520 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py
+-rw-r--r--   0        0        0      799 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py
+-rw-r--r--   0        0        0     1008 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py
+-rw-r--r--   0        0        0     6307 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/tests/__init__.py
+-rw-r--r--   0        0        0      834 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/tests/fixtures.py
+-rw-r--r--   0        0        0      408 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/tests/helpers.py
+-rw-r--r--   0        0        0     9964 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/ontology/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/__init__.py
+-rw-r--r--   0        0        0     5962 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/client.py
+-rw-r--r--   0        0        0      612 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/entities.py
+-rw-r--r--   0        0        0      150 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/errors.py
+-rw-r--r--   0        0        0     7597 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/keys_rotator.py
+-rw-r--r--   0        0        0     1919 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/keys_statuses.py
+-rw-r--r--   0        0        0      372 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/settings.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/conftest.py
+-rw-r--r--   0        0        0     2518 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/fixtures.py
+-rw-r--r--   0        0        0    19734 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/test_keys_rotator.py
+-rw-r--r--   0        0        0     2833 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/openai/tests/test_keys_statuses.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/__init__.py
+-rw-r--r--   0        0        0      228 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/domain.py
+-rw-r--r--   0        0        0      560 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/entities.py
+-rw-r--r--   0        0        0     2355 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/feed.py
+-rw-r--r--   0        0        0     1325 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/feedly.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/__init__.py
+-rw-r--r--   0        0        0     1219 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml
+-rw-r--r--   0        0        0      639 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json
+-rw-r--r--   0        0        0     4745 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml
+-rw-r--r--   0        0        0     1072 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json
+-rw-r--r--   0        0        0      966 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/make.py
+-rw-r--r--   0        0        0     1205 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/parsers/tests/test_feed.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/domain.py
+-rw-r--r--   0        0        0      280 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/entities.py
+-rw-r--r--   0        0        0      120 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/errors.py
+-rw-r--r--   0        0        0      865 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/migrations/20230702_01_LEEES-resources-table.py
+-rw-r--r--   0        0        0     3984 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/tests/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/tests/test_domain.py
+-rw-r--r--   0        0        0     9480 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/resources/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/__init__.py
+-rw-r--r--   0        0        0      884 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/domain.py
+-rw-r--r--   0        0        0      250 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/entities.py
+-rw-r--r--   0        0        0      104 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/errors.py
+-rw-r--r--   0        0        0      851 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py
+-rw-r--r--   0        0        0      603 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py
+-rw-r--r--   0        0        0     2603 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/tests/__init__.py
+-rw-r--r--   0        0        0     1239 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/tests/test_domain.py
+-rw-r--r--   0        0        0     6810 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/scores/tests/test_operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/tags/__init__.py
+-rw-r--r--   0        0        0     1578 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/tags/converters.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/tags/tests/__init__.py
+-rw-r--r--   0        0        0     1352 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/tags/tests/test_converters.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/__init__.py
+-rw-r--r--   0        0        0     1842 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/domain.py
+-rw-r--r--   0        0        0       54 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/entities.py
+-rw-r--r--   0        0        0      137 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/errors.py
+-rw-r--r--   0        0        0      732 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py
+-rw-r--r--   0        0        0      534 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py
+-rw-r--r--   0        0        0     1748 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/operations.py
+-rw-r--r--   0        0        0      581 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/settings.py
+-rw-r--r--   0        0        0      508 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/tests/asserts.py
+-rw-r--r--   0        0        0     6956 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/tests/test_domain.py
+-rw-r--r--   0        0        0     5492 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/tests/test_operations.py
+-rw-r--r--   0        0        0     2297 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/types.py
+-rw-r--r--   0        0        0      489 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/user_settings/values.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/domain.py
+-rw-r--r--   0        0        0      161 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/entities.py
+-rw-r--r--   0        0        0      111 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/errors.py
+-rw-r--r--   0        0        0      718 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/migrations/20230527_01_soIr3-users-mapping.py
+-rw-r--r--   0        0        0     1232 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/operations.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/tests/fixtures.py
+-rw-r--r--   0        0        0      348 2024-05-22 13:04:51.387570 ffun-1.5.3/ffun/users/tests/make.py
+-rw-r--r--   0        0        0     4263 2024-05-22 13:04:58.883531 ffun-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     2901 1970-01-01 00:00:00.000000 ffun-1.5.3/PKG-INFO
```

### Comparing `ffun-1.5.2/ffun/api/entities.py` & `ffun-1.5.3/ffun/api/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/api/http_handlers.py` & `ffun-1.5.3/ffun/api/http_handlers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/application/application.py` & `ffun-1.5.3/ffun/application/application.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/application/settings.py` & `ffun-1.5.3/ffun/application/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/application/user_settings.py` & `ffun-1.5.3/ffun/application/user_settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/application/workers.py` & `ffun-1.5.3/ffun/application/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/auth/dependencies.py` & `ffun-1.5.3/ffun/auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/auth/settings.py` & `ffun-1.5.3/ffun/auth/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/auth/supertokens.py` & `ffun-1.5.3/ffun/auth/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/cli/commands/configs.py` & `ffun-1.5.3/ffun/cli/commands/configs.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/cli/commands/entries.py` & `ffun-1.5.3/ffun/cli/commands/entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/cli/commands/failed_entries.py` & `ffun-1.5.3/ffun/cli/commands/failed_entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/cli/commands/meta.py` & `ffun-1.5.3/ffun/cli/commands/meta.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/cli/commands/supertokens.py` & `ffun-1.5.3/ffun/cli/commands/supertokens.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/cli/commands/workers.py` & `ffun-1.5.3/ffun/cli/commands/workers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/conftest.py` & `ffun-1.5.3/ffun/conftest.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/api.py` & `ffun-1.5.3/ffun/core/api.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/background_tasks.py` & `ffun-1.5.3/ffun/core/background_tasks.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/errors.py` & `ffun-1.5.3/ffun/core/errors.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/json.py` & `ffun-1.5.3/ffun/core/json.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/logging.py` & `ffun-1.5.3/ffun/core/logging.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/middlewares.py` & `ffun-1.5.3/ffun/core/middlewares.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/migrations.py` & `ffun-1.5.3/ffun/core/migrations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/postgresql.py` & `ffun-1.5.3/ffun/core/postgresql.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/register.py` & `ffun-1.5.3/ffun/core/register.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/sentry.py` & `ffun-1.5.3/ffun/core/sentry.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/tests/helpers.py` & `ffun-1.5.3/ffun/core/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/core/utils.py` & `ffun-1.5.3/ffun/core/utils.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/domain/tests/test_urls.py` & `ffun-1.5.3/ffun/domain/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/domain/urls.py` & `ffun-1.5.3/ffun/domain/urls.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/domain.py` & `ffun-1.5.3/ffun/feeds/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/entities.py` & `ffun-1.5.3/ffun/feeds/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py` & `ffun-1.5.3/ffun/feeds/migrations/20230329_01_ilwfq-feeds-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py` & `ffun-1.5.3/ffun/feeds/migrations/20230426_01_IiF5m-add-title-and-description.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py` & `ffun-1.5.3/ffun/feeds/migrations/20240504_01_vBDVJ-column-for-feed-unique-id.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py` & `ffun-1.5.3/ffun/feeds/migrations/20240504_02_gEapd-fill-uids-for-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py` & `ffun-1.5.3/ffun/feeds/migrations/20240512_01_jL7Mt-turn-on-unique-uids.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/operations.py` & `ffun-1.5.3/ffun/feeds/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/tests/fixtures.py` & `ffun-1.5.3/ffun/feeds/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/tests/make.py` & `ffun-1.5.3/ffun/feeds/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds/tests/test_operations.py` & `ffun-1.5.3/ffun/feeds/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_collections/collections/gamedev.py` & `ffun-1.5.3/ffun/feeds_collections/collections/gamedev.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_collections/domain.py` & `ffun-1.5.3/ffun/feeds_collections/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_collections/predefines.py` & `ffun-1.5.3/ffun/feeds_collections/predefines.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_collections/tests/fixtures.py` & `ffun-1.5.3/ffun/feeds_collections/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_discoverer/domain.py` & `ffun-1.5.3/ffun/feeds_discoverer/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_links/domain.py` & `ffun-1.5.3/ffun/feeds_links/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py` & `ffun-1.5.3/ffun/feeds_links/migrations/20230427_01_9HuHj-add-feeds-links.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_links/operations.py` & `ffun-1.5.3/ffun/feeds_links/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/feeds_links/tests/test_operations.py` & `ffun-1.5.3/ffun/feeds_links/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/background_processors.py` & `ffun-1.5.3/ffun/librarian/background_processors.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,19 +119,31 @@
             return
 
         # TODO: we could add caching here, because multiple processors can request the same entries
         #       and currently we run multiple processors in the same process
         #       but remember that for API worker such cachin may be useless or even harmful
         entries = await l_domain.get_entries_by_ids(entities_ids)
 
-        tasks = [
-            domain.process_entry(processor_id=processor_id, processor=self._processor_info.processor, entry=entry)
-            for entry in entries.values()
-            if entry is not None
-        ]
+        tasks = []
+        entries_to_remove = []
+
+        for entry_id, entry in entries.items():
+            if entry is None:
+                entries_to_remove.append(entry_id)
+                continue
+
+            tasks.append(
+                domain.process_entry(processor_id=processor_id, processor=self._processor_info.processor, entry=entry)
+            )
+
+        if entries_to_remove:
+            logger.warning("unexisted_entries_in_queue", processor_id=processor_id, entries_ids=entries_to_remove)
+            tasks.append(
+                domain.remove_entries_from_processor_queue(processor_id=processor_id, entry_ids=entries_to_remove)
+            )
 
         await asyncio.gather(*tasks, return_exceptions=True)
 
 
 def create_background_processors() -> list[EntriesProcessor]:
     return [
         EntriesProcessor(
```

### Comparing `ffun-1.5.2/ffun/librarian/domain.py` & `ffun-1.5.3/ffun/librarian/domain.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,7 +88,14 @@
     except Exception as e:
         await operations.add_entries_to_failed_storage(processor_id, [entry.id])
         raise errors.UnexpectedErrorInProcessor(processor_id=processor_id, entry_id=entry.id) from e
     finally:
         await operations.remove_entries_from_processor_queue(execute, processor_id, [entry.id])
 
     logger.info("entry_processed")
+
+
+@run_in_transaction
+async def remove_entries_from_processor_queue(
+    execute: ExecuteType, processor_id: int, entry_ids: Iterable[uuid.UUID]
+) -> None:
+    await operations.remove_entries_from_processor_queue(execute, processor_id, entry_ids)
```

### Comparing `ffun-1.5.2/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py` & `ffun-1.5.3/ffun/librarian/migrations/20240313_01_Yv74T-processors-pointers.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py` & `ffun-1.5.3/ffun/librarian/migrations/20240319_01_MTJyn-migrate-to-processors-queue.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/operations.py` & `ffun-1.5.3/ffun/librarian/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/processors/base.py` & `ffun-1.5.3/ffun/librarian/processors/base.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/processors/domain.py` & `ffun-1.5.3/ffun/librarian/processors/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/processors/openai_chat_3_5.py` & `ffun-1.5.3/ffun/librarian/processors/openai_chat_3_5.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/processors/openai_chat_3_5_functions.py` & `ffun-1.5.3/ffun/librarian/processors/openai_chat_3_5_functions.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/processors/tests/test_upper_case_title.py` & `ffun-1.5.3/ffun/librarian/processors/tests/test_upper_case_title.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/settings.py` & `ffun-1.5.3/ffun/librarian/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/tests/fixtures.py` & `ffun-1.5.3/ffun/librarian/tests/fixtures.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 @pytest.fixture
 def fake_processor_info(fake_processor_id: int) -> ProcessorInfo:
     return ProcessorInfo(
         id=fake_processor_id,
         processor=AlwaysConstantProcessor(
             name="fake_constant_processor", tags=["fake-constant-tag-1", "fake-constant-tag-2"]
         ),
-        concurrency=3,
+        concurrency=5,
     )
 
 
 @pytest.fixture
 def fake_entries_processor(fake_processor_info: ProcessorInfo) -> EntriesProcessor:
     return EntriesProcessor(processor_info=fake_processor_info, name="fake_entries_processor", delay_between_runs=0.1)
```

### Comparing `ffun-1.5.2/ffun/librarian/tests/make.py` & `ffun-1.5.3/ffun/librarian/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/tests/test_background_processors.py` & `ffun-1.5.3/ffun/librarian/tests/test_background_processors.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import uuid
 
 import pytest
 from structlog.testing import capture_logs
 
+from ffun.core.postgresql import execute
 from ffun.core.tests.helpers import assert_logs
 from ffun.librarian import operations
 from ffun.librarian.background_processors import EntriesProcessor
 from ffun.librarian.tests import make
 from ffun.library.tests import make as l_make
 from ffun.ontology import domain as o_domain
 
@@ -25,19 +26,19 @@
     @pytest.mark.asyncio
     async def test_entries_more_than_concurrency(
         self, fake_entries_processor: EntriesProcessor, loaded_feed_id: uuid.UUID
     ) -> None:
         await operations.clear_processor_queue(fake_entries_processor.id)
         await make.end_processor_pointer(fake_entries_processor.id)
 
-        entries = await l_make.n_entries(loaded_feed_id, 5)
+        entries = await l_make.n_entries(loaded_feed_id, 9)
         entries_list = list(entries.values())
         entries_list.sort(key=lambda entry: (entry.cataloged_at, entry.id))
 
-        assert fake_entries_processor.concurrency < len(entries)
+        assert fake_entries_processor.concurrency <= len(entries)
 
         with capture_logs() as logs:
             await fake_entries_processor.single_run()
 
         assert_logs(logs, no_entries_to_process=0)
 
         tags = await o_domain.get_tags_for_entries(list(entries))
@@ -66,7 +67,40 @@
 
         assert_logs(logs, no_entries_to_process=0)
 
         tags = await o_domain.get_tags_for_entries(list(entries))
 
         for entry in entries_list:
             assert tags[entry.id] == {"fake-constant-tag-1", "fake-constant-tag-2"}
+
+    @pytest.mark.asyncio
+    async def test_unexisted_entries_in_queue(
+        self, fake_entries_processor: EntriesProcessor, loaded_feed_id: uuid.UUID
+    ) -> None:
+        await operations.clear_processor_queue(fake_entries_processor.id)
+        await make.end_processor_pointer(fake_entries_processor.id)
+
+        entries = await l_make.n_entries(loaded_feed_id, 2)
+        entries_list = list(entries.values())
+        entries_list.sort(key=lambda entry: (entry.cataloged_at, entry.id))
+
+        fake_entries_ids = [uuid.uuid4() for _ in range(3)]
+
+        await operations.push_entries_to_processor_queue(
+            execute, processor_id=fake_entries_processor.id, entry_ids=fake_entries_ids
+        )
+
+        assert fake_entries_processor.concurrency >= len(entries) + len(fake_entries_ids)
+
+        with capture_logs() as logs:
+            await fake_entries_processor.single_run()
+
+        assert_logs(logs, no_entries_to_process=0, unexisted_entries_in_queue=1)
+
+        tags = await o_domain.get_tags_for_entries(list(entries))
+
+        for entry in entries_list:
+            assert tags[entry.id] == {"fake-constant-tag-1", "fake-constant-tag-2"}
+
+        entities_in_queue = await operations.get_entries_to_process(processor_id=fake_entries_processor.id, limit=100)
+
+        assert entities_in_queue == []
```

### Comparing `ffun-1.5.2/ffun/librarian/tests/test_domain.py` & `ffun-1.5.3/ffun/librarian/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/librarian/tests/test_operations.py` & `ffun-1.5.3/ffun/librarian/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/domain.py` & `ffun-1.5.3/ffun/library/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/entities.py` & `ffun-1.5.3/ffun/library/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/migrations/20230331_01_UsHwp-entries-table.py` & `ffun-1.5.3/ffun/library/migrations/20230331_01_UsHwp-entries-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py` & `ffun-1.5.3/ffun/library/migrations/20230427_01_pv33u-fix-entries-unique-index.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/migrations/20230514_01_Bwb35-processed-state.py` & `ffun-1.5.3/ffun/library/migrations/20230514_01_Bwb35-processed-state.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py` & `ffun-1.5.3/ffun/library/migrations/20240315_01_tWftt-optimize-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py` & `ffun-1.5.3/ffun/library/migrations/20240503_01_Bmzw6-remove-l-entry-process-info.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py` & `ffun-1.5.3/ffun/library/migrations/20240506_01_My4vi-remove-duplicated-entries-from-feeds.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py` & `ffun-1.5.3/ffun/library/migrations/20240506_02_zQdSl-fix-unique-index-on-l-entries.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/operations.py` & `ffun-1.5.3/ffun/library/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/tests/fixtures.py` & `ffun-1.5.3/ffun/library/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/tests/make.py` & `ffun-1.5.3/ffun/library/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/tests/test_domain.py` & `ffun-1.5.3/ffun/library/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/library/tests/test_operations.py` & `ffun-1.5.3/ffun/library/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/loader/background_loader.py` & `ffun-1.5.3/ffun/loader/background_loader.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/loader/domain.py` & `ffun-1.5.3/ffun/loader/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/loader/tests/test_domain.py` & `ffun-1.5.3/ffun/loader/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py` & `ffun-1.5.3/ffun/markers/migrations/20230419_01_9vMm5-markers-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/markers/operations.py` & `ffun-1.5.3/ffun/markers/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/markers/tests/test_operations.py` & `ffun-1.5.3/ffun/markers/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/meta/domain.py` & `ffun-1.5.3/ffun/meta/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/meta/tests/test_domain.py` & `ffun-1.5.3/ffun/meta/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/domain.py` & `ffun-1.5.3/ffun/ontology/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/entities.py` & `ffun-1.5.3/ffun/ontology/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py` & `ffun-1.5.3/ffun/ontology/migrations/20230404_01_ZUBsm-ontology-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py` & `ffun-1.5.3/ffun/ontology/migrations/20230617_01_XDdNG-rename-tags-names-to-uid.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py` & `ffun-1.5.3/ffun/ontology/migrations/20230617_02_L0MmA-tags-relationship-processor-tracking.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py` & `ffun-1.5.3/ffun/ontology/migrations/20230617_03_de7vS-tags-properties.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/operations.py` & `ffun-1.5.3/ffun/ontology/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/tests/fixtures.py` & `ffun-1.5.3/ffun/ontology/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/ontology/tests/test_operations.py` & `ffun-1.5.3/ffun/ontology/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/openai/client.py` & `ffun-1.5.3/ffun/openai/client.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/openai/entities.py` & `ffun-1.5.3/ffun/openai/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/openai/keys_rotator.py` & `ffun-1.5.3/ffun/openai/keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/openai/keys_statuses.py` & `ffun-1.5.3/ffun/openai/keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/openai/tests/fixtures.py` & `ffun-1.5.3/ffun/openai/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/openai/tests/test_keys_rotator.py` & `ffun-1.5.3/ffun/openai/tests/test_keys_rotator.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/openai/tests/test_keys_statuses.py` & `ffun-1.5.3/ffun/openai/tests/test_keys_statuses.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/entities.py` & `ffun-1.5.3/ffun/parsers/entities.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/feed.py` & `ffun-1.5.3/ffun/parsers/feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/feedly.py` & `ffun-1.5.3/ffun/parsers/feedly.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml` & `ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json` & `ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/atom_with_relative_news_links.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml` & `ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json` & `ffun-1.5.3/ffun/parsers/tests/feeds_fixtures/wordpress_rss_2_0_feed.xml.expected.json`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/tests/make.py` & `ffun-1.5.3/ffun/parsers/tests/make.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/parsers/tests/test_feed.py` & `ffun-1.5.3/ffun/parsers/tests/test_feed.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/resources/domain.py` & `ffun-1.5.3/ffun/resources/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/resources/migrations/20230702_01_LEEES-resources-table.py` & `ffun-1.5.3/ffun/resources/migrations/20230702_01_LEEES-resources-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/resources/operations.py` & `ffun-1.5.3/ffun/resources/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/resources/tests/test_domain.py` & `ffun-1.5.3/ffun/resources/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/resources/tests/test_operations.py` & `ffun-1.5.3/ffun/resources/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/scores/domain.py` & `ffun-1.5.3/ffun/scores/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py` & `ffun-1.5.3/ffun/scores/migrations/20230417_01_0XYOQ-scores-tables.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py` & `ffun-1.5.3/ffun/scores/migrations/20230813_01_l7qop-updated-at-field.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/scores/operations.py` & `ffun-1.5.3/ffun/scores/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/scores/tests/test_domain.py` & `ffun-1.5.3/ffun/scores/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/scores/tests/test_operations.py` & `ffun-1.5.3/ffun/scores/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/tags/converters.py` & `ffun-1.5.3/ffun/tags/converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/tags/tests/test_converters.py` & `ffun-1.5.3/ffun/tags/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/user_settings/domain.py` & `ffun-1.5.3/ffun/user_settings/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py` & `ffun-1.5.3/ffun/user_settings/migrations/20230701_01_7zBP0-settings-table.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py` & `ffun-1.5.3/ffun/user_settings/migrations/20230911_01_5vjXI-index-to-search-by-value.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/user_settings/operations.py` & `ffun-1.5.3/ffun/user_settings/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/user_settings/settings.py` & `ffun-1.5.3/ffun/user_settings/settings.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/user_settings/tests/test_domain.py` & `ffun-1.5.3/ffun/user_settings/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/user_settings/tests/test_operations.py` & `ffun-1.5.3/ffun/user_settings/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/user_settings/types.py` & `ffun-1.5.3/ffun/user_settings/types.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/users/domain.py` & `ffun-1.5.3/ffun/users/domain.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/users/migrations/20230527_01_soIr3-users-mapping.py` & `ffun-1.5.3/ffun/users/migrations/20230527_01_soIr3-users-mapping.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/users/operations.py` & `ffun-1.5.3/ffun/users/operations.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/ffun/users/tests/fixtures.py` & `ffun-1.5.3/ffun/users/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ffun-1.5.2/pyproject.toml` & `ffun-1.5.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ffun"
-version = "1.5.2"
+version = "1.5.3"
 description = "Backend for the Feeds Fun — web-based news reader"
 repository = "https://github.com/Tiendil/feeds.fun"
 authors = ["Aliaksei Yaletski (Tiendil) <a.eletsky@gmail.com>"]
 license = " BSD-3-Clause"
 readme = "README.md"
 homepage = "https://feeds.fun"
 keywords = ["news", "news-reader", "news-aggregator",
```

### Comparing `ffun-1.5.2/PKG-INFO` & `ffun-1.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffun
-Version: 1.5.2
+Version: 1.5.3
 Summary: Backend for the Feeds Fun — web-based news reader
 Home-page: https://feeds.fun
 License:  BSD-3-Clause
 Keywords: news,news-reader,news-aggregator,rss,rss-reader,rss-aggregator,feed,feed-reader,feed-aggregator,atom,self-hosted
 Author: Aliaksei Yaletski (Tiendil)
 Author-email: a.eletsky@gmail.com
 Requires-Python: >=3.11,<4.0
```

