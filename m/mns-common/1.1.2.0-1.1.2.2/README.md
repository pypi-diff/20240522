# Comparing `tmp/mns_common-1.1.2.0.tar.gz` & `tmp/mns_common-1.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns_common-1.1.2.0.tar", last modified: Mon May 20 14:29:08 2024, max compression
+gzip compressed data, was "mns_common-1.1.2.2.tar", last modified: Wed May 22 08:23:53 2024, max compression
```

## Comparing `mns_common-1.1.2.0.tar` & `mns_common-1.1.2.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.103164 mns_common-1.1.2.0/
--rw-rw-rw-   0        0        0       59 2024-05-20 14:29:08.102167 mns_common-1.1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.065265 mns_common-1.1.2.0/mns_common/
--rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.2.0/mns_common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.067260 mns_common-1.1.2.0/mns_common/api/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.2.0/mns_common/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.070253 mns_common-1.1.2.0/mns_common/api/akshare/
--rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.2.0/mns_common/api/akshare/__init__.py
--rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/akshare/k_line_api.py
--rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.2.0/mns_common/api/akshare/stock_bid_ask_api.py
--rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/api/akshare/stock_dt_pool.py
--rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.2.0/mns_common/api/akshare/stock_zb_pool.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/api/akshare/stock_zt_pool_api.py
--rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/api/akshare/yjyg_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.073244 mns_common-1.1.2.0/mns_common/api/em/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.2.0/mns_common/api/em/__init__.py
--rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.2.0/mns_common/api/em/east_money_stock_api.py
--rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
--rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.2.0/mns_common/api/em/east_money_stock_hk_api.py
--rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.2.0/mns_common/api/em/east_money_stock_v2_api.py
--rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/em/em_concept_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.073244 mns_common-1.1.2.0/mns_common/api/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/api/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.074241 mns_common-1.1.2.0/mns_common/api/kpl/common/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/kpl/common/__init__.py
--rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.2.0/mns_common/api/kpl/common/kpl_common_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.075239 mns_common-1.1.2.0/mns_common/api/kpl/concept/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/kpl/concept/__init__.py
--rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/api/kpl/concept/kpl_concept_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.076236 mns_common-1.1.2.0/mns_common/api/kpl/constant/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/kpl/constant/__init__.py
--rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/kpl/constant/kpl_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.076236 mns_common-1.1.2.0/mns_common/api/kpl/industry/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/kpl/industry/__init__.py
--rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/api/kpl/industry/kpl_industry_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.077234 mns_common-1.1.2.0/mns_common/api/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/kpl/selection/__init__.py
--rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.2.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.079229 mns_common-1.1.2.0/mns_common/api/kpl/symbol/
--rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/kpl/symbol/__init__.py
--rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.2.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
--rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.2.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
--rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.2.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.080227 mns_common-1.1.2.0/mns_common/api/msg/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/msg/__init__.py
--rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.2.0/mns_common/api/msg/push_msg_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.081223 mns_common-1.1.2.0/mns_common/api/ths/
--rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.2.0/mns_common/api/ths/__init__.py
--rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.2.0/mns_common/api/ths/ths_big_deal_api.py
--rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.2.0/mns_common/api/ths/ths_stock_api.py
--rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.2.0/mns_common/api/ths/ths_stock_zt_pool_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.082221 mns_common-1.1.2.0/mns_common/component/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.2.0/mns_common/component/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.083218 mns_common-1.1.2.0/mns_common/component/cache/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.2.0/mns_common/component/cache/__init__.py
--rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.2.0/mns_common/component/cache/cache_service.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.084215 mns_common-1.1.2.0/mns_common/component/classify/
--rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.1.2.0/mns_common/component/classify/__init__.py
--rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.1.2.0/mns_common/component/classify/classify_constant.py
--rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.1.2.0/mns_common/component/classify/symbol_classify_api.py
--rw-rw-rw-   0        0        0     5068 2024-05-15 08:05:35.000000 mns_common-1.1.2.0/mns_common/component/common_service_fun_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.085213 mns_common-1.1.2.0/mns_common/component/company/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/component/company/__init__.py
--rw-rw-rw-   0        0        0     7217 2024-05-17 13:48:14.000000 mns_common-1.1.2.0/mns_common/component/company/company_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.086210 mns_common-1.1.2.0/mns_common/component/concept/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/component/concept/__init__.py
--rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.2.0/mns_common/component/concept/kpl_concept_common_service_api.py
--rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.1.2.0/mns_common/component/concept/ths_concept_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.087207 mns_common-1.1.2.0/mns_common/component/data/
--rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.2.0/mns_common/component/data/__init__.py
--rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.2.0/mns_common/component/data/data_init_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.088242 mns_common-1.1.2.0/mns_common/component/industry/
--rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.2.0/mns_common/component/industry/__init__.py
--rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.2.0/mns_common/component/industry/ths_industry_index_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.089202 mns_common-1.1.2.0/mns_common/component/k_line/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/component/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.090200 mns_common-1.1.2.0/mns_common/component/k_line/clean/
--rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.2.0/mns_common/component/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.2.0/mns_common/component/k_line/clean/k_line_param.py
--rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.2.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.091197 mns_common-1.1.2.0/mns_common/component/k_line/common/
--rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.2.0/mns_common/component/k_line/common/__init__.py
--rw-rw-rw-   0        0        0     4770 2024-05-20 14:28:57.000000 mns_common-1.1.2.0/mns_common/component/k_line/common/k_line_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.092194 mns_common-1.1.2.0/mns_common/component/k_line/patterns/
--rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.2.0/mns_common/component/k_line/patterns/__init__.py
--rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.2.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
--rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.2.0/mns_common/component/k_line/patterns/pattern_Enum.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.093191 mns_common-1.1.2.0/mns_common/component/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/component/real_time/__init__.py
--rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/component/real_time/real_time_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.094188 mns_common-1.1.2.0/mns_common/component/self_choose/
--rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.2.0/mns_common/component/self_choose/__init__.py
--rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.2.0/mns_common/component/self_choose/black_list_service_api.py
--rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.2.0/mns_common/component/self_choose/self_choose_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.095186 mns_common-1.1.2.0/mns_common/component/trade/
--rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.2.0/mns_common/component/trade/__init__.py
--rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.2.0/mns_common/component/trade/trade_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.096183 mns_common-1.1.2.0/mns_common/component/trade_date/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/component/trade_date/__init__.py
--rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.1.2.0/mns_common/component/trade_date/trade_date_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.096183 mns_common-1.1.2.0/mns_common/component/zt/
--rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.0/mns_common/component/zt/__init__.py
--rw-rw-rw-   0        0        0     8650 2024-05-12 14:00:57.000000 mns_common-1.1.2.0/mns_common/component/zt/zt_common_service_api.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.098178 mns_common-1.1.2.0/mns_common/constant/
--rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.2.0/mns_common/constant/__init__.py
--rw-rw-rw-   0        0        0     2072 2024-05-20 14:27:17.000000 mns_common-1.1.2.0/mns_common/constant/db_name_constant.py
--rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.1.2.0/mns_common/constant/kpl_selection_no_choose_constant.py
--rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.1.2.0/mns_common/constant/self_choose_constant.py
--rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.1.2.0/mns_common/constant/ths_concept_no_choose_constant.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.099175 mns_common-1.1.2.0/mns_common/db/
--rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.1.2.0/mns_common/db/MongodbUtil.py
--rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.2.0/mns_common/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.101169 mns_common-1.1.2.0/mns_common/utils/
--rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.2.0/mns_common/utils/__init__.py
--rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.2.0/mns_common/utils/async_fun.py
--rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.2.0/mns_common/utils/data_frame_util.py
--rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.1.2.0/mns_common/utils/date_handle_util.py
--rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.2.0/mns_common/utils/ip_util.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:29:08.102167 mns_common-1.1.2.0/mns_common.egg-info/
--rw-rw-rw-   0        0        0       59 2024-05-20 14:29:07.000000 mns_common-1.1.2.0/mns_common.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3872 2024-05-20 14:29:08.000000 mns_common-1.1.2.0/mns_common.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 14:29:07.000000 mns_common-1.1.2.0/mns_common.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-20 14:29:07.000000 mns_common-1.1.2.0/mns_common.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 14:29:08.103164 mns_common-1.1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      466 2024-05-20 14:28:57.000000 mns_common-1.1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.331359 mns_common-1.1.2.2/
+-rw-rw-rw-   0        0        0       59 2024-05-22 08:23:53.331359 mns_common-1.1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1354 2023-12-14 15:25:31.000000 mns_common-1.1.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.287478 mns_common-1.1.2.2/mns_common/
+-rw-rw-rw-   0        0        0      163 2024-01-10 10:52:31.000000 mns_common-1.1.2.2/mns_common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.289472 mns_common-1.1.2.2/mns_common/api/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.2.2/mns_common/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.292492 mns_common-1.1.2.2/mns_common/api/akshare/
+-rw-rw-rw-   0        0        0      165 2023-12-15 04:25:30.000000 mns_common-1.1.2.2/mns_common/api/akshare/__init__.py
+-rw-rw-rw-   0        0        0     5057 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/akshare/k_line_api.py
+-rw-rw-rw-   0        0        0     5999 2024-01-05 08:16:46.000000 mns_common-1.1.2.2/mns_common/api/akshare/stock_bid_ask_api.py
+-rw-rw-rw-   0        0        0     2245 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/api/akshare/stock_dt_pool.py
+-rw-rw-rw-   0        0        0     2038 2023-12-16 13:25:10.000000 mns_common-1.1.2.2/mns_common/api/akshare/stock_zb_pool.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/api/akshare/stock_zt_pool_api.py
+-rw-rw-rw-   0        0        0     4108 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/api/akshare/yjyg_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.297451 mns_common-1.1.2.2/mns_common/api/em/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.2.2/mns_common/api/em/__init__.py
+-rw-rw-rw-   0        0        0     8352 2024-05-10 13:01:52.000000 mns_common-1.1.2.2/mns_common/api/em/east_money_stock_api.py
+-rw-rw-rw-   0        0        0     5504 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py
+-rw-rw-rw-   0        0        0     4371 2024-05-17 04:06:34.000000 mns_common-1.1.2.2/mns_common/api/em/east_money_stock_hk_api.py
+-rw-rw-rw-   0        0        0    14960 2024-05-10 12:40:48.000000 mns_common-1.1.2.2/mns_common/api/em/east_money_stock_v2_api.py
+-rw-rw-rw-   0        0        0     8285 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/em/em_concept_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.298477 mns_common-1.1.2.2/mns_common/api/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/api/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.299473 mns_common-1.1.2.2/mns_common/api/kpl/common/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/kpl/common/__init__.py
+-rw-rw-rw-   0        0        0     6536 2024-04-24 09:08:22.000000 mns_common-1.1.2.2/mns_common/api/kpl/common/kpl_common_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.299473 mns_common-1.1.2.2/mns_common/api/kpl/concept/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/kpl/concept/__init__.py
+-rw-rw-rw-   0        0        0      607 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/api/kpl/concept/kpl_concept_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.300470 mns_common-1.1.2.2/mns_common/api/kpl/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/kpl/constant/__init__.py
+-rw-rw-rw-   0        0        0      669 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/kpl/constant/kpl_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.301467 mns_common-1.1.2.2/mns_common/api/kpl/industry/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/kpl/industry/__init__.py
+-rw-rw-rw-   0        0        0      565 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/api/kpl/industry/kpl_industry_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.302464 mns_common-1.1.2.2/mns_common/api/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/kpl/selection/__init__.py
+-rw-rw-rw-   0        0        0     1926 2024-05-06 13:55:26.000000 mns_common-1.1.2.2/mns_common/api/kpl/selection/kpl_selection_plate_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.304460 mns_common-1.1.2.2/mns_common/api/kpl/symbol/
+-rw-rw-rw-   0        0        0      161 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/kpl/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4792 2024-03-22 08:55:03.000000 mns_common-1.1.2.2/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py
+-rw-rw-rw-   0        0        0     1625 2024-03-22 08:56:47.000000 mns_common-1.1.2.2/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py
+-rw-rw-rw-   0        0        0     4210 2024-04-21 02:03:32.000000 mns_common-1.1.2.2/mns_common/api/kpl/symbol/symbol_his_quotes_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.305457 mns_common-1.1.2.2/mns_common/api/msg/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/msg/__init__.py
+-rw-rw-rw-   0        0        0     1421 2024-02-03 04:57:25.000000 mns_common-1.1.2.2/mns_common/api/msg/push_msg_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.307449 mns_common-1.1.2.2/mns_common/api/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-15 03:59:01.000000 mns_common-1.1.2.2/mns_common/api/ths/__init__.py
+-rw-rw-rw-   0        0        0     3614 2023-12-22 09:50:37.000000 mns_common-1.1.2.2/mns_common/api/ths/ths_big_deal_api.py
+-rw-rw-rw-   0        0        0    40309 2024-05-14 08:22:47.000000 mns_common-1.1.2.2/mns_common/api/ths/ths_stock_api.py
+-rw-rw-rw-   0        0        0     6648 2024-05-20 06:35:22.000000 mns_common-1.1.2.2/mns_common/api/ths/ths_stock_zt_pool_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.308421 mns_common-1.1.2.2/mns_common/component/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:38:42.000000 mns_common-1.1.2.2/mns_common/component/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.309418 mns_common-1.1.2.2/mns_common/component/cache/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.2.2/mns_common/component/cache/__init__.py
+-rw-rw-rw-   0        0        0      809 2024-04-28 07:38:03.000000 mns_common-1.1.2.2/mns_common/component/cache/cache_service.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.311413 mns_common-1.1.2.2/mns_common/component/classify/
+-rw-rw-rw-   0        0        0      163 2024-01-09 08:35:24.000000 mns_common-1.1.2.2/mns_common/component/classify/__init__.py
+-rw-rw-rw-   0        0        0      522 2024-01-09 09:22:06.000000 mns_common-1.1.2.2/mns_common/component/classify/classify_constant.py
+-rw-rw-rw-   0        0        0     3880 2024-01-09 08:35:24.000000 mns_common-1.1.2.2/mns_common/component/classify/symbol_classify_api.py
+-rw-rw-rw-   0        0        0     5068 2024-05-15 08:05:35.000000 mns_common-1.1.2.2/mns_common/component/common_service_fun_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.311413 mns_common-1.1.2.2/mns_common/component/company/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/component/company/__init__.py
+-rw-rw-rw-   0        0        0     7217 2024-05-17 13:48:14.000000 mns_common-1.1.2.2/mns_common/component/company/company_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.313407 mns_common-1.1.2.2/mns_common/component/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/component/concept/__init__.py
+-rw-rw-rw-   0        0        0     3235 2024-05-09 14:23:16.000000 mns_common-1.1.2.2/mns_common/component/concept/kpl_concept_common_service_api.py
+-rw-rw-rw-   0        0        0     9637 2024-04-30 09:46:26.000000 mns_common-1.1.2.2/mns_common/component/concept/ths_concept_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.314405 mns_common-1.1.2.2/mns_common/component/data/
+-rw-rw-rw-   0        0        0      163 2024-04-28 07:37:23.000000 mns_common-1.1.2.2/mns_common/component/data/__init__.py
+-rw-rw-rw-   0        0        0     4757 2023-12-17 11:40:38.000000 mns_common-1.1.2.2/mns_common/component/data/data_init_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.315402 mns_common-1.1.2.2/mns_common/component/industry/
+-rw-rw-rw-   0        0        0      163 2024-01-13 08:34:39.000000 mns_common-1.1.2.2/mns_common/component/industry/__init__.py
+-rw-rw-rw-   0        0        0     3252 2024-01-13 08:57:34.000000 mns_common-1.1.2.2/mns_common/component/industry/ths_industry_index_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.315402 mns_common-1.1.2.2/mns_common/component/k_line/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/component/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.317397 mns_common-1.1.2.2/mns_common/component/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2024-01-09 09:22:06.000000 mns_common-1.1.2.2/mns_common/component/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-01-09 09:22:06.000000 mns_common-1.1.2.2/mns_common/component/k_line/clean/k_line_param.py
+-rw-rw-rw-   0        0        0    12593 2024-01-09 10:28:47.000000 mns_common-1.1.2.2/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.318395 mns_common-1.1.2.2/mns_common/component/k_line/common/
+-rw-rw-rw-   0        0        0      163 2023-12-22 09:41:45.000000 mns_common-1.1.2.2/mns_common/component/k_line/common/__init__.py
+-rw-rw-rw-   0        0        0     4770 2024-05-20 14:28:57.000000 mns_common-1.1.2.2/mns_common/component/k_line/common/k_line_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.319392 mns_common-1.1.2.2/mns_common/component/k_line/patterns/
+-rw-rw-rw-   0        0        0      163 2023-12-22 07:50:10.000000 mns_common-1.1.2.2/mns_common/component/k_line/patterns/__init__.py
+-rw-rw-rw-   0        0        0     1809 2023-12-22 08:25:35.000000 mns_common-1.1.2.2/mns_common/component/k_line/patterns/k_line_patterns_service_api.py
+-rw-rw-rw-   0        0        0      509 2023-12-22 09:49:23.000000 mns_common-1.1.2.2/mns_common/component/k_line/patterns/pattern_Enum.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.320389 mns_common-1.1.2.2/mns_common/component/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/component/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1378 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/component/real_time/real_time_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.321386 mns_common-1.1.2.2/mns_common/component/self_choose/
+-rw-rw-rw-   0        0        0      163 2024-05-14 15:36:27.000000 mns_common-1.1.2.2/mns_common/component/self_choose/__init__.py
+-rw-rw-rw-   0        0        0     2232 2024-05-16 05:56:38.000000 mns_common-1.1.2.2/mns_common/component/self_choose/black_list_service_api.py
+-rw-rw-rw-   0        0        0      519 2024-05-18 07:01:06.000000 mns_common-1.1.2.2/mns_common/component/self_choose/self_choose_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.322383 mns_common-1.1.2.2/mns_common/component/trade/
+-rw-rw-rw-   0        0        0      163 2024-04-27 12:44:35.000000 mns_common-1.1.2.2/mns_common/component/trade/__init__.py
+-rw-rw-rw-   0        0        0     3120 2024-05-08 07:34:38.000000 mns_common-1.1.2.2/mns_common/component/trade/trade_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.323381 mns_common-1.1.2.2/mns_common/component/trade_date/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/component/trade_date/__init__.py
+-rw-rw-rw-   0        0        0     2776 2023-12-28 13:35:59.000000 mns_common-1.1.2.2/mns_common/component/trade_date/trade_date_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.324378 mns_common-1.1.2.2/mns_common/component/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-16 12:13:22.000000 mns_common-1.1.2.2/mns_common/component/zt/__init__.py
+-rw-rw-rw-   0        0        0     9927 2024-05-22 08:23:47.000000 mns_common-1.1.2.2/mns_common/component/zt/zt_common_service_api.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.327370 mns_common-1.1.2.2/mns_common/constant/
+-rw-rw-rw-   0        0        0      163 2023-12-17 08:25:43.000000 mns_common-1.1.2.2/mns_common/constant/__init__.py
+-rw-rw-rw-   0        0        0     2072 2024-05-20 14:27:17.000000 mns_common-1.1.2.2/mns_common/constant/db_name_constant.py
+-rw-rw-rw-   0        0        0     4507 2024-01-25 14:21:07.000000 mns_common-1.1.2.2/mns_common/constant/kpl_selection_no_choose_constant.py
+-rw-rw-rw-   0        0        0      347 2024-05-01 15:03:02.000000 mns_common-1.1.2.2/mns_common/constant/self_choose_constant.py
+-rw-rw-rw-   0        0        0    12240 2024-03-11 15:08:57.000000 mns_common-1.1.2.2/mns_common/constant/ths_concept_no_choose_constant.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.328367 mns_common-1.1.2.2/mns_common/db/
+-rw-rw-rw-   0        0        0    10816 2024-04-24 14:49:25.000000 mns_common-1.1.2.2/mns_common/db/MongodbUtil.py
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:08:44.000000 mns_common-1.1.2.2/mns_common/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.330362 mns_common-1.1.2.2/mns_common/utils/
+-rw-rw-rw-   0        0        0      163 2023-12-15 04:00:46.000000 mns_common-1.1.2.2/mns_common/utils/__init__.py
+-rw-rw-rw-   0        0        0      352 2023-12-15 04:16:28.000000 mns_common-1.1.2.2/mns_common/utils/async_fun.py
+-rw-rw-rw-   0        0        0     1316 2023-12-22 08:25:35.000000 mns_common-1.1.2.2/mns_common/utils/data_frame_util.py
+-rw-rw-rw-   0        0        0     7379 2023-12-21 03:38:02.000000 mns_common-1.1.2.2/mns_common/utils/date_handle_util.py
+-rw-rw-rw-   0        0        0      451 2023-12-15 04:16:28.000000 mns_common-1.1.2.2/mns_common/utils/ip_util.py
+drwxrwxrwx   0        0        0        0 2024-05-22 08:23:53.331359 mns_common-1.1.2.2/mns_common.egg-info/
+-rw-rw-rw-   0        0        0       59 2024-05-22 08:23:53.000000 mns_common-1.1.2.2/mns_common.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3872 2024-05-22 08:23:53.000000 mns_common-1.1.2.2/mns_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 08:23:53.000000 mns_common-1.1.2.2/mns_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 08:23:53.000000 mns_common-1.1.2.2/mns_common.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 08:23:53.331359 mns_common-1.1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      466 2024-05-22 08:23:47.000000 mns_common-1.1.2.2/setup.py
```

### Comparing `mns_common-1.1.2.0/README.md` & `mns_common-1.1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/akshare/k_line_api.py` & `mns_common-1.1.2.2/mns_common/api/akshare/k_line_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/akshare/stock_bid_ask_api.py` & `mns_common-1.1.2.2/mns_common/api/akshare/stock_bid_ask_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/akshare/stock_dt_pool.py` & `mns_common-1.1.2.2/mns_common/api/akshare/stock_dt_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/akshare/stock_zb_pool.py` & `mns_common-1.1.2.2/mns_common/api/akshare/stock_zb_pool.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/akshare/stock_zt_pool_api.py` & `mns_common-1.1.2.2/mns_common/api/akshare/stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/akshare/yjyg_sync_api.py` & `mns_common-1.1.2.2/mns_common/api/akshare/yjyg_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/em/east_money_stock_api.py` & `mns_common-1.1.2.2/mns_common/api/em/east_money_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py` & `mns_common-1.1.2.2/mns_common/api/em/east_money_stock_gdfx_free_top_10_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/em/east_money_stock_hk_api.py` & `mns_common-1.1.2.2/mns_common/api/em/east_money_stock_hk_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/em/east_money_stock_v2_api.py` & `mns_common-1.1.2.2/mns_common/api/em/east_money_stock_v2_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/em/em_concept_index_api.py` & `mns_common-1.1.2.2/mns_common/api/em/em_concept_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/kpl/common/kpl_common_api.py` & `mns_common-1.1.2.2/mns_common/api/kpl/common/kpl_common_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/kpl/concept/kpl_concept_api.py` & `mns_common-1.1.2.2/mns_common/api/kpl/concept/kpl_concept_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/kpl/constant/kpl_constant.py` & `mns_common-1.1.2.2/mns_common/api/kpl/constant/kpl_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/kpl/industry/kpl_industry_api.py` & `mns_common-1.1.2.2/mns_common/api/kpl/industry/kpl_industry_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/kpl/selection/kpl_selection_plate_api.py` & `mns_common-1.1.2.2/mns_common/api/kpl/selection/kpl_selection_plate_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py` & `mns_common-1.1.2.2/mns_common/api/kpl/symbol/kpl_real_time_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py` & `mns_common-1.1.2.2/mns_common/api/kpl/symbol/kpl_symbol_common_field_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/kpl/symbol/symbol_his_quotes_api.py` & `mns_common-1.1.2.2/mns_common/api/kpl/symbol/symbol_his_quotes_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/msg/push_msg_api.py` & `mns_common-1.1.2.2/mns_common/api/msg/push_msg_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/ths/ths_big_deal_api.py` & `mns_common-1.1.2.2/mns_common/api/ths/ths_big_deal_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/ths/ths_stock_api.py` & `mns_common-1.1.2.2/mns_common/api/ths/ths_stock_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/api/ths/ths_stock_zt_pool_api.py` & `mns_common-1.1.2.2/mns_common/api/ths/ths_stock_zt_pool_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/cache/cache_service.py` & `mns_common-1.1.2.2/mns_common/component/cache/cache_service.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/classify/classify_constant.py` & `mns_common-1.1.2.2/mns_common/component/classify/classify_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/classify/symbol_classify_api.py` & `mns_common-1.1.2.2/mns_common/component/classify/symbol_classify_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/common_service_fun_api.py` & `mns_common-1.1.2.2/mns_common/component/common_service_fun_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/company/company_common_service_api.py` & `mns_common-1.1.2.2/mns_common/component/company/company_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/concept/kpl_concept_common_service_api.py` & `mns_common-1.1.2.2/mns_common/component/concept/kpl_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/concept/ths_concept_common_service_api.py` & `mns_common-1.1.2.2/mns_common/component/concept/ths_concept_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/data/data_init_api.py` & `mns_common-1.1.2.2/mns_common/component/data/data_init_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/industry/ths_industry_index_api.py` & `mns_common-1.1.2.2/mns_common/component/industry/ths_industry_index_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py` & `mns_common-1.1.2.2/mns_common/component/k_line/clean/sh_small_normal_zt_k_line_check_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/k_line/common/k_line_common_service_api.py` & `mns_common-1.1.2.2/mns_common/component/k_line/common/k_line_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/k_line/patterns/k_line_patterns_service_api.py` & `mns_common-1.1.2.2/mns_common/component/k_line/patterns/k_line_patterns_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/real_time/real_time_common_service_api.py` & `mns_common-1.1.2.2/mns_common/component/real_time/real_time_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/self_choose/black_list_service_api.py` & `mns_common-1.1.2.2/mns_common/component/self_choose/black_list_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/self_choose/self_choose_service_api.py` & `mns_common-1.1.2.2/mns_common/component/self_choose/self_choose_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/trade/trade_service_api.py` & `mns_common-1.1.2.2/mns_common/component/trade/trade_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/trade_date/trade_date_common_service_api.py` & `mns_common-1.1.2.2/mns_common/component/trade_date/trade_date_common_service_api.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/component/zt/zt_common_service_api.py` & `mns_common-1.1.2.2/mns_common/component/zt/zt_common_service_api.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,23 +8,25 @@
 
 from functools import lru_cache
 from mns_common.db.MongodbUtil import MongodbUtil
 import mns_common.utils.date_handle_util as date_handle_util
 import mns_common.api.akshare.stock_zt_pool_api as stock_zt_pool_api
 import mns_common.component.trade_date.trade_date_common_service_api as trade_date_common_service_api
 import pandas as pd
+import mns_common.constant.db_name_constant as db_name_constant
+import mns_common.utils.data_frame_util as data_frame_util
 
 mongodb_util = MongodbUtil('27017')
 
 
 @lru_cache(maxsize=None)
 def get_last_trade_day_zt(str_day):
     last_trade_day = trade_date_common_service_api.get_last_trade_day(str_day)
     query = {'str_day': last_trade_day}
-    db_stock_zt_pool = mongodb_util.find_query_data('stock_zt_pool', query)
+    db_stock_zt_pool = mongodb_util.find_query_data(db_name_constant.STOCK_ZT_POOL, query)
     if db_stock_zt_pool is None or db_stock_zt_pool.shape[0] == 0:
         db_stock_zt_pool = stock_zt_pool_api.stock_em_zt_pool_df(date_handle_util.no_slash_date(last_trade_day))
     return db_stock_zt_pool
 
 
 # 按照字段分组
 def group_by_industry(real_time_quotes_now, field):
@@ -163,9 +165,35 @@
     else:
         zb_symbol_list = list(real_time_quotes_zb['symbol'])
 
     real_time_quotes_now.loc[real_time_quotes_now['symbol'].isin(zb_symbol_list), 'is_zb'] = True
     return real_time_quotes_now
 
 
+# 获取一段时间连板股票信息
+@lru_cache(maxsize=None)
+def get_period_connected_boards_zt_pool(begin_day, end_day, connected_boards_numbers):
+    query = {"connected_boards_numbers": connected_boards_numbers,
+             "$and": [{"before_five_day": {"$gte": begin_day}}, {"before_five_day": {"$gte": end_day}}]}
+
+    stock_zt_pool_df = mongodb_util.find_query_data(db_name_constant.STOCK_ZT_POOL, query)
+    if data_frame_util.is_empty(stock_zt_pool_df):
+        zt_symbol_list = ['000001']
+    else:
+        zt_symbol_list = list(stock_zt_pool_df['symbol'])
+    return zt_symbol_list
+
+
+# 获取一段时间五板股票
+@lru_cache(maxsize=None)
+def get_period_five_boards_zt_pool(begin_day, end_day):
+    query = {"$and": [{"before_five_day": {"$gte": begin_day}}, {"before_five_day": {"$gte": end_day}}]}
+    stock_zt_pool_five_df = mongodb_util.find_query_data(db_name_constant.STOCK_ZT_POOL_FIVE, query)
+    if data_frame_util.is_empty(stock_zt_pool_five_df):
+        zt_symbol_list = ['000001']
+    else:
+        zt_symbol_list = list(stock_zt_pool_five_df['symbol'])
+    return zt_symbol_list
+
+
 if __name__ == '__main__':
     get_last_trade_day_zt('20231215')
```

### Comparing `mns_common-1.1.2.0/mns_common/constant/db_name_constant.py` & `mns_common-1.1.2.2/mns_common/constant/db_name_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/constant/kpl_selection_no_choose_constant.py` & `mns_common-1.1.2.2/mns_common/constant/kpl_selection_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/constant/ths_concept_no_choose_constant.py` & `mns_common-1.1.2.2/mns_common/constant/ths_concept_no_choose_constant.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/db/MongodbUtil.py` & `mns_common-1.1.2.2/mns_common/db/MongodbUtil.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/utils/data_frame_util.py` & `mns_common-1.1.2.2/mns_common/utils/data_frame_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common/utils/date_handle_util.py` & `mns_common-1.1.2.2/mns_common/utils/date_handle_util.py`

 * *Files identical despite different names*

### Comparing `mns_common-1.1.2.0/mns_common.egg-info/SOURCES.txt` & `mns_common-1.1.2.2/mns_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

