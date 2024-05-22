# Comparing `tmp/llama_index_readers_web-0.1.8.tar.gz` & `tmp/llama_index_readers_web-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_web-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_readers_web-0.1.9.tar", max compression
```

## Comparing `llama_index_readers_web-0.1.8.tar` & `llama_index_readers_web-0.1.9.tar`

### file list

```diff
@@ -1,55 +1,59 @@
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/README.md
--rw-r--r--   0        0        0     1432 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/__init__.py
--rw-r--r--   0        0        0     1206 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/__init__.py
--rw-r--r--   0        0        0     3697 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/base.py
--rw-r--r--   0        0        0     3465 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/__init__.py
--rw-r--r--   0        0        0     7070 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/base.py
--rw-r--r--   0        0        0       32 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/requirements.txt
--rw-r--r--   0        0        0     3701 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/__init__.py
--rw-r--r--   0        0        0     5613 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/base.py
--rw-r--r--   0        0        0       17 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/requirements.txt
--rw-r--r--   0        0        0     1996 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/__init__.py
--rw-r--r--   0        0        0     1310 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/base.py
--rw-r--r--   0        0        0       21 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/requirements.txt
--rw-r--r--   0        0        0      607 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/news/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/news/__init__.py
--rw-r--r--   0        0        0     3171 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/news/base.py
--rw-r--r--   0        0        0       12 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/news/requirements.txt
--rw-r--r--   0        0        0     2635 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/README.md
--rw-r--r--   0        0        0    85982 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/Readability.js
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/__init__.py
--rw-r--r--   0        0        0     5098 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/base.py
--rw-r--r--   0        0        0       19 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/requirements.txt
--rw-r--r--   0        0        0      521 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss/__init__.py
--rw-r--r--   0        0        0     1440 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss/base.py
--rw-r--r--   0        0        0      899 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/__init__.py
--rw-r--r--   0        0        0     3382 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/base.py
--rw-r--r--   0        0        0      571 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/sample_rss_feeds.opml
--rw-r--r--   0        0        0     1989 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/__init__.py
--rw-r--r--   0        0        0     2194 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/base.py
--rw-r--r--   0        0        0       10 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/requirements.txt
--rw-r--r--   0        0        0     1799 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/__init__.py
--rw-r--r--   0        0        0     1898 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/base.py
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/requirements.txt
--rw-r--r--   0        0        0     2001 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/__init__.py
--rw-r--r--   0        0        0     2165 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/base.py
--rw-r--r--   0        0        0       17 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/requirements.txt
--rw-r--r--   0        0        0     1084 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/__init__.py
--rw-r--r--   0        0        0     2263 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/base.py
--rw-r--r--   0        0        0       13 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/requirements.txt
--rw-r--r--   0        0        0     4098 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/README.md
--rw-r--r--   0        0        0        0 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/__init__.py
--rw-r--r--   0        0        0     4660 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/base.py
--rw-r--r--   0        0        0       36 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/requirements.txt
--rw-r--r--   0        0        0     2439 2024-04-03 20:27:10.861073 llama_index_readers_web-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 llama_index_readers_web-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.632533 llama_index_readers_web-0.1.9/README.md
+-rw-r--r--   0        0        0     1533 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/__init__.py
+-rw-r--r--   0        0        0     1206 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/async_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/async_web/__init__.py
+-rw-r--r--   0        0        0     3697 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/async_web/base.py
+-rw-r--r--   0        0        0     3465 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/beautiful_soup_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/beautiful_soup_web/__init__.py
+-rw-r--r--   0        0        0     7070 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/beautiful_soup_web/base.py
+-rw-r--r--   0        0        0       32 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/beautiful_soup_web/requirements.txt
+-rw-r--r--   0        0        0     2100 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/firecrawl_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/firecrawl_web/__init__.py
+-rw-r--r--   0        0        0     2578 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/firecrawl_web/base.py
+-rw-r--r--   0        0        0       13 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/firecrawl_web/requirements.txt
+-rw-r--r--   0        0        0     3701 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/knowledge_base/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/knowledge_base/__init__.py
+-rw-r--r--   0        0        0     5613 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/knowledge_base/base.py
+-rw-r--r--   0        0        0       17 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/knowledge_base/requirements.txt
+-rw-r--r--   0        0        0     1996 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/main_content_extractor/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/main_content_extractor/__init__.py
+-rw-r--r--   0        0        0     1310 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/main_content_extractor/base.py
+-rw-r--r--   0        0        0       21 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/main_content_extractor/requirements.txt
+-rw-r--r--   0        0        0      607 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/news/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/news/__init__.py
+-rw-r--r--   0        0        0     3171 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/news/base.py
+-rw-r--r--   0        0        0       12 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/news/requirements.txt
+-rw-r--r--   0        0        0     2635 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/readability_web/README.md
+-rw-r--r--   0        0        0    85982 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/readability_web/Readability.js
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/readability_web/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/readability_web/base.py
+-rw-r--r--   0        0        0       19 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/readability_web/requirements.txt
+-rw-r--r--   0        0        0      521 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/rss/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/rss/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/rss/base.py
+-rw-r--r--   0        0        0      899 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/rss_news/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/rss_news/__init__.py
+-rw-r--r--   0        0        0     3382 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/rss_news/base.py
+-rw-r--r--   0        0        0      571 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/rss_news/sample_rss_feeds.opml
+-rw-r--r--   0        0        0     1989 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/simple_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/simple_web/__init__.py
+-rw-r--r--   0        0        0     2194 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/simple_web/base.py
+-rw-r--r--   0        0        0       10 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/simple_web/requirements.txt
+-rw-r--r--   0        0        0     1799 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/sitemap/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/sitemap/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/sitemap/base.py
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/sitemap/requirements.txt
+-rw-r--r--   0        0        0     2001 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/trafilatura_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/trafilatura_web/__init__.py
+-rw-r--r--   0        0        0     2165 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/trafilatura_web/base.py
+-rw-r--r--   0        0        0       17 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/trafilatura_web/requirements.txt
+-rw-r--r--   0        0        0     1084 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/unstructured_web/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/unstructured_web/__init__.py
+-rw-r--r--   0        0        0     2263 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/unstructured_web/base.py
+-rw-r--r--   0        0        0       13 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/unstructured_web/requirements.txt
+-rw-r--r--   0        0        0     4098 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/whole_site/README.md
+-rw-r--r--   0        0        0        0 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/whole_site/__init__.py
+-rw-r--r--   0        0        0     4660 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/whole_site/base.py
+-rw-r--r--   0        0        0       36 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/llama_index/readers/web/whole_site/requirements.txt
+-rw-r--r--   0        0        0     2439 2024-04-15 18:22:24.636533 llama_index_readers_web-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1149 1970-01-01 00:00:00.000000 llama_index_readers_web-0.1.9/PKG-INFO
```

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/__init__.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Init file."""
 from llama_index.readers.web.async_web.base import (
     AsyncWebPageReader,
 )
 from llama_index.readers.web.beautiful_soup_web.base import (
     BeautifulSoupWebReader,
 )
+from llama_index.readers.web.firecrawl_web.base import FireCrawlWebReader
 from llama_index.readers.web.knowledge_base.base import (
     KnowledgeBaseWebReader,
 )
 from llama_index.readers.web.main_content_extractor.base import (
     MainContentExtractorReader,
 )
 from llama_index.readers.web.news.base import NewsArticleReader
@@ -33,17 +34,19 @@
 from llama_index.readers.web.unstructured_web.base import (
     UnstructuredURLLoader,
 )
 from llama_index.readers.web.whole_site.base import (
     WholeSiteReader,
 )
 
+
 __all__ = [
     "AsyncWebPageReader",
     "BeautifulSoupWebReader",
+    "FireCrawlWebReader",
     "KnowledgeBaseWebReader",
     "MainContentExtractorReader",
     "NewsArticleReader",
     "ReadabilityWebPageReader",
     "RssReader",
     "RssNewsReader",
     "SimpleWebPageReader",
```

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/async_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/async_web/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/async_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/beautiful_soup_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/beautiful_soup_web/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/beautiful_soup_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/knowledge_base/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/knowledge_base/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/knowledge_base/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/main_content_extractor/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/main_content_extractor/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/main_content_extractor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/news/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/news/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/news/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/news/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/readability_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/Readability.js` & `llama_index_readers_web-0.1.9/llama_index/readers/web/readability_web/Readability.js`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/readability_web/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/readability_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/rss/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/rss/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/rss/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/rss/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/rss_news/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/rss_news/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/rss_news/sample_rss_feeds.opml` & `llama_index_readers_web-0.1.9/llama_index/readers/web/rss_news/sample_rss_feeds.opml`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/simple_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/simple_web/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/simple_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/sitemap/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/sitemap/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/sitemap/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/trafilatura_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/trafilatura_web/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/trafilatura_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/unstructured_web/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/unstructured_web/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/unstructured_web/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/README.md` & `llama_index_readers_web-0.1.9/llama_index/readers/web/whole_site/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/llama_index/readers/web/whole_site/base.py` & `llama_index_readers_web-0.1.9/llama_index/readers/web/whole_site/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_web-0.1.8/pyproject.toml` & `llama_index_readers_web-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 description = "llama-index readers web integration"
 exclude = ["**/BUILD"]
 keywords = ["BFS", "article", "atom", "documentation", "feed", "main content extractor", "news", "readthedocs", "rss", "scraper", "selenium", "seo", "sitemap", "substack", "trafilatura", "unstructured.io", "url", "web reader", "web", "website"]
 license = "MIT"
 maintainers = ["HawkClaws", "Hironsan", "NA", "an-bluecat", "bborn", "jasonwcfan", "kravetsmic", "pandazki", "ruze00", "selamanse", "thejessezhang"]
 name = "llama-index-readers-web"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 selenium = "^4.17.2"
 chromedriver-autoinstaller = "^0.6.3"
 html2text = "^2020.1.16"
```

### Comparing `llama_index_readers_web-0.1.8/PKG-INFO` & `llama_index_readers_web-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-web
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index readers web integration
 License: MIT
 Keywords: BFS,article,atom,documentation,feed,main content extractor,news,readthedocs,rss,scraper,selenium,seo,sitemap,substack,trafilatura,unstructured.io,url,web reader,web,website
 Author: Your Name
 Author-email: you@example.com
 Maintainer: HawkClaws
 Requires-Python: >=3.8.1,<4.0
```

