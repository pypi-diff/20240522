# Comparing `tmp/unusualwhales_python_client-4.2.3.tar.gz` & `tmp/unusualwhales_python_client-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unusualwhales_python_client-4.2.3.tar", max compression
+gzip compressed data, was "unusualwhales_python_client-5.0.1.tar", max compression
```

## Comparing `unusualwhales_python_client-4.2.3.tar` & `unusualwhales_python_client-5.0.1.tar`

### file list

```diff
@@ -1,207 +1,208 @@
--rw-r--r--   0        0        0     1211 2024-05-04 17:34:12.914270 unusualwhales_python_client-4.2.3/LICENSE
--rw-r--r--   0        0        0     3107 2024-05-13 06:22:56.179296 unusualwhales_python_client-4.2.3/README.md
--rw-r--r--   0        0        0      597 2024-05-19 22:34:34.144931 unusualwhales_python_client-4.2.3/pyproject.toml
--rw-r--r--   0        0        0     6148 2024-05-19 07:40:14.959111 unusualwhales_python_client-4.2.3/unusualwhales/.DS_Store
--rw-r--r--   0        0        0      170 2024-05-14 16:56:05.151521 unusualwhales_python_client-4.2.3/unusualwhales/__init__.py
--rw-r--r--   0        0        0     6148 2024-05-17 15:31:34.867517 unusualwhales_python_client-4.2.3/unusualwhales/api/.DS_Store
--rw-r--r--   0        0        0       58 2024-05-13 00:33:10.876060 unusualwhales_python_client-4.2.3/unusualwhales/api/__init__.py
--rw-r--r--   0        0        0     1781 2024-05-05 22:58:01.830486 unusualwhales_python_client-4.2.3/unusualwhales/api/congress/__init__.py
--rw-r--r--   0        0        0     6907 2024-05-14 16:51:00.220751 unusualwhales_python_client-4.2.3/unusualwhales/api/congress/get_late_reports.py
--rw-r--r--   0        0        0     6925 2024-05-14 16:50:58.400595 unusualwhales_python_client-4.2.3/unusualwhales/api/congress/get_reports.py
--rw-r--r--   0        0        0     6916 2024-05-14 16:50:58.400580 unusualwhales_python_client-4.2.3/unusualwhales/api/congress/get_trades.py
--rw-r--r--   0        0        0     7930 2024-05-14 16:50:58.400812 unusualwhales_python_client-4.2.3/unusualwhales/api/congress/get_trades_by_member.py
--rw-r--r--   0        0        0      446 2024-05-05 22:58:01.829139 unusualwhales_python_client-4.2.3/unusualwhales/api/contract/__init__.py
--rw-r--r--   0        0        0     6040 2024-05-14 16:50:58.436664 unusualwhales_python_client-4.2.3/unusualwhales/api/contract/get_price_history.py
--rw-r--r--   0        0        0      941 2024-05-05 22:58:01.835779 unusualwhales_python_client-4.2.3/unusualwhales/api/darkpool/__init__.py
--rw-r--r--   0        0        0     6354 2024-05-14 16:50:58.416761 unusualwhales_python_client-4.2.3/unusualwhales/api/darkpool/get_trades_by_date.py
--rw-r--r--   0        0        0     7418 2024-05-14 16:50:58.416770 unusualwhales_python_client-4.2.3/unusualwhales/api/darkpool/get_trades_by_ticker.py
--rw-r--r--   0        0        0     1349 2024-05-05 22:58:01.832866 unusualwhales_python_client-4.2.3/unusualwhales/api/earnings/__init__.py
--rw-r--r--   0        0        0     5940 2024-05-14 16:50:58.432577 unusualwhales_python_client-4.2.3/unusualwhales/api/earnings/get_afterhours.py
--rw-r--r--   0        0        0     6019 2024-05-14 16:50:58.432749 unusualwhales_python_client-4.2.3/unusualwhales/api/earnings/get_premarket.py
--rw-r--r--   0        0        0     4598 2024-05-14 16:50:58.432595 unusualwhales_python_client-4.2.3/unusualwhales/api/earnings/get_ticker_earnings.py
--rw-r--r--   0        0        0     1402 2024-05-13 00:31:49.829150 unusualwhales_python_client-4.2.3/unusualwhales/api/endpoints.py
--rw-r--r--   0        0        0     1348 2024-05-05 22:58:01.830714 unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/__init__.py
--rw-r--r--   0        0        0     3925 2024-05-14 16:50:58.432768 unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/get_holdings.py
--rw-r--r--   0        0        0     4475 2024-05-14 16:50:58.432811 unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/get_info.py
--rw-r--r--   0        0        0     4757 2024-05-14 16:50:58.432793 unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/get_sector_country_weights.py
--rw-r--r--   0        0        0     4061 2024-05-14 16:50:58.432729 unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/get_ticker_exposure.py
--rw-r--r--   0        0        0     2839 2024-05-05 22:58:01.823337 unusualwhales_python_client-4.2.3/unusualwhales/api/flow/__init__.py
--rw-r--r--   0        0        0     8854 2024-05-14 16:50:58.415793 unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_contract_flow.py
--rw-r--r--   0        0        0     4355 2024-05-14 16:50:58.415780 unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_flow_by_expiry.py
--rw-r--r--   0        0        0     4838 2024-05-14 16:50:58.415765 unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_flow_by_strike.py
--rw-r--r--   0        0        0     3170 2024-05-14 16:50:58.409858 unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_full_tape.py
--rw-r--r--   0        0        0     7360 2024-05-14 16:50:58.428050 unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_order_flow.py
--rw-r--r--   0        0        0    29084 2024-05-14 16:50:58.416171 unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_ticker_order_flow.py
--rw-r--r--   0        0        0     5766 2024-05-14 16:50:58.416153 unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_unusual_flow_alerts.py
--rw-r--r--   0        0        0     6232 2024-05-05 22:58:01.822234 unusualwhales_python_client-4.2.3/unusualwhales/api/market/__init__.py
--rw-r--r--   0        0        0     3744 2024-05-14 16:50:58.416725 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_economic_calendar.py
--rw-r--r--   0        0        0     3718 2024-05-14 16:50:58.416691 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_fda_calendar.py
--rw-r--r--   0        0        0     3693 2024-05-14 16:50:58.416675 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_holidays.py
--rw-r--r--   0        0        0     3765 2024-05-14 16:50:58.416650 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_imbalances.py
--rw-r--r--   0        0        0     5681 2024-05-14 16:50:58.416749 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_insider_trades.py
--rw-r--r--   0        0        0     6188 2024-05-14 16:50:58.416738 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_market_options_volume.py
--rw-r--r--   0        0        0    12740 2024-05-14 16:50:58.416220 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_market_tide.py
--rw-r--r--   0        0        0     6984 2024-05-14 16:50:58.416714 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_market_tide_by_etf.py
--rw-r--r--   0        0        0     7643 2024-05-14 16:50:58.422952 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_open_interest_change.py
--rw-r--r--   0        0        0     4563 2024-05-14 16:50:58.416198 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_sector_stats.py
--rw-r--r--   0        0        0     5764 2024-05-14 16:50:58.416245 unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_spike.py
--rw-r--r--   0        0        0     1567 2024-05-05 22:58:01.834188 unusualwhales_python_client-4.2.3/unusualwhales/api/screener/__init__.py
--rw-r--r--   0        0        0     9114 2024-05-14 16:50:58.436720 unusualwhales_python_client-4.2.3/unusualwhales/api/screener/get_analyst_ratings.py
--rw-r--r--   0        0        0    45558 2024-05-14 16:50:58.432711 unusualwhales_python_client-4.2.3/unusualwhales/api/screener/get_option_contracts.py
--rw-r--r--   0        0        0    64290 2024-05-14 16:50:58.432678 unusualwhales_python_client-4.2.3/unusualwhales/api/screener/get_stocks.py
--rw-r--r--   0        0        0     1911 2024-05-05 22:58:01.823405 unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/__init__.py
--rw-r--r--   0        0        0     4251 2024-05-14 16:50:58.422811 unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/get_market_average_returns_by_month.py
--rw-r--r--   0        0        0     4796 2024-05-14 16:50:58.436634 unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/get_monthly_average_returns.py
--rw-r--r--   0        0        0    13768 2024-05-14 16:50:58.422794 unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/get_monthly_top_performers.py
--rw-r--r--   0        0        0     4922 2024-05-14 16:50:58.422779 unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py
--rw-r--r--   0        0        0    17216 2024-05-05 22:58:01.830003 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/__init__.py
--rw-r--r--   0        0        0     5755 2024-05-14 16:50:58.422764 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_atm_option_contracts_for_expiries.py
--rw-r--r--   0        0        0     9164 2024-05-14 16:50:58.417097 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_candles.py
--rw-r--r--   0        0        0     6193 2024-05-14 16:50:58.422567 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_daily_expiry_breakdown.py
--rw-r--r--   0        0        0    14217 2024-05-14 16:50:58.422514 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greek_exposure.py
--rw-r--r--   0        0        0     6331 2024-05-14 16:50:58.416902 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greek_exposure_by_expiry.py
--rw-r--r--   0        0        0     6399 2024-05-14 16:50:58.417006 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greek_exposure_by_strike.py
--rw-r--r--   0        0        0     6901 2024-05-14 16:50:58.416987 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greek_exposure_by_strike_expiry.py
--rw-r--r--   0        0        0     6382 2024-05-14 16:50:58.422640 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greeks_by_strike_expiry.py
--rw-r--r--   0        0        0     6223 2024-05-14 16:50:58.422594 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_info.py
--rw-r--r--   0        0        0     4935 2024-05-14 16:50:58.422714 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_insider_trades.py
--rw-r--r--   0        0        0     4688 2024-05-14 16:50:58.417114 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_max_pain.py
--rw-r--r--   0        0        0    10533 2024-05-14 16:50:58.432551 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_net_premium_ticks.py
--rw-r--r--   0        0        0     7829 2024-05-14 16:50:58.422624 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_open_interest_change.py
--rw-r--r--   0        0        0     7388 2024-05-14 16:50:58.417081 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_option_chains.py
--rw-r--r--   0        0        0    10925 2024-05-14 16:50:58.422611 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_option_contracts.py
--rw-r--r--   0        0        0     6049 2024-05-14 16:50:58.422749 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_option_volume_by_price_level.py
--rw-r--r--   0        0        0     5952 2024-05-14 16:50:58.422542 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_options_volume.py
--rw-r--r--   0        0        0     9072 2024-05-14 16:50:58.436939 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_risk_reversal_skew.py
--rw-r--r--   0        0        0     4926 2024-05-14 16:50:58.417023 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_sector_tickers.py
--rw-r--r--   0        0        0    14204 2024-05-14 16:50:58.417056 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_spot_exposures.py
--rw-r--r--   0        0        0    14533 2024-05-14 16:50:58.417039 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_spot_exposures_by_strike.py
--rw-r--r--   0        0        0     6448 2024-05-14 16:50:58.416964 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_volatility_term_structure.py
--rw-r--r--   0        0        0     7214 2024-05-14 16:50:58.422733 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_volume_by_price_level.py
--rw-r--r--   0        0        0     6097 2024-05-14 16:50:58.423065 unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_volume_open_interest_by_expiry.py
--rw-r--r--   0        0        0     7122 2024-05-13 00:28:35.664213 unusualwhales_python_client-4.2.3/unusualwhales/client.py
--rw-r--r--   0        0        0      546 2024-05-05 22:58:01.816143 unusualwhales_python_client-4.2.3/unusualwhales/errors.py
--rw-r--r--   0        0        0     6148 2024-05-17 18:14:11.372403 unusualwhales_python_client-4.2.3/unusualwhales/models/.DS_Store
--rw-r--r--   0        0        0    10021 2024-05-05 22:58:01.822073 unusualwhales_python_client-4.2.3/unusualwhales/models/__init__.py
--rw-r--r--   0        0        0     2227 2024-05-05 22:58:01.823494 unusualwhales_python_client-4.2.3/unusualwhales/models/analalyst_rating_results.py
--rw-r--r--   0        0        0      262 2024-05-05 22:58:01.779003 unusualwhales_python_client-4.2.3/unusualwhales/models/analyst_action.py
--rw-r--r--   0        0        0      267 2024-05-05 22:58:01.779493 unusualwhales_python_client-4.2.3/unusualwhales/models/analyst_field_action.py
--rw-r--r--   0        0        0      183 2024-05-05 22:58:01.758542 unusualwhales_python_client-4.2.3/unusualwhales/models/analyst_field_recommendation.py
--rw-r--r--   0        0        0     6697 2024-05-05 22:58:01.820117 unusualwhales_python_client-4.2.3/unusualwhales/models/analyst_rating.py
--rw-r--r--   0        0        0      178 2024-05-05 22:58:01.765008 unusualwhales_python_client-4.2.3/unusualwhales/models/analyst_recommendation.py
--rw-r--r--   0        0        0      428 2024-05-05 22:58:01.775125 unusualwhales_python_client-4.2.3/unusualwhales/models/analyst_sector.py
--rw-r--r--   0        0        0     5389 2024-05-14 17:46:09.508744 unusualwhales_python_client-4.2.3/unusualwhales/models/candle_data.py
--rw-r--r--   0        0        0     2098 2024-05-05 22:58:01.833898 unusualwhales_python_client-4.2.3/unusualwhales/models/candle_data_results.py
--rw-r--r--   0        0        0      251 2024-05-05 22:58:01.780257 unusualwhales_python_client-4.2.3/unusualwhales/models/candle_size.py
--rw-r--r--   0        0        0     5755 2024-05-05 22:58:01.816560 unusualwhales_python_client-4.2.3/unusualwhales/models/congressional_trade_report.py
--rw-r--r--   0        0        0     2308 2024-05-05 22:58:01.833569 unusualwhales_python_client-4.2.3/unusualwhales/models/congressional_trade_report_results.py
--rw-r--r--   0        0        0     5235 2024-05-05 22:58:01.830332 unusualwhales_python_client-4.2.3/unusualwhales/models/country_sector_exposure.py
--rw-r--r--   0        0        0     3869 2024-05-05 22:58:01.828297 unusualwhales_python_client-4.2.3/unusualwhales/models/daily_market_tide.py
--rw-r--r--   0        0        0     2240 2024-05-05 22:58:01.833609 unusualwhales_python_client-4.2.3/unusualwhales/models/daily_market_tide_response.py
--rw-r--r--   0        0        0     9770 2024-05-05 22:58:01.832534 unusualwhales_python_client-4.2.3/unusualwhales/models/darkpool_trade.py
--rw-r--r--   0        0        0     3375 2024-05-05 22:58:01.818843 unusualwhales_python_client-4.2.3/unusualwhales/models/darkpool_trade_response.py
--rw-r--r--   0        0        0     8924 2024-05-05 22:58:01.834330 unusualwhales_python_client-4.2.3/unusualwhales/models/earnings.py
--rw-r--r--   0        0        0     2069 2024-05-05 22:58:01.833907 unusualwhales_python_client-4.2.3/unusualwhales/models/earnings_results.py
--rw-r--r--   0        0        0     4185 2024-05-05 22:58:01.823207 unusualwhales_python_client-4.2.3/unusualwhales/models/economic_calendar.py
--rw-r--r--   0        0        0      189 2024-05-05 22:58:01.783710 unusualwhales_python_client-4.2.3/unusualwhales/models/economic_type.py
--rw-r--r--   0        0        0     2673 2024-05-05 22:58:01.820875 unusualwhales_python_client-4.2.3/unusualwhales/models/error_message.py
--rw-r--r--   0        0        0     1779 2024-05-05 22:58:01.822650 unusualwhales_python_client-4.2.3/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py
--rw-r--r--   0        0        0     2063 2024-05-05 22:58:01.825400 unusualwhales_python_client-4.2.3/unusualwhales/models/etf_countries_item.py
--rw-r--r--   0        0        0     3171 2024-05-05 22:58:01.822868 unusualwhales_python_client-4.2.3/unusualwhales/models/etf_info.py
--rw-r--r--   0        0        0     6423 2024-05-05 22:58:01.832037 unusualwhales_python_client-4.2.3/unusualwhales/models/etf_info_data.py
--rw-r--r--   0        0        0     2044 2024-05-05 22:58:01.818548 unusualwhales_python_client-4.2.3/unusualwhales/models/etf_sectors_item.py
--rw-r--r--   0        0        0     2953 2024-05-05 22:58:01.832447 unusualwhales_python_client-4.2.3/unusualwhales/models/expiry_breakdown.py
--rw-r--r--   0        0        0     2248 2024-05-05 22:58:01.825125 unusualwhales_python_client-4.2.3/unusualwhales/models/expiry_breakdown_result.py
--rw-r--r--   0        0        0     5086 2024-05-05 22:58:01.817753 unusualwhales_python_client-4.2.3/unusualwhales/models/fda_calendar.py
--rw-r--r--   0        0        0    10635 2024-05-05 22:58:01.817394 unusualwhales_python_client-4.2.3/unusualwhales/models/flow_alert.py
--rw-r--r--   0        0        0     2086 2024-05-05 22:58:01.816655 unusualwhales_python_client-4.2.3/unusualwhales/models/flow_alert_results.py
--rw-r--r--   0        0        0      590 2024-05-05 22:58:01.780015 unusualwhales_python_client-4.2.3/unusualwhales/models/flow_alert_rule.py
--rw-r--r--   0        0        0    12800 2024-05-05 22:58:01.827106 unusualwhales_python_client-4.2.3/unusualwhales/models/flow_per_expiry.py
--rw-r--r--   0        0        0     2139 2024-05-05 22:58:01.827194 unusualwhales_python_client-4.2.3/unusualwhales/models/flow_per_expiry_results.py
--rw-r--r--   0        0        0    12688 2024-05-05 22:58:01.819326 unusualwhales_python_client-4.2.3/unusualwhales/models/flow_per_strike.py
--rw-r--r--   0        0        0     2139 2024-05-05 22:58:01.830018 unusualwhales_python_client-4.2.3/unusualwhales/models/flow_per_strike_results.py
--rw-r--r--   0        0        0     6320 2024-05-05 22:58:01.816924 unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure.py
--rw-r--r--   0        0        0     6349 2024-05-05 22:58:01.822486 unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_by_strike.py
--rw-r--r--   0        0        0     6808 2024-05-05 22:58:01.831535 unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_by_strike_and_expiry.py
--rw-r--r--   0        0        0     2358 2024-05-05 22:58:01.821530 unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_by_strike_and_expiry_results.py
--rw-r--r--   0        0        0     2240 2024-05-05 22:58:01.827851 unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_by_strike_results.py
--rw-r--r--   0        0        0     2134 2024-05-05 22:58:01.816486 unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_results.py
--rw-r--r--   0        0        0     9046 2024-05-05 22:58:01.826947 unusualwhales_python_client-4.2.3/unusualwhales/models/greeks.py
--rw-r--r--   0        0        0     2535 2024-05-05 22:58:01.829764 unusualwhales_python_client-4.2.3/unusualwhales/models/historical_risk_reversal_skew.py
--rw-r--r--   0        0        0     2300 2024-05-05 22:58:01.822832 unusualwhales_python_client-4.2.3/unusualwhales/models/historical_risk_reversal_skew_results.py
--rw-r--r--   0        0        0     8935 2024-05-05 22:58:01.817484 unusualwhales_python_client-4.2.3/unusualwhales/models/holdings.py
--rw-r--r--   0        0        0     2648 2024-05-05 22:58:01.821969 unusualwhales_python_client-4.2.3/unusualwhales/models/holdings_response.py
--rw-r--r--   0        0        0     4229 2024-05-05 22:58:01.818954 unusualwhales_python_client-4.2.3/unusualwhales/models/imbalances_volume.py
--rw-r--r--   0        0        0     4234 2024-05-05 22:58:01.831021 unusualwhales_python_client-4.2.3/unusualwhales/models/implied_volatility_term_structure.py
--rw-r--r--   0        0        0     2348 2024-05-05 22:58:01.822055 unusualwhales_python_client-4.2.3/unusualwhales/models/implied_volatility_term_structure_results.py
--rw-r--r--   0        0        0     3185 2024-05-05 22:58:01.834435 unusualwhales_python_client-4.2.3/unusualwhales/models/insider_statistic.py
--rw-r--r--   0        0        0     2770 2024-05-05 22:58:01.816314 unusualwhales_python_client-4.2.3/unusualwhales/models/insider_statistics.py
--rw-r--r--   0        0        0      190 2024-05-05 22:58:01.766259 unusualwhales_python_client-4.2.3/unusualwhales/models/insider_trades_member_type.py
--rw-r--r--   0        0        0      345 2024-05-05 22:58:01.775861 unusualwhales_python_client-4.2.3/unusualwhales/models/insider_trades_transaction_type.py
--rw-r--r--   0        0        0      164 2024-05-05 22:58:01.778813 unusualwhales_python_client-4.2.3/unusualwhales/models/market_general_imbalance_event.py
--rw-r--r--   0        0        0      165 2024-05-05 22:58:01.783423 unusualwhales_python_client-4.2.3/unusualwhales/models/market_general_imbalance_side.py
--rw-r--r--   0        0        0      213 2024-05-05 22:58:01.776228 unusualwhales_python_client-4.2.3/unusualwhales/models/market_general_imbalance_type.py
--rw-r--r--   0        0        0      168 2024-05-05 22:58:01.773079 unusualwhales_python_client-4.2.3/unusualwhales/models/market_general_market_time.py
--rw-r--r--   0        0        0      528 2024-05-05 22:58:01.774624 unusualwhales_python_client-4.2.3/unusualwhales/models/market_general_sector.py
--rw-r--r--   0        0        0     4512 2024-05-05 22:58:01.834484 unusualwhales_python_client-4.2.3/unusualwhales/models/market_holidays.py
--rw-r--r--   0        0        0     3378 2024-05-05 22:58:01.831296 unusualwhales_python_client-4.2.3/unusualwhales/models/market_options_volume.py
--rw-r--r--   0        0        0     1710 2024-05-05 22:58:01.827677 unusualwhales_python_client-4.2.3/unusualwhales/models/market_sector_ticker_results.py
--rw-r--r--   0        0        0     2535 2024-05-05 22:58:01.830420 unusualwhales_python_client-4.2.3/unusualwhales/models/max_pain.py
--rw-r--r--   0        0        0     2159 2024-05-05 22:58:01.833744 unusualwhales_python_client-4.2.3/unusualwhales/models/max_pain_results.py
--rw-r--r--   0        0        0     3421 2024-05-05 22:58:01.833406 unusualwhales_python_client-4.2.3/unusualwhales/models/net_prem_tick.py
--rw-r--r--   0        0        0     4303 2024-05-05 22:58:01.828862 unusualwhales_python_client-4.2.3/unusualwhales/models/net_prem_tick_results.py
--rw-r--r--   0        0        0     2494 2024-05-05 22:58:01.821207 unusualwhales_python_client-4.2.3/unusualwhales/models/off_lit_price_level.py
--rw-r--r--   0        0        0     2270 2024-05-05 22:58:01.816343 unusualwhales_python_client-4.2.3/unusualwhales/models/off_lit_price_level_results.py
--rw-r--r--   0        0        0    11261 2024-05-05 22:58:01.823477 unusualwhales_python_client-4.2.3/unusualwhales/models/oi_change.py
--rw-r--r--   0        0        0     2101 2024-05-05 22:58:01.828752 unusualwhales_python_client-4.2.3/unusualwhales/models/oi_change_results.py
--rw-r--r--   0        0        0    10954 2024-05-05 22:58:01.817830 unusualwhales_python_client-4.2.3/unusualwhales/models/option_chain_contract.py
--rw-r--r--   0        0        0     2316 2024-05-05 22:58:01.818322 unusualwhales_python_client-4.2.3/unusualwhales/models/option_chain_contract_results.py
--rw-r--r--   0        0        0     2187 2024-05-05 22:58:01.818071 unusualwhales_python_client-4.2.3/unusualwhales/models/option_chains_results.py
--rw-r--r--   0        0        0    11275 2024-05-05 22:58:01.818618 unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract.py
--rw-r--r--   0        0        0     2251 2024-05-05 22:58:01.829762 unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract_results.py
--rw-r--r--   0        0        0    14866 2024-05-05 22:58:01.824112 unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract_screener_item.py
--rw-r--r--   0        0        0     2375 2024-05-05 22:58:01.831061 unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract_screener_results.py
--rw-r--r--   0        0        0      157 2024-05-05 22:58:01.768374 unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract_type.py
--rw-r--r--   0        0        0     2522 2024-05-05 22:58:01.825820 unusualwhales_python_client-4.2.3/unusualwhales/models/option_price_level.py
--rw-r--r--   0        0        0     2283 2024-05-05 22:58:01.827958 unusualwhales_python_client-4.2.3/unusualwhales/models/option_price_level_results.py
--rw-r--r--   0        0        0      149 2024-05-05 22:58:01.770159 unusualwhales_python_client-4.2.3/unusualwhales/models/option_type.py
--rw-r--r--   0        0        0      153 2024-05-05 22:58:01.771290 unusualwhales_python_client-4.2.3/unusualwhales/models/order_direction.py
--rw-r--r--   0        0        0      949 2024-05-05 22:58:01.774812 unusualwhales_python_client-4.2.3/unusualwhales/models/screener_contract_order_by_field.py
--rw-r--r--   0        0        0     1401 2024-05-05 22:58:01.780126 unusualwhales_python_client-4.2.3/unusualwhales/models/screener_order_by_field.py
--rw-r--r--   0        0        0     5330 2024-05-05 22:58:01.832188 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_market.py
--rw-r--r--   0        0        0     2245 2024-05-05 22:58:01.817561 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_market_results.py
--rw-r--r--   0        0        0     4802 2024-05-05 22:58:01.826952 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_monthly.py
--rw-r--r--   0        0        0     2864 2024-05-05 22:58:01.816371 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_monthly_results.py
--rw-r--r--   0        0        0      412 2024-05-05 22:58:01.784552 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_performance_order_by.py
--rw-r--r--   0        0        0     6634 2024-05-05 22:58:01.820876 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_performers.py
--rw-r--r--   0        0        0     2884 2024-05-05 22:58:01.822592 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_performers_results.py
--rw-r--r--   0        0        0     2957 2024-05-05 22:58:01.827974 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_year_month.py
--rw-r--r--   0        0        0     3159 2024-05-05 22:58:01.828370 unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_year_month_results.py
--rw-r--r--   0        0        0      515 2024-05-05 22:58:01.783541 unusualwhales_python_client-4.2.3/unusualwhales/models/sector.py
--rw-r--r--   0        0        0    10830 2024-05-05 22:58:01.830188 unusualwhales_python_client-4.2.3/unusualwhales/models/sector_etf.py
--rw-r--r--   0        0        0     2890 2024-05-05 22:58:01.823726 unusualwhales_python_client-4.2.3/unusualwhales/models/sector_etf_results.py
--rw-r--r--   0        0        0      173 2024-05-05 22:58:01.769865 unusualwhales_python_client-4.2.3/unusualwhales/models/side.py
--rw-r--r--   0        0        0      206 2024-05-05 22:58:01.776708 unusualwhales_python_client-4.2.3/unusualwhales/models/single_issue_type.py
--rw-r--r--   0        0        0      343 2024-05-05 22:58:01.762014 unusualwhales_python_client-4.2.3/unusualwhales/models/single_month_number.py
--rw-r--r--   0        0        0      521 2024-05-05 22:58:01.779594 unusualwhales_python_client-4.2.3/unusualwhales/models/single_sector.py
--rw-r--r--   0        0        0      334 2024-05-05 22:58:01.769228 unusualwhales_python_client-4.2.3/unusualwhales/models/single_trade_external_hour_sold_code.py
--rw-r--r--   0        0        0      312 2024-05-05 22:58:01.761864 unusualwhales_python_client-4.2.3/unusualwhales/models/single_trade_sale_cond_code.py
--rw-r--r--   0        0        0      304 2024-05-05 22:58:01.781307 unusualwhales_python_client-4.2.3/unusualwhales/models/single_trade_settlement.py
--rw-r--r--   0        0        0      275 2024-05-05 22:58:01.752668 unusualwhales_python_client-4.2.3/unusualwhales/models/single_trade_trade_code.py
--rw-r--r--   0        0        0     2304 2024-05-05 22:58:01.832942 unusualwhales_python_client-4.2.3/unusualwhales/models/spike_value.py
--rw-r--r--   0        0        0     7769 2024-05-05 22:58:01.832634 unusualwhales_python_client-4.2.3/unusualwhales/models/spot_gex_exposures_per_1_min.py
--rw-r--r--   0        0        0     2274 2024-05-05 22:58:01.833460 unusualwhales_python_client-4.2.3/unusualwhales/models/spot_gex_exposures_per_1_min_results.py
--rw-r--r--   0        0        0     8339 2024-05-05 22:58:01.833587 unusualwhales_python_client-4.2.3/unusualwhales/models/spot_greek_exposures_by_strike.py
--rw-r--r--   0        0        0     2305 2024-05-05 22:58:01.817337 unusualwhales_python_client-4.2.3/unusualwhales/models/spot_greek_exposures_by_strike_results.py
--rw-r--r--   0        0        0      202 2024-05-05 22:58:01.756301 unusualwhales_python_client-4.2.3/unusualwhales/models/stock_earnings_time.py
--rw-r--r--   0        0        0      205 2024-05-05 22:58:01.779639 unusualwhales_python_client-4.2.3/unusualwhales/models/stock_issue_type.py
--rw-r--r--   0        0        0    24207 2024-05-05 22:58:01.822193 unusualwhales_python_client-4.2.3/unusualwhales/models/stock_screener_response.py
--rw-r--r--   0        0        0     2280 2024-05-05 22:58:01.823614 unusualwhales_python_client-4.2.3/unusualwhales/models/stock_screener_response_results.py
--rw-r--r--   0        0        0     8648 2024-05-05 22:58:01.828620 unusualwhales_python_client-4.2.3/unusualwhales/models/ticker_info.py
--rw-r--r--   0        0        0     2636 2024-05-05 22:58:01.831049 unusualwhales_python_client-4.2.3/unusualwhales/models/ticker_info_results.py
--rw-r--r--   0        0        0    11609 2024-05-05 22:58:01.832705 unusualwhales_python_client-4.2.3/unusualwhales/models/ticker_options_volume.py
--rw-r--r--   0        0        0     2436 2024-05-05 22:58:01.828948 unusualwhales_python_client-4.2.3/unusualwhales/models/volume_oi_per_expiry.py
--rw-r--r--   0        0        0     2233 2024-05-05 22:58:01.816470 unusualwhales_python_client-4.2.3/unusualwhales/models/volume_oi_per_expiry_results.py
--rw-r--r--   0        0        0       25 2024-05-05 22:58:01.341037 unusualwhales_python_client-4.2.3/unusualwhales/py.typed
--rw-r--r--   0        0        0      985 2024-05-05 22:58:01.827475 unusualwhales_python_client-4.2.3/unusualwhales/types.py
--rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 unusualwhales_python_client-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-05-04 17:34:12.914270 unusualwhales_python_client-5.0.1/LICENSE
+-rw-r--r--   0        0        0     3107 2024-05-13 06:22:56.179296 unusualwhales_python_client-5.0.1/README.md
+-rw-r--r--   0        0        0      597 2024-05-21 23:11:15.227515 unusualwhales_python_client-5.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6148 2024-05-19 07:40:14.959111 unusualwhales_python_client-5.0.1/unusualwhales/.DS_Store
+-rw-r--r--   0        0        0      170 2024-05-14 16:56:05.151521 unusualwhales_python_client-5.0.1/unusualwhales/__init__.py
+-rw-r--r--   0        0        0       45 2024-05-21 23:11:44.918088 unusualwhales_python_client-5.0.1/unusualwhales/__version__.py
+-rw-r--r--   0        0        0     6148 2024-05-17 15:31:34.867517 unusualwhales_python_client-5.0.1/unusualwhales/api/.DS_Store
+-rw-r--r--   0        0        0       58 2024-05-13 00:33:10.876060 unusualwhales_python_client-5.0.1/unusualwhales/api/__init__.py
+-rw-r--r--   0        0        0     1781 2024-05-05 22:58:01.830486 unusualwhales_python_client-5.0.1/unusualwhales/api/congress/__init__.py
+-rw-r--r--   0        0        0     6907 2024-05-14 16:51:00.220751 unusualwhales_python_client-5.0.1/unusualwhales/api/congress/get_late_reports.py
+-rw-r--r--   0        0        0     6925 2024-05-14 16:50:58.400595 unusualwhales_python_client-5.0.1/unusualwhales/api/congress/get_reports.py
+-rw-r--r--   0        0        0     6916 2024-05-14 16:50:58.400580 unusualwhales_python_client-5.0.1/unusualwhales/api/congress/get_trades.py
+-rw-r--r--   0        0        0     7930 2024-05-14 16:50:58.400812 unusualwhales_python_client-5.0.1/unusualwhales/api/congress/get_trades_by_member.py
+-rw-r--r--   0        0        0      446 2024-05-05 22:58:01.829139 unusualwhales_python_client-5.0.1/unusualwhales/api/contract/__init__.py
+-rw-r--r--   0        0        0     6040 2024-05-14 16:50:58.436664 unusualwhales_python_client-5.0.1/unusualwhales/api/contract/get_price_history.py
+-rw-r--r--   0        0        0      941 2024-05-05 22:58:01.835779 unusualwhales_python_client-5.0.1/unusualwhales/api/darkpool/__init__.py
+-rw-r--r--   0        0        0     6354 2024-05-14 16:50:58.416761 unusualwhales_python_client-5.0.1/unusualwhales/api/darkpool/get_trades_by_date.py
+-rw-r--r--   0        0        0     7418 2024-05-14 16:50:58.416770 unusualwhales_python_client-5.0.1/unusualwhales/api/darkpool/get_trades_by_ticker.py
+-rw-r--r--   0        0        0     1349 2024-05-05 22:58:01.832866 unusualwhales_python_client-5.0.1/unusualwhales/api/earnings/__init__.py
+-rw-r--r--   0        0        0     5940 2024-05-14 16:50:58.432577 unusualwhales_python_client-5.0.1/unusualwhales/api/earnings/get_afterhours.py
+-rw-r--r--   0        0        0     6019 2024-05-14 16:50:58.432749 unusualwhales_python_client-5.0.1/unusualwhales/api/earnings/get_premarket.py
+-rw-r--r--   0        0        0     4598 2024-05-14 16:50:58.432595 unusualwhales_python_client-5.0.1/unusualwhales/api/earnings/get_ticker_earnings.py
+-rw-r--r--   0        0        0     1402 2024-05-13 00:31:49.829150 unusualwhales_python_client-5.0.1/unusualwhales/api/endpoints.py
+-rw-r--r--   0        0        0     1348 2024-05-05 22:58:01.830714 unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/__init__.py
+-rw-r--r--   0        0        0     3925 2024-05-14 16:50:58.432768 unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/get_holdings.py
+-rw-r--r--   0        0        0     4475 2024-05-14 16:50:58.432811 unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/get_info.py
+-rw-r--r--   0        0        0     4757 2024-05-14 16:50:58.432793 unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/get_sector_country_weights.py
+-rw-r--r--   0        0        0     4061 2024-05-14 16:50:58.432729 unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/get_ticker_exposure.py
+-rw-r--r--   0        0        0     2839 2024-05-05 22:58:01.823337 unusualwhales_python_client-5.0.1/unusualwhales/api/flow/__init__.py
+-rw-r--r--   0        0        0     8854 2024-05-14 16:50:58.415793 unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_contract_flow.py
+-rw-r--r--   0        0        0     4355 2024-05-14 16:50:58.415780 unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_flow_by_expiry.py
+-rw-r--r--   0        0        0     4838 2024-05-14 16:50:58.415765 unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_flow_by_strike.py
+-rw-r--r--   0        0        0     3170 2024-05-14 16:50:58.409858 unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_full_tape.py
+-rw-r--r--   0        0        0     7360 2024-05-14 16:50:58.428050 unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_order_flow.py
+-rw-r--r--   0        0        0    29084 2024-05-14 16:50:58.416171 unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_ticker_order_flow.py
+-rw-r--r--   0        0        0     5766 2024-05-14 16:50:58.416153 unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_unusual_flow_alerts.py
+-rw-r--r--   0        0        0     6232 2024-05-05 22:58:01.822234 unusualwhales_python_client-5.0.1/unusualwhales/api/market/__init__.py
+-rw-r--r--   0        0        0     3744 2024-05-14 16:50:58.416725 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_economic_calendar.py
+-rw-r--r--   0        0        0     3718 2024-05-14 16:50:58.416691 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_fda_calendar.py
+-rw-r--r--   0        0        0     3693 2024-05-14 16:50:58.416675 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_holidays.py
+-rw-r--r--   0        0        0     3765 2024-05-14 16:50:58.416650 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_imbalances.py
+-rw-r--r--   0        0        0     5681 2024-05-14 16:50:58.416749 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_insider_trades.py
+-rw-r--r--   0        0        0     6188 2024-05-14 16:50:58.416738 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_market_options_volume.py
+-rw-r--r--   0        0        0    12740 2024-05-14 16:50:58.416220 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_market_tide.py
+-rw-r--r--   0        0        0     6984 2024-05-14 16:50:58.416714 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_market_tide_by_etf.py
+-rw-r--r--   0        0        0     7643 2024-05-14 16:50:58.422952 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_open_interest_change.py
+-rw-r--r--   0        0        0     4563 2024-05-14 16:50:58.416198 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_sector_stats.py
+-rw-r--r--   0        0        0     5764 2024-05-14 16:50:58.416245 unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_spike.py
+-rw-r--r--   0        0        0     1567 2024-05-05 22:58:01.834188 unusualwhales_python_client-5.0.1/unusualwhales/api/screener/__init__.py
+-rw-r--r--   0        0        0     9114 2024-05-14 16:50:58.436720 unusualwhales_python_client-5.0.1/unusualwhales/api/screener/get_analyst_ratings.py
+-rw-r--r--   0        0        0    45558 2024-05-14 16:50:58.432711 unusualwhales_python_client-5.0.1/unusualwhales/api/screener/get_option_contracts.py
+-rw-r--r--   0        0        0    64290 2024-05-14 16:50:58.432678 unusualwhales_python_client-5.0.1/unusualwhales/api/screener/get_stocks.py
+-rw-r--r--   0        0        0     1911 2024-05-05 22:58:01.823405 unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/__init__.py
+-rw-r--r--   0        0        0     4251 2024-05-14 16:50:58.422811 unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/get_market_average_returns_by_month.py
+-rw-r--r--   0        0        0     4796 2024-05-14 16:50:58.436634 unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/get_monthly_average_returns.py
+-rw-r--r--   0        0        0    13768 2024-05-14 16:50:58.422794 unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/get_monthly_top_performers.py
+-rw-r--r--   0        0        0     4922 2024-05-14 16:50:58.422779 unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py
+-rw-r--r--   0        0        0    17216 2024-05-05 22:58:01.830003 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/__init__.py
+-rw-r--r--   0        0        0     5755 2024-05-14 16:50:58.422764 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_atm_option_contracts_for_expiries.py
+-rw-r--r--   0        0        0     9164 2024-05-14 16:50:58.417097 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_candles.py
+-rw-r--r--   0        0        0     6193 2024-05-14 16:50:58.422567 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_daily_expiry_breakdown.py
+-rw-r--r--   0        0        0    14217 2024-05-14 16:50:58.422514 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greek_exposure.py
+-rw-r--r--   0        0        0     6331 2024-05-14 16:50:58.416902 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greek_exposure_by_expiry.py
+-rw-r--r--   0        0        0     6399 2024-05-14 16:50:58.417006 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greek_exposure_by_strike.py
+-rw-r--r--   0        0        0     6901 2024-05-14 16:50:58.416987 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greek_exposure_by_strike_expiry.py
+-rw-r--r--   0        0        0     6382 2024-05-14 16:50:58.422640 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greeks_by_strike_expiry.py
+-rw-r--r--   0        0        0     6223 2024-05-14 16:50:58.422594 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_info.py
+-rw-r--r--   0        0        0     4935 2024-05-14 16:50:58.422714 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_insider_trades.py
+-rw-r--r--   0        0        0     4688 2024-05-14 16:50:58.417114 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_max_pain.py
+-rw-r--r--   0        0        0    10533 2024-05-14 16:50:58.432551 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_net_premium_ticks.py
+-rw-r--r--   0        0        0     7829 2024-05-14 16:50:58.422624 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_open_interest_change.py
+-rw-r--r--   0        0        0     7388 2024-05-14 16:50:58.417081 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_option_chains.py
+-rw-r--r--   0        0        0    10925 2024-05-14 16:50:58.422611 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_option_contracts.py
+-rw-r--r--   0        0        0     6049 2024-05-14 16:50:58.422749 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_option_volume_by_price_level.py
+-rw-r--r--   0        0        0     5952 2024-05-14 16:50:58.422542 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_options_volume.py
+-rw-r--r--   0        0        0     9072 2024-05-14 16:50:58.436939 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_risk_reversal_skew.py
+-rw-r--r--   0        0        0     4926 2024-05-14 16:50:58.417023 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_sector_tickers.py
+-rw-r--r--   0        0        0    14204 2024-05-14 16:50:58.417056 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_spot_exposures.py
+-rw-r--r--   0        0        0    14533 2024-05-14 16:50:58.417039 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_spot_exposures_by_strike.py
+-rw-r--r--   0        0        0     6448 2024-05-14 16:50:58.416964 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_volatility_term_structure.py
+-rw-r--r--   0        0        0     7214 2024-05-14 16:50:58.422733 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_volume_by_price_level.py
+-rw-r--r--   0        0        0     6097 2024-05-14 16:50:58.423065 unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_volume_open_interest_by_expiry.py
+-rw-r--r--   0        0        0     7122 2024-05-13 00:28:35.664213 unusualwhales_python_client-5.0.1/unusualwhales/client.py
+-rw-r--r--   0        0        0      546 2024-05-05 22:58:01.816143 unusualwhales_python_client-5.0.1/unusualwhales/errors.py
+-rw-r--r--   0        0        0     6148 2024-05-17 18:14:11.372403 unusualwhales_python_client-5.0.1/unusualwhales/models/.DS_Store
+-rw-r--r--   0        0        0    10021 2024-05-05 22:58:01.822073 unusualwhales_python_client-5.0.1/unusualwhales/models/__init__.py
+-rw-r--r--   0        0        0     2227 2024-05-05 22:58:01.823494 unusualwhales_python_client-5.0.1/unusualwhales/models/analalyst_rating_results.py
+-rw-r--r--   0        0        0      262 2024-05-05 22:58:01.779003 unusualwhales_python_client-5.0.1/unusualwhales/models/analyst_action.py
+-rw-r--r--   0        0        0      267 2024-05-05 22:58:01.779493 unusualwhales_python_client-5.0.1/unusualwhales/models/analyst_field_action.py
+-rw-r--r--   0        0        0      183 2024-05-05 22:58:01.758542 unusualwhales_python_client-5.0.1/unusualwhales/models/analyst_field_recommendation.py
+-rw-r--r--   0        0        0     6697 2024-05-05 22:58:01.820117 unusualwhales_python_client-5.0.1/unusualwhales/models/analyst_rating.py
+-rw-r--r--   0        0        0      178 2024-05-05 22:58:01.765008 unusualwhales_python_client-5.0.1/unusualwhales/models/analyst_recommendation.py
+-rw-r--r--   0        0        0      428 2024-05-05 22:58:01.775125 unusualwhales_python_client-5.0.1/unusualwhales/models/analyst_sector.py
+-rw-r--r--   0        0        0     5389 2024-05-14 17:46:09.508744 unusualwhales_python_client-5.0.1/unusualwhales/models/candle_data.py
+-rw-r--r--   0        0        0     2098 2024-05-05 22:58:01.833898 unusualwhales_python_client-5.0.1/unusualwhales/models/candle_data_results.py
+-rw-r--r--   0        0        0      251 2024-05-05 22:58:01.780257 unusualwhales_python_client-5.0.1/unusualwhales/models/candle_size.py
+-rw-r--r--   0        0        0     5755 2024-05-05 22:58:01.816560 unusualwhales_python_client-5.0.1/unusualwhales/models/congressional_trade_report.py
+-rw-r--r--   0        0        0     2308 2024-05-05 22:58:01.833569 unusualwhales_python_client-5.0.1/unusualwhales/models/congressional_trade_report_results.py
+-rw-r--r--   0        0        0     5235 2024-05-05 22:58:01.830332 unusualwhales_python_client-5.0.1/unusualwhales/models/country_sector_exposure.py
+-rw-r--r--   0        0        0     3869 2024-05-05 22:58:01.828297 unusualwhales_python_client-5.0.1/unusualwhales/models/daily_market_tide.py
+-rw-r--r--   0        0        0     2240 2024-05-05 22:58:01.833609 unusualwhales_python_client-5.0.1/unusualwhales/models/daily_market_tide_response.py
+-rw-r--r--   0        0        0     9770 2024-05-05 22:58:01.832534 unusualwhales_python_client-5.0.1/unusualwhales/models/darkpool_trade.py
+-rw-r--r--   0        0        0     3375 2024-05-05 22:58:01.818843 unusualwhales_python_client-5.0.1/unusualwhales/models/darkpool_trade_response.py
+-rw-r--r--   0        0        0     8924 2024-05-05 22:58:01.834330 unusualwhales_python_client-5.0.1/unusualwhales/models/earnings.py
+-rw-r--r--   0        0        0     2069 2024-05-05 22:58:01.833907 unusualwhales_python_client-5.0.1/unusualwhales/models/earnings_results.py
+-rw-r--r--   0        0        0     4185 2024-05-05 22:58:01.823207 unusualwhales_python_client-5.0.1/unusualwhales/models/economic_calendar.py
+-rw-r--r--   0        0        0      189 2024-05-05 22:58:01.783710 unusualwhales_python_client-5.0.1/unusualwhales/models/economic_type.py
+-rw-r--r--   0        0        0     2673 2024-05-05 22:58:01.820875 unusualwhales_python_client-5.0.1/unusualwhales/models/error_message.py
+-rw-r--r--   0        0        0     1779 2024-05-05 22:58:01.822650 unusualwhales_python_client-5.0.1/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py
+-rw-r--r--   0        0        0     2063 2024-05-05 22:58:01.825400 unusualwhales_python_client-5.0.1/unusualwhales/models/etf_countries_item.py
+-rw-r--r--   0        0        0     3171 2024-05-05 22:58:01.822868 unusualwhales_python_client-5.0.1/unusualwhales/models/etf_info.py
+-rw-r--r--   0        0        0     6423 2024-05-05 22:58:01.832037 unusualwhales_python_client-5.0.1/unusualwhales/models/etf_info_data.py
+-rw-r--r--   0        0        0     2044 2024-05-05 22:58:01.818548 unusualwhales_python_client-5.0.1/unusualwhales/models/etf_sectors_item.py
+-rw-r--r--   0        0        0     2953 2024-05-05 22:58:01.832447 unusualwhales_python_client-5.0.1/unusualwhales/models/expiry_breakdown.py
+-rw-r--r--   0        0        0     2248 2024-05-05 22:58:01.825125 unusualwhales_python_client-5.0.1/unusualwhales/models/expiry_breakdown_result.py
+-rw-r--r--   0        0        0     5086 2024-05-05 22:58:01.817753 unusualwhales_python_client-5.0.1/unusualwhales/models/fda_calendar.py
+-rw-r--r--   0        0        0    10635 2024-05-05 22:58:01.817394 unusualwhales_python_client-5.0.1/unusualwhales/models/flow_alert.py
+-rw-r--r--   0        0        0     2086 2024-05-05 22:58:01.816655 unusualwhales_python_client-5.0.1/unusualwhales/models/flow_alert_results.py
+-rw-r--r--   0        0        0      590 2024-05-05 22:58:01.780015 unusualwhales_python_client-5.0.1/unusualwhales/models/flow_alert_rule.py
+-rw-r--r--   0        0        0    12800 2024-05-05 22:58:01.827106 unusualwhales_python_client-5.0.1/unusualwhales/models/flow_per_expiry.py
+-rw-r--r--   0        0        0     2139 2024-05-05 22:58:01.827194 unusualwhales_python_client-5.0.1/unusualwhales/models/flow_per_expiry_results.py
+-rw-r--r--   0        0        0    12688 2024-05-05 22:58:01.819326 unusualwhales_python_client-5.0.1/unusualwhales/models/flow_per_strike.py
+-rw-r--r--   0        0        0     2139 2024-05-05 22:58:01.830018 unusualwhales_python_client-5.0.1/unusualwhales/models/flow_per_strike_results.py
+-rw-r--r--   0        0        0     6320 2024-05-05 22:58:01.816924 unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure.py
+-rw-r--r--   0        0        0     6349 2024-05-05 22:58:01.822486 unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_by_strike.py
+-rw-r--r--   0        0        0     6808 2024-05-05 22:58:01.831535 unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_by_strike_and_expiry.py
+-rw-r--r--   0        0        0     2358 2024-05-05 22:58:01.821530 unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_by_strike_and_expiry_results.py
+-rw-r--r--   0        0        0     2240 2024-05-05 22:58:01.827851 unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_by_strike_results.py
+-rw-r--r--   0        0        0     2134 2024-05-05 22:58:01.816486 unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_results.py
+-rw-r--r--   0        0        0     9046 2024-05-05 22:58:01.826947 unusualwhales_python_client-5.0.1/unusualwhales/models/greeks.py
+-rw-r--r--   0        0        0     2535 2024-05-05 22:58:01.829764 unusualwhales_python_client-5.0.1/unusualwhales/models/historical_risk_reversal_skew.py
+-rw-r--r--   0        0        0     2300 2024-05-05 22:58:01.822832 unusualwhales_python_client-5.0.1/unusualwhales/models/historical_risk_reversal_skew_results.py
+-rw-r--r--   0        0        0     8935 2024-05-05 22:58:01.817484 unusualwhales_python_client-5.0.1/unusualwhales/models/holdings.py
+-rw-r--r--   0        0        0     2648 2024-05-05 22:58:01.821969 unusualwhales_python_client-5.0.1/unusualwhales/models/holdings_response.py
+-rw-r--r--   0        0        0     4229 2024-05-05 22:58:01.818954 unusualwhales_python_client-5.0.1/unusualwhales/models/imbalances_volume.py
+-rw-r--r--   0        0        0     4234 2024-05-05 22:58:01.831021 unusualwhales_python_client-5.0.1/unusualwhales/models/implied_volatility_term_structure.py
+-rw-r--r--   0        0        0     2348 2024-05-05 22:58:01.822055 unusualwhales_python_client-5.0.1/unusualwhales/models/implied_volatility_term_structure_results.py
+-rw-r--r--   0        0        0     3185 2024-05-05 22:58:01.834435 unusualwhales_python_client-5.0.1/unusualwhales/models/insider_statistic.py
+-rw-r--r--   0        0        0     2770 2024-05-05 22:58:01.816314 unusualwhales_python_client-5.0.1/unusualwhales/models/insider_statistics.py
+-rw-r--r--   0        0        0      190 2024-05-05 22:58:01.766259 unusualwhales_python_client-5.0.1/unusualwhales/models/insider_trades_member_type.py
+-rw-r--r--   0        0        0      345 2024-05-05 22:58:01.775861 unusualwhales_python_client-5.0.1/unusualwhales/models/insider_trades_transaction_type.py
+-rw-r--r--   0        0        0      164 2024-05-05 22:58:01.778813 unusualwhales_python_client-5.0.1/unusualwhales/models/market_general_imbalance_event.py
+-rw-r--r--   0        0        0      165 2024-05-05 22:58:01.783423 unusualwhales_python_client-5.0.1/unusualwhales/models/market_general_imbalance_side.py
+-rw-r--r--   0        0        0      213 2024-05-05 22:58:01.776228 unusualwhales_python_client-5.0.1/unusualwhales/models/market_general_imbalance_type.py
+-rw-r--r--   0        0        0      168 2024-05-05 22:58:01.773079 unusualwhales_python_client-5.0.1/unusualwhales/models/market_general_market_time.py
+-rw-r--r--   0        0        0      528 2024-05-05 22:58:01.774624 unusualwhales_python_client-5.0.1/unusualwhales/models/market_general_sector.py
+-rw-r--r--   0        0        0     4512 2024-05-05 22:58:01.834484 unusualwhales_python_client-5.0.1/unusualwhales/models/market_holidays.py
+-rw-r--r--   0        0        0     3378 2024-05-05 22:58:01.831296 unusualwhales_python_client-5.0.1/unusualwhales/models/market_options_volume.py
+-rw-r--r--   0        0        0     1710 2024-05-05 22:58:01.827677 unusualwhales_python_client-5.0.1/unusualwhales/models/market_sector_ticker_results.py
+-rw-r--r--   0        0        0     2535 2024-05-05 22:58:01.830420 unusualwhales_python_client-5.0.1/unusualwhales/models/max_pain.py
+-rw-r--r--   0        0        0     2159 2024-05-05 22:58:01.833744 unusualwhales_python_client-5.0.1/unusualwhales/models/max_pain_results.py
+-rw-r--r--   0        0        0     3421 2024-05-05 22:58:01.833406 unusualwhales_python_client-5.0.1/unusualwhales/models/net_prem_tick.py
+-rw-r--r--   0        0        0     4303 2024-05-05 22:58:01.828862 unusualwhales_python_client-5.0.1/unusualwhales/models/net_prem_tick_results.py
+-rw-r--r--   0        0        0     2494 2024-05-05 22:58:01.821207 unusualwhales_python_client-5.0.1/unusualwhales/models/off_lit_price_level.py
+-rw-r--r--   0        0        0     2270 2024-05-05 22:58:01.816343 unusualwhales_python_client-5.0.1/unusualwhales/models/off_lit_price_level_results.py
+-rw-r--r--   0        0        0    11261 2024-05-05 22:58:01.823477 unusualwhales_python_client-5.0.1/unusualwhales/models/oi_change.py
+-rw-r--r--   0        0        0     2101 2024-05-05 22:58:01.828752 unusualwhales_python_client-5.0.1/unusualwhales/models/oi_change_results.py
+-rw-r--r--   0        0        0    10954 2024-05-05 22:58:01.817830 unusualwhales_python_client-5.0.1/unusualwhales/models/option_chain_contract.py
+-rw-r--r--   0        0        0     2316 2024-05-05 22:58:01.818322 unusualwhales_python_client-5.0.1/unusualwhales/models/option_chain_contract_results.py
+-rw-r--r--   0        0        0     2187 2024-05-05 22:58:01.818071 unusualwhales_python_client-5.0.1/unusualwhales/models/option_chains_results.py
+-rw-r--r--   0        0        0    11275 2024-05-05 22:58:01.818618 unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract.py
+-rw-r--r--   0        0        0     2251 2024-05-05 22:58:01.829762 unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract_results.py
+-rw-r--r--   0        0        0    14866 2024-05-05 22:58:01.824112 unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract_screener_item.py
+-rw-r--r--   0        0        0     2375 2024-05-05 22:58:01.831061 unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract_screener_results.py
+-rw-r--r--   0        0        0      157 2024-05-05 22:58:01.768374 unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract_type.py
+-rw-r--r--   0        0        0     2522 2024-05-05 22:58:01.825820 unusualwhales_python_client-5.0.1/unusualwhales/models/option_price_level.py
+-rw-r--r--   0        0        0     2283 2024-05-05 22:58:01.827958 unusualwhales_python_client-5.0.1/unusualwhales/models/option_price_level_results.py
+-rw-r--r--   0        0        0      149 2024-05-05 22:58:01.770159 unusualwhales_python_client-5.0.1/unusualwhales/models/option_type.py
+-rw-r--r--   0        0        0      153 2024-05-05 22:58:01.771290 unusualwhales_python_client-5.0.1/unusualwhales/models/order_direction.py
+-rw-r--r--   0        0        0      949 2024-05-05 22:58:01.774812 unusualwhales_python_client-5.0.1/unusualwhales/models/screener_contract_order_by_field.py
+-rw-r--r--   0        0        0     1401 2024-05-05 22:58:01.780126 unusualwhales_python_client-5.0.1/unusualwhales/models/screener_order_by_field.py
+-rw-r--r--   0        0        0     5330 2024-05-05 22:58:01.832188 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_market.py
+-rw-r--r--   0        0        0     2245 2024-05-05 22:58:01.817561 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_market_results.py
+-rw-r--r--   0        0        0     4802 2024-05-05 22:58:01.826952 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_monthly.py
+-rw-r--r--   0        0        0     2864 2024-05-05 22:58:01.816371 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_monthly_results.py
+-rw-r--r--   0        0        0      412 2024-05-05 22:58:01.784552 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_performance_order_by.py
+-rw-r--r--   0        0        0     6634 2024-05-05 22:58:01.820876 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_performers.py
+-rw-r--r--   0        0        0     2884 2024-05-05 22:58:01.822592 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_performers_results.py
+-rw-r--r--   0        0        0     2957 2024-05-05 22:58:01.827974 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_year_month.py
+-rw-r--r--   0        0        0     3159 2024-05-05 22:58:01.828370 unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_year_month_results.py
+-rw-r--r--   0        0        0      515 2024-05-05 22:58:01.783541 unusualwhales_python_client-5.0.1/unusualwhales/models/sector.py
+-rw-r--r--   0        0        0    10830 2024-05-05 22:58:01.830188 unusualwhales_python_client-5.0.1/unusualwhales/models/sector_etf.py
+-rw-r--r--   0        0        0     2890 2024-05-05 22:58:01.823726 unusualwhales_python_client-5.0.1/unusualwhales/models/sector_etf_results.py
+-rw-r--r--   0        0        0      173 2024-05-05 22:58:01.769865 unusualwhales_python_client-5.0.1/unusualwhales/models/side.py
+-rw-r--r--   0        0        0      206 2024-05-05 22:58:01.776708 unusualwhales_python_client-5.0.1/unusualwhales/models/single_issue_type.py
+-rw-r--r--   0        0        0      343 2024-05-05 22:58:01.762014 unusualwhales_python_client-5.0.1/unusualwhales/models/single_month_number.py
+-rw-r--r--   0        0        0      521 2024-05-05 22:58:01.779594 unusualwhales_python_client-5.0.1/unusualwhales/models/single_sector.py
+-rw-r--r--   0        0        0      334 2024-05-05 22:58:01.769228 unusualwhales_python_client-5.0.1/unusualwhales/models/single_trade_external_hour_sold_code.py
+-rw-r--r--   0        0        0      312 2024-05-05 22:58:01.761864 unusualwhales_python_client-5.0.1/unusualwhales/models/single_trade_sale_cond_code.py
+-rw-r--r--   0        0        0      304 2024-05-05 22:58:01.781307 unusualwhales_python_client-5.0.1/unusualwhales/models/single_trade_settlement.py
+-rw-r--r--   0        0        0      275 2024-05-05 22:58:01.752668 unusualwhales_python_client-5.0.1/unusualwhales/models/single_trade_trade_code.py
+-rw-r--r--   0        0        0     2304 2024-05-05 22:58:01.832942 unusualwhales_python_client-5.0.1/unusualwhales/models/spike_value.py
+-rw-r--r--   0        0        0     7769 2024-05-05 22:58:01.832634 unusualwhales_python_client-5.0.1/unusualwhales/models/spot_gex_exposures_per_1_min.py
+-rw-r--r--   0        0        0     2274 2024-05-05 22:58:01.833460 unusualwhales_python_client-5.0.1/unusualwhales/models/spot_gex_exposures_per_1_min_results.py
+-rw-r--r--   0        0        0     8339 2024-05-05 22:58:01.833587 unusualwhales_python_client-5.0.1/unusualwhales/models/spot_greek_exposures_by_strike.py
+-rw-r--r--   0        0        0     2305 2024-05-05 22:58:01.817337 unusualwhales_python_client-5.0.1/unusualwhales/models/spot_greek_exposures_by_strike_results.py
+-rw-r--r--   0        0        0      202 2024-05-05 22:58:01.756301 unusualwhales_python_client-5.0.1/unusualwhales/models/stock_earnings_time.py
+-rw-r--r--   0        0        0      205 2024-05-05 22:58:01.779639 unusualwhales_python_client-5.0.1/unusualwhales/models/stock_issue_type.py
+-rw-r--r--   0        0        0    24207 2024-05-05 22:58:01.822193 unusualwhales_python_client-5.0.1/unusualwhales/models/stock_screener_response.py
+-rw-r--r--   0        0        0     2280 2024-05-05 22:58:01.823614 unusualwhales_python_client-5.0.1/unusualwhales/models/stock_screener_response_results.py
+-rw-r--r--   0        0        0     8648 2024-05-05 22:58:01.828620 unusualwhales_python_client-5.0.1/unusualwhales/models/ticker_info.py
+-rw-r--r--   0        0        0     2636 2024-05-05 22:58:01.831049 unusualwhales_python_client-5.0.1/unusualwhales/models/ticker_info_results.py
+-rw-r--r--   0        0        0    11609 2024-05-05 22:58:01.832705 unusualwhales_python_client-5.0.1/unusualwhales/models/ticker_options_volume.py
+-rw-r--r--   0        0        0     2436 2024-05-05 22:58:01.828948 unusualwhales_python_client-5.0.1/unusualwhales/models/volume_oi_per_expiry.py
+-rw-r--r--   0        0        0     2233 2024-05-05 22:58:01.816470 unusualwhales_python_client-5.0.1/unusualwhales/models/volume_oi_per_expiry_results.py
+-rw-r--r--   0        0        0       25 2024-05-05 22:58:01.341037 unusualwhales_python_client-5.0.1/unusualwhales/py.typed
+-rw-r--r--   0        0        0      985 2024-05-05 22:58:01.827475 unusualwhales_python_client-5.0.1/unusualwhales/types.py
+-rw-r--r--   0        0        0     3744 1970-01-01 00:00:00.000000 unusualwhales_python_client-5.0.1/PKG-INFO
```

### Comparing `unusualwhales_python_client-4.2.3/LICENSE` & `unusualwhales_python_client-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/README.md` & `unusualwhales_python_client-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/pyproject.toml` & `unusualwhales_python_client-5.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "unusualwhales-python-client"
-version = "4.2.3"
+version = "5.0.1"
 description = "A client library for accessing Unusual Whales API"
 authors = ["Mac Anderson <mac@macanderson.com>"]
 readme = "README.md"
 packages = [{ include = "unusualwhales" }]
 include = ["unusualwhales/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 httpx = ">=0.20.0,<0.28.0"
-attrs = "^21.3.0"
+attrs = "^23.2.0"
 python-dateutil = "^2.8.0"
 python-dotenv = "^0.21.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/.DS_Store` & `unusualwhales_python_client-5.0.1/unusualwhales/.DS_Store`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/.DS_Store` & `unusualwhales_python_client-5.0.1/unusualwhales/api/.DS_Store`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/congress/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/congress/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/congress/get_late_reports.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/congress/get_late_reports.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/congress/get_reports.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/congress/get_reports.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/congress/get_trades.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/congress/get_trades.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/congress/get_trades_by_member.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/congress/get_trades_by_member.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/contract/get_price_history.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/contract/get_price_history.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/darkpool/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/darkpool/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/darkpool/get_trades_by_date.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/darkpool/get_trades_by_date.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/darkpool/get_trades_by_ticker.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/darkpool/get_trades_by_ticker.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/earnings/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/earnings/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/earnings/get_afterhours.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/earnings/get_afterhours.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/earnings/get_premarket.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/earnings/get_premarket.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/earnings/get_ticker_earnings.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/earnings/get_ticker_earnings.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/endpoints.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/get_holdings.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/get_holdings.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/get_info.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/get_info.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/get_sector_country_weights.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/get_sector_country_weights.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/etfs/get_ticker_exposure.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/etfs/get_ticker_exposure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/flow/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_contract_flow.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_contract_flow.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_flow_by_expiry.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_flow_by_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_flow_by_strike.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_flow_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_full_tape.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_full_tape.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_order_flow.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_order_flow.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_ticker_order_flow.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_ticker_order_flow.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/flow/get_unusual_flow_alerts.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/flow/get_unusual_flow_alerts.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_economic_calendar.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_economic_calendar.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_fda_calendar.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_fda_calendar.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_holidays.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_holidays.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_imbalances.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_imbalances.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_insider_trades.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_insider_trades.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_market_options_volume.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_market_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_market_tide.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_market_tide.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_market_tide_by_etf.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_market_tide_by_etf.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_open_interest_change.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_open_interest_change.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_sector_stats.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_sector_stats.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/market/get_spike.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/market/get_spike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/screener/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/screener/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/screener/get_analyst_ratings.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/screener/get_analyst_ratings.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/screener/get_option_contracts.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/screener/get_option_contracts.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/screener/get_stocks.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/screener/get_stocks.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/get_market_average_returns_by_month.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/get_market_average_returns_by_month.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/get_monthly_average_returns.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/get_monthly_average_returns.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/get_monthly_top_performers.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/get_monthly_top_performers.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/seasonality/get_price_changes_by_month_and_year.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_atm_option_contracts_for_expiries.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_atm_option_contracts_for_expiries.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_candles.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_candles.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_daily_expiry_breakdown.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_daily_expiry_breakdown.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greek_exposure.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greek_exposure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greek_exposure_by_expiry.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greek_exposure_by_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greek_exposure_by_strike.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greek_exposure_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greek_exposure_by_strike_expiry.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greek_exposure_by_strike_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_greeks_by_strike_expiry.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_greeks_by_strike_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_info.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_info.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_insider_trades.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_insider_trades.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_max_pain.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_max_pain.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_net_premium_ticks.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_net_premium_ticks.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_open_interest_change.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_open_interest_change.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_option_chains.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_option_chains.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_option_contracts.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_option_contracts.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_option_volume_by_price_level.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_option_volume_by_price_level.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_options_volume.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_risk_reversal_skew.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_risk_reversal_skew.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_sector_tickers.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_sector_tickers.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_spot_exposures.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_spot_exposures.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_spot_exposures_by_strike.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_spot_exposures_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_volatility_term_structure.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_volatility_term_structure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_volume_by_price_level.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_volume_by_price_level.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/api/stock/get_volume_open_interest_by_expiry.py` & `unusualwhales_python_client-5.0.1/unusualwhales/api/stock/get_volume_open_interest_by_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/client.py` & `unusualwhales_python_client-5.0.1/unusualwhales/client.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/errors.py` & `unusualwhales_python_client-5.0.1/unusualwhales/errors.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/.DS_Store` & `unusualwhales_python_client-5.0.1/unusualwhales/models/.DS_Store`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/__init__.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/__init__.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/analalyst_rating_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/analalyst_rating_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/analyst_rating.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/analyst_rating.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/candle_data.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/candle_data.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/candle_data_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/candle_data_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/congressional_trade_report.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/congressional_trade_report.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/congressional_trade_report_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/congressional_trade_report_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/country_sector_exposure.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/country_sector_exposure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/daily_market_tide.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/daily_market_tide.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/daily_market_tide_response.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/daily_market_tide_response.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/darkpool_trade.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/darkpool_trade.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/darkpool_trade_response.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/darkpool_trade_response.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/earnings.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/earnings.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/earnings_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/earnings_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/economic_calendar.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/error_message.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/error_message.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/error_message_stating_that_the_requested_element_was_not_found_causing_an_empty_result_to_be_generated.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/etf_countries_item.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/etf_countries_item.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/etf_info.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/etf_info_data.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/etf_info_data.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/etf_sectors_item.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/etf_sectors_item.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/expiry_breakdown.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/expiry_breakdown.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/expiry_breakdown_result.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/expiry_breakdown_result.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/fda_calendar.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/fda_calendar.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/flow_alert.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/flow_alert.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/flow_alert_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/flow_alert_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/flow_alert_rule.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/flow_alert_rule.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/flow_per_expiry.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/flow_per_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/flow_per_expiry_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/flow_per_expiry_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/flow_per_strike.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/flow_per_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/flow_per_strike_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/flow_per_strike_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_by_strike.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_by_strike_and_expiry.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_by_strike_and_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_by_strike_and_expiry_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_by_strike_and_expiry_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_by_strike_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_by_strike_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/greek_exposure_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/greek_exposure_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/greeks.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/greeks.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/historical_risk_reversal_skew.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/historical_risk_reversal_skew.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/historical_risk_reversal_skew_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/historical_risk_reversal_skew_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/holdings.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/holdings.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/holdings_response.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/holdings_response.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/imbalances_volume.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/imbalances_volume.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/implied_volatility_term_structure.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/implied_volatility_term_structure.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/implied_volatility_term_structure_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/implied_volatility_term_structure_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/insider_statistic.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/insider_statistic.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/insider_statistics.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/insider_statistics.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/market_general_sector.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/market_general_sector.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/market_holidays.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/market_holidays.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/market_options_volume.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/market_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/market_sector_ticker_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/market_sector_ticker_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/max_pain.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/max_pain.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/max_pain_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/max_pain_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/net_prem_tick.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/net_prem_tick.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/net_prem_tick_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/net_prem_tick_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/off_lit_price_level.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/off_lit_price_level.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/off_lit_price_level_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/off_lit_price_level_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/oi_change.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/oi_change.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/oi_change_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/oi_change_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_chain_contract.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_chain_contract.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_chain_contract_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_chain_contract_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_chains_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_chains_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract_screener_item.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract_screener_item.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_contract_screener_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_contract_screener_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_price_level.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_price_level.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/option_price_level_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/option_price_level_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/screener_contract_order_by_field.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/screener_contract_order_by_field.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/screener_order_by_field.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/screener_order_by_field.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_market.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_market.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_market_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_market_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_monthly.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_monthly.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_monthly_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_monthly_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_performers.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_performers.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_performers_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_performers_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_year_month.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_year_month.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/seasonality_year_month_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/seasonality_year_month_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/sector.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/sector.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/sector_etf.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/sector_etf.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/sector_etf_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/sector_etf_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/single_sector.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/single_sector.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/spike_value.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/spike_value.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/spot_gex_exposures_per_1_min.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/spot_gex_exposures_per_1_min.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/spot_gex_exposures_per_1_min_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/spot_gex_exposures_per_1_min_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/spot_greek_exposures_by_strike.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/spot_greek_exposures_by_strike.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/spot_greek_exposures_by_strike_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/spot_greek_exposures_by_strike_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/stock_screener_response.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/stock_screener_response.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/stock_screener_response_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/stock_screener_response_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/ticker_info.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/ticker_info.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/ticker_info_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/ticker_info_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/ticker_options_volume.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/ticker_options_volume.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/volume_oi_per_expiry.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/volume_oi_per_expiry.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/models/volume_oi_per_expiry_results.py` & `unusualwhales_python_client-5.0.1/unusualwhales/models/volume_oi_per_expiry_results.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/unusualwhales/types.py` & `unusualwhales_python_client-5.0.1/unusualwhales/types.py`

 * *Files identical despite different names*

### Comparing `unusualwhales_python_client-4.2.3/PKG-INFO` & `unusualwhales_python_client-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: unusualwhales-python-client
-Version: 4.2.3
+Version: 5.0.1
 Summary: A client library for accessing Unusual Whales API
 Author: Mac Anderson
 Author-email: mac@macanderson.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: attrs (>=21.3.0,<22.0.0)
+Requires-Dist: attrs (>=23.2.0,<24.0.0)
 Requires-Dist: httpx (>=0.20.0,<0.28.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Description-Content-Type: text/markdown
 
 # unusual-whales-api-client
 A client library for accessing Unusual Whales API
```

