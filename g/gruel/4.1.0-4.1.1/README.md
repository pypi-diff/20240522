# Comparing `tmp/gruel-4.1.0.tar.gz` & `tmp/gruel-4.1.1.tar.gz`

## Comparing `gruel-4.1.0.tar` & `gruel-4.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/__init__.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/brewer.py
--rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/core.py
--rw-r--r--   0        0        0    18595 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/crawler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/py.typed
--rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/requests.py
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/subgruel.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 gruel-4.1.0/src/gruel/template.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gruel-4.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gruel-4.1.0/LICENSE.txt
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gruel-4.1.0/README.md
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 gruel-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 gruel-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 gruel-4.1.1/src/gruel/__init__.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 gruel-4.1.1/src/gruel/brewer.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 gruel-4.1.1/src/gruel/core.py
+-rw-r--r--   0        0        0    18656 2020-02-02 00:00:00.000000 gruel-4.1.1/src/gruel/crawler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gruel-4.1.1/src/gruel/py.typed
+-rw-r--r--   0        0        0     8703 2020-02-02 00:00:00.000000 gruel-4.1.1/src/gruel/requests.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 gruel-4.1.1/src/gruel/subgruel.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 gruel-4.1.1/src/gruel/template.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 gruel-4.1.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 gruel-4.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 gruel-4.1.1/README.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 gruel-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 gruel-4.1.1/PKG-INFO
```

### Comparing `gruel-4.1.0/src/gruel/__init__.py` & `gruel-4.1.1/src/gruel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     CrawlScraper,
     LimitCheckerMixin,
     SeleniumCrawler,
     UrlManager,
 )
 from .requests import Response, Session, request, retry_on_codes
 
-__version__ = "4.1.0"
+__version__ = "4.1.1"
 __all__ = [
     "Brewer",
     "GruelFinder",
     "Gruel",
     "ChoresMixin",
     "ParserMixin",
     "request",
```

### Comparing `gruel-4.1.0/src/gruel/brewer.py` & `gruel-4.1.1/src/gruel/brewer.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.0/src/gruel/core.py` & `gruel-4.1.1/src/gruel/core.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.0/src/gruel/crawler.py` & `gruel-4.1.1/src/gruel/crawler.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,15 +309,15 @@
     def __init__(
         self,
         scrapers: Sequence[CrawlScraper] = [],
         max_depth: int | None = None,
         max_time: float | None = None,
         log_name: str | int | loggi.LogName = loggi.LogName.CLASSNAME,
         log_dir: Pathish = "logs",
-        max_threads: int = 5,
+        max_threads: int = 3,
         same_site_only: bool = True,
         custom_url_manager: UrlManager | None = None,
     ):
         """
         Create a `Crawler` instance.
 
         #### :params:
@@ -481,14 +481,15 @@
     Currently `max_threads` is hardcoded to `1`.
     """
 
     @override
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.thread_manager = ThreadManager(1)
+        self.max_depth.thread_manager = self.thread_manager
         self.user = User(True)
 
     @override
     def request_page(self, url: str) -> SeleniumResponse:
         self.user.get(url)
         return SeleniumResponse.from_selenium_user(self.user)
```

### Comparing `gruel-4.1.0/src/gruel/requests.py` & `gruel-4.1.1/src/gruel/requests.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.0/src/gruel/subgruel.py` & `gruel-4.1.1/src/gruel/subgruel.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.0/src/gruel/template.py` & `gruel-4.1.1/src/gruel/template.py`

 * *Files identical despite different names*

### Comparing `gruel-4.1.0/LICENSE.txt` & `gruel-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gruel-4.1.0/pyproject.toml` & `gruel-4.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "gruel"
 description = "Another scraping framework"
-version = "4.1.0"
+version = "4.1.1"
 dependencies = ["pathier", "printbuddies", "younotyou", "noiftimer", "requests", "whosyouragent", "quickpool", "loggi", "beautifulsoup4", "rich", "scrapetools", "typing_extensions", "urllib3", "seleniumuser"]
 readme = "README.md"
 keywords = ["scrape", "scraping", "webscraping", "webscraper", "beautifulsoup", "framework"]
 classifiers = ["Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent"]
 requires-python = ">=3.10, <=3.12"
 
 [[project.authors]]
```

### Comparing `gruel-4.1.0/PKG-INFO` & `gruel-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gruel
-Version: 4.1.0
+Version: 4.1.1
 Summary: Another scraping framework
 Project-URL: Homepage, https://github.com/matt-manes/gruel
 Project-URL: Documentation, https://github.com/matt-manes/gruel/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/gruel/tree/main/src/gruel
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: beautifulsoup,framework,scrape,scraping,webscraper,webscraping
```
