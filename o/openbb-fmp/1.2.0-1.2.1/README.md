# Comparing `tmp/openbb_fmp-1.2.0.tar.gz` & `tmp/openbb_fmp-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fmp-1.2.0.tar", max compression
+gzip compressed data, was "openbb_fmp-1.2.1.tar", max compression
```

## Comparing `openbb_fmp-1.2.0.tar` & `openbb_fmp-1.2.1.tar`

### file list

```diff
@@ -1,72 +1,73 @@
--rw-r--r--   0        0        0      351 2024-05-15 14:25:41.787335 openbb_fmp-1.2.0/README.md
--rw-r--r--   0        0        0     9101 2024-05-14 15:30:05.613337 openbb_fmp-1.2.0/openbb_fmp/__init__.py
--rw-r--r--   0        0        0       28 2024-02-29 11:03:36.842842 openbb_fmp-1.2.0/openbb_fmp/models/__init__.py
--rw-r--r--   0        0        0     3086 2024-05-10 10:40:27.292197 openbb_fmp-1.2.0/openbb_fmp/models/analyst_estimates.py
--rw-r--r--   0        0        0     2141 2024-04-08 12:02:16.633618 openbb_fmp-1.2.0/openbb_fmp/models/available_indices.py
--rw-r--r--   0        0        0    11610 2024-04-08 12:02:16.633789 openbb_fmp-1.2.0/openbb_fmp/models/balance_sheet.py
--rw-r--r--   0        0        0     2228 2024-04-08 12:02:16.633907 openbb_fmp-1.2.0/openbb_fmp/models/balance_sheet_growth.py
--rw-r--r--   0        0        0     3383 2024-04-08 12:02:16.634020 openbb_fmp-1.2.0/openbb_fmp/models/calendar_dividend.py
--rw-r--r--   0        0        0     3818 2024-04-08 12:02:16.634152 openbb_fmp-1.2.0/openbb_fmp/models/calendar_earnings.py
--rw-r--r--   0        0        0     2282 2024-04-02 11:35:59.449553 openbb_fmp-1.2.0/openbb_fmp/models/calendar_splits.py
--rw-r--r--   0        0        0     9479 2024-04-08 12:02:16.634306 openbb_fmp-1.2.0/openbb_fmp/models/cash_flow.py
--rw-r--r--   0        0        0     2704 2024-04-08 12:02:16.634395 openbb_fmp-1.2.0/openbb_fmp/models/cash_flow_growth.py
--rw-r--r--   0        0        0     3017 2024-04-08 12:02:16.634510 openbb_fmp-1.2.0/openbb_fmp/models/company_filings.py
--rw-r--r--   0        0        0     2961 2024-05-10 10:40:27.292367 openbb_fmp-1.2.0/openbb_fmp/models/company_news.py
--rw-r--r--   0        0        0     2182 2024-04-02 11:35:59.450137 openbb_fmp-1.2.0/openbb_fmp/models/company_overview.py
--rw-r--r--   0        0        0     5908 2024-05-10 11:33:20.067768 openbb_fmp-1.2.0/openbb_fmp/models/crypto_historical.py
--rw-r--r--   0        0        0     3337 2024-04-08 12:02:16.634839 openbb_fmp-1.2.0/openbb_fmp/models/crypto_search.py
--rw-r--r--   0        0        0     5901 2024-05-10 11:33:20.067963 openbb_fmp-1.2.0/openbb_fmp/models/currency_historical.py
--rw-r--r--   0        0        0     3208 2024-05-09 15:04:29.070919 openbb_fmp-1.2.0/openbb_fmp/models/currency_pairs.py
--rw-r--r--   0        0        0     6082 2024-05-10 10:40:27.293022 openbb_fmp-1.2.0/openbb_fmp/models/currency_snapshots.py
--rw-r--r--   0        0        0     2502 2024-04-02 11:35:59.451189 openbb_fmp-1.2.0/openbb_fmp/models/discovery_filings.py
--rw-r--r--   0        0        0     2614 2024-04-08 12:02:16.635270 openbb_fmp-1.2.0/openbb_fmp/models/earnings_call_transcript.py
--rw-r--r--   0        0        0     5073 2024-05-14 15:30:05.613556 openbb_fmp-1.2.0/openbb_fmp/models/economic_calendar.py
--rw-r--r--   0        0        0     5924 2024-05-10 10:40:27.293165 openbb_fmp-1.2.0/openbb_fmp/models/equity_historical.py
--rw-r--r--   0        0        0     2434 2024-04-02 11:35:59.451669 openbb_fmp-1.2.0/openbb_fmp/models/equity_ownership.py
--rw-r--r--   0        0        0     1638 2024-04-08 12:02:16.635574 openbb_fmp-1.2.0/openbb_fmp/models/equity_peers.py
--rw-r--r--   0        0        0     6114 2024-05-10 10:40:27.293312 openbb_fmp-1.2.0/openbb_fmp/models/equity_profile.py
--rw-r--r--   0        0        0     5314 2024-05-10 10:40:27.293457 openbb_fmp-1.2.0/openbb_fmp/models/equity_quote.py
--rw-r--r--   0        0        0     6835 2024-04-02 11:35:59.452060 openbb_fmp-1.2.0/openbb_fmp/models/equity_screener.py
--rw-r--r--   0        0        0     6499 2024-05-10 10:40:27.293618 openbb_fmp-1.2.0/openbb_fmp/models/equity_valuation_multiples.py
--rw-r--r--   0        0        0     3452 2024-05-10 10:40:27.293766 openbb_fmp-1.2.0/openbb_fmp/models/etf_countries.py
--rw-r--r--   0        0        0     3162 2024-05-10 10:40:27.293941 openbb_fmp-1.2.0/openbb_fmp/models/etf_equity_exposure.py
--rw-r--r--   0        0        0     6772 2024-05-09 15:04:29.071085 openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings.py
--rw-r--r--   0        0        0     2117 2024-04-02 11:35:59.452710 openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings_date.py
--rw-r--r--   0        0        0     2780 2024-04-23 10:22:39.667379 openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings_performance.py
--rw-r--r--   0        0        0     3623 2024-05-10 10:40:27.294092 openbb_fmp-1.2.0/openbb_fmp/models/etf_info.py
--rw-r--r--   0        0        0     4491 2024-04-08 12:02:16.636814 openbb_fmp-1.2.0/openbb_fmp/models/etf_search.py
--rw-r--r--   0        0        0     1915 2024-04-02 11:35:59.453264 openbb_fmp-1.2.0/openbb_fmp/models/etf_sectors.py
--rw-r--r--   0        0        0     4304 2024-05-10 10:40:27.294266 openbb_fmp-1.2.0/openbb_fmp/models/executive_compensation.py
--rw-r--r--   0        0        0    10171 2024-04-08 12:02:16.637030 openbb_fmp-1.2.0/openbb_fmp/models/financial_ratios.py
--rw-r--r--   0        0        0     5056 2024-05-10 10:40:27.294412 openbb_fmp-1.2.0/openbb_fmp/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     3771 2024-04-08 12:02:16.637259 openbb_fmp-1.2.0/openbb_fmp/models/historical_dividends.py
--rw-r--r--   0        0        0     1839 2024-04-02 11:35:59.453743 openbb_fmp-1.2.0/openbb_fmp/models/historical_employees.py
--rw-r--r--   0        0        0     3362 2024-04-02 11:35:59.453824 openbb_fmp-1.2.0/openbb_fmp/models/historical_eps.py
--rw-r--r--   0        0        0     2154 2024-04-02 11:35:59.453905 openbb_fmp-1.2.0/openbb_fmp/models/historical_splits.py
--rw-r--r--   0        0        0     8720 2024-04-08 12:02:16.637445 openbb_fmp-1.2.0/openbb_fmp/models/income_statement.py
--rw-r--r--   0        0        0     2440 2024-04-02 11:35:59.454171 openbb_fmp-1.2.0/openbb_fmp/models/income_statement_growth.py
--rw-r--r--   0        0        0     4170 2024-04-08 12:02:16.637552 openbb_fmp-1.2.0/openbb_fmp/models/index_constituents.py
--rw-r--r--   0        0        0     5832 2024-05-10 10:40:27.294557 openbb_fmp-1.2.0/openbb_fmp/models/index_historical.py
--rw-r--r--   0        0        0     3291 2024-04-02 11:35:59.454433 openbb_fmp-1.2.0/openbb_fmp/models/insider_trading.py
--rw-r--r--   0        0        0     6345 2024-04-02 11:35:59.454534 openbb_fmp-1.2.0/openbb_fmp/models/institutional_ownership.py
--rw-r--r--   0        0        0     2270 2024-04-23 10:22:39.667606 openbb_fmp-1.2.0/openbb_fmp/models/key_executives.py
--rw-r--r--   0        0        0    10619 2024-05-10 10:40:27.294661 openbb_fmp-1.2.0/openbb_fmp/models/key_metrics.py
--rw-r--r--   0        0        0     3938 2024-04-23 10:22:39.667724 openbb_fmp-1.2.0/openbb_fmp/models/market_indices.py
--rw-r--r--   0        0        0     6297 2024-04-23 10:22:39.667856 openbb_fmp-1.2.0/openbb_fmp/models/market_snapshots.py
--rw-r--r--   0        0        0     3527 2024-05-10 10:40:27.294808 openbb_fmp-1.2.0/openbb_fmp/models/price_performance.py
--rw-r--r--   0        0        0     4238 2024-05-10 10:40:27.295370 openbb_fmp-1.2.0/openbb_fmp/models/price_target.py
--rw-r--r--   0        0        0     3276 2024-05-10 10:40:27.295527 openbb_fmp-1.2.0/openbb_fmp/models/price_target_consensus.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847376 openbb_fmp-1.2.0/openbb_fmp/models/py.typed
--rw-r--r--   0        0        0     3278 2024-04-08 12:02:16.638378 openbb_fmp-1.2.0/openbb_fmp/models/revenue_business_line.py
--rw-r--r--   0        0        0     3243 2024-04-08 12:02:16.638491 openbb_fmp-1.2.0/openbb_fmp/models/revenue_geographic.py
--rw-r--r--   0        0        0     1657 2024-04-02 11:35:59.455545 openbb_fmp-1.2.0/openbb_fmp/models/risk_premium.py
--rw-r--r--   0        0        0     2135 2024-04-02 11:35:59.455637 openbb_fmp-1.2.0/openbb_fmp/models/share_statistics.py
--rw-r--r--   0        0        0     3861 2024-04-08 12:02:16.638589 openbb_fmp-1.2.0/openbb_fmp/models/treasury_rates.py
--rw-r--r--   0        0        0     2866 2024-04-08 12:02:16.638702 openbb_fmp-1.2.0/openbb_fmp/models/world_news.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.847941 openbb_fmp-1.2.0/openbb_fmp/py.typed
--rw-r--r--   0        0        0       17 2024-04-23 10:22:39.668253 openbb_fmp-1.2.0/openbb_fmp/utils/__init__.py
--rw-r--r--   0        0        0     2580 2024-04-08 12:02:16.638823 openbb_fmp-1.2.0/openbb_fmp/utils/definitions.py
--rw-r--r--   0        0        0     4246 2024-04-23 10:22:39.668404 openbb_fmp-1.2.0/openbb_fmp/utils/helpers.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.848164 openbb_fmp-1.2.0/openbb_fmp/utils/py.typed
--rw-r--r--   0        0        0      459 2024-05-15 16:06:42.123564 openbb_fmp-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 openbb_fmp-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      351 2024-05-22 11:48:40.527330 openbb_fmp-1.2.1/README.md
+-rw-r--r--   0        0        0     9208 2024-05-22 11:48:40.527330 openbb_fmp-1.2.1/openbb_fmp/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-15 09:21:56.069885 openbb_fmp-1.2.1/openbb_fmp/models/analyst_estimates.py
+-rw-r--r--   0        0        0     2141 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/available_indices.py
+-rw-r--r--   0        0        0    11610 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/balance_sheet.py
+-rw-r--r--   0        0        0     2228 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/balance_sheet_growth.py
+-rw-r--r--   0        0        0     3383 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/calendar_dividend.py
+-rw-r--r--   0        0        0     3818 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/calendar_earnings.py
+-rw-r--r--   0        0        0     2282 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/calendar_splits.py
+-rw-r--r--   0        0        0     9479 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/cash_flow.py
+-rw-r--r--   0        0        0     2704 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/cash_flow_growth.py
+-rw-r--r--   0        0        0     3017 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/company_filings.py
+-rw-r--r--   0        0        0     2961 2024-05-15 09:21:56.069885 openbb_fmp-1.2.1/openbb_fmp/models/company_news.py
+-rw-r--r--   0        0        0     2182 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/company_overview.py
+-rw-r--r--   0        0        0     5908 2024-05-15 09:21:56.069885 openbb_fmp-1.2.1/openbb_fmp/models/crypto_historical.py
+-rw-r--r--   0        0        0     3337 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/crypto_search.py
+-rw-r--r--   0        0        0     5901 2024-05-15 09:21:56.069885 openbb_fmp-1.2.1/openbb_fmp/models/currency_historical.py
+-rw-r--r--   0        0        0     3208 2024-05-15 09:21:56.069885 openbb_fmp-1.2.1/openbb_fmp/models/currency_pairs.py
+-rw-r--r--   0        0        0     6082 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/currency_snapshots.py
+-rw-r--r--   0        0        0     2502 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/discovery_filings.py
+-rw-r--r--   0        0        0     2614 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/earnings_call_transcript.py
+-rw-r--r--   0        0        0     5073 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/economic_calendar.py
+-rw-r--r--   0        0        0     5924 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/equity_historical.py
+-rw-r--r--   0        0        0     2434 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/equity_ownership.py
+-rw-r--r--   0        0        0     1638 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/equity_peers.py
+-rw-r--r--   0        0        0     6114 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/equity_profile.py
+-rw-r--r--   0        0        0     5314 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/equity_quote.py
+-rw-r--r--   0        0        0     7149 2024-05-22 11:48:40.527330 openbb_fmp-1.2.1/openbb_fmp/models/equity_screener.py
+-rw-r--r--   0        0        0     6499 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/equity_valuation_multiples.py
+-rw-r--r--   0        0        0     3452 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/etf_countries.py
+-rw-r--r--   0        0        0     3162 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/etf_equity_exposure.py
+-rw-r--r--   0        0        0     6772 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/etf_holdings.py
+-rw-r--r--   0        0        0     2117 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/etf_holdings_date.py
+-rw-r--r--   0        0        0     3623 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/etf_info.py
+-rw-r--r--   0        0        0     4491 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/etf_search.py
+-rw-r--r--   0        0        0     1915 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/etf_sectors.py
+-rw-r--r--   0        0        0     4304 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/executive_compensation.py
+-rw-r--r--   0        0        0    10171 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/financial_ratios.py
+-rw-r--r--   0        0        0     5025 2024-05-22 11:48:40.527330 openbb_fmp-1.2.1/openbb_fmp/models/forward_ebitda_estimates.py
+-rw-r--r--   0        0        0     5056 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     3771 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/historical_dividends.py
+-rw-r--r--   0        0        0     1839 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/historical_employees.py
+-rw-r--r--   0        0        0     3362 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/historical_eps.py
+-rw-r--r--   0        0        0     2154 2024-05-14 16:56:41.861864 openbb_fmp-1.2.1/openbb_fmp/models/historical_splits.py
+-rw-r--r--   0        0        0     8720 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/income_statement.py
+-rw-r--r--   0        0        0     2440 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/income_statement_growth.py
+-rw-r--r--   0        0        0     4170 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/index_constituents.py
+-rw-r--r--   0        0        0     5832 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/index_historical.py
+-rw-r--r--   0        0        0     3336 2024-05-22 11:48:40.527330 openbb_fmp-1.2.1/openbb_fmp/models/insider_trading.py
+-rw-r--r--   0        0        0     6345 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/institutional_ownership.py
+-rw-r--r--   0        0        0     2270 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/key_executives.py
+-rw-r--r--   0        0        0    12212 2024-05-22 11:48:40.527330 openbb_fmp-1.2.1/openbb_fmp/models/key_metrics.py
+-rw-r--r--   0        0        0     3938 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/market_indices.py
+-rw-r--r--   0        0        0     6297 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/market_snapshots.py
+-rw-r--r--   0        0        0     3527 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/price_performance.py
+-rw-r--r--   0        0        0     4238 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/price_target.py
+-rw-r--r--   0        0        0     3276 2024-05-15 09:21:56.073885 openbb_fmp-1.2.1/openbb_fmp/models/price_target_consensus.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/py.typed
+-rw-r--r--   0        0        0     3278 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/revenue_business_line.py
+-rw-r--r--   0        0        0     3243 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/revenue_geographic.py
+-rw-r--r--   0        0        0     1657 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/risk_premium.py
+-rw-r--r--   0        0        0     2135 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/share_statistics.py
+-rw-r--r--   0        0        0     3861 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/treasury_rates.py
+-rw-r--r--   0        0        0     2866 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/models/world_news.py
+-rw-r--r--   0        0        0     4305 2024-05-22 11:48:40.527330 openbb_fmp-1.2.1/openbb_fmp/models/yield_curve.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/py.typed
+-rw-r--r--   0        0        0       17 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/utils/__init__.py
+-rw-r--r--   0        0        0     2570 2024-05-22 11:48:40.527330 openbb_fmp-1.2.1/openbb_fmp/utils/definitions.py
+-rw-r--r--   0        0        0     4246 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/utils/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.865864 openbb_fmp-1.2.1/openbb_fmp/utils/py.typed
+-rw-r--r--   0        0        0      459 2024-05-22 13:57:14.871822 openbb_fmp-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 openbb_fmp-1.2.1/PKG-INFO
```

### Comparing `openbb_fmp-1.2.0/openbb_fmp/__init__.py` & `openbb_fmp-1.2.1/openbb_fmp/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,20 @@
 from openbb_fmp.models.equity_valuation_multiples import (
     FMPEquityValuationMultiplesFetcher,
 )
 from openbb_fmp.models.etf_countries import FMPEtfCountriesFetcher
 from openbb_fmp.models.etf_equity_exposure import FMPEtfEquityExposureFetcher
 from openbb_fmp.models.etf_holdings import FMPEtfHoldingsFetcher
 from openbb_fmp.models.etf_holdings_date import FMPEtfHoldingsDateFetcher
-from openbb_fmp.models.etf_holdings_performance import FMPEtfHoldingsPerformanceFetcher
 from openbb_fmp.models.etf_info import FMPEtfInfoFetcher
 from openbb_fmp.models.etf_search import FMPEtfSearchFetcher
 from openbb_fmp.models.etf_sectors import FMPEtfSectorsFetcher
 from openbb_fmp.models.executive_compensation import FMPExecutiveCompensationFetcher
 from openbb_fmp.models.financial_ratios import FMPFinancialRatiosFetcher
+from openbb_fmp.models.forward_ebitda_estimates import FMPForwardEbitdaEstimatesFetcher
 from openbb_fmp.models.forward_eps_estimates import FMPForwardEpsEstimatesFetcher
 from openbb_fmp.models.historical_dividends import FMPHistoricalDividendsFetcher
 from openbb_fmp.models.historical_employees import FMPHistoricalEmployeesFetcher
 from openbb_fmp.models.historical_eps import FMPHistoricalEpsFetcher
 from openbb_fmp.models.historical_splits import FMPHistoricalSplitsFetcher
 from openbb_fmp.models.income_statement import FMPIncomeStatementFetcher
 from openbb_fmp.models.income_statement_growth import FMPIncomeStatementGrowthFetcher
@@ -59,14 +59,15 @@
 from openbb_fmp.models.price_target_consensus import FMPPriceTargetConsensusFetcher
 from openbb_fmp.models.revenue_business_line import FMPRevenueBusinessLineFetcher
 from openbb_fmp.models.revenue_geographic import FMPRevenueGeographicFetcher
 from openbb_fmp.models.risk_premium import FMPRiskPremiumFetcher
 from openbb_fmp.models.share_statistics import FMPShareStatisticsFetcher
 from openbb_fmp.models.treasury_rates import FMPTreasuryRatesFetcher
 from openbb_fmp.models.world_news import FMPWorldNewsFetcher
+from openbb_fmp.models.yield_curve import FMPYieldCurveFetcher
 
 fmp_provider = Provider(
     name="fmp",
     website="https://financialmodelingprep.com",
     description="""Financial Modeling Prep is a new concept that informs you about
 stock market information (news, currencies, and stock prices).""",
     credentials=["api_key"],
@@ -98,21 +99,21 @@
         "EquityQuote": FMPEquityQuoteFetcher,
         "EquityScreener": FMPEquityScreenerFetcher,
         "EquityValuationMultiples": FMPEquityValuationMultiplesFetcher,
         "EtfCountries": FMPEtfCountriesFetcher,
         "EtfEquityExposure": FMPEtfEquityExposureFetcher,
         "EtfHoldings": FMPEtfHoldingsFetcher,
         "EtfHoldingsDate": FMPEtfHoldingsDateFetcher,
-        "EtfHoldingsPerformance": FMPEtfHoldingsPerformanceFetcher,
         "EtfInfo": FMPEtfInfoFetcher,
         "EtfPricePerformance": FMPPricePerformanceFetcher,
         "EtfSearch": FMPEtfSearchFetcher,
         "EtfSectors": FMPEtfSectorsFetcher,
         "ExecutiveCompensation": FMPExecutiveCompensationFetcher,
         "FinancialRatios": FMPFinancialRatiosFetcher,
+        "ForwardEbitdaEstimates": FMPForwardEbitdaEstimatesFetcher,
         "ForwardEpsEstimates": FMPForwardEpsEstimatesFetcher,
         "HistoricalDividends": FMPHistoricalDividendsFetcher,
         "HistoricalEmployees": FMPHistoricalEmployeesFetcher,
         "HistoricalEps": FMPHistoricalEpsFetcher,
         "HistoricalSplits": FMPHistoricalSplitsFetcher,
         "IncomeStatement": FMPIncomeStatementFetcher,
         "IncomeStatementGrowth": FMPIncomeStatementGrowthFetcher,
@@ -130,12 +131,13 @@
         "RevenueBusinessLine": FMPRevenueBusinessLineFetcher,
         "RevenueGeographic": FMPRevenueGeographicFetcher,
         "RiskPremium": FMPRiskPremiumFetcher,
         "ShareStatistics": FMPShareStatisticsFetcher,
         "TreasuryRates": FMPTreasuryRatesFetcher,
         "WorldNews": FMPWorldNewsFetcher,
         "EtfHistorical": FMPEquityHistoricalFetcher,
+        "YieldCurve": FMPYieldCurveFetcher,
     },
     repr_name="Financial Modeling Prep (FMP)",
     v3_credentials=["API_KEY_FINANCIALMODELINGPREP"],
     instructions='Go to: https://site.financialmodelingprep.com/developer/docs\n\n![FinancialModelingPrep](https://user-images.githubusercontent.com/46355364/207821920-64553d05-d461-4984-b0fe-be0368c71186.png)\n\nClick on, "Get my API KEY here", and sign up for a free account.\n\n![FinancialModelingPrep](https://user-images.githubusercontent.com/46355364/207822184-a723092e-ef42-4f87-8c55-db150f09741b.png)\n\nWith an account created, sign in and navigate to the Dashboard, which shows the assigned token. by pressing the "Dashboard" button which will show the API key.\n\n![FinancialModelingPrep](https://user-images.githubusercontent.com/46355364/207823170-dd8191db-e125-44e5-b4f3-2df0e115c91d.png)',  # noqa: E501  pylint: disable=line-too-long
 )
```

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/analyst_estimates.py` & `openbb_fmp-1.2.1/openbb_fmp/models/analyst_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/available_indices.py` & `openbb_fmp-1.2.1/openbb_fmp/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/balance_sheet.py` & `openbb_fmp-1.2.1/openbb_fmp/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/balance_sheet_growth.py` & `openbb_fmp-1.2.1/openbb_fmp/models/balance_sheet_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/calendar_dividend.py` & `openbb_fmp-1.2.1/openbb_fmp/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/calendar_earnings.py` & `openbb_fmp-1.2.1/openbb_fmp/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/calendar_splits.py` & `openbb_fmp-1.2.1/openbb_fmp/models/calendar_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/cash_flow.py` & `openbb_fmp-1.2.1/openbb_fmp/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/cash_flow_growth.py` & `openbb_fmp-1.2.1/openbb_fmp/models/cash_flow_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/company_filings.py` & `openbb_fmp-1.2.1/openbb_fmp/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/company_news.py` & `openbb_fmp-1.2.1/openbb_fmp/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/company_overview.py` & `openbb_fmp-1.2.1/openbb_fmp/models/company_overview.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/crypto_historical.py` & `openbb_fmp-1.2.1/openbb_fmp/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/crypto_search.py` & `openbb_fmp-1.2.1/openbb_fmp/models/crypto_search.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/currency_historical.py` & `openbb_fmp-1.2.1/openbb_fmp/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/currency_pairs.py` & `openbb_fmp-1.2.1/openbb_fmp/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/currency_snapshots.py` & `openbb_fmp-1.2.1/openbb_fmp/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/discovery_filings.py` & `openbb_fmp-1.2.1/openbb_fmp/models/discovery_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/earnings_call_transcript.py` & `openbb_fmp-1.2.1/openbb_fmp/models/earnings_call_transcript.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/economic_calendar.py` & `openbb_fmp-1.2.1/openbb_fmp/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/equity_historical.py` & `openbb_fmp-1.2.1/openbb_fmp/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/equity_ownership.py` & `openbb_fmp-1.2.1/openbb_fmp/models/equity_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/equity_peers.py` & `openbb_fmp-1.2.1/openbb_fmp/models/equity_peers.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/equity_profile.py` & `openbb_fmp-1.2.1/openbb_fmp/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/equity_quote.py` & `openbb_fmp-1.2.1/openbb_fmp/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/equity_screener.py` & `openbb_fmp-1.2.1/openbb_fmp/models/equity_screener.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """FMP Equity Screener Model."""
 
+# pylint: disable=unused-argument
+from copy import deepcopy
 from typing import Any, Dict, List, Literal, Optional
 
 import pandas as pd
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.equity_screener import (
     EquityScreenerData,
     EquityScreenerQueryParams,
 )
+from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_fmp.utils.definitions import EXCHANGES, SECTORS
 from openbb_fmp.utils.helpers import create_url, get_data
 from pydantic import Field
 
 
 class FMPEquityScreenerQueryParams(EquityScreenerQueryParams):
     """FMP Equity Screener Query."""
@@ -158,31 +161,34 @@
     async def aextract_data(
         query: FMPEquityScreenerQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
+        _query = deepcopy(query)
+        if _query.sector is not None:
+            _query.sector = _query.sector.replace("_", " ").title()
         url = create_url(
             version=3,
             endpoint="stock-screener",
             api_key=api_key,
-            query=query,
+            query=_query,
             exclude=["query", "is_symbol", "industry"],
         ).replace(" ", "%20")
-        return await get_data(url, **kwargs)
+        return await get_data(url, **kwargs)  # type: ignore
 
     @staticmethod
     def transform_data(
         query: FMPEquityScreenerQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPEquityScreenerData]:
         """Return the transformed data."""
+        if not data:
+            raise EmptyDataError("The request was returned empty.")
         results = pd.DataFrame(data)
-        if len(results) == 0:
-            return []
         if query.industry:
             results = results[
                 results["sector"].str.contains(query.industry, case=False)
                 | results["industry"].str.contains(query.industry, case=False)
             ]
         results["companyName"] = results["companyName"].fillna("-").replace("-", "")
         for col in results:
```

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/equity_valuation_multiples.py` & `openbb_fmp-1.2.1/openbb_fmp/models/equity_valuation_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/etf_countries.py` & `openbb_fmp-1.2.1/openbb_fmp/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/etf_equity_exposure.py` & `openbb_fmp-1.2.1/openbb_fmp/models/etf_equity_exposure.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings.py` & `openbb_fmp-1.2.1/openbb_fmp/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings_date.py` & `openbb_fmp-1.2.1/openbb_fmp/models/etf_holdings_date.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/etf_holdings_performance.py` & `openbb_fmp-1.2.1/openbb_fmp/models/key_executives.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,72 @@
-"""FMP ETF Holdings Performance Model."""
+"""FMP Key Executives Model."""
 
 # pylint: disable=unused-argument
 
-from typing import Any, Dict, List, Optional
+from datetime import (
+    date as dateType,
+)
+from typing import Any, Dict, List, Optional, Union
 
 from openbb_core.provider.abstract.fetcher import Fetcher
-from openbb_fmp.models.etf_holdings import FMPEtfHoldingsFetcher
-from openbb_fmp.models.price_performance import (
-    FMPPricePerformanceData,
-    FMPPricePerformanceFetcher,
-    FMPPricePerformanceQueryParams,
+from openbb_core.provider.standard_models.key_executives import (
+    KeyExecutivesData,
+    KeyExecutivesQueryParams,
 )
-from pandas import DataFrame
+from openbb_core.provider.utils.helpers import safe_fromtimestamp
+from openbb_fmp.utils.helpers import get_data_many
+from pydantic import field_validator
+
+
+class FMPKeyExecutivesQueryParams(KeyExecutivesQueryParams):
+    """FMP Key Executives Query.
 
+    Source: https://financialmodelingprep.com/developer/docs/#Key-Executives
+    """
 
-class FMPEtfHoldingsPerformanceQueryParams(FMPPricePerformanceQueryParams):
-    """FMP ETF Holdings Performance Query."""
 
+class FMPKeyExecutivesData(KeyExecutivesData):
+    """FMP Key Executives Data."""
 
-class FMPEtfHoldingsPerformanceData(FMPPricePerformanceData):
-    """FMP ETF Holdings Performance Data."""
+    @field_validator("titleSince", mode="before", check_fields=False)
+    @classmethod
+    def time_validate(cls, v: Union[float, int]) -> Optional[dateType]:
+        """Return the date as a datetime object."""
+        if v:
+            v = v / 1000
+            return safe_fromtimestamp(v)
+        return v  # type: ignore
 
 
-class FMPEtfHoldingsPerformanceFetcher(
+class FMPKeyExecutivesFetcher(
     Fetcher[
-        FMPEtfHoldingsPerformanceQueryParams,
-        List[FMPEtfHoldingsPerformanceData],
+        FMPKeyExecutivesQueryParams,
+        List[FMPKeyExecutivesData],
     ]
 ):
     """Transform the query, extract and transform the data from the FMP endpoints."""
 
     @staticmethod
-    def transform_query(params: Dict[str, Any]) -> FMPEtfHoldingsPerformanceQueryParams:
-        """Transform the query."""
-        return FMPEtfHoldingsPerformanceQueryParams(**params)
+    def transform_query(params: Dict[str, Any]) -> FMPKeyExecutivesQueryParams:
+        """Transform the query params."""
+        return FMPKeyExecutivesQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
-        query: FMPEtfHoldingsPerformanceQueryParams,
+        query: FMPKeyExecutivesQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
-        # Get the holdings data
-        holdings = await FMPEtfHoldingsFetcher().aextract_data(
-            FMPEtfHoldingsFetcher.transform_query({"symbol": query.symbol}),
-            credentials,
-            **kwargs,
-        )
-        if holdings is None:
-            raise RuntimeError(f"No holdings data found for {query.symbol}.")
-        holdings_list = DataFrame(holdings).asset.unique().tolist()
-        # Split into chunks of 500
-        chunks = [holdings_list[i : i + 500] for i in range(0, len(holdings_list), 500)]
-        # Get price performance for the holdings
-        holdings_performance: List[Dict] = []
-        for holding_chunk in chunks:
-            holdings_str = (
-                ",".join(holding_chunk) if len(holding_chunk) > 1 else holding_chunk[0]
-            )
-            _performance = await FMPPricePerformanceFetcher().aextract_data(
-                FMPPricePerformanceFetcher.transform_query({"symbol": holdings_str}),
-                credentials,
-                **kwargs,
-            )
-            holdings_performance.extend(_performance)
-        return holdings_performance
+        api_key = credentials.get("fmp_api_key") if credentials else ""
+
+        base_url = "https://financialmodelingprep.com/api/v3"
+        url = f"{base_url}/key-executives/{query.symbol}?apikey={api_key}"
+
+        return await get_data_many(url, **kwargs)
 
     @staticmethod
     def transform_data(
-        query: FMPEtfHoldingsPerformanceQueryParams,
-        data: List[Dict],
-        **kwargs: Any,
-    ) -> List[FMPEtfHoldingsPerformanceData]:
+        query: FMPKeyExecutivesQueryParams, data: List[Dict], **kwargs: Any
+    ) -> List[FMPKeyExecutivesData]:
         """Return the transformed data."""
-        return [FMPEtfHoldingsPerformanceData.model_validate(d) for d in data]
+        return [FMPKeyExecutivesData.model_validate(d) for d in data]
```

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/etf_info.py` & `openbb_fmp-1.2.1/openbb_fmp/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/etf_search.py` & `openbb_fmp-1.2.1/openbb_fmp/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/etf_sectors.py` & `openbb_fmp-1.2.1/openbb_fmp/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/executive_compensation.py` & `openbb_fmp-1.2.1/openbb_fmp/models/executive_compensation.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/financial_ratios.py` & `openbb_fmp-1.2.1/openbb_fmp/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/forward_eps_estimates.py` & `openbb_fmp-1.2.1/openbb_fmp/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/historical_dividends.py` & `openbb_fmp-1.2.1/openbb_fmp/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/historical_employees.py` & `openbb_fmp-1.2.1/openbb_fmp/models/historical_employees.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/historical_eps.py` & `openbb_fmp-1.2.1/openbb_fmp/models/historical_eps.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/historical_splits.py` & `openbb_fmp-1.2.1/openbb_fmp/models/historical_splits.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/income_statement.py` & `openbb_fmp-1.2.1/openbb_fmp/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/income_statement_growth.py` & `openbb_fmp-1.2.1/openbb_fmp/models/income_statement_growth.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/index_constituents.py` & `openbb_fmp-1.2.1/openbb_fmp/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/index_historical.py` & `openbb_fmp-1.2.1/openbb_fmp/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/insider_trading.py` & `openbb_fmp-1.2.1/openbb_fmp/models/insider_trading.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """FMP Insider Trading Model."""
 
+# pylint: disable=unused-argument
+
 import math
 from typing import Any, Dict, List, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.insider_trading import (
     InsiderTradingData,
     InsiderTradingQueryParams,
@@ -15,15 +17,15 @@
 
 class FMPInsiderTradingQueryParams(InsiderTradingQueryParams):
     """FMP Insider Trading Query.
 
     Source: https://site.financialmodelingprep.com/developer/docs/#Stock-Insider-Trading
     """
 
-    transaction_type: TRANSACTION_TYPES = Field(
+    transaction_type: Optional[TRANSACTION_TYPES] = Field(
         default=None,
         description="Type of the transaction.",
         alias="transactionType",
     )
 
     @model_validator(mode="after")
     @classmethod
```

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/institutional_ownership.py` & `openbb_fmp-1.2.1/openbb_fmp/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/key_metrics.py` & `openbb_fmp-1.2.1/openbb_fmp/models/key_metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """FMP Key Metrics Model."""
 
+# pylint: disable=unused-argument
+
 import asyncio
 from datetime import (
     date as dateType,
     datetime,
 )
 from typing import Any, Dict, List, Optional
 from warnings import warn
 
 from openbb_core.provider.abstract.data import ForceInt
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.key_metrics import (
     KeyMetricsData,
     KeyMetricsQueryParams,
 )
-from openbb_core.provider.utils.descriptions import DATA_DESCRIPTIONS
 from openbb_core.provider.utils.errors import EmptyDataError
 from openbb_core.provider.utils.helpers import amake_request
 from openbb_fmp.utils.helpers import response_callback
 from pydantic import Field
 
 
 class FMPKeyMetricsQueryParams(KeyMetricsQueryParams):
@@ -33,22 +34,32 @@
         default=False, description="Include trailing twelve months (TTM) data."
     )
 
 
 class FMPKeyMetricsData(KeyMetricsData):
     """FMP Key Metrics Data."""
 
-    date: dateType = Field(description=DATA_DESCRIPTIONS.get("date", ""))
-    period: str = Field(description="Period of the data.")
+    __alias_dict__ = {
+        "dividend_yield": "dividend_yiel",
+        "market_cap": "marketCap",
+        "research_and_development_to_revenue": "researchAndDevelopementToRevenue",
+        "fiscal_period": "period",
+        "period_ending": "date",
+    }
+    period_ending: dateType = Field(description="Period ending date.")
+    fiscal_period: str = Field(description="Period of the data.")
     calendar_year: Optional[ForceInt] = Field(
-        default=None, description="Calendar year."
+        default=None, description="Calendar year for the fiscal period."
     )
     revenue_per_share: Optional[float] = Field(
         default=None, description="Revenue per share"
     )
+    capex_per_share: Optional[float] = Field(
+        default=None, description="Capital expenditures per share"
+    )
     net_income_per_share: Optional[float] = Field(
         default=None, description="Net income per share"
     )
     operating_cash_flow_per_share: Optional[float] = Field(
         default=None, description="Operating cash flow per share"
     )
     free_cash_flow_per_share: Optional[float] = Field(
@@ -63,49 +74,67 @@
     )
     shareholders_equity_per_share: Optional[float] = Field(
         default=None, description="Shareholders equity per share"
     )
     interest_debt_per_share: Optional[float] = Field(
         default=None, description="Interest debt per share"
     )
-    enterprise_value: Optional[float] = Field(
-        default=None, description="Enterprise value"
-    )
-    price_to_sales_ratio: Optional[float] = Field(
-        default=None, description="Price-to-sales ratio"
+    price_to_sales: Optional[float] = Field(
+        default=None,
+        description="Price-to-sales ratio",
+        alias="priceToSalesRatio",
     )
-    pocf_ratio: Optional[float] = Field(
+    price_to_operating_cash_flow: Optional[float] = Field(
         default=None,
         description="Price-to-operating cash flow ratio",
         alias="pocfratio",
     )
-    pfcf_ratio: Optional[float] = Field(
-        default=None, description="Price-to-free cash flow ratio"
+    price_to_free_cash_flow: Optional[float] = Field(
+        default=None,
+        description="Price-to-free cash flow ratio",
+        alias="pfcfRatio",
+    )
+    price_to_book: Optional[float] = Field(
+        default=None,
+        description="Price-to-book ratio",
+        alias="pbRatio",
     )
-    pb_ratio: Optional[float] = Field(default=None, description="Price-to-book ratio")
-    ptb_ratio: Optional[float] = Field(
-        default=None, description="Price-to-tangible book ratio"
+    price_to_tangible_book: Optional[float] = Field(
+        default=None,
+        description="Price-to-tangible book ratio",
+        alias="ptbRatio",
     )
     ev_to_sales: Optional[float] = Field(
-        default=None, description="Enterprise value-to-sales ratio"
+        default=None,
+        description="Enterprise value-to-sales ratio",
+        alias="evToSales",
     )
-    enterprise_value_over_ebitda: Optional[float] = Field(
+    ev_to_ebitda: Optional[float] = Field(
         default=None,
         description="Enterprise value-to-EBITDA ratio",
         alias="enterpriseValueOverEBITDA",
     )
     ev_to_operating_cash_flow: Optional[float] = Field(
         default=None, description="Enterprise value-to-operating cash flow ratio"
     )
     ev_to_free_cash_flow: Optional[float] = Field(
         default=None, description="Enterprise value-to-free cash flow ratio"
     )
-    earnings_yield: Optional[float] = Field(default=None, description="Earnings yield")
+    earnings_yield: Optional[float] = Field(
+        default=None,
+        description="Earnings yield",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
     free_cash_flow_yield: Optional[float] = Field(
-        default=None, description="Free cash flow yield"
+        default=None,
+        description="Free cash flow yield",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
+    debt_to_market_cap: Optional[float] = Field(
+        default=None, description="Debt-to-market capitalization ratio"
     )
     debt_to_equity: Optional[float] = Field(
         default=None, description="Debt-to-equity ratio"
     )
     debt_to_assets: Optional[float] = Field(
         default=None, description="Debt-to-assets ratio"
     )
@@ -115,19 +144,14 @@
         alias="netDebtToEBITDA",
     )
     current_ratio: Optional[float] = Field(default=None, description="Current ratio")
     interest_coverage: Optional[float] = Field(
         default=None, description="Interest coverage"
     )
     income_quality: Optional[float] = Field(default=None, description="Income quality")
-    dividend_yield: Optional[float] = Field(
-        default=None,
-        description="Dividend yield, as a normalized percent.",
-        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
-    )
     payout_ratio: Optional[float] = Field(default=None, description="Payout ratio")
     sales_general_and_administrative_to_revenue: Optional[float] = Field(
         default=None,
         description="Sales general and administrative expenses-to-revenue ratio",
     )
     research_and_development_to_revenue: Optional[float] = Field(
         default=None,
@@ -145,33 +169,26 @@
     )
     capex_to_depreciation: Optional[float] = Field(
         default=None, description="Capital expenditures-to-depreciation ratio"
     )
     stock_based_compensation_to_revenue: Optional[float] = Field(
         default=None, description="Stock-based compensation-to-revenue ratio"
     )
-    graham_number: Optional[float] = Field(default=None, description="Graham number")
-    roic: Optional[float] = Field(
-        default=None, description="Return on invested capital"
-    )
-    return_on_tangible_assets: Optional[float] = Field(
-        default=None, description="Return on tangible assets"
-    )
-    graham_net_net: Optional[float] = Field(
-        default=None, description="Graham net-net working capital"
-    )
     working_capital: Optional[float] = Field(
         default=None, description="Working capital"
     )
     tangible_asset_value: Optional[float] = Field(
         default=None, description="Tangible asset value"
     )
     net_current_asset_value: Optional[float] = Field(
         default=None, description="Net current asset value"
     )
+    enterprise_value: Optional[float] = Field(
+        default=None, description="Enterprise value"
+    )
     invested_capital: Optional[float] = Field(
         default=None, description="Invested capital"
     )
     average_receivables: Optional[float] = Field(
         default=None, description="Average receivables"
     )
     average_payables: Optional[float] = Field(
@@ -194,27 +211,50 @@
     )
     payables_turnover: Optional[float] = Field(
         default=None, description="Payables turnover"
     )
     inventory_turnover: Optional[float] = Field(
         default=None, description="Inventory turnover"
     )
-    roe: Optional[float] = Field(default=None, description="Return on equity")
-    capex_per_share: Optional[float] = Field(
-        default=None, description="Capital expenditures per share"
+    return_on_equity: Optional[float] = Field(
+        default=None,
+        description="Return on equity",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+        alias="roe",
+    )
+    return_on_invested_capital: Optional[float] = Field(
+        default=None,
+        description="Return on invested capital",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+        alias="roic",
+    )
+    return_on_tangible_assets: Optional[float] = Field(
+        default=None,
+        description="Return on tangible assets",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+    )
+    dividend_yield: Optional[float] = Field(
+        default=None,
+        description="Dividend yield, as a normalized percent.",
+        json_schema_extra={"x-unit_measurement": "percent", "x-frontend_multiply": 100},
+        alias="dividendYield",
+    )
+    graham_number: Optional[float] = Field(default=None, description="Graham number")
+    graham_net_net: Optional[float] = Field(
+        default=None, description="Graham net-net working capital"
     )
 
 
 class FMPKeyMetricsFetcher(
     Fetcher[
         FMPKeyMetricsQueryParams,
         List[FMPKeyMetricsData],
     ]
 ):
-    """Transform the query, extract and transform the data from the FMP endpoints."""
+    """FMP Key Metrics Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> FMPKeyMetricsQueryParams:
         """Transform the query params."""
         return FMPKeyMetricsQueryParams(**params)
 
     @staticmethod
@@ -222,55 +262,61 @@
         query: FMPKeyMetricsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the FMP endpoint."""
         api_key = credentials.get("fmp_api_key") if credentials else ""
         base_url = "https://financialmodelingprep.com/api/v3"
-
         symbols = query.symbol.split(",")
-
         results: List = []
 
         async def get_one(symbol):
             """Get data for one symbol."""
-
-            url = f"{base_url}/key-metrics/{symbol}?period={query.period}&limit={query.limit}&apikey={api_key}"
-
+            url = (
+                f"{base_url}/key-metrics/{symbol}?period={query.period}"
+                + f"&limit={query.limit}&apikey={api_key}"
+            )
             result = await amake_request(
                 url, response_callback=response_callback, **kwargs
             )
-
             if not result:
                 warn(f"Symbol Error: No data found for {symbol}.")
 
             if result:
-
                 ttm_url = f"{base_url}/key-metrics-ttm/{symbol}?&apikey={api_key}"
                 if query.with_ttm and (
                     metrics_ttm := await amake_request(
                         ttm_url, response_callback=response_callback, **kwargs
                     )
                 ):
+                    metrics_ttm_data = {
+                        k: v
+                        for k, v in metrics_ttm[0].items()
+                        if k
+                        not in ("dividendYieldPercentageTTM", "dividendPerShareTTM")
+                    }
                     result.insert(  # type: ignore
                         0,
                         {
                             "symbol": symbol,
                             "period": "TTM",
                             "date": datetime.now().strftime("%Y-%m-%d"),
                             "calendar_year": datetime.now().year,
-                            **{k.replace("TTM", ""): v for k, v in metrics_ttm.items()},  # type: ignore
+                            **{
+                                k.replace("TTM", ""): v
+                                for k, v in metrics_ttm_data.items()
+                            },
                         },
                     )
                 results.extend(result)
 
         await asyncio.gather(*[get_one(symbol) for symbol in symbols])
 
         if not results:
-            raise EmptyDataError("No data found for given symbols.")
+            raise EmptyDataError(f"No data found for given symbols -> {query.symbol}.")
 
         return results
 
     @staticmethod
     def transform_data(
         query: FMPKeyMetricsQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[FMPKeyMetricsData]:
```

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/market_indices.py` & `openbb_fmp-1.2.1/openbb_fmp/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/market_snapshots.py` & `openbb_fmp-1.2.1/openbb_fmp/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/price_performance.py` & `openbb_fmp-1.2.1/openbb_fmp/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/price_target.py` & `openbb_fmp-1.2.1/openbb_fmp/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/price_target_consensus.py` & `openbb_fmp-1.2.1/openbb_fmp/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/revenue_business_line.py` & `openbb_fmp-1.2.1/openbb_fmp/models/revenue_business_line.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/revenue_geographic.py` & `openbb_fmp-1.2.1/openbb_fmp/models/revenue_geographic.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/risk_premium.py` & `openbb_fmp-1.2.1/openbb_fmp/models/risk_premium.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/share_statistics.py` & `openbb_fmp-1.2.1/openbb_fmp/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/treasury_rates.py` & `openbb_fmp-1.2.1/openbb_fmp/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/models/world_news.py` & `openbb_fmp-1.2.1/openbb_fmp/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/openbb_fmp/utils/definitions.py` & `openbb_fmp-1.2.1/openbb_fmp/utils/definitions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """FMP Literal Definitions."""
 
 from typing import Literal
 
 SECTORS = Literal[
-    "Consumer Cyclical",
-    "Energy",
-    "Technology",
-    "Industrials",
-    "Financial Services",
-    "Basic Materials",
-    "Communication Services",
-    "Consumer Defensive",
-    "Healthcare",
-    "Real Estate",
-    "Utilities",
-    "Industrial Goods",
-    "Financial",
-    "Services",
-    "Conglomerates",
+    "consumer_cyclical",
+    "energy",
+    "technology",
+    "industrials",
+    "financial_services",
+    "basic_materials",
+    "communication_services",
+    "consumer_defensive",
+    "healthcare",
+    "real_estate",
+    "utilities",
+    "industrial_goods",
+    "financial",
+    "services",
+    "conglomerates",
 ]
 
 EXCHANGES = Literal[
     "amex",
     "ams",
     "ase",
     "asx",
@@ -138,15 +138,14 @@
     "TWO",
     "VIE",
     "WSE",
     "XETRA",
 ]
 
 TRANSACTION_TYPES = Literal[
-    None,
     "award",
     "conversion",
     "return",
     "expire_short",
     "in_kind",
     "gift",
     "expire_long",
```

### Comparing `openbb_fmp-1.2.0/openbb_fmp/utils/helpers.py` & `openbb_fmp-1.2.1/openbb_fmp/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_fmp-1.2.0/PKG-INFO` & `openbb_fmp-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-fmp
-Version: 1.2.0
+Version: 1.2.1
 Summary: FMP extension for OpenBB
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
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Financial Modeling Prep Provider
 
 This extension integrates the [Financial Modeling Prep](https://site.financialmodelingprep.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

