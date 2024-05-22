# Comparing `tmp/cyberdrop_dl-5.3.8.tar.gz` & `tmp/cyberdrop_dl-5.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop_dl-5.3.8.tar", max compression
+gzip compressed data, was "cyberdrop_dl-5.3.9.tar", max compression
```

## Comparing `cyberdrop_dl-5.3.8.tar` & `cyberdrop_dl-5.3.9.tar`

### file list

```diff
@@ -1,98 +1,98 @@
--rw-r--r--   0        0        0    35149 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/LICENSE
--rw-r--r--   0        0        0     2165 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/README.md
--rw-r--r--   0        0        0       22 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/clients/__init__.py
--rw-r--r--   0        0        0    15961 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/clients/download_client.py
--rw-r--r--   0        0        0     2245 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/clients/errors.py
--rw-r--r--   0        0        0     7981 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/clients/scraper_client.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0        0        0    12633 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/downloader/downloader.py
--rw-r--r--   0        0        0     6672 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/main.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/__init__.py
--rw-r--r--   0        0        0     4525 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/args_manager.py
--rw-r--r--   0        0        0     1801 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/cache_manager.py
--rw-r--r--   0        0        0     5779 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/client_manager.py
--rw-r--r--   0        0        0    11962 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/config_manager.py
--rw-r--r--   0        0        0     2241 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/db_manager.py
--rw-r--r--   0        0        0     3913 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/download_manager.py
--rw-r--r--   0        0        0     3271 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/log_manager.py
--rw-r--r--   0        0        0     9122 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/manager.py
--rw-r--r--   0        0        0     4053 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/path_manager.py
--rw-r--r--   0        0        0     3138 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/managers/progress_manager.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/__init__.py
--rw-r--r--   0        0        0    10160 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawler.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.480147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/__init__.py
--rw-r--r--   0        0        0     8410 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/bunkrr_crawler.py
--rw-r--r--   0        0        0    11970 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/celebforum_crawler.py
--rw-r--r--   0        0        0     6863 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/coomer_crawler.py
--rw-r--r--   0        0        0     3080 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/cyberdrop_crawler.py
--rw-r--r--   0        0        0     7896 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/cyberfile_crawler.py
--rw-r--r--   0        0        0     4118 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/ehentai_crawler.py
--rw-r--r--   0        0        0     3401 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/erome_crawler.py
--rw-r--r--   0        0        0    12595 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/f95zone_crawler.py
--rw-r--r--   0        0        0     3303 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/fapello_crawler.py
--rw-r--r--   0        0        0     6169 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/gofile_crawler.py
--rw-r--r--   0        0        0     2630 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/hotpic_crawler.py
--rw-r--r--   0        0        0     5060 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imageban_crawler.py
--rw-r--r--   0        0        0     4848 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imgbb_crawler.py
--rw-r--r--   0        0        0     3237 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imgbox_crawler.py
--rw-r--r--   0        0        0     4146 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imgkiwi_crawler.py
--rw-r--r--   0        0        0     4598 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imgur_crawler.py
--rw-r--r--   0        0        0     6824 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/jpgchurch_crawler.py
--rw-r--r--   0        0        0     9145 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/kemono_crawler.py
--rw-r--r--   0        0        0    12298 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/leakedmodels_crawler.py
--rw-r--r--   0        0        0     3345 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/mediafire_crawler.py
--rw-r--r--   0        0        0    12523 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/nudostar_crawler.py
--rw-r--r--   0        0        0     2522 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/nudostartv_crawler.py
--rw-r--r--   0        0        0     5464 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/omegascans_crawler.py
--rw-r--r--   0        0        0     3518 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/pimpandhost_crawler.py
--rw-r--r--   0        0        0     4261 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/pixeldrain_crawler.py
--rw-r--r--   0        0        0     2827 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/postimg_crawler.py
--rw-r--r--   0        0        0     3948 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/realbooru_crawler.py
--rw-r--r--   0        0        0     7569 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/reddit_crawler.py
--rw-r--r--   0        0        0     3886 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/redgifs_crawler.py
--rw-r--r--   0        0        0     3952 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/rule34xxx_crawler.py
--rw-r--r--   0        0        0     4017 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/rule34xyz_crawler.py
--rw-r--r--   0        0        0     1865 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/saint_crawler.py
--rw-r--r--   0        0        0     4162 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/scrolller_crawler.py
--rw-r--r--   0        0        0    12759 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/simpcity_crawler.py
--rw-r--r--   0        0        0    13535 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/socialmediagirls_crawler.py
--rw-r--r--   0        0        0     4240 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/toonily_crawler.py
--rw-r--r--   0        0        0    13019 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/xbunker_crawler.py
--rw-r--r--   0        0        0     2142 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/xbunkr_crawler.py
--rw-r--r--   0        0        0     2513 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/jdownloader.py
--rw-r--r--   0        0        0    20399 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/scraper.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/__init__.py
--rw-r--r--   0        0        0     3014 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/downloads_progress.py
--rw-r--r--   0        0        0     6836 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/file_progress.py
--rw-r--r--   0        0        0     4529 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/scraping_progress.py
--rw-r--r--   0        0        0     3734 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/statistic_progress.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/__init__.py
--rw-r--r--   0        0        0     5887 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/general_prompts.py
--rw-r--r--   0        0        0    12292 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/settings_authentication_prompts.py
--rw-r--r--   0        0        0     7561 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/settings_global_prompts.py
--rw-r--r--   0        0        0    19039 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/settings_user_prompts.py
--rw-r--r--   0        0        0      755 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/url_file_prompts.py
--rw-r--r--   0        0        0     5996 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/ui/ui.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/args/__init__.py
--rw-r--r--   0        0        0     7968 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/args/args.py
--rw-r--r--   0        0        0     2659 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/args/browser_cookie_extraction.py
--rw-r--r--   0        0        0     4403 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/args/config_definitions.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/database/__init__.py
--rw-r--r--   0        0        0     1605 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/database/table_definitions.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/database/tables/__init__.py
--rw-r--r--   0        0        0     9822 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/database/tables/history_table.py
--rw-r--r--   0        0        0     1058 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/database/tables/temp_table.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/dataclasses/__init__.py
--rw-r--r--   0        0        0     1852 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/dataclasses/supported_domains.py
--rw-r--r--   0        0        0     1976 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/dataclasses/url_objects.py
--rw-r--r--   0        0        0     8403 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/sorting.py
--rw-r--r--   0        0        0        0 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/transfer/__init__.py
--rw-r--r--   0        0        0    12785 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/transfer/first_time_setup.py
--rw-r--r--   0        0        0     8301 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/transfer/transfer_v4_config.py
--rw-r--r--   0        0        0     1261 2024-05-12 02:23:40.484147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/transfer/transfer_v4_db.py
--rw-r--r--   0        0        0    10428 2024-05-12 02:23:40.488147 cyberdrop_dl-5.3.8/cyberdrop_dl/utils/utilities.py
--rw-r--r--   0        0        0      963 2024-05-12 02:23:40.488147 cyberdrop_dl-5.3.8/pyproject.toml
--rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 cyberdrop_dl-5.3.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/LICENSE
+-rw-r--r--   0        0        0     2165 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/README.md
+-rw-r--r--   0        0        0       22 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/clients/__init__.py
+-rw-r--r--   0        0        0    15961 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/clients/download_client.py
+-rw-r--r--   0        0        0     2245 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/clients/errors.py
+-rw-r--r--   0        0        0     7981 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/clients/scraper_client.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0        0        0    12633 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/downloader/downloader.py
+-rw-r--r--   0        0        0     6672 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/main.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/__init__.py
+-rw-r--r--   0        0        0     4525 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/args_manager.py
+-rw-r--r--   0        0        0     1801 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/cache_manager.py
+-rw-r--r--   0        0        0     5779 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/client_manager.py
+-rw-r--r--   0        0        0    12403 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/config_manager.py
+-rw-r--r--   0        0        0     2241 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/db_manager.py
+-rw-r--r--   0        0        0     3913 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/download_manager.py
+-rw-r--r--   0        0        0     3271 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/log_manager.py
+-rw-r--r--   0        0        0     9122 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/manager.py
+-rw-r--r--   0        0        0     4053 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/path_manager.py
+-rw-r--r--   0        0        0     3138 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/managers/progress_manager.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/__init__.py
+-rw-r--r--   0        0        0    10160 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawler.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/__init__.py
+-rw-r--r--   0        0        0     8410 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/bunkrr_crawler.py
+-rw-r--r--   0        0        0    11970 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/celebforum_crawler.py
+-rw-r--r--   0        0        0     6863 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/coomer_crawler.py
+-rw-r--r--   0        0        0     3080 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/cyberdrop_crawler.py
+-rw-r--r--   0        0        0     7896 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/cyberfile_crawler.py
+-rw-r--r--   0        0        0     4118 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/ehentai_crawler.py
+-rw-r--r--   0        0        0     3401 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/erome_crawler.py
+-rw-r--r--   0        0        0    12595 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/f95zone_crawler.py
+-rw-r--r--   0        0        0     3303 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/fapello_crawler.py
+-rw-r--r--   0        0        0     6169 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/gofile_crawler.py
+-rw-r--r--   0        0        0     2630 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/hotpic_crawler.py
+-rw-r--r--   0        0        0     5060 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imageban_crawler.py
+-rw-r--r--   0        0        0     4848 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imgbb_crawler.py
+-rw-r--r--   0        0        0     3237 2024-05-12 16:42:32.433712 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imgbox_crawler.py
+-rw-r--r--   0        0        0     4146 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imgkiwi_crawler.py
+-rw-r--r--   0        0        0     4598 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imgur_crawler.py
+-rw-r--r--   0        0        0     6824 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/jpgchurch_crawler.py
+-rw-r--r--   0        0        0     9145 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/kemono_crawler.py
+-rw-r--r--   0        0        0    12298 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/leakedmodels_crawler.py
+-rw-r--r--   0        0        0     3345 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/mediafire_crawler.py
+-rw-r--r--   0        0        0    12523 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/nudostar_crawler.py
+-rw-r--r--   0        0        0     2522 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/nudostartv_crawler.py
+-rw-r--r--   0        0        0     5464 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/omegascans_crawler.py
+-rw-r--r--   0        0        0     3518 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/pimpandhost_crawler.py
+-rw-r--r--   0        0        0     4261 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/pixeldrain_crawler.py
+-rw-r--r--   0        0        0     2827 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/postimg_crawler.py
+-rw-r--r--   0        0        0     3948 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/realbooru_crawler.py
+-rw-r--r--   0        0        0     7569 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/reddit_crawler.py
+-rw-r--r--   0        0        0     3886 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/redgifs_crawler.py
+-rw-r--r--   0        0        0     3952 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/rule34xxx_crawler.py
+-rw-r--r--   0        0        0     4017 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/rule34xyz_crawler.py
+-rw-r--r--   0        0        0     1865 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/saint_crawler.py
+-rw-r--r--   0        0        0     4162 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/scrolller_crawler.py
+-rw-r--r--   0        0        0    12759 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/simpcity_crawler.py
+-rw-r--r--   0        0        0    13535 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/socialmediagirls_crawler.py
+-rw-r--r--   0        0        0     4240 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/toonily_crawler.py
+-rw-r--r--   0        0        0    13019 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/xbunker_crawler.py
+-rw-r--r--   0        0        0     2142 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/xbunkr_crawler.py
+-rw-r--r--   0        0        0     2513 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/jdownloader.py
+-rw-r--r--   0        0        0    20399 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/scraper.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/__init__.py
+-rw-r--r--   0        0        0     3014 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/downloads_progress.py
+-rw-r--r--   0        0        0     6836 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/file_progress.py
+-rw-r--r--   0        0        0     4529 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/scraping_progress.py
+-rw-r--r--   0        0        0     3734 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/statistic_progress.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/__init__.py
+-rw-r--r--   0        0        0     5887 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/general_prompts.py
+-rw-r--r--   0        0        0    12292 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/settings_authentication_prompts.py
+-rw-r--r--   0        0        0     7561 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/settings_global_prompts.py
+-rw-r--r--   0        0        0    19039 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/settings_user_prompts.py
+-rw-r--r--   0        0        0      755 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/url_file_prompts.py
+-rw-r--r--   0        0        0     5996 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/ui/ui.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/args/__init__.py
+-rw-r--r--   0        0        0     7968 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/args/args.py
+-rw-r--r--   0        0        0     2659 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/args/browser_cookie_extraction.py
+-rw-r--r--   0        0        0     4403 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/args/config_definitions.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/database/__init__.py
+-rw-r--r--   0        0        0     1605 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/database/table_definitions.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/database/tables/__init__.py
+-rw-r--r--   0        0        0     9822 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/database/tables/history_table.py
+-rw-r--r--   0        0        0     1058 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/database/tables/temp_table.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/dataclasses/__init__.py
+-rw-r--r--   0        0        0     1852 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/dataclasses/supported_domains.py
+-rw-r--r--   0        0        0     1976 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/dataclasses/url_objects.py
+-rw-r--r--   0        0        0     8403 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/sorting.py
+-rw-r--r--   0        0        0        0 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/transfer/__init__.py
+-rw-r--r--   0        0        0    12785 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/transfer/first_time_setup.py
+-rw-r--r--   0        0        0     8301 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/transfer/transfer_v4_config.py
+-rw-r--r--   0        0        0     1261 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/transfer/transfer_v4_db.py
+-rw-r--r--   0        0        0    10428 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/cyberdrop_dl/utils/utilities.py
+-rw-r--r--   0        0        0      963 2024-05-12 16:42:32.437713 cyberdrop_dl-5.3.9/pyproject.toml
+-rw-r--r--   0        0        0     3546 1970-01-01 00:00:00.000000 cyberdrop_dl-5.3.9/PKG-INFO
```

### Comparing `cyberdrop_dl-5.3.8/LICENSE` & `cyberdrop_dl-5.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/README.md` & `cyberdrop_dl-5.3.9/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/clients/download_client.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/clients/download_client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/clients/errors.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/clients/errors.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/clients/scraper_client.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/clients/scraper_client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/downloader/downloader.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/main.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/args_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/args_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/cache_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/cache_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/client_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/client_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/config_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/config_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,14 +33,24 @@
 def _load_yaml(file: Path) -> Dict:
     """Loads a yaml file and returns it as a dict"""
     with open(file, 'r') as yaml_file:
         yaml_values = yaml.load(yaml_file.read(), Loader=yaml.FullLoader)
         return yaml_values if yaml_values else {}
 
 
+def get_keys(dl, keys=None):
+    keys = keys or []
+    if isinstance(dl, dict):
+        keys += dl.keys()
+        _ = [get_keys(x, keys) for x in dl.values()]
+    elif isinstance(dl, list):
+        _ = [get_keys(x, keys) for x in dl]
+    return list(set(keys))
+
+
 class ConfigManager:
     def __init__(self, manager: 'Manager'):
         self.manager = manager
         self.loaded_config: str = field(init=False)
 
         self.authentication_settings: Path = field(init=False)
         self.settings: Path = field(init=False)
@@ -95,72 +105,88 @@
             self.settings_data['Sorting']['sort_folder'] = DOWNLOAD_STORAGE / "Cyberdrop-DL Sorted Downloads"
             self.write_updated_settings_config()
 
     def _verify_authentication_config(self) -> None:
         """Verifies the authentication config file and creates it if it doesn't exist"""
         default_auth_data = copy.deepcopy(authentication_settings)
         existing_auth_data = _load_yaml(self.authentication_settings)
-        
-        if default_auth_data.keys() == existing_auth_data.keys():
+
+        if get_keys(default_auth_data) == get_keys(existing_auth_data):
             self.authentication_data = existing_auth_data
             return
-        
+
         self.authentication_data = _match_config_dicts(default_auth_data, existing_auth_data)
         _save_yaml(self.authentication_settings, self.authentication_data)
 
     def _verify_settings_config(self) -> None:
         """Verifies the settings config file and creates it if it doesn't exist"""
         default_settings_data = copy.deepcopy(settings)
         existing_settings_data = _load_yaml(self.settings)
         self.settings_data = _match_config_dicts(default_settings_data, existing_settings_data)
         self.settings_data['Files']['input_file'] = Path(self.settings_data['Files']['input_file'])
         self.settings_data['Files']['download_folder'] = Path(self.settings_data['Files']['download_folder'])
         self.settings_data["Logs"]["log_folder"] = Path(self.settings_data["Logs"]["log_folder"])
         self.settings_data['Sorting']['sort_folder'] = Path(self.settings_data['Sorting']['sort_folder'])
 
         # change to ints
-        self.settings_data['File_Size_Limits']['maximum_image_size'] = int(self.settings_data['File_Size_Limits']['maximum_image_size'])
-        self.settings_data['File_Size_Limits']['maximum_video_size'] = int(self.settings_data['File_Size_Limits']['maximum_video_size'])
-        self.settings_data['File_Size_Limits']['maximum_other_size'] = int(self.settings_data['File_Size_Limits']['maximum_other_size'])
-        self.settings_data['File_Size_Limits']['minimum_image_size'] = int(self.settings_data['File_Size_Limits']['minimum_image_size'])
-        self.settings_data['File_Size_Limits']['minimum_video_size'] = int(self.settings_data['File_Size_Limits']['minimum_video_size'])
-        self.settings_data['File_Size_Limits']['minimum_other_size'] = int(self.settings_data['File_Size_Limits']['minimum_other_size'])
-        
-        self.settings_data['Runtime_Options']['ui_refresh_rate'] = int(self.settings_data['Runtime_Options']['ui_refresh_rate'])
+        self.settings_data['File_Size_Limits']['maximum_image_size'] = int(
+            self.settings_data['File_Size_Limits']['maximum_image_size'])
+        self.settings_data['File_Size_Limits']['maximum_video_size'] = int(
+            self.settings_data['File_Size_Limits']['maximum_video_size'])
+        self.settings_data['File_Size_Limits']['maximum_other_size'] = int(
+            self.settings_data['File_Size_Limits']['maximum_other_size'])
+        self.settings_data['File_Size_Limits']['minimum_image_size'] = int(
+            self.settings_data['File_Size_Limits']['minimum_image_size'])
+        self.settings_data['File_Size_Limits']['minimum_video_size'] = int(
+            self.settings_data['File_Size_Limits']['minimum_video_size'])
+        self.settings_data['File_Size_Limits']['minimum_other_size'] = int(
+            self.settings_data['File_Size_Limits']['minimum_other_size'])
+
+        self.settings_data['Runtime_Options']['ui_refresh_rate'] = int(
+            self.settings_data['Runtime_Options']['ui_refresh_rate'])
         self.settings_data['Runtime_Options']['log_level'] = int(self.settings_data['Runtime_Options']['log_level'])
 
-        self.global_settings_data['General']['max_file_name_length'] = int(self.global_settings_data['General']['max_file_name_length'])
-        self.global_settings_data['General']['max_folder_name_length'] = int(self.global_settings_data['General']['max_folder_name_length'])
-        self.global_settings_data['Rate_Limiting_Options']['connection_timeout'] = int(self.global_settings_data['Rate_Limiting_Options']['connection_timeout'])
-        self.global_settings_data['Rate_Limiting_Options']['download_attempts'] = int(self.global_settings_data['Rate_Limiting_Options']['download_attempts'])
-        self.global_settings_data['Rate_Limiting_Options']['download_delay'] = int(self.global_settings_data['Rate_Limiting_Options']['download_delay'])
-        self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads'] = int(self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads'])
-        self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads_per_domain'] = int(self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads_per_domain'])
-        self.global_settings_data['Rate_Limiting_Options']['rate_limit'] = int(self.global_settings_data['Rate_Limiting_Options']['rate_limit'])
-        self.global_settings_data['Rate_Limiting_Options']['read_timeout'] = int(self.global_settings_data['Rate_Limiting_Options']['read_timeout'])
+        self.global_settings_data['General']['max_file_name_length'] = int(
+            self.global_settings_data['General']['max_file_name_length'])
+        self.global_settings_data['General']['max_folder_name_length'] = int(
+            self.global_settings_data['General']['max_folder_name_length'])
+        self.global_settings_data['Rate_Limiting_Options']['connection_timeout'] = int(
+            self.global_settings_data['Rate_Limiting_Options']['connection_timeout'])
+        self.global_settings_data['Rate_Limiting_Options']['download_attempts'] = int(
+            self.global_settings_data['Rate_Limiting_Options']['download_attempts'])
+        self.global_settings_data['Rate_Limiting_Options']['download_delay'] = int(
+            self.global_settings_data['Rate_Limiting_Options']['download_delay'])
+        self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads'] = int(
+            self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads'])
+        self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads_per_domain'] = int(
+            self.global_settings_data['Rate_Limiting_Options']['max_simultaneous_downloads_per_domain'])
+        self.global_settings_data['Rate_Limiting_Options']['rate_limit'] = int(
+            self.global_settings_data['Rate_Limiting_Options']['rate_limit'])
+        self.global_settings_data['Rate_Limiting_Options']['read_timeout'] = int(
+            self.global_settings_data['Rate_Limiting_Options']['read_timeout'])
 
-        if default_settings_data.keys() == existing_settings_data.keys():
+        if get_keys(default_settings_data) == get_keys(existing_settings_data):
             return
-        
+
         save_data = copy.deepcopy(self.settings_data)
         save_data['Files']['input_file'] = str(save_data['Files']['input_file'])
         save_data['Files']['download_folder'] = str(save_data['Files']['download_folder'])
         save_data["Logs"]["log_folder"] = str(save_data["Logs"]["log_folder"])
         save_data['Sorting']['sort_folder'] = str(save_data['Sorting']['sort_folder'])
         _save_yaml(self.settings, save_data)
 
     def _verify_global_settings_config(self) -> None:
         """Verifies the global settings config file and creates it if it doesn't exist"""
         default_global_settings_data = copy.deepcopy(global_settings)
         existing_global_settings_data = _load_yaml(self.global_settings)
-        
-        if default_global_settings_data.keys() == existing_global_settings_data.keys():
+
+        if get_keys(default_global_settings_data) == get_keys(existing_global_settings_data):
             self.global_settings_data = existing_global_settings_data
             return
-        
+
         self.global_settings_data = _match_config_dicts(default_global_settings_data, existing_global_settings_data)
         _save_yaml(self.global_settings, self.global_settings_data)
 
     """~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~"""
 
     def create_new_config(self, new_settings: Path, settings_data: Dict) -> None:
         """Creates a new settings config file"""
```

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/db_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/db_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/download_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/download_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/log_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/log_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/path_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/path_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/managers/progress_manager.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/managers/progress_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/bunkrr_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/bunkrr_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/celebforum_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/celebforum_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/coomer_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/coomer_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/cyberdrop_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/cyberdrop_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/cyberfile_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/cyberfile_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/ehentai_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/ehentai_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/erome_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/erome_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/f95zone_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/f95zone_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/fapello_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/fapello_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/gofile_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/gofile_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/hotpic_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/hotpic_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imageban_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imageban_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imgbb_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imgbb_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imgbox_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imgbox_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imgkiwi_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imgkiwi_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/imgur_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/imgur_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/jpgchurch_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/jpgchurch_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/kemono_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/kemono_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/leakedmodels_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/leakedmodels_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/mediafire_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/mediafire_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/nudostar_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/nudostar_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/nudostartv_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/nudostartv_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/omegascans_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/omegascans_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/pimpandhost_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/pimpandhost_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/pixeldrain_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/pixeldrain_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/postimg_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/postimg_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/realbooru_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/realbooru_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/reddit_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/reddit_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/redgifs_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/redgifs_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/rule34xxx_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/rule34xxx_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/rule34xyz_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/rule34xyz_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/saint_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/saint_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/scrolller_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/scrolller_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/simpcity_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/simpcity_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/socialmediagirls_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/socialmediagirls_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/toonily_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/toonily_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/xbunker_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/xbunker_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/crawlers/xbunkr_crawler.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/crawlers/xbunkr_crawler.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/jdownloader.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/jdownloader.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/scraper/scraper.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/downloads_progress.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/downloads_progress.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/file_progress.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/file_progress.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/scraping_progress.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/scraping_progress.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/progress/statistic_progress.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/progress/statistic_progress.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/general_prompts.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/general_prompts.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/settings_authentication_prompts.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/settings_authentication_prompts.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/settings_global_prompts.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/settings_global_prompts.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/settings_user_prompts.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/settings_user_prompts.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/prompts/url_file_prompts.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/prompts/url_file_prompts.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/ui/ui.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/ui/ui.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/args/args.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/args/args.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/args/browser_cookie_extraction.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/args/browser_cookie_extraction.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/args/config_definitions.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/args/config_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/database/table_definitions.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/database/table_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/database/tables/history_table.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/database/tables/history_table.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/database/tables/temp_table.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/database/tables/temp_table.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/dataclasses/supported_domains.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/dataclasses/supported_domains.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/dataclasses/url_objects.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/dataclasses/url_objects.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/sorting.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/sorting.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/transfer/first_time_setup.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/transfer/first_time_setup.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/transfer/transfer_v4_config.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/transfer/transfer_v4_config.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/transfer/transfer_v4_db.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/transfer/transfer_v4_db.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/cyberdrop_dl/utils/utilities.py` & `cyberdrop_dl-5.3.9/cyberdrop_dl/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `cyberdrop_dl-5.3.8/pyproject.toml` & `cyberdrop_dl-5.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyberdrop-dl"
-version = "5.3.8"
+version = "5.3.9"
 description = "Bulk downloader for multiple file hosts"
 authors = ["Jules Winnfield <juleswinnfieldII@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Jules-WinnfieldX/CyberDropDownloader"
 documentation = "https://jules-winnfieldx.gitbook.io/cyberdrop-dl/"
 packages = [{include = "cyberdrop_dl"}]
```

### Comparing `cyberdrop_dl-5.3.8/PKG-INFO` & `cyberdrop_dl-5.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 5.3.8
+Version: 5.3.9
 Summary: Bulk downloader for multiple file hosts
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules Winnfield
 Author-email: juleswinnfieldII@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 5.3.8 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 5.3.9 Summary: Bulk
 downloader for multiple file hosts Home-page: https://github.com/Jules-
 WinnfieldX/CyberDropDownloader Author: Jules Winnfield Author-email:
 juleswinnfieldII@protonmail.com Requires-Python: >=3.11,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-Dist:
 aiofiles (==0.8.0) Requires-Dist: aiohttp (>=3.9.1,<4.0.0) Requires-Dist:
 aiolimiter (>=1.1.0,<2.0.0) Requires-Dist: aiosqlite (==0.17.0) Requires-Dist:
```

