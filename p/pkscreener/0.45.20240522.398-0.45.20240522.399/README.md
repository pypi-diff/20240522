# Comparing `tmp/pkscreener-0.45.20240522.398.tar.gz` & `tmp/pkscreener-0.45.20240522.399.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240522.398.tar", last modified: Wed May 22 09:46:52 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240522.399.tar", last modified: Wed May 22 20:05:44 2024, max compression
```

## Comparing `pkscreener-0.45.20240522.398.tar` & `pkscreener-0.45.20240522.399.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/
--rw-rw-rw-   0        0        0     1086 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/LICENSE-Others
--rw-rw-rw-   0        0        0    27920 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/PKG-INFO
--rw-rw-rw-   0        0        0    26981 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:52.323893 pkscreener-0.45.20240522.398/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5641 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34251 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45624 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8313 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156748 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56708 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    85688 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-22 09:46:40.000000 pkscreener-0.45.20240522.398/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   147508 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1089 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    54014 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34564 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27920 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/setup.cfg
--rw-rw-rw-   0        0        0     5728 2024-05-22 09:41:49.000000 pkscreener-0.45.20240522.398/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:44.779197 pkscreener-0.45.20240522.399/
+-rw-rw-rw-   0        0        0     1086 2024-05-22 20:01:54.000000 pkscreener-0.45.20240522.399/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-22 20:01:54.000000 pkscreener-0.45.20240522.399/LICENSE-Others
+-rw-rw-rw-   0        0        0    27918 2024-05-22 20:05:44.779197 pkscreener-0.45.20240522.399/PKG-INFO
+-rw-rw-rw-   0        0        0    26979 2024-05-22 20:01:54.000000 pkscreener-0.45.20240522.399/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:44.763570 pkscreener-0.45.20240522.399/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:44.779197 pkscreener-0.45.20240522.399/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34244 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10305 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45614 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8313 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156748 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56838 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    86151 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-22 20:05:36.000000 pkscreener-0.45.20240522.399/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   147505 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1092 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    54014 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34564 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:44.763570 pkscreener-0.45.20240522.399/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27918 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-22 20:05:44.000000 pkscreener-0.45.20240522.399/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-22 20:05:44.779197 pkscreener-0.45.20240522.399/setup.cfg
+-rw-rw-rw-   0        0        0     5728 2024-05-22 20:01:55.000000 pkscreener-0.45.20240522.399/setup.py
```

### Comparing `pkscreener-0.45.20240522.398/LICENSE` & `pkscreener-0.45.20240522.399/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/LICENSE-Others` & `pkscreener-0.45.20240522.399/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/PKG-INFO` & `pkscreener-0.45.20240522.399/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240522.398
+Version: 0.45.20240522.399
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.398.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.399.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -223,15 +223,15 @@
 |  8  |       **Trend**       | By using advance algorithms, the average trendlines are computed for `N` days and their strenght is displayed depending on steepness of trendlines. (This does NOT show any trendline on chart, it is calculated internally) | `Strong Up`, `Weak Down` etc.                                                            |
 |  9  |      **Pattern**      | If the chart or the candle itself forming any important pattern in the recent timeframe or as per the selected screening option, various important patterns will be indicated here.                                          | `Momentum Gainer`, `Inside Bar (N)`,`Bullish Engulfing` etc.                             |
 
 ## Hack it your way:
 Feel free to Edit the parameters in the `pkscreener.ini` file which will be generated by the application.
 ```
 [config]
-period = 280d
+period = 1y
 daystolookback = 22
 duration = 1d
 minprice = 20.0
 maxprice = 50000.0
 volumeratio = 2.5
 consolidationpercentage = 10.0
 shuffle = y
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240522.398/README.md` & `pkscreener-0.45.20240522.399/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -201,15 +201,15 @@
 |  8  |       **Trend**       | By using advance algorithms, the average trendlines are computed for `N` days and their strenght is displayed depending on steepness of trendlines. (This does NOT show any trendline on chart, it is calculated internally) | `Strong Up`, `Weak Down` etc.                                                            |
 |  9  |      **Pattern**      | If the chart or the candle itself forming any important pattern in the recent timeframe or as per the selected screening option, various important patterns will be indicated here.                                          | `Momentum Gainer`, `Inside Bar (N)`,`Bullish Engulfing` etc.                             |
 
 ## Hack it your way:
 Feel free to Edit the parameters in the `pkscreener.ini` file which will be generated by the application.
 ```
 [config]
-period = 280d
+period = 1y
 daystolookback = 22
 duration = 1d
 minprice = 20.0
 maxprice = 50000.0
 volumeratio = 2.5
 consolidationpercentage = 10.0
 shuffle = y
@@ -252,19 +252,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener/__init__.py` & `pkscreener-0.45.20240522.399/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,28 +32,28 @@
 from PKDevTools.classes.ColorText import colorText
 from PKDevTools.classes.log import default_logger
 from PKDevTools.classes.Singleton import SingletonType, SingletonMixin
 from PKDevTools.classes.OutputControls import OutputControls
 parser = configparser.ConfigParser(strict=False)
 
 # Default attributes for Downloading Cache from Git repo
-default_period = "280d"
+default_period = "1y"
 default_duration = "1d"
 default_timeout = 2
 
 
 # This Class manages read/write of user configuration
 class tools(SingletonMixin, metaclass=SingletonType):
     def __init__(self):
         super(tools, self).__init__()
         self.consolidationPercentage = 10
         self.volumeRatio = 2.5
         self.minLTP = 20.0
         self.maxLTP = 50000
-        self.period = "280d"
+        self.period = "1y"
         self.duration = "1d"
         self.shuffleEnabled = True
         self.cacheEnabled = True
         self.stageTwo = True
         self.useEMA = False
         self.showunknowntrends = True
         self.enablePortfolioCalculations = False
@@ -211,15 +211,15 @@
                 colorText.BOLD
                 + colorText.GREEN
                 + "[+] PKScreener User Configuration:"
                 + colorText.END
             )
             try:
                 self.period = input(
-                    f"[+] Valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max\n[+] Enter number of days for which stock data to be downloaded (Days).(Optimal = 280, Current: {colorText.FAIL}{self.period}{colorText.END}): "
+                    f"[+] Valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max\n[+] Enter number of days for which stock data to be downloaded (Days).(Optimal = 1y, Current: {colorText.FAIL}{self.period}{colorText.END}): "
                 ) or self.period
                 self.daysToLookback = input(
                     f"[+] Number of recent trading periods (TimeFrame) to screen for Breakout/Consolidation (Days)(Optimal = 22, Current: {colorText.FAIL}{self.daysToLookback}{colorText.END}): "
                 ) or self.daysToLookback
                 self.duration = input(
                     f"[+] Valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo\n[+] Enter Duration of each candle (Days)(Optimal = 1, Current: {colorText.FAIL}{self.duration}{colorText.END}): "
                 ) or self.duration
@@ -510,15 +510,15 @@
 
     # Toggle the duration and period for use in intraday and swing trading
     def toggleConfig(self, candleDuration, clearCache=True):
         if candleDuration is None:
             candleDuration = self.duration.lower()
         self.getConfig(parser)
         if candleDuration[-1] in ["d"]:
-            self.period = "280d"
+            self.period = "1y"
             self.cacheEnabled = True
         if candleDuration[-1] in ["m", "h"] and not self.isIntradayConfig():
             self.period = "1d"
             self.cacheEnabled = True
         if self.isIntradayConfig():
             self.duration = candleDuration if candleDuration[-1] in ["m", "h"] else "1m"
             candleType = candleDuration.replace("m","").replace("h","")
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/Fetcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,27 +103,32 @@
                 start = PKDateUtilities.tradingDate().strftime("%Y-%m-%d")
             if end is None:
                 end = PKDateUtilities.currentDateTime().strftime("%Y-%m-%d")
             if start == end:
                 # If we send start and end dates for intraday, it comes back with empty dataframe
                 start = None
                 end = None
-        with SuppressOutput(suppress_stdout=True, suppress_stderr=True):
-            data = yf.download(
-                tickers=stockCode,
-                period=period,
-                interval=duration,
-                proxy=proxyServer,
-                progress=False,
-                rounding = True,
-                group_by='ticker',
-                timeout=self.configManager.generalTimeout/4,
-                start=start,
-                end=end
-            )
+        data = None
+        with SuppressOutput(suppress_stdout=(not printCounter), suppress_stderr=(not printCounter)):
+            try:
+                data = yf.download(
+                    tickers=stockCode,
+                    period=period,
+                    interval=duration,
+                    proxy=proxyServer,
+                    progress=False,
+                    rounding = True,
+                    group_by='ticker',
+                    timeout=self.configManager.generalTimeout/4,
+                    start=start,
+                    end=end
+                )
+            except KeyError as e:
+                default_logger().debug(e,exc_info=True)
+                pass
         if printCounter:
             sys.stdout.write("\r\033[K")
             try:
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.GREEN
                     + (
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/MenuOptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,18 +100,18 @@
     "L": "Long Term",
     "S": "Short Term (Intraday)",
     "M": "Back to the Top/Main menu",
 }
 # Valid periods: 1d,5d,1mo,3mo,6mo,1y,2y,5y,10y,ytd,max
 # Valid intervals: 1m,2m,5m,15m,30m,60m,90m,1h,1d,5d,1wk,1mo,3mo
 level2_T_MenuDict_L = {
-    "1": "Daily (280d, 1d)",
-    "2": "Weekly (280d, 1wk)",
-    "3": "Monthly (280d, 1mo)",
-    "4": "Hourly (280d, 1h)",
+    "1": "Daily (1y, 1d)",
+    "2": "Weekly (1y, 1wk)",
+    "3": "Monthly (1y, 1mo)",
+    "4": "Hourly (1y, 1h)",
     "5": "Custom",
     "M": "Back to the Top/Main menu",
 }
 level2_T_MenuDict_S = {
     "1": "1m (1d, 1m)",
     "2": "5m (1d, 5m)",
     "3": "15m (1d, 15m)",
@@ -704,15 +704,15 @@
                     ""
                 )
             return menuText
         
     def renderLevel1_T_Menus(
         self, skip=[], asList=False, renderStyle=None, parent=None
     ):
-        defaultKey = 'L' if configManager.period == '280d' else 'S'
+        defaultKey = 'L' if configManager.period == '1y' else 'S'
         menuText = self.fromDictionary(
             level1_T_MenuDict,
             renderExceptionKeys=["M"],
             renderStyle=renderStyle
             if renderStyle is not None
             else MenuRenderStyle.STANDALONE,
             skip=skip,
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/StockScreener.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,22 +97,23 @@
             with hostRef.processingCounter.get_lock():
                 hostRef.processingCounter.value += 1
 
             volumeRatio, period = self.determineBasicConfigs(stock, newlyListedOnly, volumeRatio, logLevel, hostRef, configManager, screener, userArgsLog)
             # hostRef.default_logger.info(
             #     f"For stock:{stock}, stock exists in objectDictionary:{hostRef.objectDictionaryPrimary.get(stock)}, cacheEnabled:{configManager.cacheEnabled}, isTradingTime:{self.isTradingTime}, downloadOnly:{downloadOnly}"
             # )
+            data = None
             data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef,hostRef.objectDictionaryPrimary, configManager, fetcher, period,None, testData,exchangeName)
             if not configManager.isIntradayConfig() and configManager.calculatersiintraday:
                 # Daily data is already available in "data" above.
                 # We need the intraday data for 1-d RSI values when config is not for intraday
                 intraday_data = self.getRelevantDataForStock(totalSymbols, shouldCache, stock, downloadOnly, printCounter, backtestDuration, hostRef, hostRef.objectDictionarySecondary, configManager, fetcher, "1d","1m", testData,exchangeName)
                 
             if data is not None:
-                if len(data) == 0 or len(data) < backtestDuration:
+                if len(data) == 0 or data.empty or len(data) < backtestDuration:
                     raise StockDataEmptyException(f"Data length:{len(data)}")
             else:
                 raise StockDataEmptyException(f"Data is None: {data}")
             
             bidGreaterThanAsk = False
             bidAskRatio = 0
             if executeOption == 29:
@@ -618,15 +619,15 @@
                             backtestDuration,
                         )
 
         except KeyboardInterrupt: # pragma: no cover
             # Capturing Ctr+C Here isn't a great idea
             pass
         except StockDataEmptyException as e: # pragma: no cover
-            if not data.isnull().values.all(axis=0)[0]:
+            if data is None or (data is not None and not data.isnull().values.all(axis=0)[0]):
                 hostRef.default_logger.debug(f"StockDataEmptyException:{stock}: {e}", exc_info=True)
             pass
         except ScreeningStatistics.EligibilityConditionNotMet as e:
             if userArgsLog:
                 hostRef.default_logger.debug(f"EligibilityConditionNotMet:{stock}: {e}", exc_info=True)
             pass
         except ScreeningStatistics.NotNewlyListed as e: # pragma: no cover
@@ -841,15 +842,16 @@
                         configManager.duration if duration is None else duration,
                         hostRef.proxyServer,
                         hostRef.processingResultsCounter,
                         hostRef.processingCounter,
                         totalSymbols,
                         start=start,
                         end=start,
-                        exchangeSuffix=".NS" if exchangeName == "INDIA" else ""
+                        exchangeSuffix=".NS" if exchangeName == "INDIA" else "",
+                        printCounter=printCounter
                     )
                 if hostData is not None and data is not None:
                     # During the market trading hours, we don't want to go for MFI/FV value fetching
                     # So let's copy the old saved ones.
                     try:
                         data["MF"] = hostData["MF"]
                         data["MF_Date"] = hostData["MF_Date"]
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/Utility.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,14 +797,19 @@
             try:
                 with open(cache_file, "wb") as f:
                     pickle.dump(stockDict.copy(), f, protocol=pickle.HIGHEST_PROTOCOL)
                     OutputControls().printOutput(colorText.BOLD + colorText.GREEN + "=> Done." + colorText.END)
                 if downloadOnly:
                     OutputControls().printOutput(colorText.BOLD + colorText.GREEN + f"=> {cache_file}" + colorText.END)
                     Committer.execOSCommand(f"git add {cache_file} -f >/dev/null 2>&1")
+                    if "RUNNER" not in os.environ.keys():
+                        copyFilePath = os.path.join(Archiver.get_user_outputs_dir(), f"copy_{fileName}")
+                        cacheFileSize = os.stat(cache_file).st_size if os.path.exists(cache_file) else 0
+                        if os.path.exists(cache_file) and cacheFileSize >= 1024*1024*50:
+                            shutil.copy(cache_file,copyFilePath) # copy is the saved source of truth
             except pickle.PicklingError as e:  # pragma: no cover
                 default_logger().debug(e, exc_info=True)
                 OutputControls().printOutput(
                     colorText.BOLD
                     + colorText.FAIL
                     + "=> Error while Caching Stock Data."
                     + colorText.END
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/classes/keys.py` & `pkscreener-0.45.20240522.399/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/courbd.ttf` & `pkscreener-0.45.20240522.399/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/globals.py` & `pkscreener-0.45.20240522.399/pkscreener/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,15 +397,15 @@
             input("Press <Enter> to continue...")
     elif menuOption == "T":
         if userPassedArgs is None or userPassedArgs.options is None:
             selectedMenu = m0.find(menuOption)
             m1.renderForMenu(selectedMenu=selectedMenu)
             periodOption = input(
                     colorText.BOLD + colorText.FAIL + "[+] Select option: "
-                ) or ('L' if configManager.period == '280d' else 'S')
+                ) or ('L' if configManager.period == '1y' else 'S')
             OutputControls().printOutput(colorText.END, end="")
             if periodOption is None or periodOption.upper() not in ["L","S"]:
                 return
             Utility.tools.clearScreen(forceTop=True)
             if periodOption.upper() in ["L","S"]:
                 selectedMenu = m1.find(periodOption)
                 m2.renderForMenu(selectedMenu=selectedMenu)
@@ -2881,15 +2881,15 @@
 def takeBacktestInputs(
     menuOption=None, indexOption=None, executeOption=None, backtestPeriod=0
 ):
     g10k = '"Growth of 10k"'
     OutputControls().printOutput(
         colorText.BOLD
         + colorText.GREEN
-        + f"[+] For {g10k if menuOption == 'G' else 'backtesting'}, you can choose from (1,2,3,4,5,10,15,22,30) or any other custom periods (< 280)."
+        + f"[+] For {g10k if menuOption == 'G' else 'backtesting'}, you can choose from (1,2,3,4,5,10,15,22,30) or any other custom periods (< 1y)."
     )
     try:
         if backtestPeriod == 0:
             backtestPeriod = int(
                 input(
                     colorText.BOLD
                     + colorText.FAIL
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240522.399/pkscreener/pkscreener.ini`

 * *Files 23% similar despite different names*

```diff
@@ -11,59 +11,59 @@
 000000a0: 636b 6461 7461 203d 2079 0d0a 6361 6c63  ckdata = y..calc
 000000b0: 756c 6174 6572 7369 696e 7472 6164 6179  ulatersiintraday
 000000c0: 203d 206e 0d0a 6461 7973 746f 6c6f 6f6b   = n..daystolook
 000000d0: 6261 636b 203d 2032 320d 0a64 6566 6175  back = 22..defau
 000000e0: 6c74 696e 6465 7820 3d20 3132 0d0a 6465  ltindex = 12..de
 000000f0: 6661 756c 746d 6f6e 6974 6f72 6f70 7469  faultmonitoropti
 00000100: 6f6e 7320 3d20 583a 3132 3a39 3a32 2e35  ons = X:12:9:2.5
-00000110: 7e58 3a31 323a 3233 7e58 3a31 323a 3238  ~X:12:23~X:12:28
-00000120: 7e58 3a31 323a 3331 7e7c 7b31 7d58 3a31  ~X:12:31~|{1}X:1
-00000130: 323a 3233 3a3e 7c58 3a30 3a32 373a 3e7c  2:23:>|X:0:27:>|
-00000140: 583a 303a 3331 3a7e 7c7b 327d 583a 303a  X:0:31:~|{2}X:0:
-00000150: 3331 3a7e 7c7b 337d 583a 303a 3237 3a7e  31:~|{3}X:0:27:~
-00000160: 583a 3132 3a37 3a33 3a2e 3031 3a31 7e7c  X:12:7:3:.01:1~|
-00000170: 7b35 7d58 3a30 3a35 3a30 3a34 303a 7e58  {5}X:0:5:0:40:~X
-00000180: 3a31 323a 373a 363a 317e 583a 3132 3a31  :12:7:6:1~X:12:1
-00000190: 313a 7e58 3a31 323a 3132 3a69 2035 6d7e  1:~X:12:12:i 5m~
-000001a0: 583a 3132 3a31 377e 583a 3132 3a32 347e  X:12:17~X:12:24~
-000001b0: 583a 3132 3a36 3a37 3a31 7e58 3a31 323a  X:12:6:7:1~X:12:
-000001c0: 363a 337e 583a 3132 3a36 3a38 7e58 3a31  6:3~X:12:6:8~X:1
-000001d0: 323a 363a 397e 583a 3132 3a36 3a31 303a  2:6:9~X:12:6:10:
-000001e0: 317e 583a 3132 3a37 3a33 3a2e 3032 3a31  1~X:12:7:3:.02:1
-000001f0: 7e58 3a31 323a 3133 3a69 2031 6d7e 583a  ~X:12:13:i 1m~X:
-00000200: 3132 3a32 7e7c 7b31 7d58 3a30 3a32 393a  12:2~|{1}X:0:29:
-00000210: 0d0a 6475 7261 7469 6f6e 203d 2031 640d  ..duration = 1d.
-00000220: 0a65 6e61 626c 6570 6f72 7466 6f6c 696f  .enableportfolio
-00000230: 6361 6c63 756c 6174 696f 6e73 203d 206e  calculations = n
-00000240: 0d0a 6765 6e65 7261 6c74 696d 656f 7574  ..generaltimeout
-00000250: 203d 2032 2e30 0d0a 6c6f 6773 656e 6162   = 2.0..logsenab
-00000260: 6c65 6420 3d20 6e0d 0a6c 6f6e 6774 696d  led = n..longtim
-00000270: 656f 7574 203d 2034 2e30 0d0a 6d61 7862  eout = 4.0..maxb
-00000280: 6163 6b74 6573 7477 696e 646f 7720 3d20  acktestwindow = 
-00000290: 3330 0d0a 6d61 7864 6173 6862 6f61 7264  30..maxdashboard
-000002a0: 7769 6467 6574 7370 6572 726f 7720 3d20  widgetsperrow = 
-000002b0: 350d 0a6d 6178 6e65 7477 6f72 6b72 6574  5..maxnetworkret
-000002c0: 7279 636f 756e 7420 3d20 3130 0d0a 6d61  rycount = 10..ma
-000002d0: 786e 756d 7265 7375 6c74 726f 7773 696e  xnumresultrowsin
-000002e0: 6d6f 6e69 746f 7220 3d20 330d 0a6d 6f72  monitor = 3..mor
-000002f0: 6e69 6e67 616e 616c 7973 6973 6361 6e64  ninganalysiscand
-00000300: 6c65 6e75 6d62 6572 203d 2032 350d 0a6d  lenumber = 25..m
-00000310: 6f72 6e69 6e67 616e 616c 7973 6973 6361  orninganalysisca
-00000320: 6e64 6c65 6475 7261 7469 6f6e 203d 2031  ndleduration = 1
-00000330: 6d0d 0a6f 6e6c 7973 7461 6765 7477 6f73  m..onlystagetwos
-00000340: 746f 636b 7320 3d20 790d 0a70 6572 696f  tocks = y..perio
-00000350: 6420 3d20 3238 3064 0d0a 7368 6f77 7061  d = 280d..showpa
-00000360: 7374 7374 7261 7465 6779 6461 7461 203d  ststrategydata =
-00000370: 206e 0d0a 7368 6f77 756e 6b6e 6f77 6e74   n..showunknownt
-00000380: 7265 6e64 7320 3d20 790d 0a73 6875 6666  rends = y..shuff
-00000390: 6c65 203d 2079 0d0a 7573 6565 6d61 203d  le = y..useema =
-000003a0: 206e 0d0a 0d0a 5b66 696c 7465 7273 5d0d   n....[filters].
-000003b0: 0a63 6f6e 736f 6c69 6461 7469 6f6e 7065  .consolidationpe
-000003c0: 7263 656e 7461 6765 203d 2031 302e 300d  rcentage = 10.0.
-000003d0: 0a6d 6178 7072 6963 6520 3d20 3530 3030  .maxprice = 5000
-000003e0: 302e 300d 0a6d 696e 696d 756d 6368 616e  0.0..minimumchan
-000003f0: 6765 7065 7263 656e 7461 6765 203d 2030  gepercentage = 0
-00000400: 2e30 0d0a 6d69 6e69 6d75 6d76 6f6c 756d  .0..minimumvolum
-00000410: 6520 3d20 3130 3030 300d 0a6d 696e 7072  e = 10000..minpr
-00000420: 6963 6520 3d20 3230 2e30 0d0a 766f 6c75  ice = 20.0..volu
-00000430: 6d65 7261 7469 6f20 3d20 322e 350d 0a0d  meratio = 2.5...
-00000440: 0a                                       .
+00000110: 3a7e 583a 3132 3a32 383a 7e58 3a31 323a  :~X:12:28:~X:12:
+00000120: 3233 3a7e 7c7b 317d 583a 303a 3233 3a3e  23:~|{1}X:0:23:>
+00000130: 7c58 3a30 3a32 373a 3e7c 583a 303a 3331  |X:0:27:>|X:0:31
+00000140: 3a7e 7c7b 327d 583a 303a 3331 3a7e 7c7b  :~|{2}X:0:31:~|{
+00000150: 337d 583a 303a 3237 3a7e 583a 3132 3a37  3}X:0:27:~X:12:7
+00000160: 3a33 3a2e 3031 3a31 3a7e 7c7b 357d 583a  :3:.01:1:~|{5}X:
+00000170: 303a 353a 303a 3430 3a7e 583a 3132 3a37  0:5:0:40:~X:12:7
+00000180: 3a36 3a31 3a7e 583a 3132 3a31 313a 7e58  :6:1:~X:12:11:~X
+00000190: 3a31 323a 3132 3a69 2035 6d7e 583a 3132  :12:12:i 5m~X:12
+000001a0: 3a31 373a 7e58 3a31 323a 3234 3a7e 583a  :17:~X:12:24:~X:
+000001b0: 3132 3a36 3a37 3a31 3a7e 583a 3132 3a36  12:6:7:1:~X:12:6
+000001c0: 3a33 3a7e 583a 3132 3a36 3a38 3a7e 583a  :3:~X:12:6:8:~X:
+000001d0: 3132 3a36 3a39 3a7e 583a 3132 3a36 3a31  12:6:9:~X:12:6:1
+000001e0: 303a 313a 7e58 3a31 323a 373a 333a 2e30  0:1:~X:12:7:3:.0
+000001f0: 323a 313a 7e58 3a31 323a 3133 3a69 2031  2:1:~X:12:13:i 1
+00000200: 6d7e 583a 3132 3a32 3a7e 7c7b 317d 583a  m~X:12:2:~|{1}X:
+00000210: 303a 3239 3a0d 0a64 7572 6174 696f 6e20  0:29:..duration 
+00000220: 3d20 3164 0d0a 656e 6162 6c65 706f 7274  = 1d..enableport
+00000230: 666f 6c69 6f63 616c 6375 6c61 7469 6f6e  foliocalculation
+00000240: 7320 3d20 6e0d 0a67 656e 6572 616c 7469  s = n..generalti
+00000250: 6d65 6f75 7420 3d20 322e 300d 0a6c 6f67  meout = 2.0..log
+00000260: 7365 6e61 626c 6564 203d 206e 0d0a 6c6f  senabled = n..lo
+00000270: 6e67 7469 6d65 6f75 7420 3d20 342e 300d  ngtimeout = 4.0.
+00000280: 0a6d 6178 6261 636b 7465 7374 7769 6e64  .maxbacktestwind
+00000290: 6f77 203d 2033 300d 0a6d 6178 6461 7368  ow = 30..maxdash
+000002a0: 626f 6172 6477 6964 6765 7473 7065 7272  boardwidgetsperr
+000002b0: 6f77 203d 2035 0d0a 6d61 786e 6574 776f  ow = 5..maxnetwo
+000002c0: 726b 7265 7472 7963 6f75 6e74 203d 2031  rkretrycount = 1
+000002d0: 300d 0a6d 6178 6e75 6d72 6573 756c 7472  0..maxnumresultr
+000002e0: 6f77 7369 6e6d 6f6e 6974 6f72 203d 2033  owsinmonitor = 3
+000002f0: 0d0a 6d6f 726e 696e 6761 6e61 6c79 7369  ..morninganalysi
+00000300: 7363 616e 646c 656e 756d 6265 7220 3d20  scandlenumber = 
+00000310: 3235 0d0a 6d6f 726e 696e 6761 6e61 6c79  25..morninganaly
+00000320: 7369 7363 616e 646c 6564 7572 6174 696f  siscandleduratio
+00000330: 6e20 3d20 316d 0d0a 6f6e 6c79 7374 6167  n = 1m..onlystag
+00000340: 6574 776f 7374 6f63 6b73 203d 2079 0d0a  etwostocks = y..
+00000350: 7065 7269 6f64 203d 2031 790d 0a73 686f  period = 1y..sho
+00000360: 7770 6173 7473 7472 6174 6567 7964 6174  wpaststrategydat
+00000370: 6120 3d20 6e0d 0a73 686f 7775 6e6b 6e6f  a = n..showunkno
+00000380: 776e 7472 656e 6473 203d 2079 0d0a 7368  wntrends = y..sh
+00000390: 7566 666c 6520 3d20 790d 0a75 7365 656d  uffle = y..useem
+000003a0: 6120 3d20 6e0d 0a0d 0a5b 6669 6c74 6572  a = n....[filter
+000003b0: 735d 0d0a 636f 6e73 6f6c 6964 6174 696f  s]..consolidatio
+000003c0: 6e70 6572 6365 6e74 6167 6520 3d20 3130  npercentage = 10
+000003d0: 2e30 0d0a 6d61 7870 7269 6365 203d 2035  .0..maxprice = 5
+000003e0: 3030 3030 2e30 0d0a 6d69 6e69 6d75 6d63  0000.0..minimumc
+000003f0: 6861 6e67 6570 6572 6365 6e74 6167 6520  hangepercentage 
+00000400: 3d20 302e 300d 0a6d 696e 696d 756d 766f  = 0.0..minimumvo
+00000410: 6c75 6d65 203d 2031 3030 3030 0d0a 6d69  lume = 10000..mi
+00000420: 6e70 7269 6365 203d 2032 302e 300d 0a76  nprice = 20.0..v
+00000430: 6f6c 756d 6572 6174 696f 203d 2032 2e35  olumeratio = 2.5
+00000440: 0d0a 0d0a                                ....
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240522.399/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240522.399/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240522.399/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240522.398
+Version: 0.45.20240522.399
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.398.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.399.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
@@ -223,15 +223,15 @@
 |  8  |       **Trend**       | By using advance algorithms, the average trendlines are computed for `N` days and their strenght is displayed depending on steepness of trendlines. (This does NOT show any trendline on chart, it is calculated internally) | `Strong Up`, `Weak Down` etc.                                                            |
 |  9  |      **Pattern**      | If the chart or the candle itself forming any important pattern in the recent timeframe or as per the selected screening option, various important patterns will be indicated here.                                          | `Momentum Gainer`, `Inside Bar (N)`,`Bullish Engulfing` etc.                             |
 
 ## Hack it your way:
 Feel free to Edit the parameters in the `pkscreener.ini` file which will be generated by the application.
 ```
 [config]
-period = 280d
+period = 1y
 daystolookback = 22
 duration = 1d
 minprice = 20.0
 maxprice = 50000.0
 volumeratio = 2.5
 consolidationpercentage = 10.0
 shuffle = y
@@ -274,19 +274,19 @@
 * Always backtest and analyze the stocks manually before you trade.
 * The Author(s), the software and any related/unrelated entity will not be held liable for your own investing decisions or losses. The authors or this softfware does not make any claim about the correctness of the results.
 * This screener began as a [fork](https://github.com/pranjal-joshi/Screeni-py) but has since added a lot of additional scanners, backtesting, Telegram bots, Alerts and a number of modifications and improvements.
 
 [MADE-IN-INDIA-badge]: https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange
 [MADE-IN-INDIA]: https://en.wikipedia.org/wiki/India
 [Windows-badge]: https://img.shields.io/badge/Windows-0078D6?logo=windows&logoColor=white
-[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.exe
+[Windows]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.exe
 [Linux-badge]: https://img.shields.io/badge/Linux-FCC624?logo=linux&logoColor=black
-[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.bin
+[Linux]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.bin
 [Mac OS-badge]: https://img.shields.io/badge/mac%20os-D3D3D3?logo=apple&logoColor=000000
-[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240521.394/pkscreenercli.run
+[Mac OS]: https://github.com/pkjmesra/PKScreener/releases/download/0.45.20240522.398/pkscreenercli.run
 [GitHub release (latest by date)-badge]: https://img.shields.io/github/v/release/pkjmesra/PKScreener
 [GitHub release (latest by date)]: https://github.com/pkjmesra/PKScreener/releases/latest
 [pypi-badge]: https://img.shields.io/pypi/v/pkscreener.svg?style=flat-square
 [pypi]: https://pypi.python.org/pypi/pkscreener
 [wheel-badge]: https://img.shields.io/pypi/wheel/pkscreener.svg?style=flat-square
 [GitHub all releases]: https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge
 [License-badge]: https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge
```

### Comparing `pkscreener-0.45.20240522.398/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240522.399/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240522.398/setup.py` & `pkscreener-0.45.20240522.399/setup.py`

 * *Files identical despite different names*

