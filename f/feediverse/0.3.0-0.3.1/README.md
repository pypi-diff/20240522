# Comparing `tmp/feediverse-0.3.0.tar.gz` & `tmp/feediverse-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feediverse-0.3.0.tar", last modified: Sat Feb 19 13:40:30 2022, max compression
+gzip compressed data, was "feediverse-0.3.1.tar", max compression
```

## Comparing `feediverse-0.3.0.tar` & `feediverse-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,5 @@
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2022-02-19 13:40:30.632714 feediverse-0.3.0/
--rw-rw-r--   0 ed        (1000) ed        (1000)     2315 2022-02-19 13:40:30.632714 feediverse-0.3.0/PKG-INFO
--rw-rw-r--   0 ed        (1000) ed        (1000)     1591 2022-02-19 13:37:41.000000 feediverse-0.3.0/README.md
-drwxrwxr-x   0 ed        (1000) ed        (1000)        0 2022-02-19 13:40:30.632714 feediverse-0.3.0/feediverse.egg-info/
--rw-rw-r--   0 ed        (1000) ed        (1000)     2315 2022-02-19 13:40:30.000000 feediverse-0.3.0/feediverse.egg-info/PKG-INFO
--rw-rw-r--   0 ed        (1000) ed        (1000)      238 2022-02-19 13:40:30.000000 feediverse-0.3.0/feediverse.egg-info/SOURCES.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)        1 2022-02-19 13:40:30.000000 feediverse-0.3.0/feediverse.egg-info/dependency_links.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)       48 2022-02-19 13:40:30.000000 feediverse-0.3.0/feediverse.egg-info/entry_points.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)       61 2022-02-19 13:40:30.000000 feediverse-0.3.0/feediverse.egg-info/requires.txt
--rw-rw-r--   0 ed        (1000) ed        (1000)       11 2022-02-19 13:40:30.000000 feediverse-0.3.0/feediverse.egg-info/top_level.txt
--rwxrwxr-x   0 ed        (1000) ed        (1000)     5944 2022-02-19 13:30:46.000000 feediverse-0.3.0/feediverse.py
--rw-rw-r--   0 ed        (1000) ed        (1000)       38 2022-02-19 13:40:30.632714 feediverse-0.3.0/setup.cfg
--rw-rw-r--   0 ed        (1000) ed        (1000)      711 2022-02-19 13:31:04.000000 feediverse-0.3.0/setup.py
+-rw-r--r--   0        0        0     1073 2024-05-22 11:52:40.297801 feediverse-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1591 2024-05-22 12:01:58.318912 feediverse-0.3.1/README.md
+-rwxr-xr-x   0        0        0     5944 2024-05-22 11:52:40.298214 feediverse-0.3.1/feediverse.py
+-rw-r--r--   0        0        0      485 2024-05-22 12:00:44.779177 feediverse-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2347 1970-01-01 00:00:00.000000 feediverse-0.3.1/PKG-INFO
```

### Comparing `feediverse-0.3.0/PKG-INFO` & `feediverse-0.3.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,53 @@
-Metadata-Version: 2.1
-Name: feediverse
-Version: 0.3.0
-Summary: Connect an RSS Feed to Mastodon
-Home-page: https://github.com/edsu/feediverse
-Author: Ed Summers
-Author-email: ehs@pobox.com
-License: UNKNOWN
-Description: *feediverse* will read RSS/Atom feeds and send the messages as Mastodon posts.
-        It's meant to add a little bit of spice to your timeline from other places.
-        Please use it responsibly.
-        
-        ## Install
-        
-            pip install feediverse
-        
-        ## Run
-        
-        The first time you run *feediverse* you'll need to tell it your Mastodon
-        instance and get an access token which it will save in a configuration file. If
-        you don't specify a config file it will use `~/.feediverse`:
-        
-            feediverse
-        
-        Once *feediverse* is configured you can add it to your crontab:
-        
-            */15 * * * * /usr/local/bin/feediverse    
-        
-        Run `feediverse --help` to show the command line options.
-        
-        ## Post Format
-        
-        You can customize the post format by opening the configuration file (default is
-        ~/.feediverse) and updating the *template* property of your feed. The default
-        format is:
-        
-            {title} {url}
-        
-        If you want you can use `{summary}` in your template, and add boilerplate text
-        like so:
-        
-            Bookmark: {title} {url} {summary}
-        
-        `{hashtags}` will look for tags in the feed entry and turn them into a space
-        separated list of hashtags. For some feeds (e.g. youtube-rss) you should use `{link}` instead of `{url}`.
-        
-        `{content}` is the whole content of the feed entry (with html-tags
-        stripped). Please be aware that this might easily exceed Mastodon's
-        limit of 512 characters.
-        
-        ## Multiple Feeds
-        
-        Since *feeds* is a list you can add additional feeds to watch if you want.
-        
-            ...
-            feeds:
-              - url: https://example.com/feed/
-                template: "dot com: {title} {url}"
-              - url: https://example.org/feed/
-                template: "dot org: {title} {url}"
-        
-        
-Platform: UNKNOWN
-Requires-Python: >=3.3
-Description-Content-Type: text/markdown
+*feediverse* will read RSS/Atom feeds and send the messages as Mastodon posts.
+It's meant to add a little bit of spice to your timeline from other places.
+Please use it responsibly.
+
+## Install
+
+    pip install feediverse
+
+## Run
+
+The first time you run *feediverse* you'll need to tell it your Mastodon
+instance and get an access token which it will save in a configuration file. If
+you don't specify a config file it will use `~/.feediverse`:
+
+    feediverse
+
+Once *feediverse* is configured you can add it to your crontab:
+
+    */15 * * * * /usr/local/bin/feediverse    
+
+Run `feediverse --help` to show the command line options.
+
+## Post Format
+
+You can customize the post format by opening the configuration file (default is
+~/.feediverse) and updating the *template* property of your feed. The default
+format is:
+
+    {title} {url}
+
+If you want you can use `{summary}` in your template, and add boilerplate text
+like so:
+
+    Bookmark: {title} {url} {summary}
+
+`{hashtags}` will look for tags in the feed entry and turn them into a space
+separated list of hashtags. For some feeds (e.g. youtube-rss) you should use `{link}` instead of `{url}`.
+
+`{content}` is the whole content of the feed entry (with html-tags
+stripped). Please be aware that this might easily exceed Mastodon's
+limit of 512 characters.
+
+## Multiple Feeds
+
+Since *feeds* is a list you can add additional feeds to watch if you want.
+
+    ...
+    feeds:
+      - url: https://example.com/feed/
+        template: "dot com: {title} {url}"
+      - url: https://example.org/feed/
+        template: "dot org: {title} {url}"
+
```

### Comparing `feediverse-0.3.0/README.md` & `feediverse-0.3.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: feediverse
+Version: 0.3.1
+Summary: Connect an RSS Feed to Mastodon
+License: MIT
+Author: Ed Summers
+Author-email: ehs@pobox.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: feedparser (>=6.0.11,<7.0.0)
+Requires-Dist: mastodon-py (>=1.8.1,<2.0.0)
+Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Description-Content-Type: text/markdown
+
 *feediverse* will read RSS/Atom feeds and send the messages as Mastodon posts.
 It's meant to add a little bit of spice to your timeline from other places.
 Please use it responsibly.
 
 ## Install
 
     pip install feediverse
@@ -47,7 +68,8 @@
     ...
     feeds:
       - url: https://example.com/feed/
         template: "dot com: {title} {url}"
       - url: https://example.org/feed/
         template: "dot org: {title} {url}"
 
+
```

### Comparing `feediverse-0.3.0/feediverse.py` & `feediverse-0.3.1/feediverse.py`

 * *Files identical despite different names*

