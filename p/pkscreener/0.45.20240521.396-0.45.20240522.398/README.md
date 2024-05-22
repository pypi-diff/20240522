# Comparing `tmp/pkscreener-0.45.20240521.396.tar.gz` & `tmp/pkscreener-0.45.20240522.398.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.45.20240521.396.tar", last modified: Tue May 21 21:49:46 2024, max compression
+gzip compressed data, was "pkscreener-0.45.20240522.398.tar", last modified: Wed May 22 09:46:52 2024, max compression
```

## Comparing `pkscreener-0.45.20240521.396.tar` & `pkscreener-0.45.20240522.398.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 21:49:46.411971 pkscreener-0.45.20240521.396/
--rw-rw-rw-   0        0        0     1086 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/LICENSE
--rw-rw-rw-   0        0        0     1091 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/LICENSE-Others
--rw-rw-rw-   0        0        0    27920 2024-05-21 21:49:46.411971 pkscreener-0.45.20240521.396/PKG-INFO
--rw-rw-rw-   0        0        0    26981 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 21:49:46.396346 pkscreener-0.45.20240521.396/pkscreener/
--rw-rw-rw-   0        0        0     1582 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:49:46.411971 pkscreener-0.45.20240521.396/pkscreener/classes/
--rw-rw-rw-   0        0        0    13324 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/ArtTexts.py
--rw-rw-rw-   0        0        0    10156 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0     5641 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/Barometer.py
--rw-rw-rw-   0        0        0    17333 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0     1537 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0    34249 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0    10076 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    13424 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/MarketMonitor.py
--rw-rw-rw-   0        0        0     3673 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/MarketStatus.py
--rw-rw-rw-   0        0        0    45624 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0    12534 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    24598 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/PKMarketOpenCloseAnalyser.py
--rw-rw-rw-   0        0        0    22819 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/PKScanRunner.py
--rw-rw-rw-   0        0        0     1623 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/PKScheduledTaskProgress.py
--rw-rw-rw-   0        0        0     8313 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/PKScheduler.py
--rw-rw-rw-   0        0        0     8466 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/PKSpreadsheets.py
--rw-rw-rw-   0        0        0     1907 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/PKTask.py
--rw-rw-rw-   0        0        0    18947 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0    14177 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/Portfolio.py
--rw-rw-rw-   0        0        0    49043 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/PortfolioXRay.py
--rw-rw-rw-   0        0        0   156748 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/ScreeningStatistics.py
--rw-rw-rw-   0        0        0    56708 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/StockScreener.py
--rw-rw-rw-   0        0        0     4993 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/UserMenuChoicesHandler.py
--rw-rw-rw-   0        0        0    85688 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0     3789 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/WorkflowManager.py
--rw-rw-rw-   0        0        0       28 2024-05-21 21:49:35.000000 pkscreener-0.45.20240521.396/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0     5262 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/classes/keys.py
--rw-rw-rw-   0        0        0   791436 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/courbd.ttf
--rw-rw-rw-   0        0        0   147508 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/globals.py
--rw-rw-rw-   0        0        0     1089 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/pkscreener.ini
--rw-rw-rw-   0        0        0    53062 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0    34370 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:49:46.396346 pkscreener-0.45.20240521.396/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    27920 2024-05-21 21:49:46.000000 pkscreener-0.45.20240521.396/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2024-05-21 21:49:46.000000 pkscreener-0.45.20240521.396/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 21:49:46.000000 pkscreener-0.45.20240521.396/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      120 2024-05-21 21:49:46.000000 pkscreener-0.45.20240521.396/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-21 21:49:46.000000 pkscreener-0.45.20240521.396/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-21 21:49:46.000000 pkscreener-0.45.20240521.396/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-05-21 21:49:46.411971 pkscreener-0.45.20240521.396/setup.cfg
--rw-rw-rw-   0        0        0     5728 2024-05-21 21:44:45.000000 pkscreener-0.45.20240521.396/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/
+-rw-rw-rw-   0        0        0     1086 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/LICENSE
+-rw-rw-rw-   0        0        0     1091 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/LICENSE-Others
+-rw-rw-rw-   0        0        0    27920 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/PKG-INFO
+-rw-rw-rw-   0        0        0    26981 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 09:46:52.323893 pkscreener-0.45.20240522.398/pkscreener/
+-rw-rw-rw-   0        0        0     1582 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/pkscreener/classes/
+-rw-rw-rw-   0        0        0    13324 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/ArtTexts.py
+-rw-rw-rw-   0        0        0    10156 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0     5641 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Barometer.py
+-rw-rw-rw-   0        0        0    17333 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0     1537 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0    34251 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0    10076 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    13424 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/MarketMonitor.py
+-rw-rw-rw-   0        0        0     3673 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/MarketStatus.py
+-rw-rw-rw-   0        0        0    45624 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0    12534 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    24598 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKMarketOpenCloseAnalyser.py
+-rw-rw-rw-   0        0        0    22819 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKScanRunner.py
+-rw-rw-rw-   0        0        0     1623 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKScheduledTaskProgress.py
+-rw-rw-rw-   0        0        0     8313 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKScheduler.py
+-rw-rw-rw-   0        0        0     8466 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKSpreadsheets.py
+-rw-rw-rw-   0        0        0     1907 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PKTask.py
+-rw-rw-rw-   0        0        0    18947 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0    14177 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Portfolio.py
+-rw-rw-rw-   0        0        0    49043 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/PortfolioXRay.py
+-rw-rw-rw-   0        0        0   156748 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/ScreeningStatistics.py
+-rw-rw-rw-   0        0        0    56708 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/StockScreener.py
+-rw-rw-rw-   0        0        0     4993 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/UserMenuChoicesHandler.py
+-rw-rw-rw-   0        0        0    85688 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0     3789 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/WorkflowManager.py
+-rw-rw-rw-   0        0        0       28 2024-05-22 09:46:40.000000 pkscreener-0.45.20240522.398/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0     5262 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/classes/keys.py
+-rw-rw-rw-   0        0        0   791436 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/courbd.ttf
+-rw-rw-rw-   0        0        0   147508 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/globals.py
+-rw-rw-rw-   0        0        0     1089 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/pkscreener.ini
+-rw-rw-rw-   0        0        0    54014 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0    34564 2024-05-22 09:41:48.000000 pkscreener-0.45.20240522.398/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    27920 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      120 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-22 09:46:52.000000 pkscreener-0.45.20240522.398/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-22 09:46:52.339515 pkscreener-0.45.20240522.398/setup.cfg
+-rw-rw-rw-   0        0        0     5728 2024-05-22 09:41:49.000000 pkscreener-0.45.20240522.398/setup.py
```

### Comparing `pkscreener-0.45.20240521.396/LICENSE` & `pkscreener-0.45.20240522.398/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/LICENSE-Others` & `pkscreener-0.45.20240522.398/LICENSE-Others`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/PKG-INFO` & `pkscreener-0.45.20240522.398/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.396
+Version: 0.45.20240522.398
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.396.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.398.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `pkscreener-0.45.20240521.396/README.md` & `pkscreener-0.45.20240522.398/README.md`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/__init__.py` & `pkscreener-0.45.20240522.398/pkscreener/__init__.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/ArtTexts.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/ArtTexts.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/Backtest.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/Barometer.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/Barometer.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/Changelog.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/Changelog.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/ConfigManager.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/ConfigManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,14 +368,15 @@
 
                 parser.set("filters", "consolidationPercentage", str(self.consolidationPercentage))
                 parser.set("filters", "maxPrice", str(self.maxLTP))
                 parser.set("filters", "minimumChangePercentage", str(self.minimumChangePercentage))
                 parser.set("filters", "minimumVolume", str(self.minVolume))
                 parser.set("filters", "minPrice", str(self.minLTP))
                 parser.set("filters", "volumeRatio", str(self.volumeRatio))
+
             except Exception as e:
                 default_logger().debug(e,exc_info=True)
                 from time import sleep
                 OutputControls().printOutput(colorText.FAIL + "Could not save configuration! Please check!" + colorText.END)
                 sleep(3)
                 pass
```

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/Fetcher.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/MarketMonitor.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/MarketMonitor.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/MarketStatus.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/MarketStatus.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/MenuOptions.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/PKMarketOpenCloseAnalyser.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/PKMarketOpenCloseAnalyser.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/PKScanRunner.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/PKScanRunner.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/PKScheduledTaskProgress.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/PKScheduledTaskProgress.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/PKScheduler.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/PKScheduler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/PKSpreadsheets.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/PKSpreadsheets.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/PKTask.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/PKTask.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/Pktalib.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/Portfolio.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/Portfolio.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/PortfolioXRay.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/PortfolioXRay.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/ScreeningStatistics.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/ScreeningStatistics.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/StockScreener.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/StockScreener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/UserMenuChoicesHandler.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/UserMenuChoicesHandler.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/Utility.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/WorkflowManager.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/WorkflowManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/classes/keys.py` & `pkscreener-0.45.20240522.398/pkscreener/classes/keys.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/courbd.ttf` & `pkscreener-0.45.20240522.398/pkscreener/courbd.ttf`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/globals.py` & `pkscreener-0.45.20240522.398/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/pkscreener.ini` & `pkscreener-0.45.20240522.398/pkscreener/pkscreener.ini`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/pkscreener/pkscreenerbot.py` & `pkscreener-0.45.20240522.398/pkscreener/pkscreenerbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 from pkscreener.classes.MenuOptions import MenuRenderStyle, menu, menus
 from pkscreener.classes.WorkflowManager import run_workflow
 from pkscreener.globals import showSendConfigInfo, showSendHelpInfo
 import pkscreener.classes.ConfigManager as ConfigManager
 
 monitor_proc = None
 configManager = ConfigManager.tools()
+bot_available=True
 
 try:
     from telegram import __version_info__
 except ImportError:
     __version_info__ = (0, 0, 0, 0, 0)  # type: ignore[assignment]
 
 if __version_info__ < (20, 0, 0, "alpha", 1):
@@ -145,54 +146,61 @@
                 launchIntradayMonitor()
     except:
         launchIntradayMonitor()
         pass
 
 async def start(update: Update, context: ContextTypes.DEFAULT_TYPE, updatedResults=None, monitorIndex=0,chosenBotMenuOption="") -> int:
     """Send message on `/start`."""
+    global bot_available
     updateCarrier = None
     if update is None:
         return
     else:
         if update.callback_query is not None:
             updateCarrier = update.callback_query
         if update.message is not None:
             updateCarrier = update.message
         if updateCarrier is None:
             return
     # Get user that sent /start and log his name
     user = updateCarrier.from_user
     logger.info("User %s started the conversation.", user.first_name)
+    if not bot_available:
+        updatedResults = "Apologies! The @nse_pkscreener_bot is NOT available for the time being! We are working with our host GitHub and other data source providers to sort out pending invoices and restore the services soon! Thanks for your patience and support! 🙏"
     # Build InlineKeyboard where each button has a displayed text
     # and a string as callback_data
     # The keyboard is a list of button rows, where each row is in turn
     # a list (hence `[[...]]`).
-    mns = m0.renderForMenu(asList=True)
-    if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()) or sys.argv[0].endswith(".py"):
-        mns.append(menu().create(f"MI_{monitorIndex}", "Int. Monitor", 2))
-    if user.username == OWNER_USER:
-        mns.append(menu().create(f"DV_0", ("Enbl" if not configManager.logsEnabled else "Dsbl"), 2))
+    if bot_available:
+        mns = m0.renderForMenu(asList=True)
+        if (PKDateUtilities.isTradingTime() and not PKDateUtilities.isTodayHoliday()[0]) or ("PKDevTools_Default_Log_Level" in os.environ.keys()) or sys.argv[0].endswith(".py"):
+            mns.append(menu().create(f"MI_{monitorIndex}", "Int. Monitor", 2))
+        if user.username == OWNER_USER:
+            mns.append(menu().create(f"DV_0", ("Enbl" if not configManager.logsEnabled else "Dsbl"), 2))
 
-    inlineMenus = []
-    for mnu in mns:
-        if mnu.menuKey[0:2] in TOP_LEVEL_SCANNER_MENUS:
-            inlineMenus.append(
-                InlineKeyboardButton(
-                    mnu.menuText.split("(")[0],
-                    callback_data="C" + str(mnu.menuKey),
+        inlineMenus = []
+        for mnu in mns:
+            if mnu.menuKey[0:2] in TOP_LEVEL_SCANNER_MENUS:
+                inlineMenus.append(
+                    InlineKeyboardButton(
+                        mnu.menuText.split("(")[0],
+                        callback_data="C" + str(mnu.menuKey),
+                    )
                 )
-            )
-    keyboard = [inlineMenus]
-    reply_markup = InlineKeyboardMarkup(keyboard)
-    cmds = m0.renderForMenu(
-        selectedMenu=None,
-        skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
-        asList=True,
-        renderStyle=MenuRenderStyle.STANDALONE,
-    )
+        keyboard = [inlineMenus]
+        reply_markup = InlineKeyboardMarkup(keyboard)
+        cmds = m0.renderForMenu(
+            selectedMenu=None,
+            skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
+            asList=True,
+            renderStyle=MenuRenderStyle.STANDALONE,
+        )
+    else:
+        reply_markup = None
+
     if updatedResults is None:
         cmdText = ""
         for cmd in cmds:
             cmdText = f"{cmdText}\n\n{cmd.commandTextKey()} for {cmd.commandTextLabel()}"
         menuText = f"Welcome {user.first_name}, {(user.username)}! Please choose a menu option by selecting a button from below.\n\nYou can also explore a wide variety of all other scanners by typing in \n{cmdText}\n\n OR just use the buttons below to choose."
     else:
         chosenBotMenuOption = f"{chosenBotMenuOption}\nInt. Monitor. MonitorIndex:{monitorIndex}\n{updatedResults}"
@@ -307,14 +315,18 @@
 
 async def XScanners(update: Update, context: ContextTypes.DEFAULT_TYPE) -> int:
     """Show new choice of buttons"""
     query = update.callback_query
     data = query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G").replace("CMI", "MI")
     if data[0:2] not in TOP_LEVEL_SCANNER_MENUS:
         return start(update, context)
+    global bot_available
+    if not bot_available:
+        await start(update, context)
+        return START_ROUTES
     if data.startswith("MI"):
         monitorIndex = int(data.split("_")[1])
         result_outputs, filePath = launchIntradayMonitor()
         filePath = f"{filePath}_{monitorIndex}.txt"
         monitorIndex += 1
         if monitorIndex >= configManager.maxDashboardWidgetsPerRow*configManager.maxNumResultRowsInMonitor:
             monitorIndex = 0
@@ -380,14 +392,18 @@
         query.data.upper().replace("CX", "X").replace("CB", "B").replace("CG", "G")
     )
     selection = preSelection.split("_")
     preSelection = f"{selection[0]}_{selection[1]}"
     if (selection[0].upper() not in TOP_LEVEL_SCANNER_MENUS):
         await start(update, context)
         return START_ROUTES
+    global bot_available
+    if not bot_available:
+        await start(update, context)
+        return START_ROUTES
     if selection[len(selection)-1].upper() == "H":
         await start(update, context)
         return START_ROUTES
     if len(selection) == 2 or (len(selection) == 3 and selection[2] == "P"):
         if str(selection[1]).isnumeric():
             # It's only level 2
             menuText = m2.renderForMenu(
@@ -960,15 +976,18 @@
         chat_id=int(f"-{Channel_Id}"), text=message, parse_mode=ParseMode.HTML
     )
 
 
 async def help_command(update: Update, context: ContextTypes.DEFAULT_TYPE) -> None:
     if _shouldAvoidResponse(update):
         return
-
+    global bot_available
+    if not bot_available:
+        await start(update, context)
+        return START_ROUTES
     cmds = m0.renderForMenu(
         selectedMenu=None,
         skip=TOP_LEVEL_SCANNER_SKIP_MENUS,
         asList=True,
         renderStyle=MenuRenderStyle.STANDALONE,
     )
     cmdText = ""
@@ -1114,18 +1133,19 @@
 #   context.bot.edit_message_text(
 #     chat_id=job.context.chat.id,
 #     text='NO ANSWER PROVIDED',
 #     message_id=job.context.message_id
 #   )
 
 
-def runpkscreenerbot() -> None:
+def runpkscreenerbot(availability=True) -> None:
     """Run the bot."""
     # Create the Application and pass it your bot's token.
-    global chat_idADMIN, Channel_Id
+    global chat_idADMIN, Channel_Id, bot_available
+    bot_available = availability
     Channel_Id, TOKEN, chat_idADMIN, GITHUB_TOKEN = get_secrets()
     # TOKEN = '1234567'
     # Channel_Id = 1001785195297
     application = Application.builder().token(TOKEN).build()
     # Setup conversation handler with the states FIRST and SECOND
     # Use the pattern parameter to pass CallbackQueries with specific
     # data pattern to the corresponding handlers.
@@ -1158,15 +1178,16 @@
     # application.add_handler(MessageHandler(filters.TEXT & filters.COMMAND, command_handler))
     # application.add_handler(MessageHandler(filters.COMMAND, command_handler))
     # Add ConversationHandler to application that will be used for handling updates
     addCommandsForMenuItems(application)
     application.add_handler(conv_handler)
     # ...and the error handler
     application.add_error_handler(error_handler)
-    # Run the intraday monitor
-    initializeIntradayTimer()
+    if bot_available:
+        # Run the intraday monitor
+        initializeIntradayTimer()
     # Run the bot until the user presses Ctrl-C
     application.run_polling(allowed_updates=Update.ALL_TYPES)
 
 
 if __name__ == "__main__":
     runpkscreenerbot()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pkscreener-0.45.20240521.396/pkscreener/pkscreenercli.py` & `pkscreener-0.45.20240522.398/pkscreener/pkscreenercli.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,20 @@
 argParser.add_argument(
     "--bot",
     action="store_true",
     help="Run only in telegram bot mode",
     required=False,
 )
 argParser.add_argument(
+    "--botavailable",
+    action="store_true",
+    help="Enforce whether bot is going to be available or not.",
+    required=False,
+)
+argParser.add_argument(
     "-c",
     "--croninterval",
     help="Pass interval in seconds to wait before the program is run again with same parameters",
     required=False,
 )
 argParser.add_argument(
     "-d",
@@ -669,15 +675,15 @@
         else:
             # It should have been launched only during the trading hours
             default_logger().info("--telegram option must be launched ONLY during NSE trading hours. Exiting now...")
             sys.exit(0)
     # Check and see if we're running only the telegram bot
     if args.bot:
         from pkscreener import pkscreenerbot
-        pkscreenerbot.runpkscreenerbot()
+        pkscreenerbot.runpkscreenerbot(availability=args.botavailable)
         return
     
     if args.intraday:
         configManager.toggleConfig(candleDuration=args.intraday, clearCache=False)
     else:
         configManager.toggleConfig(candleDuration='1d', clearCache=False)
     if args.options is not None:
```

### Comparing `pkscreener-0.45.20240521.396/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.45.20240522.398/pkscreener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.45.20240521.396
+Version: 0.45.20240522.398
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240521.396.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.45.20240522.398.zip
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
```

### Comparing `pkscreener-0.45.20240521.396/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.45.20240522.398/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.45.20240521.396/setup.py` & `pkscreener-0.45.20240522.398/setup.py`

 * *Files identical despite different names*

