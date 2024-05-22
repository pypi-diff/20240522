# Comparing `tmp/openbb_core-1.2.2.tar.gz` & `tmp/openbb_core-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_core-1.2.2.tar", max compression
+gzip compressed data, was "openbb_core-1.2.3.tar", max compression
```

## Comparing `openbb_core-1.2.2.tar` & `openbb_core-1.2.3.tar`

### file list

```diff
@@ -1,243 +1,246 @@
--rw-r--r--   0        0        0     2302 2024-04-02 11:35:59.266636 openbb_core-1.2.2/README.md
--rw-r--r--   0        0        0       19 2024-04-23 10:22:39.570135 openbb_core-1.2.2/openbb_core/__init__.py
--rw-r--r--   0        0        0      977 2024-04-25 15:03:16.107506 openbb_core-1.2.2/openbb_core/api/app_loader.py
--rw-r--r--   0        0        0     1972 2024-04-23 10:22:39.570481 openbb_core-1.2.2/openbb_core/api/auth/user.py
--rw-r--r--   0        0        0       34 2024-04-23 10:22:39.570645 openbb_core-1.2.2/openbb_core/api/dependency/__init__.py
--rw-r--r--   0        0        0      604 2024-02-29 11:03:36.668814 openbb_core-1.2.2/openbb_core/api/dependency/coverage.py
--rw-r--r--   0        0        0      653 2024-03-01 13:58:22.591666 openbb_core-1.2.2/openbb_core/api/dependency/system.py
--rw-r--r--   0        0        0     4206 2024-04-25 15:03:16.107765 openbb_core-1.2.2/openbb_core/api/rest_api.py
--rw-r--r--   0        0        0       30 2024-04-23 10:22:39.570887 openbb_core-1.2.2/openbb_core/api/router/__init__.py
--rw-r--r--   0        0        0     7189 2024-04-25 15:03:16.107968 openbb_core-1.2.2/openbb_core/api/router/commands.py
--rw-r--r--   0        0        0     1182 2024-04-08 12:02:16.491932 openbb_core-1.2.2/openbb_core/api/router/coverage.py
--rw-r--r--   0        0        0       40 2024-04-02 11:35:59.267527 openbb_core-1.2.2/openbb_core/api/router/helpers/__init__.py
--rw-r--r--   0        0        0     4202 2024-04-23 08:46:54.460027 openbb_core-1.2.2/openbb_core/api/router/helpers/coverage_helpers.py
--rw-r--r--   0        0        0      469 2024-04-08 12:02:16.492136 openbb_core-1.2.2/openbb_core/api/router/system.py
--rw-r--r--   0        0        0      557 2024-03-01 13:58:22.592202 openbb_core-1.2.2/openbb_core/api/router/user.py
--rw-r--r--   0        0        0       30 2024-04-23 10:22:39.571151 openbb_core-1.2.2/openbb_core/app/__init__.py
--rw-r--r--   0        0        0    19033 2024-05-10 11:33:20.067018 openbb_core-1.2.2/openbb_core/app/command_runner.py
--rw-r--r--   0        0        0      293 2024-04-08 12:02:16.492449 openbb_core-1.2.2/openbb_core/app/constants.py
--rw-r--r--   0        0        0     2563 2024-04-23 10:22:39.571883 openbb_core-1.2.2/openbb_core/app/deprecation.py
--rw-r--r--   0        0        0     6120 2024-04-25 15:03:16.111594 openbb_core-1.2.2/openbb_core/app/extension_loader.py
--rw-r--r--   0        0        0     5938 2024-04-25 15:03:16.111982 openbb_core-1.2.2/openbb_core/app/logs/formatters/formatter_with_exceptions.py
--rw-r--r--   0        0        0     2705 2024-04-25 15:03:16.112147 openbb_core-1.2.2/openbb_core/app/logs/handlers/path_tracking_file_handler.py
--rw-r--r--   0        0        0     4392 2024-04-08 12:02:16.492804 openbb_core-1.2.2/openbb_core/app/logs/handlers/posthog_handler.py
--rw-r--r--   0        0        0     2964 2024-04-23 10:22:39.572391 openbb_core-1.2.2/openbb_core/app/logs/handlers_manager.py
--rw-r--r--   0        0        0     8326 2024-04-25 15:03:16.112434 openbb_core-1.2.2/openbb_core/app/logs/logging_service.py
--rw-r--r--   0        0        0     2238 2024-04-23 10:22:39.572707 openbb_core-1.2.2/openbb_core/app/logs/models/logging_settings.py
--rw-r--r--   0        0        0      966 2024-04-23 10:22:39.572853 openbb_core-1.2.2/openbb_core/app/logs/utils/expired_files.py
--rw-r--r--   0        0        0     2247 2024-04-23 10:22:39.572965 openbb_core-1.2.2/openbb_core/app/logs/utils/utils.py
--rw-r--r--   0        0        0       29 2024-04-23 10:22:39.573057 openbb_core-1.2.2/openbb_core/app/model/__init__.py
--rw-r--r--   0        0        0       38 2024-04-23 10:22:39.573150 openbb_core-1.2.2/openbb_core/app/model/abstract/__init__.py
--rw-r--r--   0        0        0      302 2024-04-23 10:22:39.573260 openbb_core-1.2.2/openbb_core/app/model/abstract/error.py
--rw-r--r--   0        0        0       99 2024-04-23 10:22:39.573351 openbb_core-1.2.2/openbb_core/app/model/abstract/results.py
--rw-r--r--   0        0        0      551 2024-04-23 10:22:39.573483 openbb_core-1.2.2/openbb_core/app/model/abstract/singleton.py
--rw-r--r--   0        0        0      252 2024-04-23 10:22:39.573585 openbb_core-1.2.2/openbb_core/app/model/abstract/tagged.py
--rw-r--r--   0        0        0      458 2024-04-25 15:03:16.112659 openbb_core-1.2.2/openbb_core/app/model/abstract/warning.py
--rw-r--r--   0        0        0     1908 2024-04-23 10:22:39.573750 openbb_core-1.2.2/openbb_core/app/model/api_settings.py
--rw-r--r--   0        0        0     1035 2024-04-25 15:03:16.112814 openbb_core-1.2.2/openbb_core/app/model/charts/chart.py
--rw-r--r--   0        0        0     2248 2024-04-08 12:02:16.493305 openbb_core-1.2.2/openbb_core/app/model/charts/charting_settings.py
--rw-r--r--   0        0        0      398 2024-04-23 10:22:39.573965 openbb_core-1.2.2/openbb_core/app/model/command_context.py
--rw-r--r--   0        0        0     3915 2024-05-13 15:41:33.848674 openbb_core-1.2.2/openbb_core/app/model/credentials.py
--rw-r--r--   0        0        0      502 2024-04-23 10:22:39.574297 openbb_core-1.2.2/openbb_core/app/model/defaults.py
--rw-r--r--   0        0        0     7329 2024-04-25 15:03:16.113143 openbb_core-1.2.2/openbb_core/app/model/example.py
--rw-r--r--   0        0        0     2385 2024-05-10 19:27:56.003979 openbb_core-1.2.2/openbb_core/app/model/extension.py
--rw-r--r--   0        0        0     1054 2024-04-23 10:22:39.574498 openbb_core-1.2.2/openbb_core/app/model/field.py
--rw-r--r--   0        0        0      694 2024-04-23 10:22:39.574636 openbb_core-1.2.2/openbb_core/app/model/hub/hub_session.py
--rw-r--r--   0        0        0      474 2024-04-23 10:22:39.574977 openbb_core-1.2.2/openbb_core/app/model/hub/hub_user_settings.py
--rw-r--r--   0        0        0     5669 2024-04-25 15:03:16.113495 openbb_core-1.2.2/openbb_core/app/model/metadata.py
--rw-r--r--   0        0        0     9240 2024-05-10 19:27:56.004268 openbb_core-1.2.2/openbb_core/app/model/obbject.py
--rw-r--r--   0        0        0     1477 2024-05-09 13:34:29.173272 openbb_core-1.2.2/openbb_core/app/model/preferences.py
--rw-r--r--   0        0        0      536 2024-04-23 10:22:39.575520 openbb_core-1.2.2/openbb_core/app/model/profile.py
--rw-r--r--   0        0        0      801 2024-04-23 10:22:39.575578 openbb_core-1.2.2/openbb_core/app/model/python_settings.py
--rw-r--r--   0        0        0       37 2024-04-23 10:22:39.575663 openbb_core-1.2.2/openbb_core/app/model/results/__init__.py
--rw-r--r--   0        0        0      130 2024-04-23 10:22:39.575753 openbb_core-1.2.2/openbb_core/app/model/results/empty.py
--rw-r--r--   0        0        0     4044 2024-04-23 10:22:39.575870 openbb_core-1.2.2/openbb_core/app/model/system_settings.py
--rw-r--r--   0        0        0      854 2024-04-08 12:02:16.494392 openbb_core-1.2.2/openbb_core/app/model/user_settings.py
--rw-r--r--   0        0        0    21634 2024-05-10 10:40:27.270236 openbb_core-1.2.2/openbb_core/app/provider_interface.py
--rw-r--r--   0        0        0     2744 2024-04-25 15:03:16.114105 openbb_core-1.2.2/openbb_core/app/query.py
--rw-r--r--   0        0        0    23086 2024-04-25 15:03:16.114305 openbb_core-1.2.2/openbb_core/app/router.py
--rw-r--r--   0        0        0     2627 2024-04-23 10:22:39.576501 openbb_core-1.2.2/openbb_core/app/service/auth_service.py
--rw-r--r--   0        0        0    10381 2024-05-14 15:30:05.603980 openbb_core-1.2.2/openbb_core/app/service/hub_service.py
--rw-r--r--   0        0        0     3511 2024-04-25 15:03:16.114783 openbb_core-1.2.2/openbb_core/app/service/system_service.py
--rw-r--r--   0        0        0     3064 2024-04-25 15:03:16.114933 openbb_core-1.2.2/openbb_core/app/service/user_service.py
--rw-r--r--   0        0        0       30 2024-04-23 10:22:39.576930 openbb_core-1.2.2/openbb_core/app/static/__init__.py
--rw-r--r--   0        0        0     7595 2024-04-23 10:22:39.577041 openbb_core-1.2.2/openbb_core/app/static/account.py
--rw-r--r--   0        0        0     2024 2024-04-23 10:22:39.577156 openbb_core-1.2.2/openbb_core/app/static/app_factory.py
--rw-r--r--   0        0        0     1582 2024-04-23 10:22:39.577258 openbb_core-1.2.2/openbb_core/app/static/container.py
--rw-r--r--   0        0        0     1948 2024-04-23 10:22:39.577365 openbb_core-1.2.2/openbb_core/app/static/coverage.py
--rw-r--r--   0        0        0    66879 2024-05-14 15:30:05.604307 openbb_core-1.2.2/openbb_core/app/static/package_builder.py
--rw-r--r--   0        0        0     1431 2024-04-08 12:02:16.496174 openbb_core-1.2.2/openbb_core/app/static/reference_loader.py
--rw-r--r--   0        0        0      408 2024-04-08 12:02:16.496278 openbb_core-1.2.2/openbb_core/app/static/utils/console.py
--rw-r--r--   0        0        0     3077 2024-04-25 15:03:16.115099 openbb_core-1.2.2/openbb_core/app/static/utils/decorators.py
--rw-r--r--   0        0        0     2699 2024-05-10 10:40:27.271743 openbb_core-1.2.2/openbb_core/app/static/utils/filters.py
--rw-r--r--   0        0        0     1655 2024-04-25 15:03:16.115234 openbb_core-1.2.2/openbb_core/app/static/utils/linters.py
--rw-r--r--   0        0        0     5986 2024-04-25 15:03:16.115412 openbb_core-1.2.2/openbb_core/app/utils.py
--rw-r--r--   0        0        0     1809 2024-04-23 10:22:39.578140 openbb_core-1.2.2/openbb_core/app/version.py
--rw-r--r--   0        0        0     2396 2024-04-23 10:22:39.578249 openbb_core-1.2.2/openbb_core/env.py
--rw-r--r--   0        0        0      171 2024-04-08 12:02:16.496937 openbb_core-1.2.2/openbb_core/provider/__init__.py
--rw-r--r--   0        0        0       38 2024-02-29 11:03:36.674333 openbb_core-1.2.2/openbb_core/provider/abstract/__init__.py
--rw-r--r--   0        0        0      465 2024-04-25 15:03:16.115559 openbb_core-1.2.2/openbb_core/provider/abstract/annotated_result.py
--rw-r--r--   0        0        0     3494 2024-04-08 12:02:16.497126 openbb_core-1.2.2/openbb_core/provider/abstract/data.py
--rw-r--r--   0        0        0     8881 2024-05-02 09:44:26.753713 openbb_core-1.2.2/openbb_core/provider/abstract/fetcher.py
--rw-r--r--   0        0        0     1985 2024-05-14 15:30:05.604736 openbb_core-1.2.2/openbb_core/provider/abstract/provider.py
--rw-r--r--   0        0        0     2702 2024-05-10 10:40:27.272293 openbb_core-1.2.2/openbb_core/provider/abstract/query_params.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.674777 openbb_core-1.2.2/openbb_core/provider/py.typed
--rw-r--r--   0        0        0     3524 2024-05-02 09:01:30.398382 openbb_core-1.2.2/openbb_core/provider/query_executor.py
--rw-r--r--   0        0        0     1675 2024-04-25 15:03:16.115739 openbb_core-1.2.2/openbb_core/provider/registry.py
--rw-r--r--   0        0        0     8297 2024-05-10 10:40:27.272879 openbb_core-1.2.2/openbb_core/provider/registry_map.py
--rw-r--r--   0        0        0       43 2024-02-29 11:03:36.675239 openbb_core-1.2.2/openbb_core/provider/standard_models/__init__.py
--rw-r--r--   0        0        0      874 2024-04-25 15:03:16.116069 openbb_core-1.2.2/openbb_core/provider/standard_models/ameribor_rates.py
--rw-r--r--   0        0        0     3426 2024-04-08 12:02:16.497948 openbb_core-1.2.2/openbb_core/provider/standard_models/analyst_estimates.py
--rw-r--r--   0        0        0     1270 2024-04-25 15:03:16.116209 openbb_core-1.2.2/openbb_core/provider/standard_models/analyst_search.py
--rw-r--r--   0        0        0     1377 2024-05-09 13:34:29.176884 openbb_core-1.2.2/openbb_core/provider/standard_models/available_indicators.py
--rw-r--r--   0        0        0      630 2024-04-08 12:02:16.498191 openbb_core-1.2.2/openbb_core/provider/standard_models/available_indices.py
--rw-r--r--   0        0        0    19696 2024-04-03 09:25:56.556032 openbb_core-1.2.2/openbb_core/provider/standard_models/balance_of_payments.py
--rw-r--r--   0        0        0     1541 2024-04-25 15:03:16.116401 openbb_core-1.2.2/openbb_core/provider/standard_models/balance_sheet.py
--rw-r--r--   0        0        0     5809 2024-04-08 12:02:16.498533 openbb_core-1.2.2/openbb_core/provider/standard_models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3619 2024-04-25 15:03:16.116828 openbb_core-1.2.2/openbb_core/provider/standard_models/bond_prices.py
--rw-r--r--   0        0        0     2939 2024-04-25 15:03:16.117074 openbb_core-1.2.2/openbb_core/provider/standard_models/bond_reference.py
--rw-r--r--   0        0        0     2802 2024-04-25 15:03:16.117279 openbb_core-1.2.2/openbb_core/provider/standard_models/bond_trades.py
--rw-r--r--   0        0        0     1599 2024-04-25 15:03:16.117443 openbb_core-1.2.2/openbb_core/provider/standard_models/calendar_dividend.py
--rw-r--r--   0        0        0     1300 2024-04-25 15:03:16.117587 openbb_core-1.2.2/openbb_core/provider/standard_models/calendar_earnings.py
--rw-r--r--   0        0        0     2264 2024-04-25 15:03:16.117709 openbb_core-1.2.2/openbb_core/provider/standard_models/calendar_ipo.py
--rw-r--r--   0        0        0     1117 2024-04-08 12:02:16.499392 openbb_core-1.2.2/openbb_core/provider/standard_models/calendar_splits.py
--rw-r--r--   0        0        0     1560 2024-04-25 15:03:16.117834 openbb_core-1.2.2/openbb_core/provider/standard_models/cash_flow.py
--rw-r--r--   0        0        0     5087 2024-04-08 12:02:16.499607 openbb_core-1.2.2/openbb_core/provider/standard_models/cash_flow_growth.py
--rw-r--r--   0        0        0      829 2024-04-08 12:02:16.499687 openbb_core-1.2.2/openbb_core/provider/standard_models/cik_map.py
--rw-r--r--   0        0        0     2237 2024-04-08 12:02:16.499789 openbb_core-1.2.2/openbb_core/provider/standard_models/company_filings.py
--rw-r--r--   0        0        0     2424 2024-05-08 16:35:29.989158 openbb_core-1.2.2/openbb_core/provider/standard_models/company_news.py
--rw-r--r--   0        0        0     4560 2024-04-08 12:02:16.500022 openbb_core-1.2.2/openbb_core/provider/standard_models/company_overview.py
--rw-r--r--   0        0        0      766 2024-04-08 12:02:16.500083 openbb_core-1.2.2/openbb_core/provider/standard_models/compare_groups.py
--rw-r--r--   0        0        0     1057 2024-04-25 15:03:16.118094 openbb_core-1.2.2/openbb_core/provider/standard_models/composite_leading_indicator.py
--rw-r--r--   0        0        0      714 2024-02-29 11:03:36.676815 openbb_core-1.2.2/openbb_core/provider/standard_models/cot.py
--rw-r--r--   0        0        0     1246 2024-05-09 13:34:29.177209 openbb_core-1.2.2/openbb_core/provider/standard_models/cot_search.py
--rw-r--r--   0        0        0     3722 2024-05-09 13:34:29.177287 openbb_core-1.2.2/openbb_core/provider/standard_models/country_profile.py
--rw-r--r--   0        0        0     1591 2024-04-25 15:03:16.118591 openbb_core-1.2.2/openbb_core/provider/standard_models/cp.py
--rw-r--r--   0        0        0     3335 2024-04-23 10:22:39.579222 openbb_core-1.2.2/openbb_core/provider/standard_models/cpi.py
--rw-r--r--   0        0        0     2310 2024-04-25 15:03:16.118756 openbb_core-1.2.2/openbb_core/provider/standard_models/crypto_historical.py
--rw-r--r--   0        0        0      668 2024-04-08 12:02:16.500724 openbb_core-1.2.2/openbb_core/provider/standard_models/crypto_search.py
--rw-r--r--   0        0        0     2363 2024-04-25 15:03:16.118894 openbb_core-1.2.2/openbb_core/provider/standard_models/currency_historical.py
--rw-r--r--   0        0        0      732 2024-05-09 15:04:29.062516 openbb_core-1.2.2/openbb_core/provider/standard_models/currency_pairs.py
--rw-r--r--   0        0        0     2992 2024-04-25 15:03:16.119239 openbb_core-1.2.2/openbb_core/provider/standard_models/currency_reference_rates.py
--rw-r--r--   0        0        0     3125 2024-04-25 15:03:16.119360 openbb_core-1.2.2/openbb_core/provider/standard_models/currency_snapshots.py
--rw-r--r--   0        0        0     1549 2024-04-25 15:03:16.119499 openbb_core-1.2.2/openbb_core/provider/standard_models/discovery_filings.py
--rw-r--r--   0        0        0     1027 2024-04-25 15:03:16.119634 openbb_core-1.2.2/openbb_core/provider/standard_models/dwpcr_rates.py
--rw-r--r--   0        0        0     1583 2024-04-08 12:02:16.501134 openbb_core-1.2.2/openbb_core/provider/standard_models/earnings_call_transcript.py
--rw-r--r--   0        0        0     1452 2024-04-25 15:03:16.119769 openbb_core-1.2.2/openbb_core/provider/standard_models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2125 2024-05-14 15:30:05.604941 openbb_core-1.2.2/openbb_core/provider/standard_models/economic_calendar.py
--rw-r--r--   0        0        0     1680 2024-05-09 15:04:29.062707 openbb_core-1.2.2/openbb_core/provider/standard_models/economic_indicators.py
--rw-r--r--   0        0        0     1750 2024-04-25 15:03:16.120051 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_ftd.py
--rw-r--r--   0        0        0     2157 2024-05-07 10:10:32.921917 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_historical.py
--rw-r--r--   0        0        0     5757 2024-04-08 12:02:16.501659 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_info.py
--rw-r--r--   0        0        0     1392 2024-04-25 15:03:16.120282 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_nbbo.py
--rw-r--r--   0        0        0     5402 2024-04-08 12:02:16.501882 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_ownership.py
--rw-r--r--   0        0        0      855 2024-04-08 12:02:16.502012 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_peers.py
--rw-r--r--   0        0        0     1326 2024-04-25 15:03:16.120534 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_performance.py
--rw-r--r--   0        0        0     5878 2024-04-23 10:22:39.579383 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_quote.py
--rw-r--r--   0        0        0      898 2024-04-08 12:02:16.502348 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_screener.py
--rw-r--r--   0        0        0      912 2024-05-09 13:34:29.177837 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_search.py
--rw-r--r--   0        0        0     3528 2024-04-08 12:02:16.502654 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_short_interest.py
--rw-r--r--   0        0        0    10945 2024-04-08 12:02:16.502786 openbb_core-1.2.2/openbb_core/provider/standard_models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     1664 2024-04-08 12:02:16.502907 openbb_core-1.2.2/openbb_core/provider/standard_models/esg_risk_rating.py
--rw-r--r--   0        0        0     1922 2024-04-08 12:02:16.503093 openbb_core-1.2.2/openbb_core/provider/standard_models/esg_score.py
--rw-r--r--   0        0        0      951 2024-04-08 12:02:16.503199 openbb_core-1.2.2/openbb_core/provider/standard_models/esg_sector.py
--rw-r--r--   0        0        0      850 2024-04-08 12:02:16.503299 openbb_core-1.2.2/openbb_core/provider/standard_models/estr_rates.py
--rw-r--r--   0        0        0      791 2024-04-08 12:02:16.503410 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_countries.py
--rw-r--r--   0        0        0     1448 2024-05-15 11:17:30.039088 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_equity_exposure.py
--rw-r--r--   0        0        0     1980 2024-04-08 12:02:16.503633 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_historical.py
--rw-r--r--   0        0        0      871 2024-04-08 12:02:16.503765 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_historical_nav.py
--rw-r--r--   0        0        0      939 2024-04-23 10:22:39.580561 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_holdings.py
--rw-r--r--   0        0        0      640 2024-02-29 11:03:36.679311 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_holdings_date.py
--rw-r--r--   0        0        0      360 2024-04-08 12:02:16.503908 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_holdings_performance.py
--rw-r--r--   0        0        0     1027 2024-04-08 12:02:16.504049 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_info.py
--rw-r--r--   0        0        0     1576 2024-04-08 12:02:16.504179 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_performance.py
--rw-r--r--   0        0        0      644 2024-02-29 11:03:36.679587 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_search.py
--rw-r--r--   0        0        0      862 2024-04-08 12:02:16.504319 openbb_core-1.2.2/openbb_core/provider/standard_models/etf_sectors.py
--rw-r--r--   0        0        0      905 2024-05-15 11:17:30.039210 openbb_core-1.2.2/openbb_core/provider/standard_models/eu_yield_curve.py
--rw-r--r--   0        0        0     2065 2024-04-08 12:02:16.504572 openbb_core-1.2.2/openbb_core/provider/standard_models/executive_compensation.py
--rw-r--r--   0        0        0     1234 2024-04-08 12:02:16.504687 openbb_core-1.2.2/openbb_core/provider/standard_models/fed_projections.py
--rw-r--r--   0        0        0      844 2024-04-08 12:02:16.504804 openbb_core-1.2.2/openbb_core/provider/standard_models/fed_rates.py
--rw-r--r--   0        0        0     1439 2024-04-08 12:02:16.504912 openbb_core-1.2.2/openbb_core/provider/standard_models/ffrmc.py
--rw-r--r--   0        0        0     1773 2024-04-08 12:02:16.505036 openbb_core-1.2.2/openbb_core/provider/standard_models/financial_attributes.py
--rw-r--r--   0        0        0     1444 2024-04-08 12:02:16.505143 openbb_core-1.2.2/openbb_core/provider/standard_models/financial_ratios.py
--rw-r--r--   0        0        0     3970 2024-04-08 12:02:16.505225 openbb_core-1.2.2/openbb_core/provider/standard_models/form_13FHR.py
--rw-r--r--   0        0        0     2321 2024-04-23 10:22:39.580852 openbb_core-1.2.2/openbb_core/provider/standard_models/forward_eps_estimates.py
--rw-r--r--   0        0        0     1645 2024-05-14 15:30:05.605050 openbb_core-1.2.2/openbb_core/provider/standard_models/forward_pe_estimates.py
--rw-r--r--   0        0        0     2390 2024-04-23 10:22:39.580922 openbb_core-1.2.2/openbb_core/provider/standard_models/forward_sales_estimates.py
--rw-r--r--   0        0        0     2715 2024-04-03 09:24:18.659331 openbb_core-1.2.2/openbb_core/provider/standard_models/fred_search.py
--rw-r--r--   0        0        0     1204 2024-04-08 12:02:16.505455 openbb_core-1.2.2/openbb_core/provider/standard_models/fred_series.py
--rw-r--r--   0        0        0     1077 2024-04-08 12:02:16.505531 openbb_core-1.2.2/openbb_core/provider/standard_models/futures_curve.py
--rw-r--r--   0        0        0     1857 2024-04-08 12:02:16.505610 openbb_core-1.2.2/openbb_core/provider/standard_models/futures_historical.py
--rw-r--r--   0        0        0     1564 2024-04-08 12:02:16.505708 openbb_core-1.2.2/openbb_core/provider/standard_models/gdp_forecast.py
--rw-r--r--   0        0        0     1405 2024-04-08 12:02:16.505795 openbb_core-1.2.2/openbb_core/provider/standard_models/gdp_nominal.py
--rw-r--r--   0        0        0     1439 2024-04-08 12:02:16.505879 openbb_core-1.2.2/openbb_core/provider/standard_models/gdp_real.py
--rw-r--r--   0        0        0     2532 2024-04-08 12:02:16.505957 openbb_core-1.2.2/openbb_core/provider/standard_models/historical_attributes.py
--rw-r--r--   0        0        0     1271 2024-04-08 12:02:16.506053 openbb_core-1.2.2/openbb_core/provider/standard_models/historical_dividends.py
--rw-r--r--   0        0        0     2705 2024-04-08 12:02:16.506140 openbb_core-1.2.2/openbb_core/provider/standard_models/historical_employees.py
--rw-r--r--   0        0        0     1532 2024-04-08 12:02:16.506219 openbb_core-1.2.2/openbb_core/provider/standard_models/historical_eps.py
--rw-r--r--   0        0        0     1207 2024-04-08 12:02:16.506314 openbb_core-1.2.2/openbb_core/provider/standard_models/historical_splits.py
--rw-r--r--   0        0        0     1397 2024-04-08 12:02:16.506419 openbb_core-1.2.2/openbb_core/provider/standard_models/hqm.py
--rw-r--r--   0        0        0     1410 2024-04-08 12:02:16.506533 openbb_core-1.2.2/openbb_core/provider/standard_models/ice_bofa.py
--rw-r--r--   0        0        0     1556 2024-04-08 12:02:16.506619 openbb_core-1.2.2/openbb_core/provider/standard_models/income_statement.py
--rw-r--r--   0        0        0     4974 2024-04-08 12:02:16.506718 openbb_core-1.2.2/openbb_core/provider/standard_models/income_statement_growth.py
--rw-r--r--   0        0        0      750 2024-04-08 12:02:16.506824 openbb_core-1.2.2/openbb_core/provider/standard_models/index_constituents.py
--rw-r--r--   0        0        0     2408 2024-04-08 12:02:16.506908 openbb_core-1.2.2/openbb_core/provider/standard_models/index_historical.py
--rw-r--r--   0        0        0     1292 2024-04-08 12:02:16.506989 openbb_core-1.2.2/openbb_core/provider/standard_models/index_info.py
--rw-r--r--   0        0        0      691 2024-02-29 11:03:36.681716 openbb_core-1.2.2/openbb_core/provider/standard_models/index_search.py
--rw-r--r--   0        0        0      777 2024-04-08 12:02:16.507066 openbb_core-1.2.2/openbb_core/provider/standard_models/index_sectors.py
--rw-r--r--   0        0        0     1825 2024-04-08 12:02:16.507183 openbb_core-1.2.2/openbb_core/provider/standard_models/index_snapshots.py
--rw-r--r--   0        0        0      835 2024-02-29 11:03:36.681951 openbb_core-1.2.2/openbb_core/provider/standard_models/industry_pe.py
--rw-r--r--   0        0        0     3148 2024-04-08 12:02:16.507267 openbb_core-1.2.2/openbb_core/provider/standard_models/insider_trading.py
--rw-r--r--   0        0        0     1413 2024-04-08 12:02:16.507425 openbb_core-1.2.2/openbb_core/provider/standard_models/institutional_ownership.py
--rw-r--r--   0        0        0      850 2024-04-03 09:24:18.677029 openbb_core-1.2.2/openbb_core/provider/standard_models/iorb_rates.py
--rw-r--r--   0        0        0     1406 2024-04-08 12:02:16.507566 openbb_core-1.2.2/openbb_core/provider/standard_models/key_executives.py
--rw-r--r--   0        0        0     1540 2024-04-08 12:02:16.507677 openbb_core-1.2.2/openbb_core/provider/standard_models/key_metrics.py
--rw-r--r--   0        0        0     1450 2024-04-08 12:02:16.507774 openbb_core-1.2.2/openbb_core/provider/standard_models/latest_attributes.py
--rw-r--r--   0        0        0     2654 2024-04-08 12:02:16.507840 openbb_core-1.2.2/openbb_core/provider/standard_models/lbma_fixing.py
--rw-r--r--   0        0        0     1125 2024-04-08 12:02:16.507922 openbb_core-1.2.2/openbb_core/provider/standard_models/long_term_interest_rate.py
--rw-r--r--   0        0        0     1951 2024-04-08 12:02:16.508020 openbb_core-1.2.2/openbb_core/provider/standard_models/market_indices.py
--rw-r--r--   0        0        0      832 2024-02-29 11:03:36.682563 openbb_core-1.2.2/openbb_core/provider/standard_models/market_movers.py
--rw-r--r--   0        0        0     1627 2024-04-08 12:02:16.508134 openbb_core-1.2.2/openbb_core/provider/standard_models/market_snapshots.py
--rw-r--r--   0        0        0     1827 2024-04-08 12:02:16.508236 openbb_core-1.2.2/openbb_core/provider/standard_models/money_measures.py
--rw-r--r--   0        0        0     1355 2024-04-08 12:02:16.508327 openbb_core-1.2.2/openbb_core/provider/standard_models/moody.py
--rw-r--r--   0        0        0     6200 2024-05-09 13:34:29.178067 openbb_core-1.2.2/openbb_core/provider/standard_models/options_chains.py
--rw-r--r--   0        0        0     1071 2024-04-08 12:02:16.508525 openbb_core-1.2.2/openbb_core/provider/standard_models/options_unusual.py
--rw-r--r--   0        0        0     1018 2024-04-08 12:02:16.508617 openbb_core-1.2.2/openbb_core/provider/standard_models/otc_aggregate.py
--rw-r--r--   0        0        0     2906 2024-04-08 12:02:16.508712 openbb_core-1.2.2/openbb_core/provider/standard_models/price_target.py
--rw-r--r--   0        0        0     1819 2024-04-23 10:22:39.581171 openbb_core-1.2.2/openbb_core/provider/standard_models/price_target_consensus.py
--rw-r--r--   0        0        0     4043 2024-04-08 12:02:16.508945 openbb_core-1.2.2/openbb_core/provider/standard_models/recent_performance.py
--rw-r--r--   0        0        0     2336 2024-04-08 12:02:16.509044 openbb_core-1.2.2/openbb_core/provider/standard_models/reported_financials.py
--rw-r--r--   0        0        0     1928 2024-04-08 12:02:16.509150 openbb_core-1.2.2/openbb_core/provider/standard_models/revenue_business_line.py
--rw-r--r--   0        0        0     1940 2024-04-08 12:02:16.509243 openbb_core-1.2.2/openbb_core/provider/standard_models/revenue_geographic.py
--rw-r--r--   0        0        0      827 2024-04-08 12:02:16.509331 openbb_core-1.2.2/openbb_core/provider/standard_models/risk_premium.py
--rw-r--r--   0        0        0     1729 2024-04-02 11:35:59.289085 openbb_core-1.2.2/openbb_core/provider/standard_models/search_attributes.py
--rw-r--r--   0        0        0     1777 2024-02-29 11:03:36.683510 openbb_core-1.2.2/openbb_core/provider/standard_models/search_financial_attributes.py
--rw-r--r--   0        0        0      819 2024-02-29 11:03:36.683639 openbb_core-1.2.2/openbb_core/provider/standard_models/sector_pe.py
--rw-r--r--   0        0        0      494 2024-02-29 11:03:36.683703 openbb_core-1.2.2/openbb_core/provider/standard_models/sector_performance.py
--rw-r--r--   0        0        0     1864 2024-04-08 12:02:16.509420 openbb_core-1.2.2/openbb_core/provider/standard_models/share_statistics.py
--rw-r--r--   0        0        0     1128 2024-04-08 12:02:16.509468 openbb_core-1.2.2/openbb_core/provider/standard_models/short_term_interest_rate.py
--rw-r--r--   0        0        0     1463 2024-04-08 12:02:16.509556 openbb_core-1.2.2/openbb_core/provider/standard_models/short_volume.py
--rw-r--r--   0        0        0      850 2024-04-08 12:02:16.509643 openbb_core-1.2.2/openbb_core/provider/standard_models/sofr_rates.py
--rw-r--r--   0        0        0      856 2024-04-08 12:02:16.509724 openbb_core-1.2.2/openbb_core/provider/standard_models/sonia_rates.py
--rw-r--r--   0        0        0     1965 2024-04-08 12:02:16.509820 openbb_core-1.2.2/openbb_core/provider/standard_models/sp500_multiples.py
--rw-r--r--   0        0        0     1431 2024-04-23 10:22:39.581294 openbb_core-1.2.2/openbb_core/provider/standard_models/spot.py
--rw-r--r--   0        0        0      495 2024-04-08 12:02:16.509962 openbb_core-1.2.2/openbb_core/provider/standard_models/symbol_map.py
--rw-r--r--   0        0        0     1327 2024-04-08 12:02:16.510053 openbb_core-1.2.2/openbb_core/provider/standard_models/tbffr.py
--rw-r--r--   0        0        0     1342 2024-04-08 12:02:16.510132 openbb_core-1.2.2/openbb_core/provider/standard_models/tmc.py
--rw-r--r--   0        0        0      875 2024-02-29 11:03:36.684333 openbb_core-1.2.2/openbb_core/provider/standard_models/top_retail.py
--rw-r--r--   0        0        0      952 2024-04-08 12:02:16.510225 openbb_core-1.2.2/openbb_core/provider/standard_models/trailing_dividend_yield.py
--rw-r--r--   0        0        0    23339 2024-04-08 12:02:16.510364 openbb_core-1.2.2/openbb_core/provider/standard_models/treasury_auctions.py
--rw-r--r--   0        0        0     3073 2024-05-09 13:34:29.178434 openbb_core-1.2.2/openbb_core/provider/standard_models/treasury_prices.py
--rw-r--r--   0        0        0     3526 2024-05-09 15:04:29.062912 openbb_core-1.2.2/openbb_core/provider/standard_models/treasury_rates.py
--rw-r--r--   0        0        0     1113 2024-04-08 12:02:16.510669 openbb_core-1.2.2/openbb_core/provider/standard_models/unemployment.py
--rw-r--r--   0        0        0      838 2024-02-29 11:03:36.684683 openbb_core-1.2.2/openbb_core/provider/standard_models/upcoming_release_days.py
--rw-r--r--   0        0        0      949 2024-02-29 11:03:36.684745 openbb_core-1.2.2/openbb_core/provider/standard_models/us_yield_curve.py
--rw-r--r--   0        0        0     2062 2024-04-08 12:02:16.510809 openbb_core-1.2.2/openbb_core/provider/standard_models/world_news.py
--rw-r--r--   0        0        0       29 2024-02-29 11:03:36.684895 openbb_core-1.2.2/openbb_core/provider/utils/__init__.py
--rw-r--r--   0        0        0     5013 2024-04-23 10:22:39.581426 openbb_core-1.2.2/openbb_core/provider/utils/client.py
--rw-r--r--   0        0        0     1166 2024-04-08 12:02:16.511096 openbb_core-1.2.2/openbb_core/provider/utils/descriptions.py
--rw-r--r--   0        0        0      341 2024-04-02 11:35:59.291045 openbb_core-1.2.2/openbb_core/provider/utils/errors.py
--rw-r--r--   0        0        0     9699 2024-05-02 09:48:24.768519 openbb_core-1.2.2/openbb_core/provider/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.685216 openbb_core-1.2.2/openbb_core/py.typed
--rw-r--r--   0        0        0      856 2024-05-15 16:44:02.603697 openbb_core-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3577 1970-01-01 00:00:00.000000 openbb_core-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-05-14 16:56:41.529863 openbb_core-1.2.3/README.md
+-rw-r--r--   0        0        0       19 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/__init__.py
+-rw-r--r--   0        0        0     1334 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/api/app_loader.py
+-rw-r--r--   0        0        0     1972 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/auth/user.py
+-rw-r--r--   0        0        0       34 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/dependency/__init__.py
+-rw-r--r--   0        0        0      604 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/dependency/coverage.py
+-rw-r--r--   0        0        0      653 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/dependency/system.py
+-rw-r--r--   0        0        0     2354 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/api/exception_handlers.py
+-rw-r--r--   0        0        0     3213 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/api/rest_api.py
+-rw-r--r--   0        0        0       30 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/router/__init__.py
+-rw-r--r--   0        0        0     7189 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/router/commands.py
+-rw-r--r--   0        0        0     1182 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/router/coverage.py
+-rw-r--r--   0        0        0       40 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/router/helpers/__init__.py
+-rw-r--r--   0        0        0     4202 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/router/helpers/coverage_helpers.py
+-rw-r--r--   0        0        0      469 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/router/system.py
+-rw-r--r--   0        0        0      557 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/api/router/user.py
+-rw-r--r--   0        0        0       30 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/__init__.py
+-rw-r--r--   0        0        0    18955 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/command_runner.py
+-rw-r--r--   0        0        0      293 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/constants.py
+-rw-r--r--   0        0        0     2563 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/deprecation.py
+-rw-r--r--   0        0        0     6120 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/extension_loader.py
+-rw-r--r--   0        0        0     5938 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/logs/formatters/formatter_with_exceptions.py
+-rw-r--r--   0        0        0     2705 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/logs/handlers/path_tracking_file_handler.py
+-rw-r--r--   0        0        0     4392 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/logs/handlers/posthog_handler.py
+-rw-r--r--   0        0        0     2964 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/logs/handlers_manager.py
+-rw-r--r--   0        0        0     8160 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/logs/logging_service.py
+-rw-r--r--   0        0        0     2238 2024-05-14 16:56:41.529863 openbb_core-1.2.3/openbb_core/app/logs/models/logging_settings.py
+-rw-r--r--   0        0        0      966 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/logs/utils/expired_files.py
+-rw-r--r--   0        0        0     2247 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/logs/utils/utils.py
+-rw-r--r--   0        0        0       29 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/abstract/__init__.py
+-rw-r--r--   0        0        0      302 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/abstract/error.py
+-rw-r--r--   0        0        0       99 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/abstract/results.py
+-rw-r--r--   0        0        0      551 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/abstract/singleton.py
+-rw-r--r--   0        0        0      252 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/abstract/tagged.py
+-rw-r--r--   0        0        0      458 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/abstract/warning.py
+-rw-r--r--   0        0        0     1919 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/model/api_settings.py
+-rw-r--r--   0        0        0     1035 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/charts/chart.py
+-rw-r--r--   0        0        0     2248 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/charts/charting_settings.py
+-rw-r--r--   0        0        0      398 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/command_context.py
+-rw-r--r--   0        0        0     4104 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/model/credentials.py
+-rw-r--r--   0        0        0      502 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/defaults.py
+-rw-r--r--   0        0        0     7329 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/example.py
+-rw-r--r--   0        0        0     2385 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/app/model/extension.py
+-rw-r--r--   0        0        0     1054 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/field.py
+-rw-r--r--   0        0        0      694 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/hub/hub_session.py
+-rw-r--r--   0        0        0      474 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/hub/hub_user_settings.py
+-rw-r--r--   0        0        0     5669 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/metadata.py
+-rw-r--r--   0        0        0     9240 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/app/model/obbject.py
+-rw-r--r--   0        0        0     1477 2024-05-14 16:57:23.534032 openbb_core-1.2.3/openbb_core/app/model/preferences.py
+-rw-r--r--   0        0        0      536 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/profile.py
+-rw-r--r--   0        0        0      801 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/python_settings.py
+-rw-r--r--   0        0        0       37 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/results/__init__.py
+-rw-r--r--   0        0        0      130 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/results/empty.py
+-rw-r--r--   0        0        0     4044 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/system_settings.py
+-rw-r--r--   0        0        0      854 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/model/user_settings.py
+-rw-r--r--   0        0        0    21634 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/app/provider_interface.py
+-rw-r--r--   0        0        0     2744 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/query.py
+-rw-r--r--   0        0        0    23116 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/router.py
+-rw-r--r--   0        0        0     2627 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/service/auth_service.py
+-rw-r--r--   0        0        0    10381 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/app/service/hub_service.py
+-rw-r--r--   0        0        0     3511 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/service/system_service.py
+-rw-r--r--   0        0        0     2706 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/service/user_service.py
+-rw-r--r--   0        0        0       30 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/static/__init__.py
+-rw-r--r--   0        0        0     7525 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/static/account.py
+-rw-r--r--   0        0        0     2024 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/static/app_factory.py
+-rw-r--r--   0        0        0     1582 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/static/container.py
+-rw-r--r--   0        0        0     1926 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/static/coverage.py
+-rw-r--r--   0        0        0    66959 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/static/package_builder.py
+-rw-r--r--   0        0        0     1431 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/static/reference_loader.py
+-rw-r--r--   0        0        0      408 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/static/utils/console.py
+-rw-r--r--   0        0        0     2718 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/app/static/utils/decorators.py
+-rw-r--r--   0        0        0     2699 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/app/static/utils/filters.py
+-rw-r--r--   0        0        0     1655 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/static/utils/linters.py
+-rw-r--r--   0        0        0     5986 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/utils.py
+-rw-r--r--   0        0        0     1809 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/app/version.py
+-rw-r--r--   0        0        0     2396 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/env.py
+-rw-r--r--   0        0        0      171 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/provider/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/provider/abstract/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/provider/abstract/annotated_result.py
+-rw-r--r--   0        0        0     3494 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/provider/abstract/data.py
+-rw-r--r--   0        0        0     8881 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/provider/abstract/fetcher.py
+-rw-r--r--   0        0        0     1985 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/provider/abstract/provider.py
+-rw-r--r--   0        0        0     2702 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/provider/abstract/query_params.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/provider/py.typed
+-rw-r--r--   0        0        0     3524 2024-05-14 16:56:41.533863 openbb_core-1.2.3/openbb_core/provider/query_executor.py
+-rw-r--r--   0        0        0     1705 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/provider/registry.py
+-rw-r--r--   0        0        0     8297 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/provider/registry_map.py
+-rw-r--r--   0        0        0       43 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/__init__.py
+-rw-r--r--   0        0        0      874 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/ameribor_rates.py
+-rw-r--r--   0        0        0     3426 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/analyst_estimates.py
+-rw-r--r--   0        0        0     1270 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/analyst_search.py
+-rw-r--r--   0        0        0     1377 2024-05-14 16:57:23.534032 openbb_core-1.2.3/openbb_core/provider/standard_models/available_indicators.py
+-rw-r--r--   0        0        0      630 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/available_indices.py
+-rw-r--r--   0        0        0    23375 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/provider/standard_models/balance_of_payments.py
+-rw-r--r--   0        0        0     1541 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/balance_sheet.py
+-rw-r--r--   0        0        0     5809 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3619 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/bond_prices.py
+-rw-r--r--   0        0        0     2939 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/bond_reference.py
+-rw-r--r--   0        0        0     2802 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/bond_trades.py
+-rw-r--r--   0        0        0     1599 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/calendar_dividend.py
+-rw-r--r--   0        0        0     1300 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/calendar_earnings.py
+-rw-r--r--   0        0        0     2264 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/calendar_ipo.py
+-rw-r--r--   0        0        0     1117 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/calendar_splits.py
+-rw-r--r--   0        0        0     1560 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/cash_flow.py
+-rw-r--r--   0        0        0     5087 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/cash_flow_growth.py
+-rw-r--r--   0        0        0      829 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/cik_map.py
+-rw-r--r--   0        0        0     2237 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/company_filings.py
+-rw-r--r--   0        0        0     2424 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/company_news.py
+-rw-r--r--   0        0        0     4560 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/company_overview.py
+-rw-r--r--   0        0        0     1721 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/provider/standard_models/compare_company_facts.py
+-rw-r--r--   0        0        0      766 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/compare_groups.py
+-rw-r--r--   0        0        0     1057 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/composite_leading_indicator.py
+-rw-r--r--   0        0        0      714 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/cot.py
+-rw-r--r--   0        0        0     1246 2024-05-14 16:57:23.538032 openbb_core-1.2.3/openbb_core/provider/standard_models/cot_search.py
+-rw-r--r--   0        0        0     3722 2024-05-14 16:57:23.538032 openbb_core-1.2.3/openbb_core/provider/standard_models/country_profile.py
+-rw-r--r--   0        0        0     1591 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/cp.py
+-rw-r--r--   0        0        0     3335 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/cpi.py
+-rw-r--r--   0        0        0     2310 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/crypto_historical.py
+-rw-r--r--   0        0        0      668 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/crypto_search.py
+-rw-r--r--   0        0        0     2363 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/currency_historical.py
+-rw-r--r--   0        0        0      732 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/provider/standard_models/currency_pairs.py
+-rw-r--r--   0        0        0     2992 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/currency_reference_rates.py
+-rw-r--r--   0        0        0     3125 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/currency_snapshots.py
+-rw-r--r--   0        0        0     1549 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/discovery_filings.py
+-rw-r--r--   0        0        0     1027 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/dwpcr_rates.py
+-rw-r--r--   0        0        0     1583 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     1452 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2125 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/provider/standard_models/economic_calendar.py
+-rw-r--r--   0        0        0     1680 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/provider/standard_models/economic_indicators.py
+-rw-r--r--   0        0        0     1750 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_ftd.py
+-rw-r--r--   0        0        0     2157 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_historical.py
+-rw-r--r--   0        0        0     5757 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_info.py
+-rw-r--r--   0        0        0     1392 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_nbbo.py
+-rw-r--r--   0        0        0     5402 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_ownership.py
+-rw-r--r--   0        0        0      855 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_peers.py
+-rw-r--r--   0        0        0     1326 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_performance.py
+-rw-r--r--   0        0        0     5878 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_quote.py
+-rw-r--r--   0        0        0      898 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_screener.py
+-rw-r--r--   0        0        0      912 2024-05-14 16:57:23.538032 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_search.py
+-rw-r--r--   0        0        0     3528 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_short_interest.py
+-rw-r--r--   0        0        0    10945 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     1664 2024-05-14 16:56:41.537863 openbb_core-1.2.3/openbb_core/provider/standard_models/esg_risk_rating.py
+-rw-r--r--   0        0        0     1922 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/esg_score.py
+-rw-r--r--   0        0        0      951 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/esg_sector.py
+-rw-r--r--   0        0        0      850 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/estr_rates.py
+-rw-r--r--   0        0        0      791 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_countries.py
+-rw-r--r--   0        0        0     1448 2024-05-15 11:30:49.635743 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     1980 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_historical.py
+-rw-r--r--   0        0        0      871 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_historical_nav.py
+-rw-r--r--   0        0        0      939 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_holdings.py
+-rw-r--r--   0        0        0      640 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_holdings_date.py
+-rw-r--r--   0        0        0     1027 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_info.py
+-rw-r--r--   0        0        0     1576 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_performance.py
+-rw-r--r--   0        0        0      644 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_search.py
+-rw-r--r--   0        0        0      862 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/etf_sectors.py
+-rw-r--r--   0        0        0      905 2024-05-15 11:30:49.635743 openbb_core-1.2.3/openbb_core/provider/standard_models/eu_yield_curve.py
+-rw-r--r--   0        0        0     2065 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/executive_compensation.py
+-rw-r--r--   0        0        0     1234 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/fed_projections.py
+-rw-r--r--   0        0        0      844 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/fed_rates.py
+-rw-r--r--   0        0        0     1439 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/ffrmc.py
+-rw-r--r--   0        0        0     1773 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/financial_attributes.py
+-rw-r--r--   0        0        0     1444 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/financial_ratios.py
+-rw-r--r--   0        0        0     3970 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/form_13FHR.py
+-rw-r--r--   0        0        0     2607 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/provider/standard_models/forward_ebitda_estimates.py
+-rw-r--r--   0        0        0     2321 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     1645 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/provider/standard_models/forward_pe_estimates.py
+-rw-r--r--   0        0        0     2390 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     2715 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/fred_search.py
+-rw-r--r--   0        0        0     1204 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/fred_series.py
+-rw-r--r--   0        0        0     1077 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/futures_curve.py
+-rw-r--r--   0        0        0     1857 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/futures_historical.py
+-rw-r--r--   0        0        0     1564 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/gdp_forecast.py
+-rw-r--r--   0        0        0     1405 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/gdp_nominal.py
+-rw-r--r--   0        0        0     1439 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/gdp_real.py
+-rw-r--r--   0        0        0     2532 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/historical_attributes.py
+-rw-r--r--   0        0        0     1271 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/historical_dividends.py
+-rw-r--r--   0        0        0     2705 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/historical_employees.py
+-rw-r--r--   0        0        0     1532 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/historical_eps.py
+-rw-r--r--   0        0        0     1207 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/historical_splits.py
+-rw-r--r--   0        0        0     1397 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/hqm.py
+-rw-r--r--   0        0        0     1410 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/ice_bofa.py
+-rw-r--r--   0        0        0     1556 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/income_statement.py
+-rw-r--r--   0        0        0     4974 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/income_statement_growth.py
+-rw-r--r--   0        0        0      750 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/index_constituents.py
+-rw-r--r--   0        0        0     2408 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/index_historical.py
+-rw-r--r--   0        0        0     1292 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/index_info.py
+-rw-r--r--   0        0        0      691 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/index_search.py
+-rw-r--r--   0        0        0      777 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/index_sectors.py
+-rw-r--r--   0        0        0     1825 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/index_snapshots.py
+-rw-r--r--   0        0        0      835 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/industry_pe.py
+-rw-r--r--   0        0        0     3148 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/insider_trading.py
+-rw-r--r--   0        0        0     1413 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/institutional_ownership.py
+-rw-r--r--   0        0        0      850 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/iorb_rates.py
+-rw-r--r--   0        0        0     1406 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/key_executives.py
+-rw-r--r--   0        0        0     1540 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/key_metrics.py
+-rw-r--r--   0        0        0     1450 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/latest_attributes.py
+-rw-r--r--   0        0        0     2654 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/lbma_fixing.py
+-rw-r--r--   0        0        0     1125 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     1951 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/market_indices.py
+-rw-r--r--   0        0        0      832 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/market_movers.py
+-rw-r--r--   0        0        0     1627 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/market_snapshots.py
+-rw-r--r--   0        0        0     1827 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/money_measures.py
+-rw-r--r--   0        0        0     1355 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/moody.py
+-rw-r--r--   0        0        0     6200 2024-05-14 16:57:23.538032 openbb_core-1.2.3/openbb_core/provider/standard_models/options_chains.py
+-rw-r--r--   0        0        0     1071 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/options_unusual.py
+-rw-r--r--   0        0        0     1018 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/otc_aggregate.py
+-rw-r--r--   0        0        0     2906 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/price_target.py
+-rw-r--r--   0        0        0     1819 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/price_target_consensus.py
+-rw-r--r--   0        0        0     4043 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/recent_performance.py
+-rw-r--r--   0        0        0     2336 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/reported_financials.py
+-rw-r--r--   0        0        0     1928 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/revenue_business_line.py
+-rw-r--r--   0        0        0     1940 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/revenue_geographic.py
+-rw-r--r--   0        0        0      827 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/risk_premium.py
+-rw-r--r--   0        0        0     1729 2024-05-14 16:56:41.541863 openbb_core-1.2.3/openbb_core/provider/standard_models/search_attributes.py
+-rw-r--r--   0        0        0     1777 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/search_financial_attributes.py
+-rw-r--r--   0        0        0      819 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/sector_pe.py
+-rw-r--r--   0        0        0      494 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/sector_performance.py
+-rw-r--r--   0        0        0     1864 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/share_statistics.py
+-rw-r--r--   0        0        0     1128 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     1463 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/short_volume.py
+-rw-r--r--   0        0        0      850 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/sofr_rates.py
+-rw-r--r--   0        0        0      856 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/sonia_rates.py
+-rw-r--r--   0        0        0     1965 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/sp500_multiples.py
+-rw-r--r--   0        0        0     1431 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/spot.py
+-rw-r--r--   0        0        0      495 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/symbol_map.py
+-rw-r--r--   0        0        0     1327 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/tbffr.py
+-rw-r--r--   0        0        0     1342 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/tmc.py
+-rw-r--r--   0        0        0      875 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/top_retail.py
+-rw-r--r--   0        0        0      952 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0    23339 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/treasury_auctions.py
+-rw-r--r--   0        0        0     3073 2024-05-14 16:57:23.538032 openbb_core-1.2.3/openbb_core/provider/standard_models/treasury_prices.py
+-rw-r--r--   0        0        0     3526 2024-05-15 09:21:56.021885 openbb_core-1.2.3/openbb_core/provider/standard_models/treasury_rates.py
+-rw-r--r--   0        0        0     1113 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/unemployment.py
+-rw-r--r--   0        0        0      838 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/upcoming_release_days.py
+-rw-r--r--   0        0        0      949 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/us_yield_curve.py
+-rw-r--r--   0        0        0     2062 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/standard_models/world_news.py
+-rw-r--r--   0        0        0     1032 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/provider/standard_models/yield_curve.py
+-rw-r--r--   0        0        0       29 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/utils/__init__.py
+-rw-r--r--   0        0        0     5013 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/utils/client.py
+-rw-r--r--   0        0        0     1166 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/provider/utils/descriptions.py
+-rw-r--r--   0        0        0      405 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/provider/utils/errors.py
+-rw-r--r--   0        0        0     9711 2024-05-22 11:48:40.395330 openbb_core-1.2.3/openbb_core/provider/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.545863 openbb_core-1.2.3/openbb_core/py.typed
+-rw-r--r--   0        0        0      726 2024-05-22 13:51:46.830729 openbb_core-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3541 1970-01-01 00:00:00.000000 openbb_core-1.2.3/PKG-INFO
```

### Comparing `openbb_core-1.2.2/README.md` & `openbb_core-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/api/auth/user.py` & `openbb_core-1.2.3/openbb_core/api/auth/user.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/api/dependency/coverage.py` & `openbb_core-1.2.3/openbb_core/api/dependency/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/api/dependency/system.py` & `openbb_core-1.2.3/openbb_core/api/dependency/system.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/api/router/commands.py` & `openbb_core-1.2.3/openbb_core/api/router/commands.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/api/router/coverage.py` & `openbb_core-1.2.3/openbb_core/api/router/coverage.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/api/router/helpers/coverage_helpers.py` & `openbb_core-1.2.3/openbb_core/api/router/helpers/coverage_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/api/router/user.py` & `openbb_core-1.2.3/openbb_core/api/router/user.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/command_runner.py` & `openbb_core-1.2.3/openbb_core/app/command_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
         return func
 
     @classmethod
     def merge_args_and_kwargs(
         cls,
         func: Callable,
-        args: Tuple[Any],
+        args: Tuple[Any, ...],
         kwargs: Dict[str, Any],
     ) -> Dict[str, Any]:
         """Merge args and kwargs into a single dict."""
         args = deepcopy(args)
         kwargs = deepcopy(kwargs)
         parameter_list = cls.get_polished_parameter_list(func=func)
         parameter_map = {}
@@ -130,15 +130,15 @@
         def _needs_provider(func: Callable) -> bool:
             """Check if the function needs a provider."""
             parameters = signature(func).parameters.keys()
             return "provider_choices" in parameters
 
         def _has_provider(kwargs: Dict[str, Any]) -> bool:
             """Check if the kwargs already have a provider."""
-            provider_choices = kwargs.get("provider_choices", None)
+            provider_choices = kwargs.get("provider_choices")
 
             if isinstance(provider_choices, dict):  # when in python
                 return provider_choices.get("provider", None) is not None
             if isinstance(provider_choices, object):  # when running as fastapi
                 return getattr(provider_choices, "provider", None) is not None
             return False
 
@@ -152,15 +152,15 @@
             route_default: Optional[Dict[str, Optional[str]]],
         ) -> Optional[str]:
             """
             Get the default provider for the given route.
 
             Either pick it from the user defaults or from the command coverage.
             """
-            cmd_cov_given_route = command_coverage.get(route, None)
+            cmd_cov_given_route = command_coverage.get(route)
             command_cov_provider = (
                 cmd_cov_given_route[0] if cmd_cov_given_route else None
             )
 
             if route_default:
                 return route_default.get("provider", None) or command_cov_provider  # type: ignore
 
@@ -225,15 +225,16 @@
                 Any if p.annotation is Parameter.empty else p.annotation,
                 ... if p.default is Parameter.empty else p.default,
             )
             for n, p in sig.parameters.items()
         }
         # We allow extra fields to return with model with 'cc: CommandContext'
         config = ConfigDict(extra="allow", arbitrary_types_allowed=True)
-        ValidationModel = create_model(func.__name__, __config__=config, **fields)  # type: ignore  # pylint: disable=C0103
+        # pylint: disable=C0103
+        ValidationModel = create_model(func.__name__, __config__=config, **fields)  # type: ignore
         # Validate and coerce
         model = ValidationModel(**kwargs)
         ParametersBuilder._warn_kwargs(
             ParametersBuilder._as_dict(kwargs.get("extra_params", {})),
             ValidationModel,
         )
         return dict(model)
@@ -288,17 +289,15 @@
         cls,
         func: Callable,
         kwargs: Dict[str, Any],
         show_warnings: bool = True,  # pylint: disable=unused-argument   # type: ignore
     ) -> OBBject:
         """Run a command and return the output."""
         obbject = await maybe_coroutine(func, **kwargs)
-        obbject.provider = getattr(
-            kwargs.get("provider_choices", None), "provider", None
-        )
+        obbject.provider = getattr(kwargs.get("provider_choices"), "provider", None)
         return obbject
 
     @classmethod
     def _chart(
         cls,
         obbject: OBBject,
         **kwargs,
@@ -327,15 +326,15 @@
                 and "chart_params" in kwargs["kwargs"]
                 and kwargs["kwargs"].get("chart_params") is not None
             ):
                 chart_params.update(kwargs.pop("kwargs", {}).get("chart_params", {}))
 
             if chart_params:
                 kwargs.update(chart_params)
-            obbject.charting.show(render=False, **kwargs)
+            obbject.charting.show(render=False, **kwargs)  # type: ignore[attr-defined]
         except Exception as e:  # pylint: disable=broad-exception-caught
             if Env().DEBUG_MODE:
                 raise OpenBBError(e) from e
             warn(str(e), OpenBBWarning)
 
     # pylint: disable=R0913, R0914
     @classmethod
@@ -382,17 +381,14 @@
             try:
                 obbject = await cls._command(func, kwargs)
                 # pylint: disable=protected-access
                 obbject._route = route
                 obbject._standard_params = kwargs.get("standard_params", None)
                 if chart and obbject.results:
                     cls._chart(obbject, **kwargs)
-
-            except Exception as e:
-                raise OpenBBError(e) from e
             finally:
                 ls = LoggingService(system_settings, user_settings)
                 ls.log(
                     user_settings=user_settings,
                     system_settings=system_settings,
                     route=route,
                     func=func,
```

### Comparing `openbb_core-1.2.2/openbb_core/app/deprecation.py` & `openbb_core-1.2.3/openbb_core/app/deprecation.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/extension_loader.py` & `openbb_core-1.2.3/openbb_core/app/extension_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/logs/formatters/formatter_with_exceptions.py` & `openbb_core-1.2.3/openbb_core/app/logs/formatters/formatter_with_exceptions.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/logs/handlers/path_tracking_file_handler.py` & `openbb_core-1.2.3/openbb_core/app/logs/handlers/path_tracking_file_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/logs/handlers/posthog_handler.py` & `openbb_core-1.2.3/openbb_core/app/logs/handlers/posthog_handler.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/logs/handlers_manager.py` & `openbb_core-1.2.3/openbb_core/app/logs/handlers_manager.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/logs/logging_service.py` & `openbb_core-1.2.3/openbb_core/app/logs/logging_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Logging Service Module."""
 
 import json
 import logging
 from enum import Enum
 from types import TracebackType
-from typing import Any, Callable, Dict, Optional, Tuple, Type, Union, cast
+from typing import Any, Callable, Dict, Optional, Tuple, Type, Union
 
 from openbb_core.app.logs.formatters.formatter_with_exceptions import (
     FormatterWithExceptions,
 )
 from openbb_core.app.logs.handlers_manager import HandlersManager
 from openbb_core.app.logs.models.logging_settings import LoggingSettings
-from openbb_core.app.model.abstract.error import OpenBBError
 from openbb_core.app.model.abstract.singleton import SingletonMeta
 from openbb_core.app.model.system_settings import SystemSettings
 from openbb_core.app.model.user_settings import UserSettings
 from pydantic_core import to_jsonable_python
 
 
 class LoggingService(metaclass=SingletonMeta):
@@ -220,30 +219,28 @@
             # Remove CommandContext if any
             kwargs.pop("cc", None)
 
             # Truncate kwargs if too long
             kwargs = {k: str(v)[:100] for k, v in kwargs.items()}
 
             # Get execution info
-            openbb_error = cast(
-                Optional[OpenBBError], exec_info[1] if exec_info else None
-            )
+            error = str(exec_info[1]) if exec_info and len(exec_info) > 1 else None
 
             # Construct message
-            message_label = "ERROR" if openbb_error else "CMD"
+            message_label = "ERROR" if error else "CMD"
             log_message = json.dumps(
                 {
                     "route": route,
                     "input": kwargs,
-                    "error": str(openbb_error.original) if openbb_error else None,
+                    "error": error,
                     "custom_headers": custom_headers,
                 },
                 default=to_jsonable_python,
             )
             log_message = f"{message_label}: {log_message}"
 
-            log_level = logger.error if openbb_error else logger.info
+            log_level = logger.error if error else logger.info
             log_level(
                 log_message,
                 extra={"func_name_override": func.__name__},
                 exc_info=exec_info,
             )
```

### Comparing `openbb_core-1.2.2/openbb_core/app/logs/models/logging_settings.py` & `openbb_core-1.2.3/openbb_core/app/logs/models/logging_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/logs/utils/expired_files.py` & `openbb_core-1.2.3/openbb_core/app/logs/utils/expired_files.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/logs/utils/utils.py` & `openbb_core-1.2.3/openbb_core/app/logs/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/abstract/singleton.py` & `openbb_core-1.2.3/openbb_core/app/model/abstract/singleton.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/api_settings.py` & `openbb_core-1.2.3/openbb_core/app/model/api_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 class APISettings(BaseModel):
     """Settings model for FastAPI configuration."""
 
     model_config = ConfigDict(frozen=True)
 
     version: str = "1"
     title: str = "OpenBB Platform API"
-    description: str = "This is the OpenBB Platform API."
+    description: str = "Investment research for everyone, anywhere."
     terms_of_service: str = "http://example.com/terms/"
     contact_name: str = "OpenBB Team"
     contact_url: str = "https://openbb.co"
     contact_email: str = "hello@openbb.co"
     license_name: str = "MIT"
     license_url: str = (
         "https://github.com/OpenBB-finance/OpenBBTerminal/blob/develop/LICENSE"
```

### Comparing `openbb_core-1.2.2/openbb_core/app/model/charts/chart.py` & `openbb_core-1.2.3/openbb_core/app/model/charts/chart.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/charts/charting_settings.py` & `openbb_core-1.2.3/openbb_core/app/model/charts/charting_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/credentials.py` & `openbb_core-1.2.3/openbb_core/app/model/credentials.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,15 +57,15 @@
                 )
 
         return formatted
 
     def from_obbject(self) -> None:
         """Load credentials from OBBject extensions."""
         self.credentials["obbject"] = set()
-        for name, entry in ExtensionLoader().obbject_objects.items():
+        for name, entry in ExtensionLoader().obbject_objects.items():  # type: ignore[attr-defined]
             try:
                 for c in entry.credentials:
                     self.credentials["obbject"].add(c)
             except Exception as e:
                 msg = f"Error loading extension: {name}\n"
                 if Env().DEBUG_MODE:
                     traceback.print_exception(type(e), e, e.__traceback__)
@@ -112,7 +112,11 @@
         print(  # noqa: T201
             self.__class__.__name__
             + "\n\n"
             + "\n".join(
                 [f"{k}: {v}" for k, v in sorted(self.model_dump(mode="json").items())]
             )
         )
+
+    def update(self, incoming: "Credentials"):
+        """Update current credentials."""
+        self.__dict__.update(incoming.model_dump(exclude_none=True))
```

### Comparing `openbb_core-1.2.2/openbb_core/app/model/example.py` & `openbb_core-1.2.3/openbb_core/app/model/example.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/extension.py` & `openbb_core-1.2.3/openbb_core/app/model/extension.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/field.py` & `openbb_core-1.2.3/openbb_core/app/model/field.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/hub/hub_session.py` & `openbb_core-1.2.3/openbb_core/app/model/hub/hub_session.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/metadata.py` & `openbb_core-1.2.3/openbb_core/app/model/metadata.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/obbject.py` & `openbb_core-1.2.3/openbb_core/app/model/obbject.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/preferences.py` & `openbb_core-1.2.3/openbb_core/app/model/preferences.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/profile.py` & `openbb_core-1.2.3/openbb_core/app/model/profile.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/python_settings.py` & `openbb_core-1.2.3/openbb_core/app/model/python_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/system_settings.py` & `openbb_core-1.2.3/openbb_core/app/model/system_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/model/user_settings.py` & `openbb_core-1.2.3/openbb_core/app/model/user_settings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/provider_interface.py` & `openbb_core-1.2.3/openbb_core/app/provider_interface.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/query.py` & `openbb_core-1.2.3/openbb_core/app/query.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/router.py` & `openbb_core-1.2.3/openbb_core/app/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -640,15 +640,15 @@
 
     @staticmethod
     @lru_cache
     def from_extensions() -> Router:
         """Load routes from extensions."""
         router = Router()
 
-        for name, entry in ExtensionLoader().core_objects.items():
+        for name, entry in ExtensionLoader().core_objects.items():  # type: ignore[attr-defined]
             try:
                 router.include_router(router=entry, prefix=f"/{name}")
             except Exception as e:
                 msg = f"Error loading extension: {name}\n"
                 if Env().DEBUG_MODE:
                     traceback.print_exception(type(e), e, e.__traceback__)
                     raise LoadingError(msg + f"\033[91m{e}\033[0m") from e
```

### Comparing `openbb_core-1.2.2/openbb_core/app/service/auth_service.py` & `openbb_core-1.2.3/openbb_core/app/service/auth_service.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/service/hub_service.py` & `openbb_core-1.2.3/openbb_core/app/service/hub_service.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/service/system_service.py` & `openbb_core-1.2.3/openbb_core/app/service/system_service.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/service/user_service.py` & `openbb_core-1.2.3/openbb_core/app/service/user_service.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,23 +46,14 @@
         path = path or cls.USER_SETTINGS_PATH
 
         user_settings_json = user_settings.model_dump_json(
             include=cls.USER_SETTINGS_ALLOWED_FIELD_SET, indent=4
         )
         path.write_text(user_settings_json, encoding="utf-8")
 
-    @classmethod
-    def update_default(cls, user_settings: UserSettings) -> UserSettings:
-        """Update default user settings."""
-        d1 = cls.read_default_user_settings().model_dump()
-        d2 = user_settings.model_dump() if user_settings else {}
-        updated = cls._merge_dicts([d1, d2])
-
-        return UserSettings.model_validate(updated)
-
     @staticmethod
     def _merge_dicts(list_of_dicts: List[Dict[str, Any]]) -> Dict[str, Any]:
         """Merge a list of dictionaries."""
 
         def recursive_merge(d1: Dict, d2: Dict) -> Dict:
             """Recursively merge dict d2 into dict d1 if d2 is value is not None."""
             for k, v in d1.items():
```

### Comparing `openbb_core-1.2.2/openbb_core/app/static/account.py` & `openbb_core-1.2.3/openbb_core/app/static/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from openbb_core.app.service.hub_service import HubService
 from openbb_core.app.service.user_service import UserService
 
 if TYPE_CHECKING:
     from openbb_core.app.static.app_factory import BaseApp
 
 
-class Account:
+class Account:  # noqa: D205, D400
     """/account
     login
     logout
     save
     refresh
     """
 
@@ -119,16 +119,16 @@
         Returns
         -------
         Optional[UserSettings]
             User settings: profile, credentials, preferences
         """
         self._hub_service = self._create_hub_service(email, password, pat)
         incoming = self._hub_service.pull()
-        updated: UserSettings = UserService.update_default(incoming)
-        self._base_app._command_runner.user_settings = updated
+        self._base_app.user.profile = incoming.profile
+        self._base_app.user.credentials.update(incoming.credentials)
         if remember_me:
             Path(self._openbb_directory).mkdir(parents=False, exist_ok=True)
             session_file = Path(self._openbb_directory, self.SESSION_FILE)
             with open(session_file, "w") as f:
                 if not self._hub_service.session:
                     raise OpenBBError("Not connected to hub.")
 
@@ -181,18 +181,16 @@
         """
         if not self._hub_service:
             self._base_app._command_runner.user_settings = (
                 UserService.read_default_user_settings()
             )
         else:
             incoming = self._hub_service.pull()
-            updated: UserSettings = UserService.update_default(incoming)
-            updated.id = self._base_app._command_runner.user_settings.id
-            self._base_app._command_runner.user_settings = updated
-
+            self._base_app.user.profile = incoming.profile
+            self._base_app.user.credentials.update(incoming.credentials)
         if return_settings:
             return self._base_app._command_runner.user_settings
         return None
 
     @_log_account_command  # type: ignore
     def logout(self, return_settings: bool = False) -> Optional[UserSettings]:
         """Logout from hub.
```

### Comparing `openbb_core-1.2.2/openbb_core/app/static/app_factory.py` & `openbb_core-1.2.3/openbb_core/app/static/app_factory.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/static/container.py` & `openbb_core-1.2.3/openbb_core/app/static/container.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/static/coverage.py` & `openbb_core-1.2.3/openbb_core/app/static/coverage.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,21 @@
 from openbb_core.app.router import CommandMap
 from openbb_core.app.static.reference_loader import ReferenceLoader
 
 if TYPE_CHECKING:
     from openbb_core.app.static.app_factory import BaseApp
 
 
-class Coverage:
-    """Coverage class.
-
-    /coverage
-
-        providers
-        commands
-        command_model
-        command_schemas
-        reference
+class Coverage:  # noqa: D205, D400
+    """/coverage
+    providers
+    commands
+    command_model
+    command_schemas
+    reference
     """
 
     def __init__(self, app: "BaseApp"):
         """Initialize coverage."""
         self._app = app
         self._command_map = CommandMap(coverage_sep=".")
         self._provider_interface = ProviderInterface()
```

### Comparing `openbb_core-1.2.2/openbb_core/app/static/package_builder.py` & `openbb_core-1.2.3/openbb_core/app/static/package_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         """Save the reference.json file."""
         self.console.log("\nWriting reference file...")
         code = dumps(
             obj={
                 "openbb": VERSION.replace("dev", ""),
                 "info": {
                     "title": "OpenBB Platform (Python)",
-                    "description": "This is the OpenBB Platform (Python).",
+                    "description": "Investment research for everyone, anywhere.",
                     "core": CORE_VERSION.replace("dev", ""),
                     "extensions": ext_map,
                 },
                 "paths": ReferenceGenerator.get_paths(self.route_map),
                 "routers": ReferenceGenerator.get_routers(self.route_map),
             },
             indent=4,
@@ -1044,15 +1044,15 @@
         return ""
 
     @classmethod
     def generate_model_docstring(
         cls,
         model_name: str,
         summary: str,
-        explicit_params: dict,
+        explicit_params: Dict[str, Parameter],
         kwarg_params: dict,
         returns: Dict[str, FieldInfo],
         results_type: str,
         sections: List[str],
     ) -> str:
         """Create the docstring for model."""
 
@@ -1067,16 +1067,18 @@
             return type_str
 
         def format_description(description: str) -> str:
             """Format description in docstrings."""
             description = description.replace("\n", f"\n{create_indent(2)}")
             return description
 
-        def get_param_info(parameter: Parameter) -> Tuple[str, str]:
+        def get_param_info(parameter: Optional[Parameter]) -> Tuple[str, str]:
             """Get the parameter info."""
+            if not parameter:
+                return "", ""
             annotation = getattr(parameter, "_annotation", None)
             if isinstance(annotation, _AnnotatedAlias):
                 args = getattr(annotation, "__args__", []) if annotation else []
                 p_type = args[0] if args else None
             else:
                 p_type = annotation
             type_ = (
@@ -1119,15 +1121,15 @@
                 docstring += f"{create_indent(3)}{format_description(description)}\n"
 
         if "returns" in sections:
             # Returns
             docstring += "\n"
             docstring += f"{create_indent(2)}Returns\n"
             docstring += f"{create_indent(2)}-------\n"
-            providers, _ = get_param_info(explicit_params.get("provider", None))
+            providers, _ = get_param_info(explicit_params.get("provider"))
             docstring += cls.get_OBBject_description(results_type, providers)
 
             # Schema
             underline = "-" * len(model_name)
             docstring += f"\n{create_indent(2)}{model_name}\n"
             docstring += f"{create_indent(2)}{underline}\n"
 
@@ -1296,15 +1298,15 @@
                         path_list.append(sub_path)
 
         return path_list
 
     @staticmethod
     def get_route(path: str, route_map: Dict[str, BaseRoute]):
         """Get the route from the path."""
-        return route_map.get(path, None)
+        return route_map.get(path)
 
     @staticmethod
     def get_child_path_list(path: str, path_list: List[str]) -> List[str]:
         """Get the child path list."""
         direct_children = []
         for p in path_list:
             if p.startswith(path):
```

### Comparing `openbb_core-1.2.2/openbb_core/app/static/reference_loader.py` & `openbb_core-1.2.3/openbb_core/app/static/reference_loader.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/static/utils/decorators.py` & `openbb_core-1.2.3/openbb_core/app/static/utils/decorators.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,51 +43,43 @@
 def exception_handler(func: Callable[P, R]) -> Callable[P, R]:
     """Handle exceptions, attempting to focus on the last call from the traceback."""
 
     @wraps(func)
     def wrapper(*f_args, **f_kwargs):
         try:
             return func(*f_args, **f_kwargs)
-        except (ValidationError, Exception) as e:
-            # If the DEBUG_MODE is enabled, raise the exception with complete traceback
+        except (ValidationError, OpenBBError, Exception) as e:
             if Env().DEBUG_MODE:
                 raise
 
             # Get the last traceback object from the exception
             tb = e.__traceback__
             if tb:
                 while tb.tb_next is not None:
                     tb = tb.tb_next
 
             if isinstance(e, ValidationError):
                 error_list = []
-
-                validation_error = f"{e.error_count()} validations errors in {e.title}"
-                for error in e.errors():
-                    arg = ".".join(map(str, error["loc"]))
-                    arg_error = f"Arg {arg} ->\n"
-                    error_details = (
-                        f"{error['msg']} "
-                        f"[validation_error_type={error['type']}, "
-                        f"input_type={type(error['input']).__name__}, "
-                        f"input_value={error['input']}]\n"
-                    )
-                    url = error.get("url")
-                    error_info = (
-                        f"    For further information visit {url}\n" if url else ""
+                validation_error = f"{e.error_count()} validations error(s)"
+                for err in e.errors(include_url=False):
+                    loc = ".".join(
+                        [
+                            str(i)
+                            for i in err.get("loc", ())
+                            if i not in ("standard_params", "extra_params")
+                        ]
                     )
-                    error_list.append(arg_error + error_details + error_info)
-
+                    _input = err.get("input", "")
+                    msg = err.get("msg", "")
+                    error_list.append(f"[Arg] {loc} -> input: {_input} -> {msg}")
                 error_list.insert(0, validation_error)
                 error_str = "\n".join(error_list)
-
-                raise OpenBBError(
-                    f"\nType -> ValidationError \n\nDetails -> {error_str}"
-                ).with_traceback(tb) from None
-
-            # If the error is not a ValidationError, then it is a generic exception
-            error_type = getattr(e, "original", e).__class__.__name__
-            raise OpenBBError(
-                f"\nType -> {error_type}\n\nDetail -> {str(e)}"
-            ).with_traceback(tb) from None
+                raise OpenBBError(f"\n[Error] -> {error_str}").with_traceback(
+                    tb
+                ) from None
+            if isinstance(e, OpenBBError):
+                raise OpenBBError(f"\n[Error] -> {str(e)}").with_traceback(tb) from None
+            raise OpenBBError("\n[Error] -> Unexpected error.").with_traceback(
+                tb
+            ) from None
 
     return wrapper
```

### Comparing `openbb_core-1.2.2/openbb_core/app/static/utils/filters.py` & `openbb_core-1.2.3/openbb_core/app/static/utils/filters.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/static/utils/linters.py` & `openbb_core-1.2.3/openbb_core/app/static/utils/linters.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/utils.py` & `openbb_core-1.2.3/openbb_core/app/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/app/version.py` & `openbb_core-1.2.3/openbb_core/app/version.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/env.py` & `openbb_core-1.2.3/openbb_core/env.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/abstract/data.py` & `openbb_core-1.2.3/openbb_core/provider/abstract/data.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/abstract/fetcher.py` & `openbb_core-1.2.3/openbb_core/provider/abstract/fetcher.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/abstract/provider.py` & `openbb_core-1.2.3/openbb_core/provider/abstract/provider.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/abstract/query_params.py` & `openbb_core-1.2.3/openbb_core/provider/abstract/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/query_executor.py` & `openbb_core-1.2.3/openbb_core/provider/query_executor.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/registry.py` & `openbb_core-1.2.3/openbb_core/provider/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     @staticmethod
     @lru_cache
     def from_extensions() -> Registry:
         """Load providers from entry points."""
         registry = Registry()
 
-        for name, entry in ExtensionLoader().provider_objects.items():
+        for name, entry in ExtensionLoader().provider_objects.items():  # type: ignore[attr-defined]
             try:
                 registry.include_provider(provider=entry)
             except Exception as e:
                 msg = f"Error loading extension: {name}\n"
                 if Env().DEBUG_MODE:
                     traceback.print_exception(type(e), e, e.__traceback__)
                     raise LoadingError(msg + f"\033[91m{e}\033[0m") from e
```

### Comparing `openbb_core-1.2.2/openbb_core/provider/registry_map.py` & `openbb_core-1.2.3/openbb_core/provider/registry_map.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/ameribor_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/analyst_estimates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/analyst_search.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/available_indicators.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/available_indices.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/balance_of_payments.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/balance_of_payments.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,14 +11,93 @@
 from openbb_core.provider.abstract.query_params import QueryParams
 
 
 class BalanceOfPaymentsQueryParams(QueryParams):
     """Balance Of Payments Query."""
 
 
+class BP6BopUsdData(Data):
+    """OECD BP6 Balance of Payments Items, in USD."""
+
+    period: dateType = Field(
+        default=None,
+        description="The date representing the beginning of the reporting period.",
+    )
+    balance_percent_of_gdp: Optional[float] = Field(
+        default=None,
+        description="Current Account Balance as Percent of GDP",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
+    balance_total: Optional[float] = Field(
+        default=None, description="Current Account Total Balance (USD)"
+    )
+    balance_total_services: Optional[float] = Field(
+        default=None, description="Current Account Total Services Balance (USD)"
+    )
+    balance_total_secondary_income: Optional[float] = Field(
+        default=None, description="Current Account Total Secondary Income Balance (USD)"
+    )
+    balance_total_goods: Optional[float] = Field(
+        default=None, description="Current Account Total Goods Balance (USD)"
+    )
+    balance_total_primary_income: Optional[float] = Field(
+        default=None, description="Current Account Total Primary Income Balance (USD)"
+    )
+    credits_services_percent_of_goods_and_services: Optional[float] = Field(
+        default=None,
+        description="Current Account Credits Services as Percent of Goods and Services",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
+    credits_services_percent_of_current_account: Optional[float] = Field(
+        default=None,
+        description="Current Account Credits Services as Percent of Current Account",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
+    credits_total_services: Optional[float] = Field(
+        default=None, description="Current Account Credits Total Services (USD)"
+    )
+    credits_total_goods: Optional[float] = Field(
+        default=None, description="Current Account Credits Total Goods (USD)"
+    )
+    credits_total_primary_income: Optional[float] = Field(
+        default=None, description="Current Account Credits Total Primary Income (USD)"
+    )
+    credits_total_secondary_income: Optional[float] = Field(
+        default=None, description="Current Account Credits Total Secondary Income (USD)"
+    )
+    credits_total: Optional[float] = Field(
+        default=None, description="Current Account Credits Total (USD)"
+    )
+    debits_services_percent_of_goods_and_services: Optional[float] = Field(
+        default=None,
+        description="Current Account Debits Services as Percent of Goods and Services",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
+    debits_services_percent_of_current_account: Optional[float] = Field(
+        default=None,
+        description="Current Account Debits Services as Percent of Current Account",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
+    debits_total_services: Optional[float] = Field(
+        default=None, description="Current Account Debits Total Services (USD)"
+    )
+    debits_total_goods: Optional[float] = Field(
+        default=None, description="Current Account Debits Total Goods (USD)"
+    )
+    debits_total_primary_income: Optional[float] = Field(
+        default=None, description="Current Account Debits Total Primary Income (USD)"
+    )
+    debits_total: Optional[float] = Field(
+        default=None, description="Current Account Debits Total (USD)"
+    )
+    debits_total_secondary_income: Optional[float] = Field(
+        default=None, description="Current Account Debits Total Secondary Income (USD)"
+    )
+
+
 class ECBMain(Data):
     """ECB Main Balance of Payments Items."""
 
     period: dateType = Field(
         default=None,
         description="The date representing the beginning of the reporting period.",
     )
```

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/balance_sheet.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/balance_sheet_growth.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/bond_prices.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/bond_reference.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/bond_reference.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/bond_trades.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/bond_trades.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/calendar_dividend.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/calendar_earnings.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/calendar_ipo.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/calendar_splits.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/cash_flow.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/cash_flow_growth.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/cik_map.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/cik_map.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/company_filings.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/company_news.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/company_overview.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/compare_groups.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/composite_leading_indicator.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/cot.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/cot_search.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/country_profile.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/cp.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/cpi.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/crypto_historical.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/crypto_search.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/currency_historical.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/currency_pairs.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/currency_reference_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/currency_snapshots.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/discovery_filings.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/dwpcr_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/earnings_call_transcript.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/ecb_interest_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/economic_calendar.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/economic_indicators.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/economic_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_ftd.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_ftd.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_historical.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_info.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_nbbo.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_ownership.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_peers.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_performance.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_quote.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_screener.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_screener.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_search.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_short_interest.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/equity_valuation_multiples.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/esg_risk_rating.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/esg_risk_rating.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/esg_score.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/esg_score.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/esg_sector.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/esg_sector.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/estr_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_countries.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_equity_exposure.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_historical.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_historical_nav.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_historical_nav.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_holdings.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_holdings_date.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_info.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_performance.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_search.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/etf_sectors.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/eu_yield_curve.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/executive_compensation.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/fed_projections.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/fed_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/ffrmc.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/financial_attributes.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/financial_ratios.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/form_13FHR.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/form_13FHR.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/forward_eps_estimates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/forward_pe_estimates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/forward_pe_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/forward_sales_estimates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/fred_search.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/fred_search.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/fred_series.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/futures_curve.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/futures_historical.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/gdp_forecast.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/gdp_nominal.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/gdp_real.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/historical_attributes.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/historical_dividends.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/historical_employees.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/historical_eps.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/historical_splits.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/hqm.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/ice_bofa.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/income_statement.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/income_statement_growth.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/index_constituents.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/index_historical.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/index_info.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/index_info.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/index_search.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/index_sectors.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/index_snapshots.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/industry_pe.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/industry_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/insider_trading.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/institutional_ownership.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/iorb_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/key_executives.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/key_metrics.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/latest_attributes.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/lbma_fixing.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/long_term_interest_rate.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/market_indices.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/market_movers.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/market_movers.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/market_snapshots.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/money_measures.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/moody.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/options_chains.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/options_unusual.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/otc_aggregate.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/price_target.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/price_target_consensus.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/recent_performance.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/recent_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/reported_financials.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/revenue_business_line.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/revenue_geographic.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/risk_premium.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/search_attributes.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/search_financial_attributes.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/search_financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/sector_pe.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/sector_pe.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/share_statistics.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/short_term_interest_rate.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/short_volume.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/sofr_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/sonia_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/sp500_multiples.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/spot.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/tbffr.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/tmc.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/top_retail.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/trailing_dividend_yield.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/treasury_auctions.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/treasury_prices.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/treasury_rates.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/unemployment.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/upcoming_release_days.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/upcoming_release_days.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/us_yield_curve.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/standard_models/world_news.py` & `openbb_core-1.2.3/openbb_core/provider/standard_models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/utils/client.py` & `openbb_core-1.2.3/openbb_core/provider/utils/client.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/utils/descriptions.py` & `openbb_core-1.2.3/openbb_core/provider/utils/descriptions.py`

 * *Files identical despite different names*

### Comparing `openbb_core-1.2.2/openbb_core/provider/utils/helpers.py` & `openbb_core-1.2.3/openbb_core/provider/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Optional,
     TypeVar,
     Union,
     cast,
 )
 
 import requests
-from anyio import start_blocking_portal
+from anyio.from_thread import start_blocking_portal
 from typing_extensions import ParamSpec
 
 from openbb_core.provider.abstract.data import Data
 from openbb_core.provider.utils.client import (
     ClientResponse,
     ClientSession,
     get_user_agent,
```

### Comparing `openbb_core-1.2.2/pyproject.toml` & `openbb_core-1.2.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "openbb-core"
-version = "1.2.2"
-description = "OpenBB package with core functionality"
+version = "1.2.3"
+description = "OpenBB package with core functionality."
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_core" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -14,24 +14,17 @@
 pandas = ">=1.5.3"
 html5lib = "^1.1"
 fastapi = "^0.111.0"
 uuid7 = "^0.1.0"
 posthog = "^3.3.1"
 python-multipart = "^0.0.7"
 pydantic = "^2.5.1"
-requests = "^2.31.0"
+requests = "^2.32.1"
 importlib-metadata = "^6.8.0"
 python-dotenv = "^1.0.0"
 aiohttp = "^3.9.5"
-ruff = "^0.1.6"
+ruff = ">=0.1.6,<=0.4.4"  # Needed here to lint generated code
 pyjwt = "^2.8.0"
-anyio = "^3.7.0"  # TODO: Migrate to v4
-
-[tool.poetry.group.dev.dependencies]
-pytest = "^7.0.0"
-pytest-subtests = "^0.11.0"
-pytest-recorder = "^0.2.4"
-pytest-asyncio = "^0.23.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openbb_core-1.2.2/PKG-INFO` & `openbb_core-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: openbb-core
-Version: 1.2.2
-Summary: OpenBB package with core functionality
+Version: 1.2.3
+Summary: OpenBB package with core functionality.
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
-Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
 Requires-Dist: importlib-metadata (>=6.8.0,<7.0.0)
 Requires-Dist: pandas (>=1.5.3)
 Requires-Dist: posthog (>=3.3.1,<4.0.0)
 Requires-Dist: pydantic (>=2.5.1,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-multipart (>=0.0.7,<0.0.8)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: ruff (>=0.1.6,<0.2.0)
+Requires-Dist: requests (>=2.32.1,<3.0.0)
+Requires-Dist: ruff (>=0.1.6,<=0.4.4)
 Requires-Dist: uuid7 (>=0.1.0,<0.2.0)
 Requires-Dist: uvicorn (>=0.24,<0.25)
 Requires-Dist: websockets (>=12.0,<13.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Platform - Core
```

