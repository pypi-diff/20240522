# Comparing `tmp/koalafolio-0.9.2.tar.gz` & `tmp/koalafolio-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\koalafolio-0.9.2.tar", last modified: Fri Sep  4 11:17:19 2020, max compression
+gzip compressed data, was "dist\koalafolio-0.9.3.tar", last modified: Tue Sep  8 12:03:51 2020, max compression
```

## Comparing `koalafolio-0.9.2.tar` & `koalafolio-0.9.3.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/
--rw-rw-rw-   0        0        0      117 2019-04-07 08:37:15.000000 koalafolio-0.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2810 2020-09-04 11:17:19.000000 koalafolio-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0     1817 2019-10-02 14:30:53.000000 koalafolio-0.9.2/README.rst
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio/
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio/Import/
--rw-rw-rw-   0        0        0    46756 2020-09-04 09:32:04.000000 koalafolio-0.9.2/koalafolio/Import/Converter.py
--rw-rw-rw-   0        0        0    17203 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/Import/Models.py
--rw-rw-rw-   0        0        0    14573 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/Import/RegexPatterns.py
--rw-rw-rw-   0        0        0     5281 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/Import/TradeImporter.py
--rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/Import/__init__.py
--rw-rw-rw-   0        0        0     4655 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/Import/apiImport.py
--rw-rw-rw-   0        0        0    53978 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/KoalaIcon.png
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio/PcpCore/
--rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/PcpCore/__init__.py
--rw-rw-rw-   0        0        0    35925 2020-09-04 10:08:04.000000 koalafolio-0.9.2/koalafolio/PcpCore/core.py
--rw-rw-rw-   0        0        0     1852 2019-04-07 17:59:05.000000 koalafolio-0.9.2/koalafolio/PcpCore/logger.py
--rw-rw-rw-   0        0        0     5720 2020-03-01 11:14:36.000000 koalafolio-0.9.2/koalafolio/PcpCore/settings.py
--rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/__init__.py
--rw-rw-rw-   0        0        0      203 2019-04-07 17:59:05.000000 koalafolio-0.9.2/koalafolio/__main__.py
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio/exp/
--rw-rw-rw-   0        0        0     3340 2019-06-26 12:11:20.000000 koalafolio-0.9.2/koalafolio/exp/QTranslate.py
--rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/exp/__init__.py
--rw-rw-rw-   0        0        0    14095 2019-06-26 12:11:20.000000 koalafolio-0.9.2/koalafolio/exp/profitExport.py
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio/graphics/
--rw-rw-rw-   0        0        0     2787 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/graphics/delete.png
--rw-rw-rw-   0        0        0     4512 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/graphics/export.png
--rw-rw-rw-   0        0        0     4792 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/graphics/import.png
--rw-rw-rw-   0        0        0     2247 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/graphics/left.png
--rw-rw-rw-   0        0        0     4039 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/graphics/portfolio.png
--rw-rw-rw-   0        0        0     1954 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/graphics/right.png
--rw-rw-rw-   0        0        0     6353 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/graphics/settings.png
--rw-rw-rw-   0        0        0     4669 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/graphics/trades.png
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio/gui/
--rw-rw-rw-   0        0        0    15123 2019-10-26 19:13:52.000000 koalafolio-0.9.2/koalafolio/gui/QApiImport.py
--rw-rw-rw-   0        0        0    20495 2019-06-26 12:11:20.000000 koalafolio-0.9.2/koalafolio/gui/QCharts.py
--rw-rw-rw-   0        0        0     2789 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/gui/QLogger.py
--rw-rw-rw-   0        0        0    53924 2019-06-26 12:11:20.000000 koalafolio-0.9.2/koalafolio/gui/QPortfolioTable.py
--rw-rw-rw-   0        0        0    12147 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/gui/QSettings.py
--rw-rw-rw-   0        0        0    18317 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/gui/QStyle.py
--rw-rw-rw-   0        0        0     4441 2019-06-26 12:11:20.000000 koalafolio-0.9.2/koalafolio/gui/QThreads.py
--rw-rw-rw-   0        0        0    19131 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/gui/QTradeTable.py
--rw-rw-rw-   0        0        0    18536 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/gui/Qcontrols.py
--rw-rw-rw-   0        0        0    46341 2019-10-26 19:13:52.000000 koalafolio-0.9.2/koalafolio/gui/Qpages.py
--rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/gui/__init__.py
--rw-rw-rw-   0        0        0    17236 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/gui_root.py
--rw-rw-rw-   0        0        0    51526 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/koalaicon.ico
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio/web/
--rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.2/koalafolio/web/__init__.py
--rw-rw-rw-   0        0        0     4526 2019-04-10 21:02:28.000000 koalafolio-0.9.2/koalafolio/web/cryptocompare.py
--rw-rw-rw-   0        0        0     3316 2019-06-26 12:11:20.000000 koalafolio-0.9.2/koalafolio/web/cryptocompareApi.py
--rw-rw-rw-   0        0        0      903 2019-10-02 14:30:53.000000 koalafolio-0.9.2/koalafolio/web/krakenApi.py
-drwxrwxrwx   0        0        0        0 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio.egg-info/
--rw-rw-rw-   0        0        0     2810 2020-09-04 11:17:18.000000 koalafolio-0.9.2/koalafolio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1428 2020-09-04 11:17:19.000000 koalafolio-0.9.2/koalafolio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-09-04 11:17:18.000000 koalafolio-0.9.2/koalafolio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2020-09-04 11:17:18.000000 koalafolio-0.9.2/koalafolio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      119 2020-09-04 11:17:18.000000 koalafolio-0.9.2/koalafolio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2020-09-04 11:17:18.000000 koalafolio-0.9.2/koalafolio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-09-04 11:17:19.000000 koalafolio-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1111 2020-09-04 11:01:29.000000 koalafolio-0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/
+-rw-rw-rw-   0        0        0      117 2019-04-07 08:37:15.000000 koalafolio-0.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2810 2020-09-08 12:03:51.000000 koalafolio-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1817 2020-09-06 19:25:10.000000 koalafolio-0.9.3/README.rst
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio/
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio/Import/
+-rw-rw-rw-   0        0        0    46756 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/Import/Converter.py
+-rw-rw-rw-   0        0        0    17203 2020-09-06 19:21:26.000000 koalafolio-0.9.3/koalafolio/Import/Models.py
+-rw-rw-rw-   0        0        0    14573 2020-09-06 19:21:26.000000 koalafolio-0.9.3/koalafolio/Import/RegexPatterns.py
+-rw-rw-rw-   0        0        0     5281 2020-09-06 19:21:26.000000 koalafolio-0.9.3/koalafolio/Import/TradeImporter.py
+-rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/Import/__init__.py
+-rw-rw-rw-   0        0        0     4655 2020-09-06 19:21:26.000000 koalafolio-0.9.3/koalafolio/Import/apiImport.py
+-rw-rw-rw-   0        0        0    53978 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/KoalaIcon.png
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio/PcpCore/
+-rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/PcpCore/__init__.py
+-rw-rw-rw-   0        0        0    36080 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/PcpCore/core.py
+-rw-rw-rw-   0        0        0     1852 2019-04-07 17:59:05.000000 koalafolio-0.9.3/koalafolio/PcpCore/logger.py
+-rw-rw-rw-   0        0        0     7382 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/PcpCore/settings.py
+-rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/__init__.py
+-rw-rw-rw-   0        0        0      203 2019-04-07 17:59:05.000000 koalafolio-0.9.3/koalafolio/__main__.py
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio/exp/
+-rw-rw-rw-   0        0        0     3340 2019-06-26 12:11:20.000000 koalafolio-0.9.3/koalafolio/exp/QTranslate.py
+-rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/exp/__init__.py
+-rw-rw-rw-   0        0        0    14095 2019-06-26 12:11:20.000000 koalafolio-0.9.3/koalafolio/exp/profitExport.py
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio/graphics/
+-rw-rw-rw-   0        0        0     2787 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/graphics/delete.png
+-rw-rw-rw-   0        0        0     4512 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/graphics/export.png
+-rw-rw-rw-   0        0        0     4792 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/graphics/import.png
+-rw-rw-rw-   0        0        0     2247 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/graphics/left.png
+-rw-rw-rw-   0        0        0     4039 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/graphics/portfolio.png
+-rw-rw-rw-   0        0        0     1954 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/graphics/right.png
+-rw-rw-rw-   0        0        0     6353 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/graphics/settings.png
+-rw-rw-rw-   0        0        0     4669 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/graphics/trades.png
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio/gui/
+-rw-rw-rw-   0        0        0    15260 2020-09-07 10:04:06.000000 koalafolio-0.9.3/koalafolio/gui/QApiImport.py
+-rw-rw-rw-   0        0        0    20495 2019-06-26 12:11:20.000000 koalafolio-0.9.3/koalafolio/gui/QCharts.py
+-rw-rw-rw-   0        0        0     2789 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/gui/QLogger.py
+-rw-rw-rw-   0        0        0    54648 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/gui/QPortfolioTable.py
+-rw-rw-rw-   0        0        0    12889 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/gui/QSettings.py
+-rw-rw-rw-   0        0        0    18317 2020-09-06 19:21:26.000000 koalafolio-0.9.3/koalafolio/gui/QStyle.py
+-rw-rw-rw-   0        0        0     5107 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/gui/QThreads.py
+-rw-rw-rw-   0        0        0    19131 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/gui/QTradeTable.py
+-rw-rw-rw-   0        0        0    18536 2020-09-06 19:21:26.000000 koalafolio-0.9.3/koalafolio/gui/Qcontrols.py
+-rw-rw-rw-   0        0        0    47053 2020-09-06 19:39:52.000000 koalafolio-0.9.3/koalafolio/gui/Qpages.py
+-rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/gui/__init__.py
+-rw-rw-rw-   0        0        0    17236 2020-09-06 19:21:26.000000 koalafolio-0.9.3/koalafolio/gui_root.py
+-rw-rw-rw-   0        0        0    51526 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/koalaicon.ico
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio/web/
+-rw-rw-rw-   0        0        0        0 2019-04-07 08:37:15.000000 koalafolio-0.9.3/koalafolio/web/__init__.py
+-rw-rw-rw-   0        0        0     6777 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/web/coingeckoApi.py
+-rw-rw-rw-   0        0        0     4526 2019-04-10 21:02:28.000000 koalafolio-0.9.3/koalafolio/web/cryptocompare.py
+-rw-rw-rw-   0        0        0     3655 2020-09-06 19:25:10.000000 koalafolio-0.9.3/koalafolio/web/cryptocompareApi.py
+-rw-rw-rw-   0        0        0      903 2020-09-06 19:21:26.000000 koalafolio-0.9.3/koalafolio/web/krakenApi.py
+drwxrwxrwx   0        0        0        0 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio.egg-info/
+-rw-rw-rw-   0        0        0     2810 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1459 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      131 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2020-09-08 12:03:51.000000 koalafolio-0.9.3/koalafolio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-09-08 12:03:51.000000 koalafolio-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2020-09-06 19:25:10.000000 koalafolio-0.9.3/setup.py
```

### Comparing `koalafolio-0.9.2/PKG-INFO` & `koalafolio-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koalafolio
-Version: 0.9.2
+Version: 0.9.3
 Summary: portfolio app for crypto trading and tax reporting
 Home-page: https://github.com/2martin2/pycryptoportfolio
 Author: 2martin2
 Author-email: 2martin2@protonmail.com
 License: GPL-3.0
 Description: pycryptoportfolio
         ******************
```

### Comparing `koalafolio-0.9.2/README.rst` & `koalafolio-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/Import/Converter.py` & `koalafolio-0.9.3/koalafolio/Import/Converter.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/Import/Models.py` & `koalafolio-0.9.3/koalafolio/Import/Models.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/Import/RegexPatterns.py` & `koalafolio-0.9.3/koalafolio/Import/RegexPatterns.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/Import/TradeImporter.py` & `koalafolio-0.9.3/koalafolio/Import/TradeImporter.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/Import/apiImport.py` & `koalafolio-0.9.3/koalafolio/Import/apiImport.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/KoalaIcon.png` & `koalafolio-0.9.3/koalafolio/KoalaIcon.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/PcpCore/core.py` & `koalafolio-0.9.3/koalafolio/PcpCore/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,18 +89,18 @@
 
     # return length of values
     def __len__(self):
         return len(self.value)
 
     # get item using []
     def __getitem__(self, key):
-        return self.value[key]
+        return self.value[key.upper()]
 
     def __setitem__(self, key, value):
-        self.value[key] = value
+        self.value[key.upper()] = value
 
     def __lt__(self, other):
         val = 1
         for key in self.value:
             if key in other.value and self.value[key] != 0 and other.value[key] != 0:
                 val *= self.value[key]/other.value[key]
         return val < 1
@@ -153,17 +153,22 @@
     # sub another CoinValue and return a new object
     def __sub__(self, other):
         return self.copy().sub(other)
 
     def fromDict(self, dictionary):
         for key in self.value:
             try:
-                self.value[key] = dictionary[key]
+                self.value[key] = dictionary[key.upper()]
             except KeyError:
                 pass
+            try:
+                self.value[key] = dictionary[key.lower()]
+            except KeyError:
+                pass
+
         return self
 
     # set value of all CoinValues
     def setValue(self, value):
         for key in self.value:
             self.value[key] = value
         return self
```

### Comparing `koalafolio-0.9.2/koalafolio/PcpCore/logger.py` & `koalafolio-0.9.3/koalafolio/PcpCore/logger.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/PcpCore/settings.py` & `koalafolio-0.9.3/koalafolio/PcpCore/settings.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,31 +31,34 @@
             self.saveSettings()
         return self
 
     def initSettings(self):
         # set default settings
         # general settings
         self['general'] = {}
-        self['general']['version'] = '0.9.2'
+        self['general']['version'] = '0.9.3'
         self['general']['timeModeDaywise'] = 'True'
         self['general']['priceUpdateInterval(s)'] = '100'
+        self['general']['priceApiSwitch(cryptocompare/coingecko/mixed)'] = 'mixed'
         # proxy settings
         self['proxies'] = {}
         self['proxies']['http'] = ''
         self['proxies']['https'] = ''
         # import settings
         self['import'] = {}
         self['import']['ignoreTradeIDs'] = 'False'
         self['import']['importFileTypes'] = '(csv|txt|xlsx|xlsm|xls|json)'
         # coin settings
         self['currency'] = {}
         self['currency']['defaultReportCurrency'] = 'EUR'
         self['currency']['defaultDisplayCurrencies'] = 'EUR,USD,BTC'
         self['currency']['isFiat'] = 'EUR,USD,GBP,JPY,CNY,RUB,AUD,CAD,SGD,PLN,HKD,CHF,INR,BRL,KRW,NZD,ZAR'
         self['currency']['coinswapdict'] = "{'HOT':'HOLO','HOT*':'HOLO','XBT':'BTC','IOT':'MIOTA','IOTA':'MIOTA'}"
+        self['currency']['coinswapdictcryptocompareapi'] = "{'HOT':'HOLO','HOT*':'HOLO','XBT':'BTC','IOT':'MIOTA','IOTA':'MIOTA'}"
+        self['currency']['coinswapdictcoingeckoapi'] = "{'HOLO':'HOT','HOT*':'HOT','XBT':'BTC','IOT':'MIOTA','IOTA':'MIOTA','SAFEX':'SFT'}"
         # tax settings
         self['tax'] = {}
         self['tax']['taxfreelimit'] = 'True'
         self['tax']['taxfreelimityears'] = '1'
         self['tax']['exportLanguage'] = 'en'
 
     def saveSettings(self):
@@ -67,15 +70,15 @@
         except Exception as ex:
             logger.globalLogger.error('error in saveSettings: ' + str(ex))
             return False
 
     def readSettings(self):
         try:
             self.read(self.filePath)
-            self['general']['version'] = '0.9.2'
+            self['general']['version'] = '0.9.3'
             logger.globalLogger.info('settings loaded')
         except Exception as ex:
             logger.globalLogger.error('settings can not be loaded: ' + str(ex))
             self.resetDefault()
 
     def resetDefault(self):
         try:
@@ -90,32 +93,36 @@
     def timeModeDaywise(self):
         return self.getboolean('general', 'timeModeDaywise')
 
     def priceUpdateInterval(self):
         priceUpdateInterval = self.getfloat('general', 'priceUpdateInterval(s)')
         return 2 if priceUpdateInterval <= 2 else priceUpdateInterval
 
+    def priceApiSwitch(self):
+        return self['general']['priceApiSwitch(cryptocompare/coingecko/mixed)']
+
     def proxies(self):
         if self['proxies']['http'] and self['proxies']['https']:
             return {'http': self['proxies']['http'], 'https': self['proxies']['https']}
         return {}
 
     def ignoreTradeIds(self):
         return self.getboolean('import', 'ignoreTradeIDs')
 
     def displayCurrencies(self):
-        return self['currency']['defaultDisplayCurrencies'].split(',')
+        return self['currency']['defaultDisplayCurrencies'].upper().split(',')
     
     def setDisplayCurrencies(self, currencies):
         self['currency']['defaultDisplayCurrencies'] = ','.join(currencies)
 
     def reportCurrency(self):
         # report currency should be included in display currencies, otherwise prices are not available
         if self['currency']['defaultReportCurrency'] in self.displayCurrencies():
             return self['currency']['defaultReportCurrency']
+        logger.globalLogger.warning('defaultReportCurrency is not part of defaultDisplayCurrencies. First displayCurrency will be used for reports.')
         return self.displayCurrencies()[0]
 
     def setReportCurrency(self, cur):
         if cur in self.displayCurrencies():
             self['currency']['defaultReportCurrency'] = cur
 
     def fiatList(self):
@@ -125,18 +132,38 @@
         self['currency']['isFiat'] = ','.join(fiatList)
 
     def coinSwapDict(self):
         try:
             if dictRegex.match(self['currency']['coinswapdict']):
                 return ast.literal_eval(self['currency']['coinswapdict'])
             else:
-                raise SyntaxError('coinSwapList in settings.txt has invalid Syntax')
+                raise SyntaxError('coinswapdict in settings.txt has invalid Syntax')
         except Exception as ex:
-            return dict()
             logger.globalLogger.warning('error while parsing coinswapdict from settings: ' + str(ex))
+        return dict()
+
+    def coinSwapDictCryptocompare(self):
+        try:
+            if dictRegex.match(self['currency']['coinswapdictcryptocompareapi']):
+                return ast.literal_eval(self['currency']['coinswapdictcryptocompareapi'])
+            else:
+                raise SyntaxError('coinswapdictcryptocompareapi in settings.txt has invalid Syntax')
+        except Exception as ex:
+            logger.globalLogger.warning('error while parsing coinswapdictcryptocompareapi from settings: ' + str(ex))
+        return dict()
+
+    def coinSwapDictCoinGecko(self):
+        try:
+            if dictRegex.match(self['currency']['coinswapdictcoingeckoapi']):
+                return ast.literal_eval(self['currency']['coinswapdictcoingeckoapi'])
+            else:
+                raise SyntaxError('coinswapdictcoingeckoapi in settings.txt has invalid Syntax')
+        except Exception as ex:
+            logger.globalLogger.warning('error while parsing coinswapdictcoingeckoapi from settings: ' + str(ex))
+        return dict()
 
     def taxSettings(self):
         tax = {}
         try:
             tax['taxfreelimit'] = self.getboolean('tax', 'taxfreelimit')
         except ValueError:
             tax['taxfreelimit'] = True
```

### Comparing `koalafolio-0.9.2/koalafolio/exp/QTranslate.py` & `koalafolio-0.9.3/koalafolio/exp/QTranslate.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/exp/profitExport.py` & `koalafolio-0.9.3/koalafolio/exp/profitExport.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/graphics/delete.png` & `koalafolio-0.9.3/koalafolio/graphics/delete.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/graphics/export.png` & `koalafolio-0.9.3/koalafolio/graphics/export.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/graphics/import.png` & `koalafolio-0.9.3/koalafolio/graphics/import.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/graphics/left.png` & `koalafolio-0.9.3/koalafolio/graphics/left.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/graphics/portfolio.png` & `koalafolio-0.9.3/koalafolio/graphics/portfolio.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/graphics/right.png` & `koalafolio-0.9.3/koalafolio/graphics/right.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/graphics/settings.png` & `koalafolio-0.9.3/koalafolio/graphics/settings.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/graphics/trades.png` & `koalafolio-0.9.3/koalafolio/graphics/trades.png`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/gui/QApiImport.py` & `koalafolio-0.9.3/koalafolio/gui/QApiImport.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,17 @@
 
     def unlockDb(self):
         pw = self.pwInput.text()
         self.model.unlockDatabase(pw)
 
     def lockDb(self):
         self.pwInput.clear()
+        self.keyInput.clear()
+        self.secretInput.clear()
+        self.apiSelectDropdown.clear()
         self.model.lockDatabase()
 
     def deleteDatabase(self):
         self.deleteDbButton.setDisabled(True)
         self.deleteDbButtonEnableBox.setCheckState(False)
         self.model.deleteDatabase()
 
@@ -349,15 +352,16 @@
                 self.keyInput.setText(key)
                 self.secretInput.setText(secret)
 
     def saveKeys(self):
         apiname = self.directApiSelectDropdown.currentText()
         key = self.keyInput.text()
         secret = self.secretInput.text()
-        self.model.addKeys(self.pwInput.text(), apiname, key, secret)
+        if key and secret:
+            self.model.addKeys(self.pwInput.text(), apiname, key, secret)
 
     def deleteKeys(self):
         apiname = self.apiSelectDropdown.currentText()
         self.model.deleteKeys(self.pwInput.text(), apiname)
 
     def deleteDbButtonEnableBoxChanged(self, state):
         if state:
```

### Comparing `koalafolio-0.9.2/koalafolio/gui/QCharts.py` & `koalafolio-0.9.3/koalafolio/gui/QCharts.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/gui/QLogger.py` & `koalafolio-0.9.3/koalafolio/gui/QLogger.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/gui/QPortfolioTable.py` & `koalafolio-0.9.3/koalafolio/gui/QPortfolioTable.py`

 * *Files 1% similar despite different names*

```diff
@@ -412,14 +412,27 @@
             coinBalance2, key2, cols2 = index2.data()
             if cols1 >= 2:
                 return coinBalance1.getCurrentValue()[key1] < coinBalance2.getCurrentValue()[key2]
             else:
                 return coinBalance1.getChange24h(key1) < coinBalance2.getChange24h(key2)
         return index1.data() < index2.data()
 
+    def filterAcceptsRow(self, source_row, source_parent):
+        if settings.mySettings.getGuiSetting('hideLowBalanceCoins'):
+            index = self.sourceModel().index(source_row, 1, source_parent)
+            data = self.sourceModel().data(index)
+            if data.balance <= 0:
+                return False
+        if settings.mySettings.getGuiSetting('hideLowValueCoins'):
+            index = self.sourceModel().index(source_row, 1, source_parent)
+            data = self.sourceModel().data(index)
+            if data.getCurrentValue()[settings.mySettings.reportCurrency()] <= settings.mySettings.getGuiSetting('lowValueFilterLimit(reportCurrency)'):
+                return False
+        return True
+
 # %% portfolio table delegate
 # class QCoinBalanceDelegate(qtwidgets.QStyledItemDelegate):
 class QCoinTableDelegate(qtwidgets.QStyledItemDelegate):
     def __init__(self, *args, **kwargs):
         super(QCoinTableDelegate, self).__init__(*args, **kwargs)
 
         self.marginV = 4  # vertical margin
```

### Comparing `koalafolio-0.9.2/koalafolio/gui/QSettings.py` & `koalafolio-0.9.3/koalafolio/gui/QSettings.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,14 +50,17 @@
         self['gui']['portfolioFilterRow'] = '3'
         self['gui']['tradeFilterRow'] = '2'
         self['gui']['portfolioFilterDir'] = (str(qt.DescendingOrder))
         self['gui']['tradeFilterDir'] = str(qt.AscendingOrder)
         self['gui']['toolTipsEnabled'] = 'True'
         self['gui']['performanceChartIndex'] = '0'
         self['gui']['tradesEditLock'] = 'True'
+        self['gui']['hideLowBalanceCoins'] = 'True'
+        self['gui']['hideLowValueCoins'] = 'False'
+        self['gui']['lowValueFilterLimit(reportCurrency)'] = '50'
 
         super(QSettings, self).initSettings()
 
     def getWindowProperties(self):
         windowProperties = {}
         try:
             size = [int(s) for s in self['window']['windowsize'].split('x')]
@@ -148,14 +151,26 @@
             gui['performanceChartIndex'] = self.getint('gui', 'performanceChartIndex')
         except ValueError:
             gui['performanceChartIndex'] = 0
         try:
             gui['tradesEditLock'] = self.getboolean('gui', 'tradesEditLock')
         except ValueError:
             gui['tradesEditLock'] = True
+        try:
+            gui['hideLowBalanceCoins'] = self.getboolean('gui', 'hideLowBalanceCoins')
+        except ValueError:
+            gui['hideLowBalanceCoins'] = True
+        try:
+            gui['hideLowValueCoins'] = self.getboolean('gui', 'hideLowValueCoins')
+        except ValueError:
+            gui['hideLowValueCoins'] = False
+        try:
+            gui['lowValueFilterLimit(reportCurrency)'] = self.getfloat('gui', 'lowValueFilterLimit(reportCurrency)')
+        except ValueError:
+            gui['lowValueFilterLimit(reportCurrency)'] = 50
         return gui
 
     def getGuiSetting(self, key):
         return self.getGuiSettings()[key]
 
     def setGuiSettings(self, gui):
         for key in gui:
```

### Comparing `koalafolio-0.9.2/koalafolio/gui/QStyle.py` & `koalafolio-0.9.3/koalafolio/gui/QStyle.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/gui/QThreads.py` & `koalafolio-0.9.3/koalafolio/gui/QThreads.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @author: Martin
 """
 import PyQt5.QtGui as qtgui
 import PyQt5.QtWidgets as qtwidgets
 import PyQt5.QtCore as qtcore
 import koalafolio.gui.QSettings as settings
 import koalafolio.web.cryptocompareApi as ccapi
+import koalafolio.web.coingeckoApi as coinGecko
 import koalafolio.PcpCore.core as core
 from PIL.ImageQt import ImageQt
 import koalafolio.gui.QLogger as logger
 
 localLogger = logger.globalLogger
 
 
@@ -26,30 +27,39 @@
         super(CryptoCompare, self).__init__()
 
         # self.histPrices = {}
         self.tradeBuffer = core.TradeList()
 
     def loadPrices(self, coins):
         if coins:
-            prices = ccapi.getCoinPrices(coins)
+            if settings.mySettings.priceApiSwitch() == 'coinGecko':
+                prices = coinGecko.getCoinPrices(coins)
+            else:
+                prices = ccapi.getCoinPrices(coins)
+
             self.coinPricesLoaded.emit(prices)
 
     def loadCoinIcons(self, coins):
         if coins:
-            icons = ccapi.getIcons(coins)
+            if settings.mySettings.priceApiSwitch() == 'coinGecko':
+                icons = coinGecko.getIcons(coins)
+            else:
+                icons = ccapi.getIcons(coins)
             qicons = {}
             for key in coins:  # convert images to QIcon
                 try:
                     if icons[key]:
                         im = icons[key].convert("RGBA")
                         qim = ImageQt(im)
                         qpix = qtgui.QPixmap.fromImage(qim)
                         qicons[key] = qtgui.QIcon(qpix)
-                except:
+                except KeyError:
                     localLogger.warning('no icon available for ' + key)  # ignore invalid key
+                except Exception as ex:
+                    localLogger.error('error converting icon: ' + str(ex))
             self.coinIconsLoaded.emit(qicons)
 
     def loadHistoricalPrices(self, tradeList):
         newTrades = False
         # copy trades to buffer
         for trade in tradeList:
             if not trade.valueLoaded:
@@ -58,15 +68,18 @@
                     newTrades = True
         histPrices = {}
         counter = 0
         while not self.tradeBuffer.isEmpty():
             trade = self.tradeBuffer.trades.pop()
             try:
                 if not trade.valueLoaded:
-                    histPrices[trade.tradeID] = ccapi.getHistoricalPrice(trade)
+                    if settings.mySettings.priceApiSwitch() == 'coinGecko':
+                        histPrices[trade.tradeID] = coinGecko.getHistoricalPrice(trade)
+                    else:
+                        histPrices[trade.tradeID] = ccapi.getHistoricalPrice(trade)
                     counter += 1
             except ConnectionRefusedError:
                 # save failed trade for next time
                 trade.tradeBuffer.append(trade)
                 # stop here and retry next time
                 break
             if counter >= 100:
```

### Comparing `koalafolio-0.9.2/koalafolio/gui/QTradeTable.py` & `koalafolio-0.9.3/koalafolio/gui/QTradeTable.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/gui/Qcontrols.py` & `koalafolio-0.9.3/koalafolio/gui/Qcontrols.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/gui/Qpages.py` & `koalafolio-0.9.3/koalafolio/gui/Qpages.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,15 +217,19 @@
         super(ImportPage, self).__init__(parent=parent, controller=controller)
 
         self.initData()
 
         # %%  stacked Layout for import pages
         self.importSelectPage = ImportSelectPage(parent=self, controller=self)
         self.importPreviewPage = ImportPreviewPage(parent=self, controller=self)
+        self.controller.startRefresh.connect(self.importPreviewPage.clearLabelStyle)
+        self.controller.endRefresh.connect(self.importPreviewPage.setLabelStyle)
         self.importFinishPage = ImportFinishPage(parent=self, controller=self)
+        self.controller.startRefresh.connect(self.importFinishPage.clearLabelStyle)
+        self.controller.endRefresh.connect(self.importFinishPage.setLabelStyle)
         self.pages = [self.importSelectPage, self.importPreviewPage, self.importFinishPage]
         self.stackedContentLayout = qtwidgets.QStackedLayout(self)
         for page in self.pages:
             # stacked content layout
             self.stackedContentLayout.addWidget(page)
 
         self.refresh()
@@ -524,22 +528,18 @@
         self.fileNameLabel = qtwidgets.QLabel("FileName", self.infoFrame)
         self.infoLabel = qtwidgets.QLabel("", self.infoFrame)
 
         self.infoLayout = qtwidgets.QHBoxLayout(self.infoFrame)
         self.infoLayout.addWidget(self.fileNameLabel)
         self.infoLayout.addSpacerItem(qtwidgets.QSpacerItem(10, 10))
         self.infoLayout.addWidget(self.infoLabel)
-
         self.legendWhiteLabel = qtwidgets.QLabel("white: new trades", self)
         self.legendGrayLabel = qtwidgets.QLabel("gray: trades that are already existent", self)
-        color = style.myStyle.getQColor('TEXT_HIGHLIGHTED_MIDLIGHT')
-        self.legendGrayLabel.setStyleSheet('QLabel {color: ' + color.name() + '}')
         self.legendRedLabel = qtwidgets.QLabel("red: new trades that are very similar to existent trades (make sure you really want to import them!)", self)
-        color = style.myStyle.getQColor('NEGATIV')
-        self.legendRedLabel.setStyleSheet('QLabel {color: ' + color.name() + '}')
+        self.setLabelStyle()
 
         self.legendLayout = qtwidgets.QHBoxLayout()
         self.legendLayout.addWidget(self.legendWhiteLabel)
         self.legendLayout.addSpacerItem(qtwidgets.QSpacerItem(10, 10))
         self.legendLayout.addWidget(self.legendGrayLabel)
         self.legendLayout.addSpacerItem(qtwidgets.QSpacerItem(10, 10))
         self.legendLayout.addWidget(self.legendRedLabel)
@@ -672,14 +672,24 @@
         else:
             self.controller.showFrame(self.controller.IMPORTSELECTPAGEINDEX)
 
     def exchangeChanged(self):
         self.tradeListTemp.setExchange(self.exchangeInput.text())
         self.feeListTemp.setExchange(self.exchangeInput.text())
 
+    def clearLabelStyle(self):
+        self.legendGrayLabel.setStyleSheet("")
+        self.legendRedLabel.setStyleSheet("")
+
+    def setLabelStyle(self):
+        color = style.myStyle.getQColor('TEXT_HIGHLIGHTED_MIDLIGHT')
+        self.legendGrayLabel.setStyleSheet('QLabel {color: ' + color.name() + '}')
+        color = style.myStyle.getQColor('NEGATIV')
+        self.legendRedLabel.setStyleSheet('QLabel {color: ' + color.name() + '}')
+
 
 class ImportFinishPage(SubPage):
     def __init__(self, parent, controller):
         super(ImportFinishPage, self).__init__(parent=parent, controller=controller)
 
         self.statusLabel = qtwidgets.QLabel('status', self)
 
@@ -709,19 +719,16 @@
         self.horzButtonLayout.addWidget(self.cancelButton)
         self.horzButtonLayout.addWidget(self.removeSelectButton)
         self.horzButtonLayout.addWidget(self.acceptButton)
         self.horzButtonLayout.addStretch()
 
         self.legendWhiteLabel = qtwidgets.QLabel("white: new trades", self)
         self.legendGrayLabel = qtwidgets.QLabel("gray: trades that are already existent (will not be imported)", self)
-        color = style.myStyle.getQColor('TEXT_HIGHLIGHTED_MIDLIGHT')
-        self.legendGrayLabel.setStyleSheet('QLabel {color: ' + color.name() + '}')
         self.legendRedLabel = qtwidgets.QLabel("red: new trades that are very similar to existent trades (make sure you really want to import them!)", self)
-        color = style.myStyle.getQColor('NEGATIV')
-        self.legendRedLabel.setStyleSheet('QLabel {color: ' + color.name() + '}')
+        self.setLabelStyle()
 
         self.legendLayout = qtwidgets.QHBoxLayout()
         self.legendLayout.addWidget(self.legendWhiteLabel)
         self.legendLayout.addSpacerItem(qtwidgets.QSpacerItem(10, 10))
         self.legendLayout.addWidget(self.legendGrayLabel)
         self.legendLayout.addSpacerItem(qtwidgets.QSpacerItem(10, 10))
         self.legendLayout.addWidget(self.legendRedLabel)
@@ -758,19 +765,28 @@
         # merge trades with database
         self.controller.finishImport()
 
     def deleteSelectedTrades(self):
         # remove all trades that are not selected
         self.lastFocusTable.deleteSelectedTrades()
 
-
     def cancelTrades(self):
         # delete trades and go back to file selection
         self.controller.showFrame(self.controller.IMPORTSELECTPAGEINDEX)
 
+    def clearLabelStyle(self):
+        self.legendGrayLabel.setStyleSheet("")
+        self.legendRedLabel.setStyleSheet("")
+
+    def setLabelStyle(self):
+        color = style.myStyle.getQColor('TEXT_HIGHLIGHTED_MIDLIGHT')
+        self.legendGrayLabel.setStyleSheet('QLabel {color: ' + color.name() + '}')
+        color = style.myStyle.getQColor('NEGATIV')
+        self.legendRedLabel.setStyleSheet('QLabel {color: ' + color.name() + '}')
+
 
 # %% export page for exporting csv, txt, xls ...
 class ExportPage(Page):
     def __init__(self, parent, controller):
         super(ExportPage, self).__init__(parent=parent, controller=controller)
 
         self.fileDialog = qtwidgets.QFileDialog(self)
```

### Comparing `koalafolio-0.9.2/koalafolio/gui_root.py` & `koalafolio-0.9.3/koalafolio/gui_root.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/koalaicon.ico` & `koalafolio-0.9.3/koalafolio/koalaicon.ico`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/web/cryptocompare.py` & `koalafolio-0.9.3/koalafolio/web/cryptocompare.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio/web/cryptocompareApi.py` & `koalafolio-0.9.3/koalafolio/web/cryptocompareApi.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import koalafolio.PcpCore.core as core
 import koalafolio.PcpCore.settings as settings
 import time
 import koalafolio.PcpCore.logger as logger
 from PIL import Image
 from io import BytesIO
 import requests
+import koalafolio.web.coingeckoApi as coinGecko
 
 
 # coinList = cryptcomp.get_coin_list(format=True)
 #
 # price = cryptcomp.get_price(['BTC', 'ETH', 'EOS'], ['USD','EUR','BTC'])
 #
 # pricehist = cryptcomp.get_historical_price('ETH', ['USD','EUR','BTC'], datetime.datetime(2017,6,6))
@@ -61,26 +62,32 @@
 def getIcon(coin, *args, **kwargs):
     if settings.mySettings.proxies():
         proxies = settings.mySettings.proxies()
     else:
         proxies = {}
     coinInfo = cryptcomp.get_coin_general_info(coin, *args, **kwargs)
     try:
-        imageResponse = requests.get(cryptcomp.URL_CRYPTOCOMPARE + coinInfo['Data'][0]['CoinInfo']['ImageUrl'], proxies=proxies, timeout=10)
-    except:
+        imageResponse = requests.get(cryptcomp.URL_CRYPTOCOMPARE + coinInfo['Data'][0]['CoinInfo']['ImageUrl'], proxies=proxies, timeout=100)
+    except Exception as ex:
+        logger.globalLogger.warning('error in getIcon: ' + str(ex))
         return None
     return Image.open(BytesIO(imageResponse.content))
 
 def getIcons(coins, *args, **kwargs):
     if settings.mySettings.proxies():
         proxies = settings.mySettings.proxies()
     else:
         proxies = {}
     coinInfo = cryptcomp.get_coin_general_info(coins, *args, **kwargs)
-    icons = {}
+    if settings.mySettings.priceApiSwitch() == 'mixed':
+        icons = coinGecko.getIcons(coins)
+    else:
+        icons = {}
     try:
         for data in coinInfo['Data']:
-            imageResponse = requests.get(cryptcomp.URL_CRYPTOCOMPARE + data['CoinInfo']['ImageUrl'], proxies=proxies, timeout=10)
-            icons[data['CoinInfo']['Name']] = Image.open(BytesIO(imageResponse.content))
+            coin = data['CoinInfo']['Name']
+            if coin not in icons:
+                imageResponse = requests.get(cryptcomp.URL_CRYPTOCOMPARE + data['CoinInfo']['ImageUrl'], proxies=proxies, timeout=100)
+                icons[data['CoinInfo']['Name']] = Image.open(BytesIO(imageResponse.content))
     except Exception as ex:
         logger.globalLogger.warning('error in getIcons: ' + str(ex))
     return icons
```

### Comparing `koalafolio-0.9.2/koalafolio/web/krakenApi.py` & `koalafolio-0.9.3/koalafolio/web/krakenApi.py`

 * *Files identical despite different names*

### Comparing `koalafolio-0.9.2/koalafolio.egg-info/PKG-INFO` & `koalafolio-0.9.3/koalafolio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koalafolio
-Version: 0.9.2
+Version: 0.9.3
 Summary: portfolio app for crypto trading and tax reporting
 Home-page: https://github.com/2martin2/pycryptoportfolio
 Author: 2martin2
 Author-email: 2martin2@protonmail.com
 License: GPL-3.0
 Description: pycryptoportfolio
         ******************
```

### Comparing `koalafolio-0.9.2/koalafolio.egg-info/SOURCES.txt` & `koalafolio-0.9.3/koalafolio.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,10 +41,11 @@
 koalafolio/gui/QStyle.py
 koalafolio/gui/QThreads.py
 koalafolio/gui/QTradeTable.py
 koalafolio/gui/Qcontrols.py
 koalafolio/gui/Qpages.py
 koalafolio/gui/__init__.py
 koalafolio/web/__init__.py
+koalafolio/web/coingeckoApi.py
 koalafolio/web/cryptocompare.py
 koalafolio/web/cryptocompareApi.py
 koalafolio/web/krakenApi.py
```

