# Comparing `tmp/openbb-4.2.0.tar.gz` & `tmp/openbb-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb-4.2.0.tar", max compression
+gzip compressed data, was "openbb-4.2.1.tar", max compression
```

## Comparing `openbb-4.2.0.tar` & `openbb-4.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     6831 2024-05-14 15:30:05.603784 openbb-4.2.0/README.md
--rw-r--r--   0        0        0     1440 2024-04-19 16:15:24.596053 openbb-4.2.0/openbb/__init__.py
--rw-r--r--   0        0        0  1388724 2024-05-15 16:52:56.040988 openbb-4.2.0/openbb/assets/reference.json
--rw-r--r--   0        0        0     2813 2024-05-15 16:52:58.371668 openbb-4.2.0/openbb/package/__extensions__.py
--rw-r--r--   0        0        0     3213 2024-05-15 16:52:59.077314 openbb-4.2.0/openbb/package/crypto.py
--rw-r--r--   0        0        0     6510 2024-05-15 16:52:59.094288 openbb-4.2.0/openbb/package/crypto_price.py
--rw-r--r--   0        0        0    12781 2024-05-15 16:52:59.125206 openbb-4.2.0/openbb/package/currency.py
--rw-r--r--   0        0        0     6406 2024-05-15 16:52:59.082143 openbb-4.2.0/openbb/package/currency_price.py
--rw-r--r--   0        0        0      770 2024-05-15 16:52:59.060809 openbb-4.2.0/openbb/package/derivatives.py
--rw-r--r--   0        0        0    11875 2024-05-15 16:52:59.131890 openbb-4.2.0/openbb/package/derivatives_options.py
--rw-r--r--   0        0        0    66004 2024-05-15 16:52:59.861868 openbb-4.2.0/openbb/package/economy.py
--rw-r--r--   0        0        0    12211 2024-05-15 16:52:59.249552 openbb-4.2.0/openbb/package/economy_gdp.py
--rw-r--r--   0        0        0    27499 2024-05-15 16:52:59.257403 openbb-4.2.0/openbb/package/equity.py
--rw-r--r--   0        0        0    17987 2024-05-15 16:52:59.258884 openbb-4.2.0/openbb/package/equity_calendar.py
--rw-r--r--   0        0        0     2721 2024-05-15 16:52:59.116699 openbb-4.2.0/openbb/package/equity_compare.py
--rw-r--r--   0        0        0    25269 2024-05-15 16:52:59.456686 openbb-4.2.0/openbb/package/equity_discovery.py
--rw-r--r--   0        0        0    44027 2024-05-15 16:52:59.509604 openbb-4.2.0/openbb/package/equity_estimates.py
--rw-r--r--   0        0        0   162443 2024-05-15 16:53:00.068053 openbb-4.2.0/openbb/package/equity_fundamental.py
--rw-r--r--   0        0        0    30003 2024-05-15 16:52:59.366405 openbb-4.2.0/openbb/package/equity_ownership.py
--rw-r--r--   0        0        0    26567 2024-05-15 16:52:59.322870 openbb-4.2.0/openbb/package/equity_price.py
--rw-r--r--   0        0        0     3624 2024-05-15 16:52:59.207330 openbb-4.2.0/openbb/package/equity_shorts.py
--rw-r--r--   0        0        0    74919 2024-05-15 16:52:59.792912 openbb-4.2.0/openbb/package/etf.py
--rw-r--r--   0        0        0     4432 2024-05-15 16:52:59.314458 openbb-4.2.0/openbb/package/fixedincome.py
--rw-r--r--   0        0        0    19184 2024-05-15 16:52:59.699814 openbb-4.2.0/openbb/package/fixedincome_corporate.py
--rw-r--r--   0        0        0     6895 2024-05-15 16:52:59.394971 openbb-4.2.0/openbb/package/fixedincome_government.py
--rw-r--r--   0        0        0    25497 2024-05-15 16:52:59.810160 openbb-4.2.0/openbb/package/fixedincome_rate.py
--rw-r--r--   0        0        0    10713 2024-05-15 16:52:59.603344 openbb-4.2.0/openbb/package/fixedincome_spreads.py
--rw-r--r--   0        0        0    11652 2024-05-15 16:52:59.626851 openbb-4.2.0/openbb/package/index.py
--rw-r--r--   0        0        0    20686 2024-05-15 16:52:59.695594 openbb-4.2.0/openbb/package/news.py
--rw-r--r--   0        0        0      458 2024-05-15 16:52:58.380378 openbb-4.2.0/openbb/package/regulators.py
--rw-r--r--   0        0        0        0 2024-04-19 16:15:24.603580 openbb-4.2.0/openbb/py.typed
--rw-r--r--   0        0        0     2913 2024-05-15 16:21:25.260535 openbb-4.2.0/pyproject.toml
--rw-r--r--   0        0        0    10428 1970-01-01 00:00:00.000000 openbb-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     6831 2024-05-15 09:21:56.017885 openbb-4.2.1/README.md
+-rw-r--r--   0        0        0     1440 2024-05-14 16:56:41.653864 openbb-4.2.1/openbb/__init__.py
+-rw-r--r--   0        0        0  1450111 2024-05-22 13:45:28.101437 openbb-4.2.1/openbb/assets/reference.json
+-rw-r--r--   0        0        0     2813 2024-05-22 13:45:28.125437 openbb-4.2.1/openbb/package/__extensions__.py
+-rw-r--r--   0        0        0     3299 2024-05-22 13:45:28.333438 openbb-4.2.1/openbb/package/crypto.py
+-rw-r--r--   0        0        0     6510 2024-05-22 13:45:28.349438 openbb-4.2.1/openbb/package/crypto_price.py
+-rw-r--r--   0        0        0    12909 2024-05-22 13:45:28.365438 openbb-4.2.1/openbb/package/currency.py
+-rw-r--r--   0        0        0     6402 2024-05-22 13:45:28.349438 openbb-4.2.1/openbb/package/currency_price.py
+-rw-r--r--   0        0        0      770 2024-05-22 13:45:28.317438 openbb-4.2.1/openbb/package/derivatives.py
+-rw-r--r--   0        0        0    12062 2024-05-22 13:45:28.361438 openbb-4.2.1/openbb/package/derivatives_options.py
+-rw-r--r--   0        0        0    72312 2024-05-22 13:45:28.709439 openbb-4.2.1/openbb/package/economy.py
+-rw-r--r--   0        0        0    12355 2024-05-22 13:45:28.405438 openbb-4.2.1/openbb/package/economy_gdp.py
+-rw-r--r--   0        0        0    27681 2024-05-22 13:45:28.453438 openbb-4.2.1/openbb/package/equity.py
+-rw-r--r--   0        0        0    18353 2024-05-22 13:45:28.461438 openbb-4.2.1/openbb/package/equity_calendar.py
+-rw-r--r--   0        0        0     8280 2024-05-22 13:45:28.397438 openbb-4.2.1/openbb/package/equity_compare.py
+-rw-r--r--   0        0        0    25823 2024-05-22 13:45:28.565439 openbb-4.2.1/openbb/package/equity_discovery.py
+-rw-r--r--   0        0        0    49838 2024-05-22 13:45:28.597439 openbb-4.2.1/openbb/package/equity_estimates.py
+-rw-r--r--   0        0        0   164143 2024-05-22 13:45:28.961440 openbb-4.2.1/openbb/package/equity_fundamental.py
+-rw-r--r--   0        0        0    30441 2024-05-22 13:45:28.521438 openbb-4.2.1/openbb/package/equity_ownership.py
+-rw-r--r--   0        0        0    26777 2024-05-22 13:45:28.545438 openbb-4.2.1/openbb/package/equity_price.py
+-rw-r--r--   0        0        0     3710 2024-05-22 13:45:28.501438 openbb-4.2.1/openbb/package/equity_shorts.py
+-rw-r--r--   0        0        0    71518 2024-05-22 13:45:28.673439 openbb-4.2.1/openbb/package/etf.py
+-rw-r--r--   0        0        0     4538 2024-05-22 13:45:28.541438 openbb-4.2.1/openbb/package/fixedincome.py
+-rw-r--r--   0        0        0    19482 2024-05-22 13:45:28.705439 openbb-4.2.1/openbb/package/fixedincome_corporate.py
+-rw-r--r--   0        0        0    11964 2024-05-22 13:45:28.693439 openbb-4.2.1/openbb/package/fixedincome_government.py
+-rw-r--r--   0        0        0    26229 2024-05-22 13:45:28.737439 openbb-4.2.1/openbb/package/fixedincome_rate.py
+-rw-r--r--   0        0        0    10857 2024-05-22 13:45:28.645439 openbb-4.2.1/openbb/package/fixedincome_spreads.py
+-rw-r--r--   0        0        0    11786 2024-05-22 13:45:28.681439 openbb-4.2.1/openbb/package/index.py
+-rw-r--r--   0        0        0    20834 2024-05-22 13:45:28.773439 openbb-4.2.1/openbb/package/news.py
+-rw-r--r--   0        0        0      458 2024-05-22 13:45:28.121437 openbb-4.2.1/openbb/package/regulators.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.665864 openbb-4.2.1/openbb/py.typed
+-rw-r--r--   0        0        0     2950 2024-05-22 14:02:31.404865 openbb-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10465 1970-01-01 00:00:00.000000 openbb-4.2.1/PKG-INFO
```

### Comparing `openbb-4.2.0/README.md` & `openbb-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openbb-4.2.0/openbb/__init__.py` & `openbb-4.2.1/openbb/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb-4.2.0/openbb/assets/reference.json` & `openbb-4.2.1/openbb/assets/reference.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.979479580578652%*

 * *Differences: {"'info'": "{'description': 'Investment research for everyone, anywhere.'}",*

 * * "'paths'": '{\'/currency/search\': {\'examples\': "\\nExamples\\n--------\\n\\n```python\\nfrom '*

 * *            "openbb import obb\\nobb.currency.search(provider='fmp')\\n# Search for 'EUR' currency "*

 * *            "pair using 'intrinio' as provider.\\nobb.currency.search(provider='intrinio', "*

 * *            "query='EUR')\\n# Search for terms  using 'polygon' as "*

 * *            'provider.\\nobb.currency.search(provider=\'polygon\', query= […]*

```diff
@@ -1,11 +1,11 @@
 {
     "info": {
         "core": "1.2.2",
-        "description": "This is the OpenBB Platform (Python).",
+        "description": "Investment research for everyone, anywhere.",
         "extensions": {
             "openbb_core_extension": [
                 "commodity@1.1.0",
                 "crypto@1.2.0",
                 "currency@1.2.0",
                 "derivatives@1.2.0",
                 "economy@1.2.0",
@@ -751,15 +751,15 @@
                 ]
             },
             "deprecated": {
                 "flag": null,
                 "message": null
             },
             "description": "Currency Search.\n\nSearch available currency pairs.\nCurrency pairs are the national currencies from two countries coupled for trading on\nthe foreign exchange (FX) marketplace.\nBoth currencies will have exchange rates on which the trade will have its position basis.\nAll trading within the forex market, whether selling, buying, or trading, will take place through currency pairs.\n(ref: Investopedia)\nMajor currency pairs include pairs such as EUR/USD, USD/JPY, GBP/USD, etc.",
-            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.currency.search(provider='fmp')\n# Search for 'EUR' currency pair using 'intrinio' as provider.\nobb.currency.search(provider='intrinio', query='EUR')\n# Search for terms  using 'polygon' as provider.\nobb.currency.search(provider='polygon', query='Euro zone')\n```\n\n",
+            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.currency.search(provider='fmp')\n# Search for 'EUR' currency pair using 'intrinio' as provider.\nobb.currency.search(provider='intrinio', query='EUR')\n# Search for terms  using 'polygon' as provider.\nobb.currency.search(provider='polygon', query='EUR')\n```\n\n",
             "model": "CurrencyPairs",
             "parameters": {
                 "fmp": [],
                 "intrinio": [],
                 "polygon": [],
                 "standard": [
                     {
@@ -1932,15 +1932,15 @@
                 ]
             },
             "deprecated": {
                 "flag": null,
                 "message": null
             },
             "description": "Get the complete options chain for a ticker.",
-            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.derivatives.options.unusual(provider='intrinio')\n# Use the 'symbol' parameter to get the most recent activity for a specific symbol.\nobb.derivatives.options.unusual(symbol='TSLA', provider='intrinio')\n```\n\n",
+            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.derivatives.options.unusual(symbol='TSLA', provider='intrinio')\n# Use the 'symbol' parameter to get the most recent activity for a specific symbol.\nobb.derivatives.options.unusual(symbol='TSLA', provider='intrinio')\n```\n\n",
             "model": "OptionsUnusual",
             "parameters": {
                 "intrinio": [
                     {
                         "choices": null,
                         "default": null,
                         "description": "Start date of the data, in YYYY-MM-DD format. If no symbol is supplied, requests are only allowed for a single date. Use the start_date for the target date. Intrinio appears to have data beginning Feb/2022, but is unclear when it actually began.",
@@ -2226,14 +2226,262 @@
                         "description": "Extra info.",
                         "name": "extra",
                         "type": "Dict[str, Any]"
                     }
                 ]
             }
         },
+        "/economy/balance_of_payments": {
+            "data": {
+                "fred": [],
+                "standard": [
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The date representing the beginning of the reporting period.",
+                        "name": "period",
+                        "optional": true,
+                        "type": "date"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Balance as Percent of GDP",
+                        "name": "balance_percent_of_gdp",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Total Balance (USD)",
+                        "name": "balance_total",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Total Services Balance (USD)",
+                        "name": "balance_total_services",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Total Secondary Income Balance (USD)",
+                        "name": "balance_total_secondary_income",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Total Goods Balance (USD)",
+                        "name": "balance_total_goods",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Total Primary Income Balance (USD)",
+                        "name": "balance_total_primary_income",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Credits Services as Percent of Goods and Services",
+                        "name": "credits_services_percent_of_goods_and_services",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Credits Services as Percent of Current Account",
+                        "name": "credits_services_percent_of_current_account",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Credits Total Services (USD)",
+                        "name": "credits_total_services",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Credits Total Goods (USD)",
+                        "name": "credits_total_goods",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Credits Total Primary Income (USD)",
+                        "name": "credits_total_primary_income",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Credits Total Secondary Income (USD)",
+                        "name": "credits_total_secondary_income",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Credits Total (USD)",
+                        "name": "credits_total",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Debits Services as Percent of Goods and Services",
+                        "name": "debits_services_percent_of_goods_and_services",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Debits Services as Percent of Current Account",
+                        "name": "debits_services_percent_of_current_account",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Debits Total Services (USD)",
+                        "name": "debits_total_services",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Debits Total Goods (USD)",
+                        "name": "debits_total_goods",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Debits Total Primary Income (USD)",
+                        "name": "debits_total_primary_income",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Debits Total (USD)",
+                        "name": "debits_total",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Current Account Debits Total Secondary Income (USD)",
+                        "name": "debits_total_secondary_income",
+                        "optional": true,
+                        "type": "float"
+                    }
+                ]
+            },
+            "deprecated": {
+                "flag": null,
+                "message": null
+            },
+            "description": "Balance of Payments Reports.",
+            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.economy.balance_of_payments(provider='fred')\nobb.economy.balance_of_payments(provider='fred', country=brazil)\n```\n\n",
+            "model": "BalanceOfPayments",
+            "parameters": {
+                "fred": [
+                    {
+                        "choices": "argentina,australia,austria,belgium,brazil,canada,chile,china,colombia,costa_rica,czechia,denmark,estonia,finland,france,germany,greece,hungary,iceland,india,indonesia,ireland,israel,italy,japan,korea,latvia,lithuania,luxembourg,mexico,netherlands,new_zealand,norway,poland,portugal,russia,saudi_arabia,slovak_republic,slovenia,south_africa,spain,sweden,switzerland,turkey,united_kingdom,united_states,g7,g20",
+                        "default": "united_states",
+                        "description": "The country to get data. Enter as a 3-letter ISO country code, default is USA.",
+                        "name": "country",
+                        "optional": true,
+                        "type": "Literal['argentina', 'australia', 'austria', 'belgium', 'brazil', 'canada', 'chile', 'china', 'colombia', 'costa_rica', 'czechia', 'denmark', 'estonia', 'finland', 'france', 'germany', 'greece', 'hungary', 'iceland', 'india', 'indonesia', 'ireland', 'israel', 'italy', 'japan', 'korea', 'latvia', 'lithuania', 'luxembourg', 'mexico', 'netherlands', 'new_zealand', 'norway', 'poland', 'portugal', 'russia', 'saudi_arabia', 'slovak_republic', 'slovenia', 'south_africa', 'spain', 'sweden', 'switzerland', 'turkey', 'united_kingdom', 'united_states', 'g7', 'g20']"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Start date of the data, in YYYY-MM-DD format.",
+                        "name": "start_date",
+                        "optional": true,
+                        "type": "Union[date, str]"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "End date of the data, in YYYY-MM-DD format.",
+                        "name": "end_date",
+                        "optional": true,
+                        "type": "Union[date, str]"
+                    }
+                ],
+                "standard": [
+                    {
+                        "default": "fred",
+                        "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fred' if there is no default.",
+                        "name": "provider",
+                        "optional": true,
+                        "type": "Literal['fred']"
+                    }
+                ]
+            },
+            "returns": {
+                "OBBject": [
+                    {
+                        "description": "Serializable results.",
+                        "name": "results",
+                        "type": "List[BalanceOfPayments]"
+                    },
+                    {
+                        "description": "Provider name.",
+                        "name": "provider",
+                        "type": "Optional[Literal['fred']]"
+                    },
+                    {
+                        "description": "List of warnings.",
+                        "name": "warnings",
+                        "type": "Optional[List[Warning_]]"
+                    },
+                    {
+                        "description": "Chart object.",
+                        "name": "chart",
+                        "type": "Optional[Chart]"
+                    },
+                    {
+                        "description": "Extra info.",
+                        "name": "extra",
+                        "type": "Dict[str, Any]"
+                    }
+                ]
+            }
+        },
         "/economy/calendar": {
             "data": {
                 "fmp": [
                     {
                         "choices": null,
                         "default": null,
                         "description": "Value change since previous.",
@@ -5627,14 +5875,528 @@
                         "description": "Extra info.",
                         "name": "extra",
                         "type": "Dict[str, Any]"
                     }
                 ]
             }
         },
+        "/equity/compare/company_facts": {
+            "data": {
+                "sec": [
+                    {
+                        "choices": null,
+                        "default": "",
+                        "description": "Central Index Key (CIK) for the requested entity.",
+                        "name": "cik",
+                        "optional": false,
+                        "type": "Union[str, int]"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Geographic location of the reporting entity.",
+                        "name": "location",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The SEC form associated with the fact or concept.",
+                        "name": "form",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The frame ID associated with the fact or concept, if applicable.",
+                        "name": "frame",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": "",
+                        "description": "SEC filing accession number associated with the reported fact or concept.",
+                        "name": "accession",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": "",
+                        "description": "The display name of the fact or concept.",
+                        "name": "fact",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The unit of measurement for the fact or concept.",
+                        "name": "unit",
+                        "optional": true,
+                        "type": "str"
+                    }
+                ],
+                "standard": [
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Symbol representing the entity requested in the data.",
+                        "name": "symbol",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Name of the entity.",
+                        "name": "name",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": "",
+                        "description": "The reported value of the fact or concept.",
+                        "name": "value",
+                        "optional": false,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The date when the report was filed.",
+                        "name": "reported_date",
+                        "optional": true,
+                        "type": "date"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The start date of the reporting period.",
+                        "name": "period_beginning",
+                        "optional": true,
+                        "type": "date"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The end date of the reporting period.",
+                        "name": "period_ending",
+                        "optional": true,
+                        "type": "date"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The fiscal year.",
+                        "name": "fiscal_year",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The fiscal period of the fiscal year.",
+                        "name": "fiscal_period",
+                        "optional": true,
+                        "type": "str"
+                    }
+                ]
+            },
+            "deprecated": {
+                "flag": null,
+                "message": null
+            },
+            "description": "Copmare reported company facts and fundamental data points.",
+            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.compare.company_facts(provider='sec')\nobb.equity.compare.company_facts(provider='sec', fact='PaymentsForRepurchaseOfCommonStock', year=2023)\nobb.equity.compare.company_facts(provider='sec', symbol='NVDA,AAPL,AMZN,MSFT,GOOG,SMCI', fact='RevenueFromContractWithCustomerExcludingAssessedTax', year=2024)\n```\n\n",
+            "model": "CompareCompanyFacts",
+            "parameters": {
+                "sec": [
+                    {
+                        "choices": [
+                            "AccountsPayableCurrent",
+                            "AccountsReceivableNet",
+                            "AccountsReceivableNetCurrent",
+                            "AccrualForTaxesOtherThanIncomeTaxesCurrent",
+                            "AccrualForTaxesOtherThanIncomeTaxesCurrentAndNoncurrent",
+                            "AccruedIncomeTaxesCurrent",
+                            "AccruedIncomeTaxesNoncurrent",
+                            "AccruedInsuranceCurrent",
+                            "AccruedLiabilitiesCurrent",
+                            "AccumulatedDepreciationDepletionAndAmortizationPropertyPlantAndEquipment",
+                            "AccumulatedOtherComprehensiveIncomeLossNetOfTax",
+                            "AcquisitionsNetOfCashAcquiredAndPurchasesOfIntangibleAndOtherAssets",
+                            "AdjustmentsToAdditionalPaidInCapitalSharebasedCompensationRequisiteServicePeriodRecognitionValue",
+                            "AdvertisingExpense",
+                            "AllocatedShareBasedCompensationExpense",
+                            "AntidilutiveSecuritiesExcludedFromComputationOfEarningsPerShareAmount",
+                            "AssetImpairmentCharges",
+                            "Assets",
+                            "AssetsCurrent",
+                            "AssetsNoncurrent",
+                            "BuildingsAndImprovementsGross",
+                            "CapitalLeaseObligationsCurrent",
+                            "CapitalLeaseObligationsNoncurrent",
+                            "Cash",
+                            "CashAndCashEquivalentsAtCarryingValue",
+                            "CashCashEquivalentsAndShortTermInvestments",
+                            "CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents",
+                            "CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations",
+                            "CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsPeriodIncreaseDecreaseIncludingExchangeRateEffect",
+                            "CommercialPaper",
+                            "CommitmentsAndContingencies",
+                            "CommonStockDividendsPerShareCashPaid",
+                            "CommonStockDividendsPerShareDeclared",
+                            "CommonStocksIncludingAdditionalPaidInCapital",
+                            "ComprehensiveIncomeNetOfTax",
+                            "ComprehensiveIncomeNetOfTaxAttributableToNoncontrollingInterest",
+                            "ComprehensiveIncomeNetOfTaxIncludingPortionAttributableToNoncontrollingInterest",
+                            "ConstructionInProgressGross",
+                            "ContractWithCustomerAssetNet",
+                            "ContractWithCustomerLiability",
+                            "ContractWithCustomerLiabilityCurrent",
+                            "ContractWithCustomerLiabilityNoncurrent",
+                            "CostOfGoodsAndServicesSold",
+                            "CostOfRevenue",
+                            "CurrentFederalTaxExpenseBenefit",
+                            "CurrentForeignTaxExpenseBenefit",
+                            "CurrentIncomeTaxExpenseBenefit",
+                            "CurrentStateAndLocalTaxExpenseBenefit",
+                            "DebtInstrumentFaceAmount",
+                            "DebtInstrumentFairValue",
+                            "DebtLongtermAndShorttermCombinedAmount",
+                            "DeferredFederalIncomeTaxExpenseBenefit",
+                            "DeferredForeignIncomeTaxExpenseBenefit",
+                            "DeferredIncomeTaxExpenseBenefit",
+                            "DeferredIncomeTaxLiabilities",
+                            "DeferredIncomeTaxLiabilitiesNet",
+                            "DeferredIncomeTaxesAndTaxCredits",
+                            "DeferredRevenue",
+                            "DeferredTaxAssetsGross",
+                            "DeferredTaxAssetsLiabilitiesNet",
+                            "DeferredTaxAssetsNet",
+                            "DeferredTaxLiabilities",
+                            "DefinedContributionPlanCostRecognized",
+                            "Depreciation",
+                            "DepreciationAmortizationAndAccretionNet",
+                            "DepreciationAmortizationAndOther",
+                            "DepreciationAndAmortization",
+                            "DepreciationDepletionAndAmortization",
+                            "DerivativeCollateralObligationToReturnCash",
+                            "DerivativeCollateralRightToReclaimCash",
+                            "DerivativeFairValueOfDerivativeNet",
+                            "DerivativeLiabilityCollateralRightToReclaimCashOffset",
+                            "DerivativeNotionalAmount",
+                            "DistributedEarnings",
+                            "Dividends",
+                            "DividendsCash",
+                            "DividendsPayableAmountPerShare",
+                            "DividendsPayableCurrent",
+                            "EarningsPerShareBasic",
+                            "EarningsPerShareDiluted",
+                            "EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents",
+                            "EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations",
+                            "EmployeeRelatedLiabilitiesCurrent",
+                            "EmployeeRelatedLiabilitiesCurrentAndNoncurrent",
+                            "EmployeeServiceShareBasedCompensationTaxBenefitFromCompensationExpense",
+                            "FinanceLeaseInterestExpense",
+                            "FinanceLeaseInterestPaymentOnLiability",
+                            "FinanceLeaseLiability",
+                            "FinanceLeaseLiabilityCurrent",
+                            "FinanceLeaseLiabilityNoncurrent",
+                            "FinanceLeaseLiabilityPaymentsDue",
+                            "FinanceLeaseLiabilityPaymentsDueAfterYearFive",
+                            "FinanceLeaseLiabilityPaymentsDueNextTwelveMonths",
+                            "FinanceLeaseLiabilityPaymentsDueYearFive",
+                            "FinanceLeaseLiabilityPaymentsDueYearFour",
+                            "FinanceLeaseLiabilityPaymentsDueYearThree",
+                            "FinanceLeaseLiabilityPaymentsDueYearTwo",
+                            "FinanceLeaseLiabilityPaymentsRemainderOfFiscalYear",
+                            "FinanceLeaseLiabilityUndiscountedExcessAmount",
+                            "FinanceLeasePrincipalPayments",
+                            "FinanceLeaseRightOfUseAsset",
+                            "FinancingReceivableAllowanceForCreditLosses",
+                            "FiniteLivedIntangibleAssetsNet",
+                            "FixturesAndEquipmentGross",
+                            "GainLossOnInvestments",
+                            "GainLossOnInvestmentsAndDerivativeInstruments",
+                            "GainLossOnSaleOfBusiness",
+                            "GainsLossesOnExtinguishmentOfDebt",
+                            "GeneralAndAdministrativeExpense",
+                            "Goodwill",
+                            "GrossProfit",
+                            "ImpairmentOfIntangibleAssetsExcludingGoodwill",
+                            "ImpairmentOfIntangibleAssetsIndefinitelivedExcludingGoodwill",
+                            "IncomeLossFromContinuingOperations",
+                            "IncomeLossFromContinuingOperationsAttributableToNoncontrollingEntity",
+                            "IncomeLossFromContinuingOperationsBeforeIncomeTaxesExtraordinaryItemsNoncontrollingInterest",
+                            "IncomeLossFromContinuingOperationsPerBasicShare",
+                            "IncomeLossFromContinuingOperationsPerDilutedShare",
+                            "IncomeTaxExpenseBenefit",
+                            "IncomeTaxesPaid",
+                            "IncomeTaxesPaidNet",
+                            "IncreaseDecreaseInAccountsAndOtherReceivables",
+                            "IncreaseDecreaseInAccountsPayable",
+                            "IncreaseDecreaseInAccountsReceivable",
+                            "IncreaseDecreaseInAccruedIncomeTaxesPayable",
+                            "IncreaseDecreaseInAccruedLiabilities",
+                            "IncreaseDecreaseInAccruedTaxesPayable",
+                            "IncreaseDecreaseInContractWithCustomerLiability",
+                            "IncreaseDecreaseInDeferredIncomeTaxes",
+                            "IncreaseDecreaseInInventories",
+                            "IncreaseDecreaseInOtherCurrentAssets",
+                            "IncreaseDecreaseInOtherCurrentLiabilities",
+                            "IncreaseDecreaseInOtherNoncurrentAssets",
+                            "IncreaseDecreaseInOtherNoncurrentLiabilities",
+                            "IncreaseDecreaseInPensionPlanObligations",
+                            "IncrementalCommonSharesAttributableToShareBasedPaymentArrangements",
+                            "InterestAndDebtExpense",
+                            "InterestExpenseDebt",
+                            "InterestIncomeExpenseNet",
+                            "InterestPaid",
+                            "InterestPaidNet",
+                            "InventoryNet",
+                            "InvestmentIncomeInterest",
+                            "Land",
+                            "LeaseAndRentalExpense",
+                            "LesseeOperatingLeaseLiabilityPaymentsDue",
+                            "LesseeOperatingLeaseLiabilityPaymentsDueAfterYearFive",
+                            "LesseeOperatingLeaseLiabilityPaymentsDueNextTwelveMonths",
+                            "LesseeOperatingLeaseLiabilityPaymentsDueYearFive",
+                            "LesseeOperatingLeaseLiabilityPaymentsDueYearFour",
+                            "LesseeOperatingLeaseLiabilityPaymentsDueYearThree",
+                            "LesseeOperatingLeaseLiabilityPaymentsDueYearTwo",
+                            "LesseeOperatingLeaseLiabilityPaymentsRemainderOfFiscalYear",
+                            "LettersOfCreditOutstandingAmount",
+                            "Liabilities",
+                            "LiabilitiesAndStockholdersEquity",
+                            "LiabilitiesCurrent",
+                            "LineOfCredit",
+                            "LineOfCreditFacilityMaximumBorrowingCapacity",
+                            "LongTermDebt",
+                            "LongTermDebtCurrent",
+                            "LongTermDebtMaturitiesRepaymentsOfPrincipalAfterYearFive",
+                            "LongTermDebtMaturitiesRepaymentsOfPrincipalInNextTwelveMonths",
+                            "LongTermDebtMaturitiesRepaymentsOfPrincipalInYearFive",
+                            "LongTermDebtMaturitiesRepaymentsOfPrincipalInYearFour",
+                            "LongTermDebtMaturitiesRepaymentsOfPrincipalInYearThree",
+                            "LongTermDebtMaturitiesRepaymentsOfPrincipalInYearTwo",
+                            "LongTermDebtMaturitiesRepaymentsOfPrincipalRemainderOfFiscalYear",
+                            "LongTermDebtNoncurrent",
+                            "LongTermInvestments",
+                            "LossContingencyEstimateOfPossibleLoss",
+                            "MachineryAndEquipmentGross",
+                            "MarketableSecuritiesCurrent",
+                            "MarketableSecuritiesNoncurrent",
+                            "MinorityInterest",
+                            "NetCashProvidedByUsedInFinancingActivities",
+                            "NetCashProvidedByUsedInInvestingActivities",
+                            "NetCashProvidedByUsedInOperatingActivities",
+                            "NetIncomeLoss",
+                            "NetIncomeLossAttributableToNoncontrollingInterest",
+                            "NetIncomeLossAttributableToNonredeemableNoncontrollingInterest",
+                            "NetIncomeLossAttributableToRedeemableNoncontrollingInterest",
+                            "NoncurrentAssets",
+                            "NoncurrentAssets",
+                            "NoninterestIncome",
+                            "NonoperatingIncomeExpense",
+                            "NotesReceivableNet",
+                            "OperatingExpenses",
+                            "OperatingIncomeLoss",
+                            "OperatingLeaseCost",
+                            "OperatingLeaseLiability",
+                            "OperatingLeaseLiabilityCurrent",
+                            "OperatingLeaseLiabilityNoncurrent",
+                            "OperatingLeaseRightOfUseAsset",
+                            "OtherAccruedLiabilitiesCurrent",
+                            "OtherAssetsCurrent",
+                            "OtherAssetsNoncurrent",
+                            "OtherComprehensiveIncomeLossAvailableForSaleSecuritiesAdjustmentNetOfTax",
+                            "OtherComprehensiveIncomeLossCashFlowHedgeGainLossAfterReclassificationAndTax",
+                            "OtherComprehensiveIncomeLossDerivativeInstrumentGainLossafterReclassificationandTax",
+                            "OtherComprehensiveIncomeLossDerivativeInstrumentGainLossbeforeReclassificationafterTax",
+                            "OtherComprehensiveIncomeLossForeignCurrencyTransactionAndTranslationAdjustmentNetOfTax",
+                            "OtherComprehensiveIncomeLossNetOfTax",
+                            "OtherComprehensiveIncomeLossNetOfTaxPortionAttributableToParent",
+                            "OtherComprehensiveIncomeUnrealizedHoldingGainLossOnSecuritiesArisingDuringPeriodNetOfTax",
+                            "OtherIncome",
+                            "OtherLiabilitiesCurrent",
+                            "OtherLiabilitiesNoncurrent",
+                            "OtherLongTermDebt",
+                            "OtherNoncashIncomeExpense",
+                            "PaymentsForCapitalImprovements",
+                            "PaymentsForProceedsFromBusinessesAndInterestInAffiliates",
+                            "PaymentsForProceedsFromOtherInvestingActivities",
+                            "PaymentsForRent",
+                            "PaymentsForRepurchaseOfCommonStock",
+                            "PaymentsOfDebtExtinguishmentCosts",
+                            "PaymentsOfDividends",
+                            "PaymentsOfDividendsMinorityInterest",
+                            "PaymentsToAcquireInvestments",
+                            "PaymentsToAcquirePropertyPlantAndEquipment",
+                            "PreferredStockSharesOutstanding",
+                            "PreferredStockValue",
+                            "PrepaidExpenseAndOtherAssetsCurrent",
+                            "PrepaidExpenseCurrent",
+                            "ProceedsFromDebtMaturingInMoreThanThreeMonths",
+                            "ProceedsFromDebtNetOfIssuanceCosts",
+                            "ProceedsFromDivestitureOfBusinesses",
+                            "ProceedsFromInvestments",
+                            "ProceedsFromIssuanceOfCommonStock",
+                            "ProceedsFromIssuanceOfDebt",
+                            "ProceedsFromIssuanceOfLongTermDebt",
+                            "ProceedsFromIssuanceOfUnsecuredDebt",
+                            "ProceedsFromIssuanceOrSaleOfEquity",
+                            "ProceedsFromMaturitiesPrepaymentsAndCallsOfAvailableForSaleSecurities",
+                            "ProceedsFromPaymentsForOtherFinancingActivities",
+                            "ProceedsFromPaymentsToMinorityShareholders",
+                            "ProceedsFromRepaymentsOfShortTermDebt",
+                            "ProceedsFromRepaymentsOfShortTermDebtMaturingInThreeMonthsOrLess",
+                            "ProceedsFromSaleOfPropertyPlantAndEquipment",
+                            "ProceedsFromStockOptionsExercised",
+                            "ProfitLoss",
+                            "PropertyPlantAndEquipmentGross",
+                            "PropertyPlantAndEquipmentNet",
+                            "ReceivablesNetCurrent",
+                            "RedeemableNoncontrollingInterestEquityCarryingAmount",
+                            "RepaymentsOfDebtMaturingInMoreThanThreeMonths",
+                            "RepaymentsOfLongTermDebt",
+                            "ResearchAndDevelopmentExpense",
+                            "RestrictedCash",
+                            "RestrictedCashAndCashEquivalents",
+                            "RestrictedStockExpense",
+                            "RestructuringCharges",
+                            "RetainedEarningsAccumulatedDeficit",
+                            "RevenueFromContractWithCustomerExcludingAssessedTax",
+                            "Revenues",
+                            "SecuredLongTermDebt",
+                            "SellingAndMarketingExpense",
+                            "SellingGeneralAndAdministrativeExpense",
+                            "ShareBasedCompensation",
+                            "ShortTermBorrowings",
+                            "ShortTermInvestments",
+                            "StockIssuedDuringPeriodValueNewIssues",
+                            "StockOptionPlanExpense",
+                            "StockRedeemedOrCalledDuringPeriodValue",
+                            "StockRepurchasedAndRetiredDuringPeriodValue",
+                            "StockRepurchasedDuringPeriodValue",
+                            "StockholdersEquity",
+                            "StockholdersEquityIncludingPortionAttributableToNoncontrollingInterest",
+                            "StockholdersEquityOther",
+                            "TaxesPayableCurrent",
+                            "TradingSecuritiesDebt",
+                            "TreasuryStockAcquiredAverageCostPerShare",
+                            "TreasuryStockSharesAcquired",
+                            "UnrealizedGainLossOnInvestments",
+                            "UnrecognizedTaxBenefits",
+                            "UnsecuredDebt",
+                            "VariableLeaseCost",
+                            "WeightedAverageNumberDilutedSharesOutstandingAdjustment",
+                            "WeightedAverageNumberOfDilutedSharesOutstanding",
+                            "WeightedAverageNumberOfSharesOutstandingBasic"
+                        ],
+                        "default": "Revenues",
+                        "description": "Fact or concept from the SEC taxonomy, in UpperCamelCase. Defaults to, 'Revenues'. AAPL, MSFT, GOOG, BRK-A currently report revenue as, 'RevenueFromContractWithCustomerExcludingAssessedTax'. In previous years, they have reported as 'Revenues'.",
+                        "name": "fact",
+                        "optional": true,
+                        "type": "Literal['AccountsPayableCurrent', 'AccountsReceivableNet', 'AccountsReceivableNetCurrent', 'AccrualForTaxesOtherThanIncomeTaxesCurrent', 'AccrualForTaxesOtherThanIncomeTaxesCurrentAndNoncurrent', 'AccruedIncomeTaxesCurrent', 'AccruedIncomeTaxesNoncurrent', 'AccruedInsuranceCurrent', 'AccruedLiabilitiesCurrent', 'AccumulatedDepreciationDepletionAndAmortizationPropertyPlantAndEquipment', 'AccumulatedOtherComprehensiveIncomeLossNetOfTax', 'AcquisitionsNetOfCashAcquiredAndPurchasesOfIntangibleAndOtherAssets', 'AdjustmentsToAdditionalPaidInCapitalSharebasedCompensationRequisiteServicePeriodRecognitionValue', 'AdvertisingExpense', 'AllocatedShareBasedCompensationExpense', 'AntidilutiveSecuritiesExcludedFromComputationOfEarningsPerShareAmount', 'Assets', 'AssetsCurrent', 'AssetsNoncurrent', 'NoncurrentAssets', 'AssetImpairmentCharges', 'BuildingsAndImprovementsGross', 'CapitalLeaseObligationsCurrent', 'CapitalLeaseObligationsNoncurrent', 'Cash', 'CashAndCashEquivalentsAtCarryingValue', 'CashCashEquivalentsAndShortTermInvestments', 'CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents', 'CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations', 'CashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsPeriodIncreaseDecreaseIncludingExchangeRateEffect', 'CommitmentsAndContingencies', 'CommercialPaper', 'CommonStockDividendsPerShareDeclared', 'CommonStockDividendsPerShareCashPaid', 'CommonStocksIncludingAdditionalPaidInCapital', 'ComprehensiveIncomeNetOfTax', 'ComprehensiveIncomeNetOfTaxAttributableToNoncontrollingInterest', 'ComprehensiveIncomeNetOfTaxIncludingPortionAttributableToNoncontrollingInterest', 'ConstructionInProgressGross', 'ContractWithCustomerAssetNet', 'ContractWithCustomerLiability', 'ContractWithCustomerLiabilityCurrent', 'ContractWithCustomerLiabilityNoncurrent', 'CostOfRevenue', 'CostOfGoodsAndServicesSold', 'CurrentFederalTaxExpenseBenefit', 'CurrentForeignTaxExpenseBenefit', 'CurrentIncomeTaxExpenseBenefit', 'CurrentStateAndLocalTaxExpenseBenefit', 'DebtInstrumentFaceAmount', 'DebtInstrumentFairValue', 'DebtLongtermAndShorttermCombinedAmount', 'DeferredFederalIncomeTaxExpenseBenefit', 'DeferredForeignIncomeTaxExpenseBenefit', 'DeferredIncomeTaxExpenseBenefit', 'DeferredIncomeTaxesAndTaxCredits', 'DeferredIncomeTaxLiabilities', 'DeferredIncomeTaxLiabilitiesNet', 'DeferredRevenue', 'DeferredTaxAssetsGross', 'DeferredTaxAssetsLiabilitiesNet', 'DeferredTaxAssetsNet', 'DeferredTaxLiabilities', 'DefinedContributionPlanCostRecognized', 'Depreciation', 'DepreciationAmortizationAndAccretionNet', 'DepreciationAmortizationAndOther', 'DepreciationAndAmortization', 'DepreciationDepletionAndAmortization', 'DerivativeCollateralObligationToReturnCash', 'DerivativeCollateralRightToReclaimCash', 'DerivativeFairValueOfDerivativeNet', 'DerivativeLiabilityCollateralRightToReclaimCashOffset', 'DerivativeNotionalAmount', 'Dividends', 'DividendsCash', 'DividendsPayableAmountPerShare', 'DividendsPayableCurrent', 'DistributedEarnings', 'EarningsPerShareBasic', 'EarningsPerShareDiluted', 'EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalents', 'EffectOfExchangeRateOnCashCashEquivalentsRestrictedCashAndRestrictedCashEquivalentsIncludingDisposalGroupAndDiscontinuedOperations', 'EmployeeRelatedLiabilitiesCurrent', 'EmployeeRelatedLiabilitiesCurrentAndNoncurrent', 'EmployeeServiceShareBasedCompensationTaxBenefitFromCompensationExpense', 'FinanceLeaseInterestExpense', 'FinanceLeaseInterestPaymentOnLiability', 'FinanceLeaseLiability', 'FinanceLeaseLiabilityCurrent', 'FinanceLeaseLiabilityNoncurrent', 'FinanceLeaseLiabilityPaymentsDue', 'FinanceLeaseLiabilityPaymentsDueAfterYearFive', 'FinanceLeaseLiabilityPaymentsDueNextTwelveMonths', 'FinanceLeaseLiabilityPaymentsDueYearFive', 'FinanceLeaseLiabilityPaymentsDueYearFour', 'FinanceLeaseLiabilityPaymentsDueYearThree', 'FinanceLeaseLiabilityPaymentsDueYearTwo', 'FinanceLeaseLiabilityPaymentsRemainderOfFiscalYear', 'FinanceLeaseLiabilityUndiscountedExcessAmount', 'FinanceLeasePrincipalPayments', 'FinanceLeaseRightOfUseAsset', 'FinancingReceivableAllowanceForCreditLosses', 'FiniteLivedIntangibleAssetsNet', 'FixturesAndEquipmentGross', 'GainLossOnInvestments', 'GainLossOnInvestmentsAndDerivativeInstruments', 'GainLossOnSaleOfBusiness', 'GainsLossesOnExtinguishmentOfDebt', 'GeneralAndAdministrativeExpense', 'Goodwill', 'GrossProfit', 'ImpairmentOfIntangibleAssetsExcludingGoodwill', 'ImpairmentOfIntangibleAssetsIndefinitelivedExcludingGoodwill', 'IncomeLossFromContinuingOperations', 'IncomeLossFromContinuingOperationsAttributableToNoncontrollingEntity', 'IncomeLossFromContinuingOperationsBeforeIncomeTaxesExtraordinaryItemsNoncontrollingInterest', 'IncomeLossFromContinuingOperationsPerBasicShare', 'IncomeLossFromContinuingOperationsPerDilutedShare', 'InterestAndDebtExpense', 'IncomeTaxExpenseBenefit', 'IncomeTaxesPaid', 'IncomeTaxesPaidNet', 'IncreaseDecreaseInAccountsAndOtherReceivables', 'IncreaseDecreaseInAccountsPayable', 'IncreaseDecreaseInAccountsReceivable', 'IncreaseDecreaseInAccruedLiabilities', 'IncreaseDecreaseInAccruedIncomeTaxesPayable', 'IncreaseDecreaseInAccruedTaxesPayable', 'IncreaseDecreaseInContractWithCustomerLiability', 'IncreaseDecreaseInDeferredIncomeTaxes', 'IncreaseDecreaseInInventories', 'IncreaseDecreaseInOtherCurrentAssets', 'IncreaseDecreaseInOtherCurrentLiabilities', 'IncreaseDecreaseInOtherNoncurrentAssets', 'IncreaseDecreaseInOtherNoncurrentLiabilities', 'IncreaseDecreaseInPensionPlanObligations', 'IncrementalCommonSharesAttributableToShareBasedPaymentArrangements', 'InterestExpenseDebt', 'InterestIncomeExpenseNet', 'InterestPaid', 'InterestPaidNet', 'InventoryNet', 'InvestmentIncomeInterest', 'Land', 'LeaseAndRentalExpense', 'LesseeOperatingLeaseLiabilityPaymentsDue', 'LesseeOperatingLeaseLiabilityPaymentsDueAfterYearFive', 'LesseeOperatingLeaseLiabilityPaymentsDueNextTwelveMonths', 'LesseeOperatingLeaseLiabilityPaymentsDueYearFive', 'LesseeOperatingLeaseLiabilityPaymentsDueYearFour', 'LesseeOperatingLeaseLiabilityPaymentsDueYearThree', 'LesseeOperatingLeaseLiabilityPaymentsDueYearTwo', 'LesseeOperatingLeaseLiabilityPaymentsRemainderOfFiscalYear', 'LettersOfCreditOutstandingAmount', 'Liabilities', 'LiabilitiesAndStockholdersEquity', 'LiabilitiesCurrent', 'LineOfCredit', 'LineOfCreditFacilityMaximumBorrowingCapacity', 'LongTermDebt', 'LongTermDebtCurrent', 'LongTermDebtMaturitiesRepaymentsOfPrincipalAfterYearFive', 'LongTermDebtMaturitiesRepaymentsOfPrincipalInNextTwelveMonths', 'LongTermDebtMaturitiesRepaymentsOfPrincipalInYearFive', 'LongTermDebtMaturitiesRepaymentsOfPrincipalInYearFour', 'LongTermDebtMaturitiesRepaymentsOfPrincipalInYearThree', 'LongTermDebtMaturitiesRepaymentsOfPrincipalInYearTwo', 'LongTermDebtMaturitiesRepaymentsOfPrincipalRemainderOfFiscalYear', 'LongTermDebtNoncurrent', 'LongTermInvestments', 'LossContingencyEstimateOfPossibleLoss', 'MachineryAndEquipmentGross', 'MarketableSecuritiesCurrent', 'MarketableSecuritiesNoncurrent', 'MinorityInterest', 'NetCashProvidedByUsedInFinancingActivities', 'NetCashProvidedByUsedInInvestingActivities', 'NetCashProvidedByUsedInOperatingActivities', 'NetIncomeLoss', 'NetIncomeLossAttributableToNoncontrollingInterest', 'NetIncomeLossAttributableToNonredeemableNoncontrollingInterest', 'NetIncomeLossAttributableToRedeemableNoncontrollingInterest', 'NonoperatingIncomeExpense', 'NoninterestIncome', 'NotesReceivableNet', 'OperatingExpenses', 'OperatingIncomeLoss', 'OperatingLeaseCost', 'OperatingLeaseLiability', 'OperatingLeaseLiabilityCurrent', 'OperatingLeaseLiabilityNoncurrent', 'OperatingLeaseRightOfUseAsset', 'OtherAccruedLiabilitiesCurrent', 'OtherAssetsCurrent', 'OtherAssetsNoncurrent', 'OtherComprehensiveIncomeLossAvailableForSaleSecuritiesAdjustmentNetOfTax', 'OtherComprehensiveIncomeLossCashFlowHedgeGainLossAfterReclassificationAndTax', 'OtherComprehensiveIncomeLossDerivativeInstrumentGainLossafterReclassificationandTax', 'OtherComprehensiveIncomeLossDerivativeInstrumentGainLossbeforeReclassificationafterTax', 'OtherComprehensiveIncomeLossForeignCurrencyTransactionAndTranslationAdjustmentNetOfTax', 'OtherComprehensiveIncomeLossNetOfTax', 'OtherComprehensiveIncomeLossNetOfTaxPortionAttributableToParent', 'OtherComprehensiveIncomeUnrealizedHoldingGainLossOnSecuritiesArisingDuringPeriodNetOfTax', 'OtherIncome', 'OtherLiabilitiesCurrent', 'OtherLiabilitiesNoncurrent', 'OtherLongTermDebt', 'OtherNoncashIncomeExpense', 'PaymentsForCapitalImprovements', 'PaymentsOfDividends', 'PaymentsOfDividendsMinorityInterest', 'PaymentsForProceedsFromBusinessesAndInterestInAffiliates', 'PaymentsForProceedsFromOtherInvestingActivities', 'PaymentsForRent', 'PaymentsForRepurchaseOfCommonStock', 'PaymentsOfDebtExtinguishmentCosts', 'PaymentsToAcquireInvestments', 'PaymentsToAcquirePropertyPlantAndEquipment', 'PreferredStockSharesOutstanding', 'PreferredStockValue', 'PrepaidExpenseAndOtherAssetsCurrent', 'PrepaidExpenseCurrent', 'ProceedsFromDebtMaturingInMoreThanThreeMonths', 'ProceedsFromDebtNetOfIssuanceCosts', 'ProceedsFromDivestitureOfBusinesses', 'ProceedsFromInvestments', 'ProceedsFromIssuanceOfCommonStock', 'ProceedsFromIssuanceOfDebt', 'ProceedsFromIssuanceOfLongTermDebt', 'ProceedsFromIssuanceOfUnsecuredDebt', 'ProceedsFromIssuanceOrSaleOfEquity', 'ProceedsFromMaturitiesPrepaymentsAndCallsOfAvailableForSaleSecurities', 'ProceedsFromPaymentsForOtherFinancingActivities', 'ProceedsFromPaymentsToMinorityShareholders', 'ProceedsFromRepaymentsOfShortTermDebt', 'ProceedsFromRepaymentsOfShortTermDebtMaturingInThreeMonthsOrLess', 'ProceedsFromSaleOfPropertyPlantAndEquipment', 'ProceedsFromStockOptionsExercised', 'ProfitLoss', 'PropertyPlantAndEquipmentGross', 'PropertyPlantAndEquipmentNet', 'ReceivablesNetCurrent', 'RedeemableNoncontrollingInterestEquityCarryingAmount', 'RepaymentsOfDebtMaturingInMoreThanThreeMonths', 'RepaymentsOfLongTermDebt', 'ResearchAndDevelopmentExpense', 'RestrictedCash', 'RestrictedCashAndCashEquivalents', 'RestrictedStockExpense', 'RestructuringCharges', 'RetainedEarningsAccumulatedDeficit', 'Revenues', 'RevenueFromContractWithCustomerExcludingAssessedTax', 'SecuredLongTermDebt', 'SellingAndMarketingExpense', 'SellingGeneralAndAdministrativeExpense', 'ShareBasedCompensation', 'ShortTermBorrowings', 'ShortTermInvestments', 'StockholdersEquity', 'StockholdersEquityIncludingPortionAttributableToNoncontrollingInterest', 'StockholdersEquityOther', 'StockIssuedDuringPeriodValueNewIssues', 'StockOptionPlanExpense', 'StockRedeemedOrCalledDuringPeriodValue', 'StockRepurchasedDuringPeriodValue', 'StockRepurchasedAndRetiredDuringPeriodValue', 'TaxesPayableCurrent', 'TradingSecuritiesDebt', 'TreasuryStockAcquiredAverageCostPerShare', 'TreasuryStockSharesAcquired', 'UnrealizedGainLossOnInvestments', 'UnrecognizedTaxBenefits', 'UnsecuredDebt', 'VariableLeaseCost', 'WeightedAverageNumberOfDilutedSharesOutstanding', 'WeightedAverageNumberOfSharesOutstandingBasic', 'WeightedAverageNumberDilutedSharesOutstandingAdjustment']"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The year to retrieve the data for. If not provided, the current year is used. When symbol(s) are provided, excluding the year will return all reported values for the concept.",
+                        "name": "year",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The fiscal period to retrieve the data for. If not provided, the most recent quarter is used. This parameter is ignored when a symbol is supplied.",
+                        "name": "fiscal_period",
+                        "optional": true,
+                        "type": "Literal['fy', 'q1', 'q2', 'q3', 'q4']"
+                    },
+                    {
+                        "choices": null,
+                        "default": false,
+                        "description": "Whether to retrieve instantaneous data. See the notes above for more information. Defaults to False. Some facts are only available as instantaneous data. The function will automatically attempt the inverse of this parameter if the initial fiscal quarter request fails. This parameter is ignored when a symbol is supplied.",
+                        "name": "instantaneous",
+                        "optional": true,
+                        "type": "bool"
+                    },
+                    {
+                        "choices": null,
+                        "default": true,
+                        "description": "Whether to use cache for the request. Defaults to True.",
+                        "name": "use_cache",
+                        "optional": true,
+                        "type": "bool"
+                    }
+                ],
+                "standard": [
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Symbol to get data for. Multiple items allowed for provider(s): sec.",
+                        "name": "symbol",
+                        "optional": true,
+                        "type": "Union[str, List[str]]"
+                    },
+                    {
+                        "choices": null,
+                        "default": "",
+                        "description": "The fact to lookup, typically a GAAP-reporting measure. Choices vary by provider.",
+                        "name": "fact",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "default": "sec",
+                        "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'sec' if there is no default.",
+                        "name": "provider",
+                        "optional": true,
+                        "type": "Literal['sec']"
+                    }
+                ]
+            },
+            "returns": {
+                "OBBject": [
+                    {
+                        "description": "Serializable results.",
+                        "name": "results",
+                        "type": "List[CompareCompanyFacts]"
+                    },
+                    {
+                        "description": "Provider name.",
+                        "name": "provider",
+                        "type": "Optional[Literal['sec']]"
+                    },
+                    {
+                        "description": "List of warnings.",
+                        "name": "warnings",
+                        "type": "Optional[List[Warning_]]"
+                    },
+                    {
+                        "description": "Chart object.",
+                        "name": "chart",
+                        "type": "Optional[Chart]"
+                    },
+                    {
+                        "description": "Extra info.",
+                        "name": "extra",
+                        "type": "Dict[str, Any]"
+                    }
+                ]
+            }
+        },
         "/equity/compare/peers": {
             "data": {
                 "fmp": [],
                 "standard": [
                     {
                         "choices": null,
                         "default": "",
@@ -7569,14 +8331,242 @@
                         "description": "Extra info.",
                         "name": "extra",
                         "type": "Dict[str, Any]"
                     }
                 ]
             }
         },
+        "/equity/estimates/forward_ebitda": {
+            "data": {
+                "fmp": [],
+                "intrinio": [
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The type of estimate.",
+                        "name": "conensus_type",
+                        "optional": true,
+                        "type": "Literal['ebitda', 'ebit', 'enterprise_value', 'cash_flow_per_share', 'pretax_income']"
+                    }
+                ],
+                "standard": [
+                    {
+                        "choices": null,
+                        "default": "",
+                        "description": "Symbol representing the entity requested in the data.",
+                        "name": "symbol",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Name of the entity.",
+                        "name": "name",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The date of the last update.",
+                        "name": "last_updated",
+                        "optional": true,
+                        "type": "date"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The end date of the reporting period.",
+                        "name": "period_ending",
+                        "optional": true,
+                        "type": "date"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Fiscal year for the estimate.",
+                        "name": "fiscal_year",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Fiscal quarter for the estimate.",
+                        "name": "fiscal_period",
+                        "optional": true,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Calendar year for the estimate.",
+                        "name": "calendar_year",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Calendar quarter for the estimate.",
+                        "name": "calendar_period",
+                        "optional": true,
+                        "type": "Union[int, str]"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The EBITDA estimate low for the period.",
+                        "name": "low_estimate",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The EBITDA estimate high for the period.",
+                        "name": "high_estimate",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The EBITDA estimate mean for the period.",
+                        "name": "mean",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The EBITDA estimate median for the period.",
+                        "name": "median",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The EBITDA estimate standard deviation for the period.",
+                        "name": "standard_deviation",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Number of analysts providing estimates for the period.",
+                        "name": "number_of_analysts",
+                        "optional": true,
+                        "type": "int"
+                    }
+                ]
+            },
+            "deprecated": {
+                "flag": null,
+                "message": null
+            },
+            "description": "Get forward EBITDA estimates.",
+            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.equity.estimates.forward_ebitda(provider='intrinio')\nobb.equity.estimates.forward_ebitda(symbol='AAPL', fiscal_period=annual, provider='intrinio')\nobb.equity.estimates.forward_ebitda(symbol='AAPL,MSFT', fiscal_period=quarter, provider='fmp')\n```\n\n",
+            "model": "ForwardEbitdaEstimates",
+            "parameters": {
+                "fmp": [
+                    {
+                        "choices": null,
+                        "default": "annual",
+                        "description": "The future fiscal period to retrieve estimates for.",
+                        "name": "fiscal_period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The number of data entries to return.",
+                        "name": "limit",
+                        "optional": true,
+                        "type": "int"
+                    },
+                    {
+                        "choices": null,
+                        "default": false,
+                        "description": "If True, the data will include all past data and the limit will be ignored.",
+                        "name": "include_historical",
+                        "optional": true,
+                        "type": "bool"
+                    }
+                ],
+                "intrinio": [
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Filter for only full-year or quarterly estimates.",
+                        "name": "fiscal_period",
+                        "optional": true,
+                        "type": "Literal['annual', 'quarter']"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Limit the EBITDA estimates to this type.",
+                        "name": "estimate_type",
+                        "optional": true,
+                        "type": "Literal['ebitda', 'ebit', 'enterprise_value', 'cash_flow_per_share', 'pretax_income']"
+                    }
+                ],
+                "standard": [
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Symbol to get data for. Multiple items allowed for provider(s): fmp, intrinio.",
+                        "name": "symbol",
+                        "optional": true,
+                        "type": "Union[str, List[str]]"
+                    },
+                    {
+                        "default": "fmp",
+                        "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
+                        "name": "provider",
+                        "optional": true,
+                        "type": "Literal['fmp', 'intrinio']"
+                    }
+                ]
+            },
+            "returns": {
+                "OBBject": [
+                    {
+                        "description": "Serializable results.",
+                        "name": "results",
+                        "type": "List[ForwardEbitdaEstimates]"
+                    },
+                    {
+                        "description": "Provider name.",
+                        "name": "provider",
+                        "type": "Optional[Literal['fmp', 'intrinio']]"
+                    },
+                    {
+                        "description": "List of warnings.",
+                        "name": "warnings",
+                        "type": "Optional[List[Warning_]]"
+                    },
+                    {
+                        "description": "Chart object.",
+                        "name": "chart",
+                        "type": "Optional[Chart]"
+                    },
+                    {
+                        "description": "Extra info.",
+                        "name": "extra",
+                        "type": "Dict[str, Any]"
+                    }
+                ]
+            }
+        },
         "/equity/estimates/forward_eps": {
             "data": {
                 "fmp": [],
                 "intrinio": [
                     {
                         "choices": null,
                         "default": null,
@@ -7860,15 +8850,15 @@
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "The date the data was last updated.",
-                        "name": "last_udpated",
+                        "name": "last_updated",
                         "optional": true,
                         "type": "date"
                     }
                 ],
                 "standard": [
                     {
                         "choices": null,
@@ -8819,34 +9809,34 @@
                         "name": "action",
                         "optional": true,
                         "type": "Literal['downgrades', 'maintains', 'reinstates', 'reiterates', 'upgrades', 'assumes', 'initiates', 'terminates', 'removes', 'suspends', 'firm_dissolved']"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "Comma-separated list of analyst (person) IDs. Omitting will bring back all available analysts.",
+                        "description": "Comma-separated list of analyst (person) IDs. Omitting will bring back all available analysts. Multiple items allowed for provider(s): benzinga.",
                         "name": "analyst_ids",
                         "optional": true,
-                        "type": "Union[List[str], str]"
+                        "type": "Union[Union[List[str], str], List[Union[List[str], str]]]"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "Comma-separated list of firm IDs.",
+                        "description": "Comma-separated list of firm IDs. Multiple items allowed for provider(s): benzinga.",
                         "name": "firm_ids",
                         "optional": true,
-                        "type": "Union[List[str], str]"
+                        "type": "Union[Union[List[str], str], List[Union[List[str], str]]]"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "Comma-separated list of fields to include in the response. See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields.",
+                        "description": "Comma-separated list of fields to include in the response. See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields. Multiple items allowed for provider(s): benzinga.",
                         "name": "fields",
                         "optional": true,
-                        "type": "Union[List[str], str]"
+                        "type": "Union[Union[List[str], str], List[Union[List[str], str]]]"
                     }
                 ],
                 "fmp": [
                     {
                         "choices": null,
                         "default": false,
                         "description": "Include upgrades and downgrades in the response.",
@@ -12850,15 +13840,15 @@
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Type of the SEC filing form.",
                         "name": "form_type",
                         "optional": true,
-                        "type": "Literal['1', '1-A', '1-A POS', '1-A-W', '1-E', '1-E AD', '1-K', '1-SA', '1-U', '1-Z', '1-Z-W', '10-12B', '10-12G', '10-D', '10-K', '10-KT', '10-Q', '10-QT', '11-K', '11-KT', '13F-HR', '13F-NT', '13FCONP', '144', '15-12B', '15-12G', '15-15D', '15F-12B', '15F-12G', '15F-15D', '18-12B', '18-K', '19B-4E', '2-A', '2-AF', '2-E', '20-F', '20FR12B', '20FR12G', '24F-2NT', '25', '25-NSE', '253G1', '253G2', '253G3', '253G4', '3', '305B2', '34-12H', '4', '40-17F1', '40-17F2', '40-17G', '40-17GCS', '40-202A', '40-203A', '40-206A', '40-24B2', '40-33', '40-6B', '40-8B25', '40-8F-2', '40-APP', '40-F', '40-OIP', '40FR12B', '40FR12G', '424A', '424B1', '424B2', '424B3', '424B4', '424B5', '424B7', '424B8', '424H', '425', '485APOS', '485BPOS', '485BXT', '486APOS', '486BPOS', '486BXT', '487', '497', '497AD', '497H2', '497J', '497K', '497VPI', '497VPU', '5', '6-K', '6B NTC', '6B ORDR', '8-A12B', '8-A12G', '8-K', '8-K12B', '8-K12G3', '8-K15D5', '8-M', '8F-2 NTC', '8F-2 ORDR', '9-M', 'ABS-15G', 'ABS-EE', 'ADN-MTL', 'ADV-E', 'ADV-H-C', 'ADV-H-T', 'ADV-NR', 'ANNLRPT', 'APP NTC', 'APP ORDR', 'APP WD', 'APP WDG', 'ARS', 'ATS-N', 'ATS-N-C', 'ATS-N/UA', 'AW', 'AW WD', 'C', 'C-AR', 'C-AR-W', 'C-TR', 'C-TR-W', 'C-U', 'C-U-W', 'C-W', 'CB', 'CERT', 'CERTARCA', 'CERTBATS', 'CERTCBO', 'CERTNAS', 'CERTNYS', 'CERTPAC', 'CFPORTAL', 'CFPORTAL-W', 'CORRESP', 'CT ORDER', 'D', 'DEF 14A', 'DEF 14C', 'DEFA14A', 'DEFA14C', 'DEFC14A', 'DEFC14C', 'DEFM14A', 'DEFM14C', 'DEFN14A', 'DEFR14A', 'DEFR14C', 'DEL AM', 'DFAN14A', 'DFRN14A', 'DOS', 'DOSLTR', 'DRS', 'DRSLTR', 'DSTRBRPT', 'EFFECT', 'F-1', 'F-10', 'F-10EF', 'F-10POS', 'F-1MEF', 'F-3', 'F-3ASR', 'F-3D', 'F-3DPOS', 'F-3MEF', 'F-4', 'F-4 POS', 'F-4MEF', 'F-6', 'F-6 POS', 'F-6EF', 'F-7', 'F-7 POS', 'F-8', 'F-8 POS', 'F-80', 'F-80POS', 'F-9', 'F-9 POS', 'F-N', 'F-X', 'FOCUSN', 'FWP', 'G-405', 'G-405N', 'G-FIN', 'G-FINW', 'IRANNOTICE', 'MA', 'MA-A', 'MA-I', 'MA-W', 'MSD', 'MSDCO', 'MSDW', 'N-1', 'N-14', 'N-14 8C', 'N-14MEF', 'N-18F1', 'N-1A', 'N-2', 'N-2 POSASR', 'N-23C-2', 'N-23C3A', 'N-23C3B', 'N-23C3C', 'N-2ASR', 'N-2MEF', 'N-30B-2', 'N-30D', 'N-4', 'N-5', 'N-54A', 'N-54C', 'N-6', 'N-6F', 'N-8A', 'N-8B-2', 'N-8F', 'N-8F NTC', 'N-8F ORDR', 'N-CEN', 'N-CR', 'N-CSR', 'N-CSRS', 'N-MFP', 'N-MFP1', 'N-MFP2', 'N-PX', 'N-Q', 'N-VP', 'N-VPFS', 'NO ACT', 'NPORT-EX', 'NPORT-NP', 'NPORT-P', 'NRSRO-CE', 'NRSRO-UPD', 'NSAR-A', 'NSAR-AT', 'NSAR-B', 'NSAR-BT', 'NSAR-U', 'NT 10-D', 'NT 10-K', 'NT 10-Q', 'NT 11-K', 'NT 20-F', 'NT N-CEN', 'NT N-MFP', 'NT N-MFP1', 'NT N-MFP2', 'NT NPORT-EX', 'NT NPORT-P', 'NT-NCEN', 'NT-NCSR', 'NT-NSAR', 'NTFNCEN', 'NTFNCSR', 'NTFNSAR', 'NTN 10D', 'NTN 10K', 'NTN 10Q', 'NTN 20F', 'OIP NTC', 'OIP ORDR', 'POS 8C', 'POS AM', 'POS AMI', 'POS EX', 'POS462B', 'POS462C', 'POSASR', 'PRE 14A', 'PRE 14C', 'PREC14A', 'PREC14C', 'PREM14A', 'PREM14C', 'PREN14A', 'PRER14A', 'PRER14C', 'PRRN14A', 'PX14A6G', 'PX14A6N', 'QRTLYRPT', 'QUALIF', 'REG-NR', 'REVOKED', 'RW', 'RW WD', 'S-1', 'S-11', 'S-11MEF', 'S-1MEF', 'S-20', 'S-3', 'S-3ASR', 'S-3D', 'S-3DPOS', 'S-3MEF', 'S-4', 'S-4 POS', 'S-4EF', 'S-4MEF', 'S-6', 'S-8', 'S-8 POS', 'S-B', 'S-BMEF', 'SBSE', 'SBSE-A', 'SBSE-BD', 'SBSE-C', 'SBSE-W', 'SC 13D', 'SC 13E1', 'SC 13E3', 'SC 13G', 'SC 14D9', 'SC 14F1', 'SC 14N', 'SC TO-C', 'SC TO-I', 'SC TO-T', 'SC13E4F', 'SC14D1F', 'SC14D9C', 'SC14D9F', 'SD', 'SDR', 'SE', 'SEC ACTION', 'SEC STAFF ACTION', 'SEC STAFF LETTER', 'SF-1', 'SF-3', 'SL', 'SP 15D2', 'STOP ORDER', 'SUPPL', 'T-3', 'TA-1', 'TA-2', 'TA-W', 'TACO', 'TH', 'TTW', 'UNDER', 'UPLOAD', 'WDL-REQ', 'X-17A-5']"
+                        "type": "Literal['1', '1-A', '1-A_POS', '1-A-W', '1-E', '1-E_AD', '1-K', '1-SA', '1-U', '1-Z', '1-Z-W', '10-12B', '10-12G', '10-D', '10-K', '10-KT', '10-Q', '10-QT', '11-K', '11-KT', '13F-HR', '13F-NT', '13FCONP', '144', '15-12B', '15-12G', '15-15D', '15F-12B', '15F-12G', '15F-15D', '18-12B', '18-K', '19B-4E', '2-A', '2-AF', '2-E', '20-F', '20FR12B', '20FR12G', '24F-2NT', '25', '25-NSE', '253G1', '253G2', '253G3', '253G4', '3', '305B2', '34-12H', '4', '40-17F1', '40-17F2', '40-17G', '40-17GCS', '40-202A', '40-203A', '40-206A', '40-24B2', '40-33', '40-6B', '40-8B25', '40-8F-2', '40-APP', '40-F', '40-OIP', '40FR12B', '40FR12G', '424A', '424B1', '424B2', '424B3', '424B4', '424B5', '424B7', '424B8', '424H', '425', '485APOS', '485BPOS', '485BXT', '486APOS', '486BPOS', '486BXT', '487', '497', '497AD', '497H2', '497J', '497K', '497VPI', '497VPU', '5', '6-K', '6B_NTC', '6B_ORDR', '8-A12B', '8-A12G', '8-K', '8-K12B', '8-K12G3', '8-K15D5', '8-M', '8F-2_NTC', '8F-2_ORDR', '9-M', 'ABS-15G', 'ABS-EE', 'ADN-MTL', 'ADV-E', 'ADV-H-C', 'ADV-H-T', 'ADV-NR', 'ANNLRPT', 'APP_NTC', 'APP_ORDR', 'APP_WD', 'APP_WDG', 'ARS', 'ATS-N', 'ATS-N-C', 'ATS-N/UA', 'AW', 'AW_WD', 'C', 'C-AR', 'C-AR-W', 'C-TR', 'C-TR-W', 'C-U', 'C-U-W', 'C-W', 'CB', 'CERT', 'CERTARCA', 'CERTBATS', 'CERTCBO', 'CERTNAS', 'CERTNYS', 'CERTPAC', 'CFPORTAL', 'CFPORTAL-W', 'CORRESP', 'CT_ORDER', 'D', 'DEF_14A', 'DEF_14C', 'DEFA14A', 'DEFA14C', 'DEFC14A', 'DEFC14C', 'DEFM14A', 'DEFM14C', 'DEFN14A', 'DEFR14A', 'DEFR14C', 'DEL_AM', 'DFAN14A', 'DFRN14A', 'DOS', 'DOSLTR', 'DRS', 'DRSLTR', 'DSTRBRPT', 'EFFECT', 'F-1', 'F-10', 'F-10EF', 'F-10POS', 'F-1MEF', 'F-3', 'F-3ASR', 'F-3D', 'F-3DPOS', 'F-3MEF', 'F-4', 'F-4_POS', 'F-4MEF', 'F-6', 'F-6_POS', 'F-6EF', 'F-7', 'F-7_POS', 'F-8', 'F-8_POS', 'F-80', 'F-80POS', 'F-9', 'F-9_POS', 'F-N', 'F-X', 'FOCUSN', 'FWP', 'G-405', 'G-405N', 'G-FIN', 'G-FINW', 'IRANNOTICE', 'MA', 'MA-A', 'MA-I', 'MA-W', 'MSD', 'MSDCO', 'MSDW', 'N-1', 'N-14', 'N-14_8C', 'N-14MEF', 'N-18F1', 'N-1A', 'N-2', 'N-2_POSASR', 'N-23C-2', 'N-23C3A', 'N-23C3B', 'N-23C3C', 'N-2ASR', 'N-2MEF', 'N-30B-2', 'N-30D', 'N-4', 'N-5', 'N-54A', 'N-54C', 'N-6', 'N-6F', 'N-8A', 'N-8B-2', 'N-8F', 'N-8F_NTC', 'N-8F_ORDR', 'N-CEN', 'N-CR', 'N-CSR', 'N-CSRS', 'N-MFP', 'N-MFP1', 'N-MFP2', 'N-PX', 'N-Q', 'N-VP', 'N-VPFS', 'NO_ACT', 'NPORT-EX', 'NPORT-NP', 'NPORT-P', 'NRSRO-CE', 'NRSRO-UPD', 'NSAR-A', 'NSAR-AT', 'NSAR-B', 'NSAR-BT', 'NSAR-U', 'NT_10-D', 'NT_10-K', 'NT_10-Q', 'NT_11-K', 'NT_20-F', 'NT_N-CEN', 'NT_N-MFP', 'NT_N-MFP1', 'NT_N-MFP2', 'NT_NPORT-EX', 'NT_NPORT-P', 'NT-NCEN', 'NT-NCSR', 'NT-NSAR', 'NTFNCEN', 'NTFNCSR', 'NTFNSAR', 'NTN_10D', 'NTN_10K', 'NTN_10Q', 'NTN_20F', 'OIP_NTC', 'OIP_ORDR', 'POS_8C', 'POS_AM', 'POS_AMI', 'POS_EX', 'POS462B', 'POS462C', 'POSASR', 'PRE_14A', 'PRE_14C', 'PREC14A', 'PREC14C', 'PREM14A', 'PREM14C', 'PREN14A', 'PRER14A', 'PRER14C', 'PRRN14A', 'PX14A6G', 'PX14A6N', 'QRTLYRPT', 'QUALIF', 'REG-NR', 'REVOKED', 'RW', 'RW_WD', 'S-1', 'S-11', 'S-11MEF', 'S-1MEF', 'S-20', 'S-3', 'S-3ASR', 'S-3D', 'S-3DPOS', 'S-3MEF', 'S-4', 'S-4_POS', 'S-4EF', 'S-4MEF', 'S-6', 'S-8', 'S-8_POS', 'S-B', 'S-BMEF', 'SBSE', 'SBSE-A', 'SBSE-BD', 'SBSE-C', 'SBSE-W', 'SC_13D', 'SC_13E1', 'SC_13E3', 'SC_13G', 'SC_14D9', 'SC_14F1', 'SC_14N', 'SC_TO-C', 'SC_TO-I', 'SC_TO-T', 'SC13E4F', 'SC14D1F', 'SC14D9C', 'SC14D9F', 'SD', 'SDR', 'SE', 'SEC_ACTION', 'SEC_STAFF_ACTION', 'SEC_STAFF_LETTER', 'SF-1', 'SF-3', 'SL', 'SP_15D2', 'STOP_ORDER', 'SUPPL', 'T-3', 'TA-1', 'TA-2', 'TA-W', 'TACO', 'TH', 'TTW', 'UNDER', 'UPLOAD', 'WDL-REQ', 'X-17A-5']"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Lookup filings by Central Index Key (CIK) instead of by symbol.",
                         "name": "cik",
                         "optional": true,
@@ -15575,31 +16565,31 @@
         },
         "/equity/fundamental/metrics": {
             "data": {
                 "fmp": [
                     {
                         "choices": null,
                         "default": "",
-                        "description": "The date of the data.",
-                        "name": "date",
+                        "description": "Period ending date.",
+                        "name": "period_ending",
                         "optional": false,
                         "type": "date"
                     },
                     {
                         "choices": null,
                         "default": "",
                         "description": "Period of the data.",
-                        "name": "period",
+                        "name": "fiscal_period",
                         "optional": false,
                         "type": "str"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "Calendar year.",
+                        "description": "Calendar year for the fiscal period.",
                         "name": "calendar_year",
                         "optional": true,
                         "type": "int"
                     },
                     {
                         "choices": null,
                         "default": null,
@@ -15607,14 +16597,22 @@
                         "name": "revenue_per_share",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
+                        "description": "Capital expenditures per share",
+                        "name": "capex_per_share",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
                         "description": "Net income per share",
                         "name": "net_income_per_share",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
@@ -15671,56 +16669,48 @@
                         "name": "interest_debt_per_share",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "Enterprise value",
-                        "name": "enterprise_value",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
                         "description": "Price-to-sales ratio",
-                        "name": "price_to_sales_ratio",
+                        "name": "price_to_sales",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Price-to-operating cash flow ratio",
-                        "name": "pocf_ratio",
+                        "name": "price_to_operating_cash_flow",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Price-to-free cash flow ratio",
-                        "name": "pfcf_ratio",
+                        "name": "price_to_free_cash_flow",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Price-to-book ratio",
-                        "name": "pb_ratio",
+                        "name": "price_to_book",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Price-to-tangible book ratio",
-                        "name": "ptb_ratio",
+                        "name": "price_to_tangible_book",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Enterprise value-to-sales ratio",
@@ -15728,15 +16718,15 @@
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Enterprise value-to-EBITDA ratio",
-                        "name": "enterprise_value_over_ebitda",
+                        "name": "ev_to_ebitda",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Enterprise value-to-operating cash flow ratio",
@@ -15767,14 +16757,22 @@
                         "name": "free_cash_flow_yield",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
+                        "description": "Debt-to-market capitalization ratio",
+                        "name": "debt_to_market_cap",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
                         "description": "Debt-to-equity ratio",
                         "name": "debt_to_equity",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
@@ -15815,22 +16813,14 @@
                         "name": "income_quality",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "Dividend yield, as a normalized percent.",
-                        "name": "dividend_yield",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
                         "description": "Payout ratio",
                         "name": "payout_ratio",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
@@ -15887,46 +16877,14 @@
                         "name": "stock_based_compensation_to_revenue",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "Graham number",
-                        "name": "graham_number",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Return on invested capital",
-                        "name": "roic",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Return on tangible assets",
-                        "name": "return_on_tangible_assets",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Graham net-net working capital",
-                        "name": "graham_net_net",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
                         "description": "Working capital",
                         "name": "working_capital",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
@@ -15943,14 +16901,22 @@
                         "name": "net_current_asset_value",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
+                        "description": "Enterprise value",
+                        "name": "enterprise_value",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
                         "description": "Invested capital",
                         "name": "invested_capital",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
@@ -16024,23 +16990,55 @@
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Return on equity",
-                        "name": "roe",
+                        "name": "return_on_equity",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "Capital expenditures per share",
-                        "name": "capex_per_share",
+                        "description": "Return on invested capital",
+                        "name": "return_on_invested_capital",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Return on tangible assets",
+                        "name": "return_on_tangible_assets",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Dividend yield, as a normalized percent.",
+                        "name": "dividend_yield",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Graham number",
+                        "name": "graham_number",
+                        "optional": true,
+                        "type": "float"
+                    },
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "Graham net-net working capital",
+                        "name": "graham_net_net",
                         "optional": true,
                         "type": "float"
                     }
                 ],
                 "intrinio": [
                     {
                         "choices": null,
@@ -19853,15 +20851,15 @@
                 "fmp": [
                     {
                         "choices": null,
                         "default": null,
                         "description": "Type of the transaction.",
                         "name": "transaction_type",
                         "optional": true,
-                        "type": "Literal[None, 'award', 'conversion', 'return', 'expire_short', 'in_kind', 'gift', 'expire_long', 'discretionary', 'other', 'small', 'exempt', 'otm', 'purchase', 'sale', 'tender', 'will', 'itm', 'trust']"
+                        "type": "Literal['award', 'conversion', 'return', 'expire_short', 'in_kind', 'gift', 'expire_long', 'discretionary', 'other', 'small', 'exempt', 'otm', 'purchase', 'sale', 'tender', 'will', 'itm', 'trust']"
                     }
                 ],
                 "intrinio": [
                     {
                         "choices": null,
                         "default": "",
                         "description": "Start date of the data, in YYYY-MM-DD format.",
@@ -23188,15 +24186,15 @@
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Filter by sector.",
                         "name": "sector",
                         "optional": true,
-                        "type": "Literal['Consumer Cyclical', 'Energy', 'Technology', 'Industrials', 'Financial Services', 'Basic Materials', 'Communication Services', 'Consumer Defensive', 'Healthcare', 'Real Estate', 'Utilities', 'Industrial Goods', 'Financial', 'Services', 'Conglomerates']"
+                        "type": "Literal['consumer_cyclical', 'energy', 'technology', 'industrials', 'financial_services', 'basic_materials', 'communication_services', 'consumer_defensive', 'healthcare', 'real_estate', 'utilities', 'industrial_goods', 'financial', 'services', 'conglomerates']"
                     },
                     {
                         "choices": null,
                         "default": null,
                         "description": "Filter by industry.",
                         "name": "industry",
                         "optional": true,
@@ -25388,222 +26386,14 @@
                         "description": "Extra info.",
                         "name": "extra",
                         "type": "Dict[str, Any]"
                     }
                 ]
             }
         },
-        "/etf/holdings_performance": {
-            "data": {
-                "fmp": [
-                    {
-                        "choices": null,
-                        "default": "",
-                        "description": "The ticker symbol.",
-                        "name": "symbol",
-                        "optional": false,
-                        "type": "str"
-                    }
-                ],
-                "standard": [
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Symbol representing the entity requested in the data.",
-                        "name": "symbol",
-                        "optional": true,
-                        "type": "str"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "One-day return.",
-                        "name": "one_day",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Week to date return.",
-                        "name": "wtd",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "One-week return.",
-                        "name": "one_week",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Month to date return.",
-                        "name": "mtd",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "One-month return.",
-                        "name": "one_month",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Quarter to date return.",
-                        "name": "qtd",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Three-month return.",
-                        "name": "three_month",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Six-month return.",
-                        "name": "six_month",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Year to date return.",
-                        "name": "ytd",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "One-year return.",
-                        "name": "one_year",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Two-year return.",
-                        "name": "two_year",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Three-year return.",
-                        "name": "three_year",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Four-year",
-                        "name": "four_year",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Five-year return.",
-                        "name": "five_year",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Ten-year return.",
-                        "name": "ten_year",
-                        "optional": true,
-                        "type": "float"
-                    },
-                    {
-                        "choices": null,
-                        "default": null,
-                        "description": "Return from the beginning of the time series.",
-                        "name": "max",
-                        "optional": true,
-                        "type": "float"
-                    }
-                ]
-            },
-            "deprecated": {
-                "flag": true,
-                "message": "This endpoint is deprecated; pass a list of holdings symbols directly to `/equity/price/performance` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.2."
-            },
-            "description": "Get the recent price performance of each ticker held in the ETF.",
-            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.etf.holdings_performance(symbol='XLK', provider='fmp')\n```\n\n",
-            "model": "EtfHoldingsPerformance",
-            "parameters": {
-                "fmp": [],
-                "standard": [
-                    {
-                        "choices": null,
-                        "default": "",
-                        "description": "Symbol to get data for. Multiple items allowed for provider(s): fmp.",
-                        "name": "symbol",
-                        "optional": false,
-                        "type": "Union[str, List[str]]"
-                    },
-                    {
-                        "default": "fmp",
-                        "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'fmp' if there is no default.",
-                        "name": "provider",
-                        "optional": true,
-                        "type": "Literal['fmp']"
-                    }
-                ]
-            },
-            "returns": {
-                "OBBject": [
-                    {
-                        "description": "Serializable results.",
-                        "name": "results",
-                        "type": "List[EtfHoldingsPerformance]"
-                    },
-                    {
-                        "description": "Provider name.",
-                        "name": "provider",
-                        "type": "Optional[Literal['fmp']]"
-                    },
-                    {
-                        "description": "List of warnings.",
-                        "name": "warnings",
-                        "type": "Optional[List[Warning_]]"
-                    },
-                    {
-                        "description": "Chart object.",
-                        "name": "chart",
-                        "type": "Optional[Chart]"
-                    },
-                    {
-                        "description": "Extra info.",
-                        "name": "extra",
-                        "type": "Dict[str, Any]"
-                    }
-                ]
-            }
-        },
         "/etf/info": {
             "data": {
                 "fmp": [
                     {
                         "choices": null,
                         "default": null,
                         "description": "Company of the ETF.",
@@ -28395,16 +29185,16 @@
                         "name": "rate",
                         "optional": false,
                         "type": "float"
                     }
                 ]
             },
             "deprecated": {
-                "flag": null,
-                "message": null
+                "flag": true,
+                "message": "This endpoint will be removed in a future version. Use, `/fixedincome/government/yield_curve`, instead. Deprecated in OpenBB Platform V4.2 to be removed in V4.4."
             },
             "description": "US Yield Curve. Get United States yield curve.",
             "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.fixedincome.government.us_yield_curve(provider='fred')\nobb.fixedincome.government.us_yield_curve(inflation_adjusted=True, provider='fred')\n```\n\n",
             "model": "USYieldCurve",
             "parameters": {
                 "fred": [],
                 "standard": [
@@ -28459,14 +29249,151 @@
                         "description": "Extra info.",
                         "name": "extra",
                         "type": "Dict[str, Any]"
                     }
                 ]
             }
         },
+        "/fixedincome/government/yield_curve": {
+            "data": {
+                "econdb": [],
+                "federal_reserve": [],
+                "fmp": [],
+                "fred": [],
+                "standard": [
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "The date of the data.",
+                        "name": "date",
+                        "optional": true,
+                        "type": "date"
+                    },
+                    {
+                        "choices": null,
+                        "default": "",
+                        "description": "Maturity length of the security.",
+                        "name": "maturity",
+                        "optional": false,
+                        "type": "str"
+                    },
+                    {
+                        "choices": null,
+                        "default": "",
+                        "description": "The yield as a normalized percent (0.05 is 5%)",
+                        "name": "rate",
+                        "optional": false,
+                        "type": "float"
+                    }
+                ]
+            },
+            "deprecated": {
+                "flag": null,
+                "message": null
+            },
+            "description": "Get yield curve data by country and date.",
+            "examples": "\nExamples\n--------\n\n```python\nfrom openbb import obb\nobb.fixedincome.government.yield_curve(provider='federal_reserve')\nobb.fixedincome.government.yield_curve(date='2023-05-01,2024-05-01', provider='fmp')\nobb.fixedincome.government.yield_curve(date='2023-05-01', country=united_kingdom, provider='econdb')\nobb.fixedincome.government.yield_curve(provider='fred', yield_curve_type=real, date='2023-05-01,2024-05-01')\n```\n\n",
+            "model": "YieldCurve",
+            "parameters": {
+                "econdb": [
+                    {
+                        "choices": [
+                            "australia",
+                            "canada",
+                            "china",
+                            "hong_kong",
+                            "india",
+                            "japan",
+                            "mexico",
+                            "new_zealand",
+                            "russia",
+                            "saudi_arabia",
+                            "singapore",
+                            "south_africa",
+                            "south_korea",
+                            "taiwan",
+                            "thailand",
+                            "united_kingdom",
+                            "united_states"
+                        ],
+                        "default": "united_states",
+                        "description": "The country to get data. New Zealand, Mexico, Singapore, and Thailand have only monthly data. The nearest date to the requested one will be used.",
+                        "name": "country",
+                        "optional": true,
+                        "type": "Literal['australia', 'canada', 'china', 'hong_kong', 'india', 'japan', 'mexico', 'new_zealand', 'russia', 'saudi_arabia', 'singapore', 'south_africa', 'south_korea', 'taiwan', 'thailand', 'united_kingdom', 'united_states']"
+                    },
+                    {
+                        "choices": null,
+                        "default": true,
+                        "description": "If true, cache the request for four hours.",
+                        "name": "use_cache",
+                        "optional": true,
+                        "type": "bool"
+                    }
+                ],
+                "federal_reserve": [],
+                "fmp": [],
+                "fred": [
+                    {
+                        "choices": null,
+                        "default": "nominal",
+                        "description": "Yield curve type. Nominal and Real Rates are available daily, others are monthly. The closest date to the requested date will be returned.",
+                        "name": "yield_curve_type",
+                        "optional": true,
+                        "type": "Literal['nominal', 'real', 'breakeven', 'corporate_spot', 'corporate_par']"
+                    }
+                ],
+                "standard": [
+                    {
+                        "choices": null,
+                        "default": null,
+                        "description": "A specific date to get data for. By default is the current data. Multiple items allowed for provider(s): econdb, federal_reserve, fmp, fred.",
+                        "name": "date",
+                        "optional": true,
+                        "type": "Union[Union[str, str], List[Union[str, str]]]"
+                    },
+                    {
+                        "default": "econdb",
+                        "description": "The provider to use for the query, by default None. If None, the provider specified in defaults is selected or 'econdb' if there is no default.",
+                        "name": "provider",
+                        "optional": true,
+                        "type": "Literal['econdb', 'federal_reserve', 'fmp', 'fred']"
+                    }
+                ]
+            },
+            "returns": {
+                "OBBject": [
+                    {
+                        "description": "Serializable results.",
+                        "name": "results",
+                        "type": "List[YieldCurve]"
+                    },
+                    {
+                        "description": "Provider name.",
+                        "name": "provider",
+                        "type": "Optional[Literal['econdb', 'federal_reserve', 'fmp', 'fred']]"
+                    },
+                    {
+                        "description": "List of warnings.",
+                        "name": "warnings",
+                        "type": "Optional[List[Warning_]]"
+                    },
+                    {
+                        "description": "Chart object.",
+                        "name": "chart",
+                        "type": "Optional[Chart]"
+                    },
+                    {
+                        "description": "Extra info.",
+                        "name": "extra",
+                        "type": "Dict[str, Any]"
+                    }
+                ]
+            }
+        },
         "/fixedincome/rate/ameribor": {
             "data": {
                 "fred": [],
                 "standard": [
                     {
                         "choices": null,
                         "default": "",
@@ -30819,23 +31746,23 @@
                         "name": "is_spam",
                         "optional": true,
                         "type": "bool"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "News stories will have a business relevance score more than this value. Unsupported for yahoo source.",
+                        "description": "News stories will have a business relevance score more than this value. Unsupported for yahoo source. Value is a decimal between 0 and 1.",
                         "name": "business_relevance_greater_than",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "News stories will have a business relevance score less than this value. Unsupported for yahoo source.",
+                        "description": "News stories will have a business relevance score less than this value. Unsupported for yahoo source. Value is a decimal between 0 and 1.",
                         "name": "business_relevance_less_than",
                         "optional": true,
                         "type": "float"
                     }
                 ],
                 "polygon": [
                     {
@@ -31362,23 +32289,23 @@
                         "name": "is_spam",
                         "optional": true,
                         "type": "bool"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "News stories will have a business relevance score more than this value. Unsupported for yahoo source.",
+                        "description": "News stories will have a business relevance score more than this value. Unsupported for yahoo source. Value is a decimal between 0 and 1.",
                         "name": "business_relevance_greater_than",
                         "optional": true,
                         "type": "float"
                     },
                     {
                         "choices": null,
                         "default": null,
-                        "description": "News stories will have a business relevance score less than this value. Unsupported for yahoo source.",
+                        "description": "News stories will have a business relevance score less than this value. Unsupported for yahoo source. Value is a decimal between 0 and 1.",
                         "name": "business_relevance_less_than",
                         "optional": true,
                         "type": "float"
                     }
                 ],
                 "standard": [
                     {
```

### Comparing `openbb-4.2.0/openbb/package/__extensions__.py` & `openbb-4.2.1/openbb/package/__extensions__.py`

 * *Files identical despite different names*

### Comparing `openbb-4.2.0/openbb/package/crypto.py` & `openbb-4.2.1/openbb/package/crypto.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,14 +87,18 @@
         """  # noqa: E501
 
         return self._run(
             "/crypto/search",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/crypto/search", ("fmp",),
+                        provider,
+                        "/crypto/search",
+                        ("fmp",),
                     )
                 },
-                standard_params={"query": query,},
+                standard_params={
+                    "query": query,
+                },
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/crypto_price.py` & `openbb-4.2.1/openbb/package/crypto_price.py`

 * *Files identical despite different names*

### Comparing `openbb-4.2.0/openbb/package/currency.py` & `openbb-4.2.1/openbb/package/currency.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,26 +111,30 @@
         Examples
         --------
         >>> from openbb import obb
         >>> obb.currency.search(provider='fmp')
         >>> # Search for 'EUR' currency pair using 'intrinio' as provider.
         >>> obb.currency.search(provider='intrinio', query='EUR')
         >>> # Search for terms  using 'polygon' as provider.
-        >>> obb.currency.search(provider='polygon', query='Euro zone')
+        >>> obb.currency.search(provider='polygon', query='EUR')
         """  # noqa: E501
 
         return self._run(
             "/currency/search",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/currency/search", ("fmp", "intrinio", "polygon"),
+                        provider,
+                        "/currency/search",
+                        ("fmp", "intrinio", "polygon"),
                     )
                 },
-                standard_params={"query": query,},
+                standard_params={
+                    "query": query,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def snapshots(
@@ -271,15 +275,17 @@
         """  # noqa: E501
 
         return self._run(
             "/currency/snapshots",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/currency/snapshots", ("fmp", "polygon"),
+                        provider,
+                        "/currency/snapshots",
+                        ("fmp", "polygon"),
                     )
                 },
                 standard_params={
                     "base": base,
                     "quote_type": quote_type,
                     "counter_currencies": counter_currencies,
                 },
```

### Comparing `openbb-4.2.0/openbb/package/currency_price.py` & `openbb-4.2.1/openbb/package/currency_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             Optional[Literal["fmp", "polygon", "tiingo", "yfinance"]],
             OpenBBField(
                 description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
-        """    Currency Historical Price. Currency historical data.
+        """Currency Historical Price. Currency historical data.
 
         Currency historical prices refer to the past exchange rates of one currency against
         another over a specific period.
         This data provides insight into the fluctuations and trends in the foreign exchange market,
         helping analysts, traders, and economists understand currency performance,
         evaluate economic health, and make predictions about future movements.
```

### Comparing `openbb-4.2.0/openbb/package/derivatives.py` & `openbb-4.2.1/openbb/package/derivatives.py`

 * *Files identical despite different names*

### Comparing `openbb-4.2.0/openbb/package/derivatives_options.py` & `openbb-4.2.1/openbb/package/derivatives_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,18 +159,22 @@
         """  # noqa: E501
 
         return self._run(
             "/derivatives/options/chains",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/derivatives/options/chains", ("intrinio",),
+                        provider,
+                        "/derivatives/options/chains",
+                        ("intrinio",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def unusual(
@@ -252,24 +256,28 @@
             The total number of contracts involved in a single transaction. (provider: intrinio)
         total_value : Optional[Union[int, float]]
             The aggregated value of all option contract premiums included in the trade. (provider: intrinio)
 
         Examples
         --------
         >>> from openbb import obb
-        >>> obb.derivatives.options.unusual(provider='intrinio')
+        >>> obb.derivatives.options.unusual(symbol='TSLA', provider='intrinio')
         >>> # Use the 'symbol' parameter to get the most recent activity for a specific symbol.
         >>> obb.derivatives.options.unusual(symbol='TSLA', provider='intrinio')
         """  # noqa: E501
 
         return self._run(
             "/derivatives/options/unusual",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/derivatives/options/unusual", ("intrinio",),
+                        provider,
+                        "/derivatives/options/unusual",
+                        ("intrinio",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/economy.py` & `openbb-4.2.1/openbb/package/economy.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
 class ROUTER_economy(Container):
     """/economy
     available_indicators
+    balance_of_payments
     calendar
     composite_leading_indicator
     country_profile
     cpi
     fred_regional
     fred_search
     fred_series
@@ -108,15 +109,125 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/available_indicators",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/available_indicators", ("econdb",),
+                        provider,
+                        "/economy/available_indicators",
+                        ("econdb",),
+                    )
+                },
+                standard_params={},
+                extra_params=kwargs,
+            )
+        )
+
+    @exception_handler
+    @validate
+    def balance_of_payments(
+        self,
+        provider: Annotated[
+            Optional[Literal["fred"]],
+            OpenBBField(
+                description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fred' if there is\n    no default."
+            ),
+        ] = None,
+        **kwargs
+    ) -> OBBject:
+        """Balance of Payments Reports.
+
+        Parameters
+        ----------
+        provider : Optional[Literal['fred']]
+            The provider to use for the query, by default None.
+            If None, the provider specified in defaults is selected or 'fred' if there is
+            no default.
+        country : Literal['argentina', 'australia', 'austria', 'belgium', 'brazil', 'canada', 'chile', 'china', 'colombia', 'costa_rica', 'czechia', 'denmark', 'estonia', 'finland', 'france', 'germany', 'greece', 'hungary', 'iceland', 'india', 'indonesia', 'ireland', 'israel', 'italy', 'japan', 'korea', 'latvia', 'lithuania', 'luxembourg', 'mexico', 'netherlands', 'new_zealand', 'norway', 'poland', 'portugal', 'russia', 'saudi_arabia', 'slovak_republic', 'slovenia', 'south_africa', 'spain', 'sweden', 'switzerland', 'turkey', 'united_kingdom', 'united_states', 'g7', 'g20']
+            The country to get data. Enter as a 3-letter ISO country code, default is USA. (provider: fred)
+        start_date : Optional[datetime.date]
+            Start date of the data, in YYYY-MM-DD format. (provider: fred)
+        end_date : Optional[datetime.date]
+            End date of the data, in YYYY-MM-DD format. (provider: fred)
+
+        Returns
+        -------
+        OBBject
+            results : List[BalanceOfPayments]
+                Serializable results.
+            provider : Optional[Literal['fred']]
+                Provider name.
+            warnings : Optional[List[Warning_]]
+                List of warnings.
+            chart : Optional[Chart]
+                Chart object.
+            extra : Dict[str, Any]
+                Extra info.
+
+        BalanceOfPayments
+        -----------------
+        period : Optional[date]
+            The date representing the beginning of the reporting period.
+        balance_percent_of_gdp : Optional[float]
+            Current Account Balance as Percent of GDP
+        balance_total : Optional[float]
+            Current Account Total Balance (USD)
+        balance_total_services : Optional[float]
+            Current Account Total Services Balance (USD)
+        balance_total_secondary_income : Optional[float]
+            Current Account Total Secondary Income Balance (USD)
+        balance_total_goods : Optional[float]
+            Current Account Total Goods Balance (USD)
+        balance_total_primary_income : Optional[float]
+            Current Account Total Primary Income Balance (USD)
+        credits_services_percent_of_goods_and_services : Optional[float]
+            Current Account Credits Services as Percent of Goods and Services
+        credits_services_percent_of_current_account : Optional[float]
+            Current Account Credits Services as Percent of Current Account
+        credits_total_services : Optional[float]
+            Current Account Credits Total Services (USD)
+        credits_total_goods : Optional[float]
+            Current Account Credits Total Goods (USD)
+        credits_total_primary_income : Optional[float]
+            Current Account Credits Total Primary Income (USD)
+        credits_total_secondary_income : Optional[float]
+            Current Account Credits Total Secondary Income (USD)
+        credits_total : Optional[float]
+            Current Account Credits Total (USD)
+        debits_services_percent_of_goods_and_services : Optional[float]
+            Current Account Debits Services as Percent of Goods and Services
+        debits_services_percent_of_current_account : Optional[float]
+            Current Account Debits Services as Percent of Current Account
+        debits_total_services : Optional[float]
+            Current Account Debits Total Services (USD)
+        debits_total_goods : Optional[float]
+            Current Account Debits Total Goods (USD)
+        debits_total_primary_income : Optional[float]
+            Current Account Debits Total Primary Income (USD)
+        debits_total : Optional[float]
+            Current Account Debits Total (USD)
+        debits_total_secondary_income : Optional[float]
+            Current Account Debits Total Secondary Income (USD)
+
+        Examples
+        --------
+        >>> from openbb import obb
+        >>> obb.economy.balance_of_payments(provider='fred')
+        >>> obb.economy.balance_of_payments(provider='fred', country='brazil')
+        """  # noqa: E501
+
+        return self._run(
+            "/economy/balance_of_payments",
+            **filter_inputs(
+                provider_choices={
+                    "provider": self._get_provider(
+                        provider,
+                        "/economy/balance_of_payments",
+                        ("fred",),
                     )
                 },
                 standard_params={},
                 extra_params=kwargs,
             )
         )
 
@@ -238,18 +349,23 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/calendar",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/calendar", ("fmp", "tradingeconomics"),
+                        provider,
+                        "/economy/calendar",
+                        ("fmp", "tradingeconomics"),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
                 info={
                     "country": {"tradingeconomics": {"multiple_items_allowed": True}},
                     "calendar_id": {
                         "tradingeconomics": {"multiple_items_allowed": True}
                     },
                 },
@@ -328,18 +444,23 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/composite_leading_indicator",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/composite_leading_indicator", ("oecd",),
+                        provider,
+                        "/economy/composite_leading_indicator",
+                        ("oecd",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def country_profile(
@@ -427,18 +548,22 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/country_profile",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/country_profile", ("econdb",),
+                        provider,
+                        "/economy/country_profile",
+                        ("econdb",),
                     )
                 },
-                standard_params={"country": country,},
+                standard_params={
+                    "country": country,
+                },
                 extra_params=kwargs,
                 info={"country": {"econdb": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -590,15 +715,19 @@
         >>> obb.economy.cpi(country='united_states,united_kingdom', units='growth_previous', provider='fred')
         """  # noqa: E501
 
         return self._run(
             "/economy/cpi",
             **filter_inputs(
                 provider_choices={
-                    "provider": self._get_provider(provider, "/economy/cpi", ("fred",),)
+                    "provider": self._get_provider(
+                        provider,
+                        "/economy/cpi",
+                        ("fred",),
+                    )
                 },
                 standard_params={
                     "country": country,
                     "units": units,
                     "frequency": frequency,
                     "harmonized": harmonized,
                     "start_date": start_date,
@@ -740,15 +869,17 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/fred_regional",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/fred_regional", ("fred",),
+                        provider,
+                        "/economy/fred_regional",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                     "limit": limit,
@@ -869,18 +1000,22 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/fred_search",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/fred_search", ("fred",),
+                        provider,
+                        "/economy/fred_search",
+                        ("fred",),
                     )
                 },
-                standard_params={"query": query,},
+                standard_params={
+                    "query": query,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def fred_series(
@@ -1004,15 +1139,17 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/fred_series",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/fred_series", ("fred", "intrinio"),
+                        provider,
+                        "/economy/fred_series",
+                        ("fred", "intrinio"),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                     "limit": limit,
@@ -1131,15 +1268,17 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/indicators",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/indicators", ("econdb",),
+                        provider,
+                        "/economy/indicators",
+                        ("econdb",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "country": country,
                     "start_date": start_date,
                     "end_date": end_date,
@@ -1230,18 +1369,23 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/long_term_interest_rate",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/long_term_interest_rate", ("oecd",),
+                        provider,
+                        "/economy/long_term_interest_rate",
+                        ("oecd",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def money_measures(
@@ -1325,15 +1469,17 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/money_measures",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/money_measures", ("federal_reserve",),
+                        provider,
+                        "/economy/money_measures",
+                        ("federal_reserve",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "adjusted": adjusted,
                 },
@@ -1394,15 +1540,17 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/risk_premium",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/risk_premium", ("fmp",),
+                        provider,
+                        "/economy/risk_premium",
+                        ("fmp",),
                     )
                 },
                 standard_params={},
                 extra_params=kwargs,
             )
         )
 
@@ -1482,18 +1630,23 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/short_term_interest_rate",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/short_term_interest_rate", ("oecd",),
+                        provider,
+                        "/economy/short_term_interest_rate",
+                        ("oecd",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def unemployment(
@@ -1570,14 +1723,19 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/unemployment",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/unemployment", ("oecd",),
+                        provider,
+                        "/economy/unemployment",
+                        ("oecd",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/economy_gdp.py` & `openbb-4.2.1/openbb/package/economy_gdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,17 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/gdp/forecast",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/gdp/forecast", ("oecd",),
+                        provider,
+                        "/economy/gdp/forecast",
+                        ("oecd",),
                     )
                 },
                 standard_params={
                     "period": period,
                     "start_date": start_date,
                     "end_date": end_date,
                     "type": type,
@@ -190,15 +192,17 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/gdp/nominal",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/gdp/nominal", ("oecd",),
+                        provider,
+                        "/economy/gdp/nominal",
+                        ("oecd",),
                     )
                 },
                 standard_params={
                     "units": units,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
@@ -278,15 +282,17 @@
         """  # noqa: E501
 
         return self._run(
             "/economy/gdp/real",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/economy/gdp/real", ("oecd",),
+                        provider,
+                        "/economy/gdp/real",
+                        ("oecd",),
                     )
                 },
                 standard_params={
                     "units": units,
                     "start_date": start_date,
                     "end_date": end_date,
                 },
```

### Comparing `openbb-4.2.0/openbb/package/equity.py` & `openbb-4.2.1/openbb/package/equity.py`

 * *Files 4% similar despite different names*

```diff
@@ -421,18 +421,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/profile",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/profile", ("fmp", "intrinio", "yfinance"),
+                        provider,
+                        "/equity/profile",
+                        ("fmp", "intrinio", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {
                         "fmp": {"multiple_items_allowed": True},
                         "intrinio": {"multiple_items_allowed": True},
                         "yfinance": {"multiple_items_allowed": True},
                     }
@@ -483,15 +487,15 @@
             Filter by dividend amount greater than this value. (provider: fmp)
         dividend_max : Optional[float]
             Filter by dividend amount less than this value. (provider: fmp)
         is_etf : Optional[bool]
             If true, returns only ETFs. (provider: fmp)
         is_active : Optional[bool]
             If false, returns only inactive tickers. (provider: fmp)
-        sector : Optional[Literal['Consumer Cyclical', 'Energy', 'Technology', 'Industrials', 'Financial Services', 'Basic Materials', 'Communication Services', 'Consumer Defensive', 'Healthcare', 'Real Estate', 'Utilities', 'Industrial Goods', 'Financial', 'Services', 'Conglomerates']]
+        sector : Optional[Literal['consumer_cyclical', 'energy', 'technology', 'industrials', 'financial_services', 'basic_materials', 'communication_services', 'consumer_defensive', 'healthcare', 'real_estate', 'utilities', 'industrial_goods', 'financial', 'services', 'conglomerates']]
             Filter by sector. (provider: fmp)
         industry : Optional[str]
             Filter by industry. (provider: fmp)
         country : Optional[str]
             Filter by country, as a two-letter country code. (provider: fmp)
         exchange : Optional[Literal['amex', 'ams', 'ase', 'asx', 'ath', 'bme', 'bru', 'bud', 'bue', 'cai', 'cnq', 'cph', 'dfm', 'doh', 'etf', 'euronext', 'hel', 'hkse', 'ice', 'iob', 'ist', 'jkt', 'jnb', 'jpx', 'kls', 'koe', 'ksc', 'kuw', 'lse', 'mex', 'mutual_fund', 'nasdaq', 'neo', 'nse', 'nyse', 'nze', 'osl', 'otc', 'pnk', 'pra', 'ris', 'sao', 'sau', 'set', 'sgo', 'shh', 'shz', 'six', 'sto', 'tai', 'tlv', 'tsx', 'two', 'vie', 'wse', 'xetra']]
             Filter by exchange. (provider: fmp)
@@ -550,15 +554,17 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/screener",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/screener", ("fmp",),
+                        provider,
+                        "/equity/screener",
+                        ("fmp",),
                     )
                 },
                 standard_params={},
                 extra_params=kwargs,
             )
         )
 
@@ -637,15 +643,17 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/search",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/search", ("intrinio", "sec"),
+                        provider,
+                        "/equity/search",
+                        ("intrinio", "sec"),
                     )
                 },
                 standard_params={
                     "query": query,
                     "is_symbol": is_symbol,
                     "use_cache": use_cache,
                 },
```

### Comparing `openbb-4.2.0/openbb/package/equity_calendar.py` & `openbb-4.2.1/openbb/package/equity_calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,18 +97,23 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/calendar/dividend",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/calendar/dividend", ("fmp",),
+                        provider,
+                        "/equity/calendar/dividend",
+                        ("fmp",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def earnings(
@@ -190,18 +195,23 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/calendar/earnings",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/calendar/earnings", ("fmp",),
+                        provider,
+                        "/equity/calendar/earnings",
+                        ("fmp",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def ipo(
@@ -322,15 +332,17 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/calendar/ipo",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/calendar/ipo", ("intrinio",),
+                        provider,
+                        "/equity/calendar/ipo",
+                        ("intrinio",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "start_date": start_date,
                     "end_date": end_date,
                     "limit": limit,
@@ -408,14 +420,19 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/calendar/splits",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/calendar/splits", ("fmp",),
+                        provider,
+                        "/equity/calendar/splits",
+                        ("fmp",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/equity_compare.py` & `openbb-4.2.1/openbb/package/equity_shorts.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,80 +6,101 @@
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
 from typing_extensions import Annotated
 
 
-class ROUTER_equity_compare(Container):
-    """/equity/compare
-    peers
+class ROUTER_equity_shorts(Container):
+    """/equity/shorts
+    fails_to_deliver
     """
 
     def __repr__(self) -> str:
         return self.__doc__ or ""
 
     @exception_handler
     @validate
-    def peers(
+    def fails_to_deliver(
         self,
         symbol: Annotated[str, OpenBBField(description="Symbol to get data for.")],
         provider: Annotated[
-            Optional[Literal["fmp"]],
+            Optional[Literal["sec"]],
             OpenBBField(
-                description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
+                description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'sec' if there is\n    no default."
             ),
         ] = None,
         **kwargs
     ) -> OBBject:
-        """Get the closest peers for a given company.
-
-        Peers consist of companies trading on the same exchange, operating within the same sector
-        and with comparable market capitalizations.
-
+        """Get reported Fail-to-deliver (FTD) data.
 
         Parameters
         ----------
         symbol : str
             Symbol to get data for.
-        provider : Optional[Literal['fmp']]
+        provider : Optional[Literal['sec']]
             The provider to use for the query, by default None.
-            If None, the provider specified in defaults is selected or 'fmp' if there is
+            If None, the provider specified in defaults is selected or 'sec' if there is
             no default.
+        limit : Optional[int]
+
+                Limit the number of reports to parse, from most recent.
+                Approximately 24 reports per year, going back to 2009.
+                 (provider: sec)
+        skip_reports : Optional[int]
+
+                Skip N number of reports from current. A value of 1 will skip the most recent report.
+                 (provider: sec)
+        use_cache : Optional[bool]
+            Whether or not to use cache for the request, default is True. Each reporting period is a separate URL, new reports will be added to the cache. (provider: sec)
 
         Returns
         -------
         OBBject
-            results : EquityPeers
+            results : List[EquityFTD]
                 Serializable results.
-            provider : Optional[Literal['fmp']]
+            provider : Optional[Literal['sec']]
                 Provider name.
             warnings : Optional[List[Warning_]]
                 List of warnings.
             chart : Optional[Chart]
                 Chart object.
             extra : Dict[str, Any]
                 Extra info.
 
-        EquityPeers
-        -----------
-        peers_list : List[str]
-            A list of equity peers based on sector, exchange and market cap.
+        EquityFTD
+        ---------
+        settlement_date : Optional[date]
+            The settlement date of the fail.
+        symbol : Optional[str]
+            Symbol representing the entity requested in the data.
+        cusip : Optional[str]
+            CUSIP of the Security.
+        quantity : Optional[int]
+            The number of fails on that settlement date.
+        price : Optional[float]
+            The price at the previous closing price from the settlement date.
+        description : Optional[str]
+            The description of the Security.
 
         Examples
         --------
         >>> from openbb import obb
-        >>> obb.equity.compare.peers(symbol='AAPL', provider='fmp')
+        >>> obb.equity.shorts.fails_to_deliver(symbol='AAPL', provider='sec')
         """  # noqa: E501
 
         return self._run(
-            "/equity/compare/peers",
+            "/equity/shorts/fails_to_deliver",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/compare/peers", ("fmp",),
+                        provider,
+                        "/equity/shorts/fails_to_deliver",
+                        ("sec",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/equity_discovery.py` & `openbb-4.2.1/openbb/package/equity_discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,18 +98,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/discovery/active",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/discovery/active", ("yfinance",),
+                        provider,
+                        "/equity/discovery/active",
+                        ("yfinance",),
                     )
                 },
-                standard_params={"sort": sort,},
+                standard_params={
+                    "sort": sort,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def aggressive_small_caps(
@@ -187,15 +191,17 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/discovery/aggressive_small_caps",
                         ("yfinance",),
                     )
                 },
-                standard_params={"sort": sort,},
+                standard_params={
+                    "sort": sort,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def filings(
@@ -288,15 +294,17 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/discovery/filings",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/discovery/filings", ("fmp",),
+                        provider,
+                        "/equity/discovery/filings",
+                        ("fmp",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "form_type": form_type,
                     "limit": limit,
@@ -377,18 +385,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/discovery/gainers",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/discovery/gainers", ("yfinance",),
+                        provider,
+                        "/equity/discovery/gainers",
+                        ("yfinance",),
                     )
                 },
-                standard_params={"sort": sort,},
+                standard_params={
+                    "sort": sort,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def growth_tech(
@@ -461,18 +473,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/discovery/growth_tech",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/discovery/growth_tech", ("yfinance",),
+                        provider,
+                        "/equity/discovery/growth_tech",
+                        ("yfinance",),
                     )
                 },
-                standard_params={"sort": sort,},
+                standard_params={
+                    "sort": sort,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def losers(
@@ -545,18 +561,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/discovery/losers",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/discovery/losers", ("yfinance",),
+                        provider,
+                        "/equity/discovery/losers",
+                        ("yfinance",),
                     )
                 },
-                standard_params={"sort": sort,},
+                standard_params={
+                    "sort": sort,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def undervalued_growth(
@@ -629,18 +649,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/discovery/undervalued_growth",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/discovery/undervalued_growth", ("yfinance",),
+                        provider,
+                        "/equity/discovery/undervalued_growth",
+                        ("yfinance",),
                     )
                 },
-                standard_params={"sort": sort,},
+                standard_params={
+                    "sort": sort,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def undervalued_large_caps(
@@ -718,11 +742,13 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/discovery/undervalued_large_caps",
                         ("yfinance",),
                     )
                 },
-                standard_params={"sort": sort,},
+                standard_params={
+                    "sort": sort,
+                },
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/equity_estimates.py` & `openbb-4.2.1/openbb/package/equity_estimates.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from typing_extensions import Annotated
 
 
 class ROUTER_equity_estimates(Container):
     """/equity/estimates
     analyst_search
     consensus
+    forward_ebitda
     forward_eps
     forward_pe
     forward_sales
     historical
     price_target
     """
 
@@ -208,18 +209,23 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/estimates/analyst_search",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/estimates/analyst_search", ("benzinga",),
+                        provider,
+                        "/equity/estimates/analyst_search",
+                        ("benzinga",),
                     )
                 },
-                standard_params={"analyst_name": analyst_name, "firm_name": firm_name,},
+                standard_params={
+                    "analyst_name": analyst_name,
+                    "firm_name": firm_name,
+                },
                 extra_params=kwargs,
                 info={
                     "analyst_name": {"benzinga": {"multiple_items_allowed": True}},
                     "firm_name": {"benzinga": {"multiple_items_allowed": True}},
                     "analyst_ids": {"benzinga": {"multiple_items_allowed": True}},
                     "firm_ids": {"benzinga": {"multiple_items_allowed": True}},
                     "fields": {"benzinga": {"multiple_items_allowed": True}},
@@ -322,28 +328,146 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/estimates/consensus",
                         ("fmp", "intrinio", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {
                         "fmp": {"multiple_items_allowed": True},
                         "intrinio": {"multiple_items_allowed": True},
                         "yfinance": {"multiple_items_allowed": True},
                     }
                 },
             )
         )
 
     @exception_handler
     @validate
+    def forward_ebitda(
+        self,
+        symbol: Annotated[
+            Union[str, None, List[Optional[str]]],
+            OpenBBField(
+                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio."
+            ),
+        ] = None,
+        provider: Annotated[
+            Optional[Literal["fmp", "intrinio"]],
+            OpenBBField(
+                description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
+            ),
+        ] = None,
+        **kwargs
+    ) -> OBBject:
+        """Get forward EBITDA estimates.
+
+        Parameters
+        ----------
+        symbol : Union[str, None, List[Optional[str]]]
+            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio.
+        provider : Optional[Literal['fmp', 'intrinio']]
+            The provider to use for the query, by default None.
+            If None, the provider specified in defaults is selected or 'fmp' if there is
+            no default.
+        fiscal_period : Optional[Literal['annual', 'quarter']]
+            The future fiscal period to retrieve estimates for. (provider: fmp);
+            Filter for only full-year or quarterly estimates. (provider: intrinio)
+        limit : Optional[int]
+            The number of data entries to return. (provider: fmp)
+        include_historical : bool
+            If True, the data will include all past data and the limit will be ignored. (provider: fmp)
+        estimate_type : Optional[Literal['ebitda', 'ebit', 'enterprise_value', 'cash_flow_per_share', 'pretax_income']]
+            Limit the EBITDA estimates to this type. (provider: intrinio)
+
+        Returns
+        -------
+        OBBject
+            results : List[ForwardEbitdaEstimates]
+                Serializable results.
+            provider : Optional[Literal['fmp', 'intrinio']]
+                Provider name.
+            warnings : Optional[List[Warning_]]
+                List of warnings.
+            chart : Optional[Chart]
+                Chart object.
+            extra : Dict[str, Any]
+                Extra info.
+
+        ForwardEbitdaEstimates
+        ----------------------
+        symbol : str
+            Symbol representing the entity requested in the data.
+        name : Optional[str]
+            Name of the entity.
+        last_updated : Optional[date]
+            The date of the last update.
+        period_ending : Optional[date]
+            The end date of the reporting period.
+        fiscal_year : Optional[int]
+            Fiscal year for the estimate.
+        fiscal_period : Optional[str]
+            Fiscal quarter for the estimate.
+        calendar_year : Optional[int]
+            Calendar year for the estimate.
+        calendar_period : Optional[Union[int, str]]
+            Calendar quarter for the estimate.
+        low_estimate : Optional[int]
+            The EBITDA estimate low for the period.
+        high_estimate : Optional[int]
+            The EBITDA estimate high for the period.
+        mean : Optional[int]
+            The EBITDA estimate mean for the period.
+        median : Optional[int]
+            The EBITDA estimate median for the period.
+        standard_deviation : Optional[int]
+            The EBITDA estimate standard deviation for the period.
+        number_of_analysts : Optional[int]
+            Number of analysts providing estimates for the period.
+        conensus_type : Optional[Literal['ebitda', 'ebit', 'enterprise_value', 'cash_flow_per_share', 'pretax_income']]
+            The type of estimate. (provider: intrinio)
+
+        Examples
+        --------
+        >>> from openbb import obb
+        >>> obb.equity.estimates.forward_ebitda(provider='intrinio')
+        >>> obb.equity.estimates.forward_ebitda(symbol='AAPL', fiscal_period='annual', provider='intrinio')
+        >>> obb.equity.estimates.forward_ebitda(symbol='AAPL,MSFT', fiscal_period='quarter', provider='fmp')
+        """  # noqa: E501
+
+        return self._run(
+            "/equity/estimates/forward_ebitda",
+            **filter_inputs(
+                provider_choices={
+                    "provider": self._get_provider(
+                        provider,
+                        "/equity/estimates/forward_ebitda",
+                        ("fmp", "intrinio"),
+                    )
+                },
+                standard_params={
+                    "symbol": symbol,
+                },
+                extra_params=kwargs,
+                info={
+                    "symbol": {
+                        "fmp": {"multiple_items_allowed": True},
+                        "intrinio": {"multiple_items_allowed": True},
+                    }
+                },
+            )
+        )
+
+    @exception_handler
+    @validate
     def forward_eps(
         self,
         symbol: Annotated[
             Union[str, None, List[Optional[str]]],
             OpenBBField(
                 description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp, intrinio."
             ),
@@ -440,18 +564,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/estimates/forward_eps",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/estimates/forward_eps", ("fmp", "intrinio"),
+                        provider,
+                        "/equity/estimates/forward_eps",
+                        ("fmp", "intrinio"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {
                         "fmp": {"multiple_items_allowed": True},
                         "intrinio": {"multiple_items_allowed": True},
                     }
                 },
@@ -517,33 +645,37 @@
             Estimated PE ratio four fiscal years from now.
         year5 : Optional[float]
             Estimated PE ratio five fiscal years from now.
         peg_ratio_year1 : Optional[float]
             Estimated Forward PEG ratio for the next fiscal year. (provider: intrinio)
         eps_ttm : Optional[float]
             The latest trailing twelve months earnings per share. (provider: intrinio)
-        last_udpated : Optional[date]
+        last_updated : Optional[date]
             The date the data was last updated. (provider: intrinio)
 
         Examples
         --------
         >>> from openbb import obb
         >>> obb.equity.estimates.forward_pe(provider='intrinio')
         >>> obb.equity.estimates.forward_pe(symbol='AAPL,MSFT,GOOG', provider='intrinio')
         """  # noqa: E501
 
         return self._run(
             "/equity/estimates/forward_pe",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/estimates/forward_pe", ("intrinio",),
+                        provider,
+                        "/equity/estimates/forward_pe",
+                        ("intrinio",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"intrinio": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -651,18 +783,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/estimates/forward_sales",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/estimates/forward_sales", ("intrinio",),
+                        provider,
+                        "/equity/estimates/forward_sales",
+                        ("intrinio",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"intrinio": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -765,18 +901,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/estimates/historical",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/estimates/historical", ("fmp",),
+                        provider,
+                        "/equity/estimates/historical",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -822,19 +962,19 @@
         updated : Optional[Union[datetime.date, int]]
             Records last Updated Unix timestamp (UTC). This will force the sort order to be Greater Than or Equal to the timestamp indicated. The date can be a date string or a Unix timestamp. The date string must be in the format of YYYY-MM-DD. (provider: benzinga)
         importance : Optional[int]
             Importance level to filter by. Uses Greater Than or Equal To the importance indicated (provider: benzinga)
         action : Optional[Literal['downgrades', 'maintains', 'reinstates', 'reiterates', 'upgrades', 'assumes', 'initiates', 'terminates', 'removes', 'suspends', 'firm_dissolved']]
             Filter by a specific action_company. (provider: benzinga)
         analyst_ids : Optional[Union[List[str], str]]
-            Comma-separated list of analyst (person) IDs. Omitting will bring back all available analysts. (provider: benzinga)
+            Comma-separated list of analyst (person) IDs. Omitting will bring back all available analysts. Multiple comma separated items allowed. (provider: benzinga)
         firm_ids : Optional[Union[List[str], str]]
-            Comma-separated list of firm IDs. (provider: benzinga)
+            Comma-separated list of firm IDs. Multiple comma separated items allowed. (provider: benzinga)
         fields : Optional[Union[List[str], str]]
-            Comma-separated list of fields to include in the response. See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields. (provider: benzinga)
+            Comma-separated list of fields to include in the response. See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields. Multiple comma separated items allowed. (provider: benzinga)
         with_grade : bool
             Include upgrades and downgrades in the response. (provider: fmp)
 
         Returns
         -------
         OBBject
             results : List[PriceTarget]
@@ -916,20 +1056,28 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/estimates/price_target",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/estimates/price_target", ("benzinga", "fmp"),
+                        provider,
+                        "/equity/estimates/price_target",
+                        ("benzinga", "fmp"),
                     )
                 },
-                standard_params={"symbol": symbol, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {
-                        "benzinga": {"multiple_items_allowed": True},
+                        "benzinga": ["multiple_items_allowed"],
                         "fmp": {"multiple_items_allowed": True},
-                    }
+                    },
+                    "analyst_ids": {"benzinga": ["multiple_items_allowed"]},
+                    "firm_ids": {"benzinga": ["multiple_items_allowed"]},
+                    "fields": {"benzinga": ["multiple_items_allowed"]},
                 },
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/equity_fundamental.py` & `openbb-4.2.1/openbb/package/equity_fundamental.py`

 * *Files 2% similar despite different names*

```diff
@@ -393,15 +393,19 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/fundamental/balance",
                         ("fmp", "intrinio", "polygon", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol, "period": period, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "period": period,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def balance_growth(
@@ -540,18 +544,23 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/balance_growth",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/balance_growth", ("fmp",),
+                        provider,
+                        "/equity/fundamental/balance_growth",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def cash(
@@ -807,15 +816,19 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/fundamental/cash",
                         ("fmp", "intrinio", "polygon", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol, "period": period, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "period": period,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def cash_growth(
@@ -936,18 +949,23 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/cash_growth",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/cash_growth", ("fmp",),
+                        provider,
+                        "/equity/fundamental/cash_growth",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def dividends(
@@ -1114,18 +1132,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/employee_count",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/employee_count", ("fmp",),
+                        provider,
+                        "/equity/fundamental/employee_count",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def filings(
@@ -1475,18 +1497,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/historical_eps",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/historical_eps", ("fmp",),
+                        provider,
+                        "/equity/fundamental/historical_eps",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def historical_splits(
@@ -1543,18 +1569,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/historical_splits",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/historical_splits", ("fmp",),
+                        provider,
+                        "/equity/fundamental/historical_splits",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def income(
@@ -1904,15 +1934,19 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/fundamental/income",
                         ("fmp", "intrinio", "polygon", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol, "period": period, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "period": period,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def income_growth(
@@ -2031,18 +2065,24 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/income_growth",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/income_growth", ("fmp",),
+                        provider,
+                        "/equity/fundamental/income_growth",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol, "limit": limit, "period": period,},
+                standard_params={
+                    "symbol": symbol,
+                    "limit": limit,
+                    "period": period,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def latest_attributes(
@@ -2115,15 +2155,18 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/fundamental/latest_attributes",
                         ("intrinio",),
                     )
                 },
-                standard_params={"symbol": symbol, "tag": tag,},
+                standard_params={
+                    "symbol": symbol,
+                    "tag": tag,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {"intrinio": {"multiple_items_allowed": True}},
                     "tag": {"intrinio": {"multiple_items_allowed": True}},
                 },
             )
         )
@@ -2194,18 +2237,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/management",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/management", ("fmp", "yfinance"),
+                        provider,
+                        "/equity/fundamental/management",
+                        ("fmp", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def management_compensation(
@@ -2296,15 +2343,17 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/fundamental/management_compensation",
                         ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -2367,22 +2416,24 @@
         ----------
         symbol : Optional[str]
             Symbol representing the entity requested in the data.
         market_cap : Optional[float]
             Market capitalization
         pe_ratio : Optional[float]
             Price-to-earnings ratio (P/E ratio)
-        date : Optional[date]
-            The date of the data. (provider: fmp)
-        period : Optional[str]
+        period_ending : Optional[date]
+            Period ending date. (provider: fmp)
+        fiscal_period : Optional[str]
             Period of the data. (provider: fmp)
         calendar_year : Optional[int]
-            Calendar year. (provider: fmp)
+            Calendar year for the fiscal period. (provider: fmp)
         revenue_per_share : Optional[float]
             Revenue per share (provider: fmp, yfinance)
+        capex_per_share : Optional[float]
+            Capital expenditures per share (provider: fmp)
         net_income_per_share : Optional[float]
             Net income per share (provider: fmp)
         operating_cash_flow_per_share : Optional[float]
             Operating cash flow per share (provider: fmp)
         free_cash_flow_per_share : Optional[float]
             Free cash flow per share (provider: fmp)
         cash_per_share : Optional[float]
@@ -2391,53 +2442,51 @@
             Book value per share (provider: fmp)
         tangible_book_value_per_share : Optional[float]
             Tangible book value per share (provider: fmp)
         shareholders_equity_per_share : Optional[float]
             Shareholders equity per share (provider: fmp)
         interest_debt_per_share : Optional[float]
             Interest debt per share (provider: fmp)
-        enterprise_value : Optional[int]
-            Enterprise value (provider: fmp, intrinio, yfinance)
-        price_to_sales_ratio : Optional[float]
+        price_to_sales : Optional[float]
             Price-to-sales ratio (provider: fmp)
-        pocf_ratio : Optional[float]
+        price_to_operating_cash_flow : Optional[float]
             Price-to-operating cash flow ratio (provider: fmp)
-        pfcf_ratio : Optional[float]
+        price_to_free_cash_flow : Optional[float]
             Price-to-free cash flow ratio (provider: fmp)
-        pb_ratio : Optional[float]
-            Price-to-book ratio (provider: fmp)
-        ptb_ratio : Optional[float]
-            Price-to-tangible book ratio (provider: fmp)
+        price_to_book : Optional[float]
+            Price-to-book ratio (provider: fmp, intrinio, yfinance)
+        price_to_tangible_book : Optional[float]
+            Price-to-tangible book ratio (provider: fmp, intrinio)
         ev_to_sales : Optional[float]
             Enterprise value-to-sales ratio (provider: fmp)
-        enterprise_value_over_ebitda : Optional[float]
+        ev_to_ebitda : Optional[float]
             Enterprise value-to-EBITDA ratio (provider: fmp)
         ev_to_operating_cash_flow : Optional[float]
             Enterprise value-to-operating cash flow ratio (provider: fmp)
         ev_to_free_cash_flow : Optional[float]
             Enterprise value-to-free cash flow ratio (provider: fmp)
         earnings_yield : Optional[float]
             Earnings yield (provider: fmp);
             Earnings yield, as a normalized percent. (provider: intrinio)
         free_cash_flow_yield : Optional[float]
             Free cash flow yield (provider: fmp)
+        debt_to_market_cap : Optional[float]
+            Debt-to-market capitalization ratio (provider: fmp)
         debt_to_equity : Optional[float]
             Debt-to-equity ratio (provider: fmp, yfinance)
         debt_to_assets : Optional[float]
             Debt-to-assets ratio (provider: fmp)
         net_debt_to_ebitda : Optional[float]
             Net debt-to-EBITDA ratio (provider: fmp)
         current_ratio : Optional[float]
             Current ratio (provider: fmp, yfinance)
         interest_coverage : Optional[float]
             Interest coverage (provider: fmp)
         income_quality : Optional[float]
             Income quality (provider: fmp)
-        dividend_yield : Optional[float]
-            Dividend yield, as a normalized percent. (provider: fmp, intrinio, yfinance)
         payout_ratio : Optional[float]
             Payout ratio (provider: fmp, yfinance)
         sales_general_and_administrative_to_revenue : Optional[float]
             Sales general and administrative expenses-to-revenue ratio (provider: fmp)
         research_and_development_to_revenue : Optional[float]
             Research and development expenses-to-revenue ratio (provider: fmp)
         intangibles_to_total_assets : Optional[float]
@@ -2446,28 +2495,22 @@
             Capital expenditures-to-operating cash flow ratio (provider: fmp)
         capex_to_revenue : Optional[float]
             Capital expenditures-to-revenue ratio (provider: fmp)
         capex_to_depreciation : Optional[float]
             Capital expenditures-to-depreciation ratio (provider: fmp)
         stock_based_compensation_to_revenue : Optional[float]
             Stock-based compensation-to-revenue ratio (provider: fmp)
-        graham_number : Optional[float]
-            Graham number (provider: fmp)
-        roic : Optional[float]
-            Return on invested capital (provider: fmp)
-        return_on_tangible_assets : Optional[float]
-            Return on tangible assets (provider: fmp)
-        graham_net_net : Optional[float]
-            Graham net-net working capital (provider: fmp)
         working_capital : Optional[float]
             Working capital (provider: fmp)
         tangible_asset_value : Optional[float]
             Tangible asset value (provider: fmp)
         net_current_asset_value : Optional[float]
             Net current asset value (provider: fmp)
+        enterprise_value : Optional[int]
+            Enterprise value (provider: fmp, intrinio, yfinance)
         invested_capital : Optional[float]
             Invested capital (provider: fmp)
         average_receivables : Optional[float]
             Average receivables (provider: fmp)
         average_payables : Optional[float]
             Average payables (provider: fmp)
         average_inventory : Optional[float]
@@ -2480,22 +2523,29 @@
             Days of inventory on hand (provider: fmp)
         receivables_turnover : Optional[float]
             Receivables turnover (provider: fmp)
         payables_turnover : Optional[float]
             Payables turnover (provider: fmp)
         inventory_turnover : Optional[float]
             Inventory turnover (provider: fmp)
-        roe : Optional[float]
-            Return on equity (provider: fmp)
-        capex_per_share : Optional[float]
-            Capital expenditures per share (provider: fmp)
-        price_to_book : Optional[float]
-            Price to book ratio. (provider: intrinio, yfinance)
-        price_to_tangible_book : Optional[float]
-            Price to tangible book ratio. (provider: intrinio)
+        return_on_equity : Optional[float]
+            Return on equity (provider: fmp);
+            Return on equity, as a normalized percent. (provider: intrinio);
+            Return on equity, as a normalized percent. (provider: yfinance)
+        return_on_invested_capital : Optional[float]
+            Return on invested capital (provider: fmp);
+            Return on invested capital, as a normalized percent. (provider: intrinio)
+        return_on_tangible_assets : Optional[float]
+            Return on tangible assets (provider: fmp)
+        dividend_yield : Optional[float]
+            Dividend yield, as a normalized percent. (provider: fmp, intrinio, yfinance)
+        graham_number : Optional[float]
+            Graham number (provider: fmp)
+        graham_net_net : Optional[float]
+            Graham net-net working capital (provider: fmp)
         price_to_revenue : Optional[float]
             Price to revenue ratio. (provider: intrinio)
         quick_ratio : Optional[float]
             Quick ratio. (provider: intrinio, yfinance)
         gross_margin : Optional[float]
             Gross margin, as a normalized percent. (provider: intrinio, yfinance)
         ebit_margin : Optional[float]
@@ -2516,18 +2566,14 @@
             Net income growth, as a normalized percent. (provider: intrinio)
         free_cash_flow_to_firm_growth : Optional[float]
             Free cash flow to firm growth, as a normalized percent. (provider: intrinio)
         invested_capital_growth : Optional[float]
             Invested capital growth, as a normalized percent. (provider: intrinio)
         return_on_assets : Optional[float]
             Return on assets, as a normalized percent. (provider: intrinio, yfinance)
-        return_on_equity : Optional[float]
-            Return on equity, as a normalized percent. (provider: intrinio, yfinance)
-        return_on_invested_capital : Optional[float]
-            Return on invested capital, as a normalized percent. (provider: intrinio)
         ebitda : Optional[int]
             Earnings before interest, taxes, depreciation, and amortization. (provider: intrinio)
         ebit : Optional[int]
             Earnings before interest and taxes. (provider: intrinio)
         long_term_debt : Optional[int]
             Long-term debt. (provider: intrinio)
         total_debt : Optional[int]
@@ -2609,15 +2655,19 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/fundamental/metrics",
                         ("fmp", "intrinio", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol, "period": period, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "period": period,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {
                         "fmp": {"multiple_items_allowed": True},
                         "intrinio": {"multiple_items_allowed": True},
                         "yfinance": {"multiple_items_allowed": True},
                     }
@@ -2800,18 +2850,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/multiples",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/multiples", ("fmp",),
+                        provider,
+                        "/equity/fundamental/multiples",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -2944,18 +2998,22 @@
         )
 
         return self._run(
             "/equity/fundamental/overview",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/overview", ("fmp",),
+                        provider,
+                        "/equity/fundamental/overview",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def ratios(
@@ -3135,18 +3193,24 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/ratios",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/ratios", ("fmp", "intrinio"),
+                        provider,
+                        "/equity/fundamental/ratios",
+                        ("fmp", "intrinio"),
                     )
                 },
-                standard_params={"symbol": symbol, "period": period, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "period": period,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def reported_financials(
@@ -3320,15 +3384,17 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/revenue_per_geography",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/revenue_per_geography", ("fmp",),
+                        provider,
+                        "/equity/fundamental/revenue_per_geography",
+                        ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "period": period,
                     "structure": structure,
                 },
@@ -3407,15 +3473,17 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/revenue_per_segment",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/revenue_per_segment", ("fmp",),
+                        provider,
+                        "/equity/fundamental/revenue_per_segment",
+                        ("fmp",),
                     )
                 },
                 standard_params={
                     "symbol": symbol,
                     "period": period,
                     "structure": structure,
                 },
@@ -3504,15 +3572,18 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/fundamental/search_attributes",
                         ("intrinio",),
                     )
                 },
-                standard_params={"query": query, "limit": limit,},
+                standard_params={
+                    "query": query,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def trailing_dividend_yield(
@@ -3579,15 +3650,18 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/fundamental/trailing_dividend_yield",
                         ("tiingo",),
                     )
                 },
-                standard_params={"symbol": symbol, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def transcript(
@@ -3651,14 +3725,19 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/fundamental/transcript",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/fundamental/transcript", ("fmp",),
+                        provider,
+                        "/equity/fundamental/transcript",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol, "year": year,},
+                standard_params={
+                    "symbol": symbol,
+                    "year": year,
+                },
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/equity_ownership.py` & `openbb-4.2.1/openbb/package/equity_ownership.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,18 +130,24 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/ownership/form_13f",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/ownership/form_13f", ("sec",),
+                        provider,
+                        "/equity/ownership/form_13f",
+                        ("sec",),
                     )
                 },
-                standard_params={"symbol": symbol, "date": date, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "date": date,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def insider_trading(
@@ -166,15 +172,15 @@
             Symbol to get data for.
         limit : int
             The number of data entries to return.
         provider : Optional[Literal['fmp', 'intrinio']]
             The provider to use for the query, by default None.
             If None, the provider specified in defaults is selected or 'fmp' if there is
             no default.
-        transaction_type : Literal[None, 'award', 'conversion', 'return', 'expire_short', 'in_kind', 'gift', 'expire_long', 'discretionary', 'other', 'small', 'exempt', 'otm', 'purchase', 'sale', 'tender', 'will', 'itm', 'trust']
+        transaction_type : Optional[Literal['award', 'conversion', 'return', 'expire_short', 'in_kind', 'gift', 'expire_long', 'discretionary', 'other', 'small', 'exempt', 'otm', 'purchase', 'sale', 'tender', 'will', 'itm', 'trust']]
             Type of the transaction. (provider: fmp)
         start_date : Optional[datetime.date]
             Start date of the data, in YYYY-MM-DD format. (provider: intrinio)
         end_date : Optional[datetime.date]
             End date of the data, in YYYY-MM-DD format. (provider: intrinio)
         ownership_type : Optional[Literal['D', 'I']]
             Type of ownership. (provider: intrinio)
@@ -269,15 +275,18 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/ownership/insider_trading",
                         ("fmp", "intrinio"),
                     )
                 },
-                standard_params={"symbol": symbol, "limit": limit,},
+                standard_params={
+                    "symbol": symbol,
+                    "limit": limit,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def institutional(
@@ -402,18 +411,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/ownership/institutional",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/ownership/institutional", ("fmp",),
+                        provider,
+                        "/equity/ownership/institutional",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def major_holders(
@@ -552,18 +565,24 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/ownership/major_holders",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/ownership/major_holders", ("fmp",),
+                        provider,
+                        "/equity/ownership/major_holders",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol, "date": date, "page": page,},
+                standard_params={
+                    "symbol": symbol,
+                    "date": date,
+                    "page": page,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def share_statistics(
@@ -658,12 +677,14 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/ownership/share_statistics",
                         ("fmp", "intrinio", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"yfinance": {"multiple_items_allowed": True}}},
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/equity_price.py` & `openbb-4.2.1/openbb/package/equity_price.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,18 +287,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/price/nbbo",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/price/nbbo", ("polygon",),
+                        provider,
+                        "/equity/price/nbbo",
+                        ("polygon",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def performance(
@@ -386,18 +390,22 @@
         """  # noqa: E501
 
         return self._run(
             "/equity/price/performance",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/equity/price/performance", ("fmp",),
+                        provider,
+                        "/equity/price/performance",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -559,15 +567,17 @@
                 provider_choices={
                     "provider": self._get_provider(
                         provider,
                         "/equity/price/quote",
                         ("fmp", "intrinio", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {
                         "fmp": {"multiple_items_allowed": True},
                         "intrinio": {"multiple_items_allowed": True},
                         "yfinance": {"multiple_items_allowed": True},
                     }
```

### Comparing `openbb-4.2.0/openbb/package/etf.py` & `openbb-4.2.1/openbb/package/etf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 ### THIS FILE IS AUTO-GENERATED. DO NOT EDIT. ###
 
 import datetime
 from typing import List, Literal, Optional, Union
-from warnings import simplefilter, warn
 
-from openbb_core.app.deprecation import OpenBBDeprecationWarning
 from openbb_core.app.model.field import OpenBBField
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.static.container import Container
 from openbb_core.app.static.utils.decorators import exception_handler, validate
 from openbb_core.app.static.utils.filters import filter_inputs
-from typing_extensions import Annotated, deprecated
+from typing_extensions import Annotated
 
 
 class ROUTER_etf(Container):
     """/etf
     countries
     equity_exposure
     historical
     holdings
     holdings_date
-    holdings_performance
     info
     price_performance
     search
     sectors
     """
 
     def __repr__(self) -> str:
@@ -85,18 +82,22 @@
         """  # noqa: E501
 
         return self._run(
             "/etf/countries",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/etf/countries", ("fmp",),
+                        provider,
+                        "/etf/countries",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -163,18 +164,22 @@
         """  # noqa: E501
 
         return self._run(
             "/etf/equity_exposure",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/etf/equity_exposure", ("fmp",),
+                        provider,
+                        "/etf/equity_exposure",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
@@ -598,18 +603,22 @@
         """  # noqa: E501
 
         return self._run(
             "/etf/holdings",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/etf/holdings", ("fmp", "intrinio", "sec"),
+                        provider,
+                        "/etf/holdings",
+                        ("fmp", "intrinio", "sec"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def holdings_date(
@@ -664,130 +673,23 @@
         """  # noqa: E501
 
         return self._run(
             "/etf/holdings_date",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/etf/holdings_date", ("fmp",),
+                        provider,
+                        "/etf/holdings_date",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
-                extra_params=kwargs,
-            )
-        )
-
-    @exception_handler
-    @validate
-    @deprecated(
-        "This endpoint is deprecated; pass a list of holdings symbols directly to `/equity/price/performance` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.2.",
-        category=OpenBBDeprecationWarning,
-    )
-    def holdings_performance(
-        self,
-        symbol: Annotated[
-            Union[str, List[str]],
-            OpenBBField(
-                description="Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp."
-            ),
-        ],
-        provider: Annotated[
-            Optional[Literal["fmp"]],
-            OpenBBField(
-                description="The provider to use for the query, by default None.\n    If None, the provider specified in defaults is selected or 'fmp' if there is\n    no default."
-            ),
-        ] = None,
-        **kwargs
-    ) -> OBBject:
-        """Get the recent price performance of each ticker held in the ETF.
-
-        Parameters
-        ----------
-        symbol : Union[str, List[str]]
-            Symbol to get data for. Multiple comma separated items allowed for provider(s): fmp.
-        provider : Optional[Literal['fmp']]
-            The provider to use for the query, by default None.
-            If None, the provider specified in defaults is selected or 'fmp' if there is
-            no default.
-
-        Returns
-        -------
-        OBBject
-            results : List[EtfHoldingsPerformance]
-                Serializable results.
-            provider : Optional[Literal['fmp']]
-                Provider name.
-            warnings : Optional[List[Warning_]]
-                List of warnings.
-            chart : Optional[Chart]
-                Chart object.
-            extra : Dict[str, Any]
-                Extra info.
-
-        EtfHoldingsPerformance
-        ----------------------
-        symbol : Optional[str]
-            Symbol representing the entity requested in the data.
-        one_day : Optional[float]
-            One-day return.
-        wtd : Optional[float]
-            Week to date return.
-        one_week : Optional[float]
-            One-week return.
-        mtd : Optional[float]
-            Month to date return.
-        one_month : Optional[float]
-            One-month return.
-        qtd : Optional[float]
-            Quarter to date return.
-        three_month : Optional[float]
-            Three-month return.
-        six_month : Optional[float]
-            Six-month return.
-        ytd : Optional[float]
-            Year to date return.
-        one_year : Optional[float]
-            One-year return.
-        two_year : Optional[float]
-            Two-year return.
-        three_year : Optional[float]
-            Three-year return.
-        four_year : Optional[float]
-            Four-year
-        five_year : Optional[float]
-            Five-year return.
-        ten_year : Optional[float]
-            Ten-year return.
-        max : Optional[float]
-            Return from the beginning of the time series.
-
-        Examples
-        --------
-        >>> from openbb import obb
-        >>> obb.etf.holdings_performance(symbol='XLK', provider='fmp')
-        """  # noqa: E501
-
-        simplefilter("always", DeprecationWarning)
-        warn(
-            "This endpoint is deprecated; pass a list of holdings symbols directly to `/equity/price/performance` instead. Deprecated in OpenBB Platform V4.1 to be removed in V4.2.",
-            category=DeprecationWarning,
-            stacklevel=2,
-        )
-
-        return self._run(
-            "/etf/holdings_performance",
-            **filter_inputs(
-                provider_choices={
-                    "provider": self._get_provider(
-                        provider, "/etf/holdings_performance", ("fmp",),
-                    )
+                standard_params={
+                    "symbol": symbol,
                 },
-                standard_params={"symbol": symbol,},
                 extra_params=kwargs,
-                info={"symbol": {"fmp": {"multiple_items_allowed": True}}},
             )
         )
 
     @exception_handler
     @validate
     def info(
         self,
@@ -1158,18 +1060,22 @@
         """  # noqa: E501
 
         return self._run(
             "/etf/info",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/etf/info", ("fmp", "intrinio", "yfinance"),
+                        provider,
+                        "/etf/info",
+                        ("fmp", "intrinio", "yfinance"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {
                         "fmp": {"multiple_items_allowed": True},
                         "intrinio": {"multiple_items_allowed": True},
                         "yfinance": {"multiple_items_allowed": True},
                     }
@@ -1299,18 +1205,22 @@
         """  # noqa: E501
 
         return self._run(
             "/etf/price_performance",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/etf/price_performance", ("fmp", "intrinio"),
+                        provider,
+                        "/etf/price_performance",
+                        ("fmp", "intrinio"),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
                 info={
                     "symbol": {
                         "fmp": {"multiple_items_allowed": True},
                         "intrinio": {"multiple_items_allowed": True},
                     }
                 },
@@ -1413,18 +1323,22 @@
         """  # noqa: E501
 
         return self._run(
             "/etf/search",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/etf/search", ("fmp", "intrinio"),
+                        provider,
+                        "/etf/search",
+                        ("fmp", "intrinio"),
                     )
                 },
-                standard_params={"query": query,},
+                standard_params={
+                    "query": query,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def sectors(
@@ -1478,13 +1392,19 @@
         >>> obb.etf.sectors(symbol='SPY', provider='fmp')
         """  # noqa: E501
 
         return self._run(
             "/etf/sectors",
             **filter_inputs(
                 provider_choices={
-                    "provider": self._get_provider(provider, "/etf/sectors", ("fmp",),)
+                    "provider": self._get_provider(
+                        provider,
+                        "/etf/sectors",
+                        ("fmp",),
+                    )
+                },
+                standard_params={
+                    "symbol": symbol,
                 },
-                standard_params={"symbol": symbol,},
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/fixedincome.py` & `openbb-4.2.1/openbb/package/fixedincome.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,18 +118,23 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/sofr",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/sofr", ("fred",),
+                        provider,
+                        "/fixedincome/sofr",
+                        ("fred",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @property
     def spreads(self):
         # pylint: disable=import-outside-toplevel
```

### Comparing `openbb-4.2.0/openbb/package/fixedincome_corporate.py` & `openbb-4.2.1/openbb/package/fixedincome_corporate.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,15 +108,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/corporate/commercial_paper",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/corporate/commercial_paper", ("fred",),
+                        provider,
+                        "/fixedincome/corporate/commercial_paper",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "maturity": maturity,
                     "category": category,
@@ -199,18 +201,23 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/corporate/hqm",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/corporate/hqm", ("fred",),
+                        provider,
+                        "/fixedincome/corporate/hqm",
+                        ("fred",),
                     )
                 },
-                standard_params={"date": date, "yield_curve": yield_curve,},
+                standard_params={
+                    "date": date,
+                    "yield_curve": yield_curve,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def ice_bofa(
@@ -294,15 +301,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/corporate/ice_bofa",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/corporate/ice_bofa", ("fred",),
+                        provider,
+                        "/fixedincome/corporate/ice_bofa",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "index_type": index_type,
                 },
@@ -385,15 +394,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/corporate/moody",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/corporate/moody", ("fred",),
+                        provider,
+                        "/fixedincome/corporate/moody",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "index_type": index_type,
                 },
@@ -486,15 +497,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/corporate/spot_rates",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/corporate/spot_rates", ("fred",),
+                        provider,
+                        "/fixedincome/corporate/spot_rates",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "maturity": maturity,
                     "category": category,
```

### Comparing `openbb-4.2.0/openbb/package/fixedincome_rate.py` & `openbb-4.2.1/openbb/package/fixedincome_rate.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,18 +95,23 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/rate/ameribor",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/rate/ameribor", ("fred",),
+                        provider,
+                        "/fixedincome/rate/ameribor",
+                        ("fred",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def dpcredit(
@@ -177,18 +182,23 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/rate/dpcredit",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/rate/dpcredit", ("fred",),
+                        provider,
+                        "/fixedincome/rate/dpcredit",
+                        ("fred",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def ecb(
@@ -265,15 +275,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/rate/ecb",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/rate/ecb", ("fred",),
+                        provider,
+                        "/fixedincome/rate/ecb",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "interest_rate_type": interest_rate_type,
                 },
@@ -350,18 +362,23 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/rate/effr",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/rate/effr", ("federal_reserve", "fred"),
+                        provider,
+                        "/fixedincome/rate/effr",
+                        ("federal_reserve", "fred"),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def effr_forecast(
@@ -432,15 +449,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/rate/effr_forecast",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/rate/effr_forecast", ("fred",),
+                        provider,
+                        "/fixedincome/rate/effr_forecast",
+                        ("fred",),
                     )
                 },
                 standard_params={},
                 extra_params=kwargs,
             )
         )
 
@@ -514,18 +533,23 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/rate/estr",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/rate/estr", ("fred",),
+                        provider,
+                        "/fixedincome/rate/estr",
+                        ("fred",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def iorb(
@@ -592,18 +616,23 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/rate/iorb",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/rate/iorb", ("fred",),
+                        provider,
+                        "/fixedincome/rate/iorb",
+                        ("fred",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     def sonia(
@@ -673,14 +702,19 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/rate/sonia",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/rate/sonia", ("fred",),
+                        provider,
+                        "/fixedincome/rate/sonia",
+                        ("fred",),
                     )
                 },
-                standard_params={"start_date": start_date, "end_date": end_date,},
+                standard_params={
+                    "start_date": start_date,
+                    "end_date": end_date,
+                },
                 extra_params=kwargs,
             )
         )
```

### Comparing `openbb-4.2.0/openbb/package/fixedincome_spreads.py` & `openbb-4.2.1/openbb/package/fixedincome_spreads.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/spreads/tcm",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/spreads/tcm", ("fred",),
+                        provider,
+                        "/fixedincome/spreads/tcm",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "maturity": maturity,
                 },
@@ -184,15 +186,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/spreads/tcm_effr",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/spreads/tcm_effr", ("fred",),
+                        provider,
+                        "/fixedincome/spreads/tcm_effr",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "maturity": maturity,
                 },
@@ -274,15 +278,17 @@
         """  # noqa: E501
 
         return self._run(
             "/fixedincome/spreads/treasury_effr",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/fixedincome/spreads/treasury_effr", ("fred",),
+                        provider,
+                        "/fixedincome/spreads/treasury_effr",
+                        ("fred",),
                     )
                 },
                 standard_params={
                     "start_date": start_date,
                     "end_date": end_date,
                     "maturity": maturity,
                 },
```

### Comparing `openbb-4.2.0/openbb/package/index.py` & `openbb-4.2.1/openbb/package/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,17 @@
         """  # noqa: E501
 
         return self._run(
             "/index/available",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/index/available", ("fmp", "yfinance"),
+                        provider,
+                        "/index/available",
+                        ("fmp", "yfinance"),
                     )
                 },
                 standard_params={},
                 extra_params=kwargs,
             )
         )
 
@@ -158,18 +160,22 @@
         """  # noqa: E501
 
         return self._run(
             "/index/constituents",
             **filter_inputs(
                 provider_choices={
                     "provider": self._get_provider(
-                        provider, "/index/constituents", ("fmp",),
+                        provider,
+                        "/index/constituents",
+                        ("fmp",),
                     )
                 },
-                standard_params={"symbol": symbol,},
+                standard_params={
+                    "symbol": symbol,
+                },
                 extra_params=kwargs,
             )
         )
 
     @exception_handler
     @validate
     @deprecated(
```

### Comparing `openbb-4.2.0/openbb/package/news.py` & `openbb-4.2.1/openbb/package/news.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,17 +108,17 @@
         word_count_greater_than : Optional[int]
             News stories will have a word count greater than this value. Unsupported for yahoo source. (provider: intrinio)
         word_count_less_than : Optional[int]
             News stories will have a word count less than this value. Unsupported for yahoo source. (provider: intrinio)
         is_spam : Optional[bool]
             Filter whether it is marked as spam or not. Unsupported for yahoo source. (provider: intrinio)
         business_relevance_greater_than : Optional[float]
-            News stories will have a business relevance score more than this value. Unsupported for yahoo source. (provider: intrinio)
+            News stories will have a business relevance score more than this value. Unsupported for yahoo source. Value is a decimal between 0 and 1. (provider: intrinio)
         business_relevance_less_than : Optional[float]
-            News stories will have a business relevance score less than this value. Unsupported for yahoo source. (provider: intrinio)
+            News stories will have a business relevance score less than this value. Unsupported for yahoo source. Value is a decimal between 0 and 1. (provider: intrinio)
         offset : Optional[int]
             Page offset, used in conjunction with limit. (provider: tiingo)
 
         Returns
         -------
         OBBject
             results : List[CompanyNews]
@@ -169,15 +169,15 @@
         summary : Optional[str]
             The summary of the news article. (provider: intrinio)
         topics : Optional[str]
             The topics related to the news article. (provider: intrinio)
         word_count : Optional[int]
             The word count of the news article. (provider: intrinio)
         business_relevance : Optional[float]
-             	How strongly correlated the news article is to the business (provider: intrinio)
+                How strongly correlated the news article is to the business (provider: intrinio)
         sentiment : Optional[str]
             The sentiment of the news article - i.e, negative, positive. (provider: intrinio)
         sentiment_confidence : Optional[float]
             The confidence score of the sentiment rating. (provider: intrinio)
         language : Optional[str]
             The language of the news article. (provider: intrinio)
         spam : Optional[bool]
@@ -323,17 +323,17 @@
         word_count_greater_than : Optional[int]
             News stories will have a word count greater than this value. Unsupported for yahoo source. (provider: intrinio)
         word_count_less_than : Optional[int]
             News stories will have a word count less than this value. Unsupported for yahoo source. (provider: intrinio)
         is_spam : Optional[bool]
             Filter whether it is marked as spam or not. Unsupported for yahoo source. (provider: intrinio)
         business_relevance_greater_than : Optional[float]
-            News stories will have a business relevance score more than this value. Unsupported for yahoo source. (provider: intrinio)
+            News stories will have a business relevance score more than this value. Unsupported for yahoo source. Value is a decimal between 0 and 1. (provider: intrinio)
         business_relevance_less_than : Optional[float]
-            News stories will have a business relevance score less than this value. Unsupported for yahoo source. (provider: intrinio)
+            News stories will have a business relevance score less than this value. Unsupported for yahoo source. Value is a decimal between 0 and 1. (provider: intrinio)
         offset : Optional[int]
             Page offset, used in conjunction with limit. (provider: tiingo)
 
         Returns
         -------
         OBBject
             results : List[WorldNews]
@@ -380,15 +380,15 @@
         summary : Optional[str]
             The summary of the news article. (provider: intrinio)
         topics : Optional[str]
             The topics related to the news article. (provider: intrinio)
         word_count : Optional[int]
             The word count of the news article. (provider: intrinio)
         business_relevance : Optional[float]
-             	How strongly correlated the news article is to the business (provider: intrinio)
+                How strongly correlated the news article is to the business (provider: intrinio)
         sentiment : Optional[str]
             The sentiment of the news article - i.e, negative, positive. (provider: intrinio)
         sentiment_confidence : Optional[float]
             The confidence score of the sentiment rating. (provider: intrinio)
         language : Optional[str]
             The language of the news article. (provider: intrinio)
         spam : Optional[bool]
```

### Comparing `openbb-4.2.0/pyproject.toml` & `openbb-4.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 [tool.poetry]
 name = "openbb"
-version = "4.2.0"
-description = "OpenBB"
+version = "4.2.1"
+description = "Investment research for everyone, anywhere."
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
-openbb-benzinga = "^1.2.0"
-openbb-econdb = "^1.1.0"
-openbb-federal-reserve = "^1.2.0"
-openbb-fmp = "^1.2.0"
-openbb-fred = "^1.2.0"
-openbb-intrinio = "^1.2.0"
-openbb-oecd = "^1.2.0"
-openbb-polygon = "^1.2.0"
-openbb-sec = "^1.2.0"
-openbb-tiingo = "^1.2.0"
-openbb-tradingeconomics = "^1.2.0"
-openbb-yfinance = "^1.2.0"
-
-openbb-commodity = "^1.1.0"
-openbb-crypto = "^1.2.0"
-openbb-currency = "^1.2.0"
-openbb-derivatives = "^1.2.0"
-openbb-economy = "^1.2.0"
-openbb-equity = "^1.2.0"
-openbb-etf = "^1.2.0"
-openbb-fixedincome = "^1.2.0"
-openbb-index = "^1.2.0"
-openbb-news = "^1.2.0"
-openbb-regulators = "^1.2.0"
+openbb-benzinga = "^1.2.1"
+openbb-econdb = "^1.1.1"
+openbb-federal-reserve = "^1.2.1"
+openbb-fmp = "^1.2.1"
+openbb-fred = "^1.2.1"
+openbb-intrinio = "^1.2.1"
+openbb-oecd = "^1.2.1"
+openbb-polygon = "^1.2.1"
+openbb-sec = "^1.2.1"
+openbb-tiingo = "^1.2.1"
+openbb-tradingeconomics = "^1.2.1"
+openbb-yfinance = "^1.2.1"
+
+openbb-commodity = "^1.1.1"
+openbb-crypto = "^1.2.1"
+openbb-currency = "^1.2.1"
+openbb-derivatives = "^1.2.1"
+openbb-economy = "^1.2.1"
+openbb-equity = "^1.2.1"
+openbb-etf = "^1.2.1"
+openbb-fixedincome = "^1.2.1"
+openbb-index = "^1.2.1"
+openbb-news = "^1.2.1"
+openbb-regulators = "^1.2.1"
 
 # Community dependencies
-openbb-alpha-vantage = { version = "^1.2.0", optional = true }
-openbb-biztoc = { version = "^1.2.0", optional = true }
-openbb-cboe = { version = "^1.2.0", optional = true }
-openbb-ecb = { version = "^1.2.0", optional = true }
-openbb-finra = { version = "^1.2.0", optional = true }
-openbb-finviz = { version = "^1.1.0", optional = true }
-openbb-government-us = { version = "^1.2.0", optional = true }
-openbb-nasdaq = { version = "^1.2.0", optional = true }
-openbb-seeking-alpha = { version = "^1.2.0", optional = true }
-openbb-stockgrid = { version = "^1.2.0", optional = true }
-openbb-tmx = { version = "^1.1.0", optional = true }
-openbb-tradier = { version = "^1.1.0", optional = true }
-openbb-wsj = { version = "^1.2.0", optional = true }
-
-openbb-charting = { version = "^2.1.0", optional = true }
-openbb-econometrics = { version = "^1.2.0", optional = true }
-openbb-quantitative = { version = "^1.2.0", optional = true }
-openbb-technical = { version = "^1.2.0", optional = true }
+openbb-alpha-vantage = { version = "^1.2.1", optional = true }
+openbb-biztoc = { version = "^1.2.1", optional = true }
+openbb-cboe = { version = "^1.2.1", optional = true }
+openbb-ecb = { version = "^1.2.1", optional = true }
+openbb-finra = { version = "^1.2.1", optional = true }
+openbb-finviz = { version = "^1.1.1", optional = true }
+openbb-government-us = { version = "^1.2.1", optional = true }
+openbb-nasdaq = { version = "^1.2.1", optional = true }
+openbb-seeking-alpha = { version = "^1.2.1", optional = true }
+openbb-stockgrid = { version = "^1.2.1", optional = true }
+openbb-tmx = { version = "^1.1.1", optional = true }
+openbb-tradier = { version = "^1.1.1", optional = true }
+openbb-wsj = { version = "^1.2.1", optional = true }
+
+openbb-charting = { version = "^2.1.1", optional = true }
+openbb-econometrics = { version = "^1.2.1", optional = true }
+openbb-quantitative = { version = "^1.2.1", optional = true }
+openbb-technical = { version = "^1.2.1", optional = true }
 
 [tool.poetry.extras]
 alpha_vantage = ["openbb-alpha-vantage"]
 biztoc = ["openbb-biztoc"]
 cboe = ["openbb-cboe"]
 charting = ["openbb-charting"]
 ecb = ["openbb-ecb"]
```

### Comparing `openbb-4.2.0/PKG-INFO` & `openbb-4.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: openbb
-Version: 4.2.0
-Summary: OpenBB
+Version: 4.2.1
+Summary: Investment research for everyone, anywhere.
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -26,55 +26,55 @@
 Provides-Extra: quantitative
 Provides-Extra: seeking-alpha
 Provides-Extra: stockgrid
 Provides-Extra: technical
 Provides-Extra: tmx
 Provides-Extra: tradier
 Provides-Extra: wsj
-Requires-Dist: openbb-alpha-vantage (>=1.2.0,<2.0.0) ; extra == "alpha-vantage" or extra == "all"
-Requires-Dist: openbb-benzinga (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-biztoc (>=1.2.0,<2.0.0) ; extra == "biztoc" or extra == "all"
-Requires-Dist: openbb-cboe (>=1.2.0,<2.0.0) ; extra == "cboe" or extra == "all"
-Requires-Dist: openbb-charting (>=2.1.0,<3.0.0) ; extra == "charting" or extra == "all"
-Requires-Dist: openbb-commodity (>=1.1.0,<2.0.0)
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
-Requires-Dist: openbb-crypto (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-currency (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-derivatives (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-ecb (>=1.2.0,<2.0.0) ; extra == "ecb" or extra == "all"
-Requires-Dist: openbb-econdb (>=1.1.0,<2.0.0)
-Requires-Dist: openbb-econometrics (>=1.2.0,<2.0.0) ; extra == "econometrics" or extra == "all"
-Requires-Dist: openbb-economy (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-equity (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-etf (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-federal-reserve (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-finra (>=1.2.0,<2.0.0) ; extra == "finra" or extra == "all"
-Requires-Dist: openbb-finviz (>=1.1.0,<2.0.0) ; extra == "finviz" or extra == "all"
-Requires-Dist: openbb-fixedincome (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-fmp (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-fred (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-government-us (>=1.2.0,<2.0.0) ; extra == "government-us" or extra == "all"
-Requires-Dist: openbb-index (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-intrinio (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-nasdaq (>=1.2.0,<2.0.0) ; extra == "nasdaq" or extra == "all"
-Requires-Dist: openbb-news (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-oecd (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-polygon (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-quantitative (>=1.2.0,<2.0.0) ; extra == "quantitative" or extra == "all"
-Requires-Dist: openbb-regulators (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-sec (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-seeking-alpha (>=1.2.0,<2.0.0) ; extra == "seeking-alpha" or extra == "all"
-Requires-Dist: openbb-stockgrid (>=1.2.0,<2.0.0) ; extra == "stockgrid" or extra == "all"
-Requires-Dist: openbb-technical (>=1.2.0,<2.0.0) ; extra == "technical" or extra == "all"
-Requires-Dist: openbb-tiingo (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-tmx (>=1.1.0,<2.0.0) ; extra == "tmx" or extra == "all"
-Requires-Dist: openbb-tradier (>=1.1.0,<2.0.0) ; extra == "tradier" or extra == "all"
-Requires-Dist: openbb-tradingeconomics (>=1.2.0,<2.0.0)
-Requires-Dist: openbb-wsj (>=1.2.0,<2.0.0) ; extra == "wsj" or extra == "all"
-Requires-Dist: openbb-yfinance (>=1.2.0,<2.0.0)
+Requires-Dist: openbb-alpha-vantage (>=1.2.1,<2.0.0) ; extra == "alpha-vantage" or extra == "all"
+Requires-Dist: openbb-benzinga (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-biztoc (>=1.2.1,<2.0.0) ; extra == "biztoc" or extra == "all"
+Requires-Dist: openbb-cboe (>=1.2.1,<2.0.0) ; extra == "cboe" or extra == "all"
+Requires-Dist: openbb-charting (>=2.1.1,<3.0.0) ; extra == "charting" or extra == "all"
+Requires-Dist: openbb-commodity (>=1.1.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
+Requires-Dist: openbb-crypto (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-currency (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-derivatives (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-ecb (>=1.2.1,<2.0.0) ; extra == "ecb" or extra == "all"
+Requires-Dist: openbb-econdb (>=1.1.1,<2.0.0)
+Requires-Dist: openbb-econometrics (>=1.2.1,<2.0.0) ; extra == "econometrics" or extra == "all"
+Requires-Dist: openbb-economy (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-equity (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-etf (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-federal-reserve (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-finra (>=1.2.1,<2.0.0) ; extra == "finra" or extra == "all"
+Requires-Dist: openbb-finviz (>=1.1.1,<2.0.0) ; extra == "finviz" or extra == "all"
+Requires-Dist: openbb-fixedincome (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-fmp (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-fred (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-government-us (>=1.2.1,<2.0.0) ; extra == "government-us" or extra == "all"
+Requires-Dist: openbb-index (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-intrinio (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-nasdaq (>=1.2.1,<2.0.0) ; extra == "nasdaq" or extra == "all"
+Requires-Dist: openbb-news (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-oecd (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-polygon (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-quantitative (>=1.2.1,<2.0.0) ; extra == "quantitative" or extra == "all"
+Requires-Dist: openbb-regulators (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-sec (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-seeking-alpha (>=1.2.1,<2.0.0) ; extra == "seeking-alpha" or extra == "all"
+Requires-Dist: openbb-stockgrid (>=1.2.1,<2.0.0) ; extra == "stockgrid" or extra == "all"
+Requires-Dist: openbb-technical (>=1.2.1,<2.0.0) ; extra == "technical" or extra == "all"
+Requires-Dist: openbb-tiingo (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-tmx (>=1.1.1,<2.0.0) ; extra == "tmx" or extra == "all"
+Requires-Dist: openbb-tradier (>=1.1.1,<2.0.0) ; extra == "tradier" or extra == "all"
+Requires-Dist: openbb-tradingeconomics (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-wsj (>=1.2.1,<2.0.0) ; extra == "wsj" or extra == "all"
+Requires-Dist: openbb-yfinance (>=1.2.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Platform
 
 [![Downloads](https://static.pepy.tech/badge/openbb)](https://pepy.tech/project/openbb)
 [![LatestRelease](https://badge.fury.io/py/openbb.svg)](https://github.com/OpenBB-finance/OpenBBTerminal)
```

