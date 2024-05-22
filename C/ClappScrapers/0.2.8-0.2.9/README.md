# Comparing `tmp/ClappScrapers-0.2.8.tar.gz` & `tmp/ClappScrapers-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ClappScrapers-0.2.8.tar", last modified: Thu Feb  1 08:52:05 2024, max compression
+gzip compressed data, was "ClappScrapers-0.2.9.tar", last modified: Thu Feb  1 09:49:50 2024, max compression
```

## Comparing `ClappScrapers-0.2.8.tar` & `ClappScrapers-0.2.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.020435 ClappScrapers-0.2.8/ClappScrapers/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.020435 ClappScrapers-0.2.8/ClappScrapers/den_rental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/den_rental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.020435 ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/boligportalspider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.020435 ClappScrapers-0.2.8/ClappScrapers/fin_rental/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/fin_rental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/finlandrentalspider.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/ClappScrapers/funda_scraper/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/funda_scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/ClappScrapers/funda_scraper/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/funda_scraper/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/funda_scraper/config/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/funda_scraper/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/funda_scraper/scrape.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/funda_scraper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/
--rw-r--r--   0 runner    (1001) docker     (127)    12527 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/Nieuwbouwspider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/items.py
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/middlewares.py
--rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/ClappScrapers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-01 08:52:05.000000 ClappScrapers-0.2.8/ClappScrapers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-01 08:52:05.000000 ClappScrapers-0.2.8/ClappScrapers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 08:52:05.000000 ClappScrapers-0.2.8/ClappScrapers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-01 08:52:05.000000 ClappScrapers-0.2.8/ClappScrapers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-01 08:52:05.000000 ClappScrapers-0.2.8/ClappScrapers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 08:52:05.024435 ClappScrapers-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-01 08:51:51.000000 ClappScrapers-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.482446 ClappScrapers-0.2.9/ClappScrapers/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.482446 ClappScrapers-0.2.9/ClappScrapers/den_rental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/den_rental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/boligportalspider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/ClappScrapers/fin_rental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/fin_rental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/finlandrentalspider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/ClappScrapers/funda_scraper/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/funda_scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/ClappScrapers/funda_scraper/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/funda_scraper/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/funda_scraper/config/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6862 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/funda_scraper/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/funda_scraper/scrape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/funda_scraper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/Nieuwbouwspider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/middlewares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6216 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/ClappScrapers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-01 09:49:50.000000 ClappScrapers-0.2.9/ClappScrapers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-01 09:49:50.000000 ClappScrapers-0.2.9/ClappScrapers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-01 09:49:50.000000 ClappScrapers-0.2.9/ClappScrapers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-01 09:49:50.000000 ClappScrapers-0.2.9/ClappScrapers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-01 09:49:50.000000 ClappScrapers-0.2.9/ClappScrapers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-01 09:49:50.486446 ClappScrapers-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-01 09:49:38.000000 ClappScrapers-0.2.9/setup.py
```

### Comparing `ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/boligportalspider.py` & `ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/boligportalspider.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/extension.py` & `ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/extension.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/middlewares.py` & `ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/middlewares.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/pipelines.py` & `ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/pipelines.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/den_rental/spider/settings.py` & `ClappScrapers-0.2.9/ClappScrapers/den_rental/spider/settings.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/extension.py` & `ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/extension.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/finlandrentalspider.py` & `ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/finlandrentalspider.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/middlewares.py` & `ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/middlewares.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/pipelines.py` & `ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/pipelines.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/fin_rental/spider/settings.py` & `ClappScrapers-0.2.9/ClappScrapers/fin_rental/spider/settings.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/funda_scraper/preprocess.py` & `ClappScrapers-0.2.9/ClappScrapers/funda_scraper/preprocess.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/funda_scraper/scrape.py` & `ClappScrapers-0.2.9/ClappScrapers/funda_scraper/scrape.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/funda_scraper/utils.py` & `ClappScrapers-0.2.9/ClappScrapers/funda_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/Nieuwbouwspider.py` & `ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/Nieuwbouwspider.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,15 @@
 
 
                             house_info ={
                                  
                                 'house_source':response.url,
                                 'bouwnummer':clean_text(house.css('td')[0].get()) if len(house.css('td')) > 0 else None,
                                 'prijs':clean_text(house.css('td')[1].get()) if len(house.css('td')) > 1 else None,
+                                'prijs_conditie':'V.O.N',
                                 'kaveloppervlak':'' if clean_text(house.css('td')[2].get()) == "" else clean_text(house.css('td')[2].get()) if len(house.css('td')) > 2 else None,
                                 'woonoppervlak':clean_text(house.css('td')[3].get()) if len(house.css('td')) > 3 else None,
                                 'slaapkamer':clean_text(house.css('td')[4].get()) if len(house.css('td')) > 4 else None,
                                 'inhoud':clean_text(house.css('td')[5].get()) if len(house.css('td')) > 5 else None,
                                 'status':clean_text(house.css('td')[6].get()) if len(house.css('td')) > 6 else None,  
                                         
                             }
```

### Comparing `ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/extension.py` & `ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/extension.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/middlewares.py` & `ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/middlewares.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/pipelines.py` & `ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/pipelines.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers/nieuwbouw/spider/settings.py` & `ClappScrapers-0.2.9/ClappScrapers/nieuwbouw/spider/settings.py`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/ClappScrapers.egg-info/PKG-INFO` & `ClappScrapers-0.2.9/ClappScrapers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ClappScrapers
-Version: 0.2.8
+Version: 0.2.9
 Summary: Clappform Python scraper
 Home-page: https://github.com/ClappFormOrg/clappform-scraper
 Author: Clappform B.V.
 Author-email: info@clappform.com
 License: MIT
 Keywords: scraper
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ClappScrapers-0.2.8/ClappScrapers.egg-info/SOURCES.txt` & `ClappScrapers-0.2.9/ClappScrapers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/LICENSE` & `ClappScrapers-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ClappScrapers-0.2.8/PKG-INFO` & `ClappScrapers-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ClappScrapers
-Version: 0.2.8
+Version: 0.2.9
 Summary: Clappform Python scraper
 Home-page: https://github.com/ClappFormOrg/clappform-scraper
 Author: Clappform B.V.
 Author-email: info@clappform.com
 License: MIT
 Keywords: scraper
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ClappScrapers-0.2.8/setup.py` & `ClappScrapers-0.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
     
 
 setuptools.setup(
     name="ClappScrapers",
-    version="0.2.8",
+    version="0.2.9",
     description="Clappform Python scraper",
     author = "Clappform B.V.",
     author_email = "info@clappform.com",
     long_description=readme(),
     long_description_content_type="text/markdown",
 
     license="MIT",
```

