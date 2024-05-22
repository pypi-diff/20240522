# Comparing `tmp/osu-wiki-tools-2.2.1.tar.gz` & `tmp/osu_wiki_tools-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osu-wiki-tools-2.2.1.tar", last modified: Tue Dec 12 11:22:36 2023, max compression
+gzip compressed data, was "osu_wiki_tools-2.3.0.tar", last modified: Wed May 22 13:05:48 2024, max compression
```

## Comparing `osu-wiki-tools-2.2.1.tar` & `osu_wiki_tools-2.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-12-12 11:22:36.110074 osu-wiki-tools-2.2.1/
--rw-rw-rw-   0        0        0     1083 2022-06-05 22:05:02.000000 osu-wiki-tools-2.2.1/LICENCE.md
--rw-rw-rw-   0        0        0     1059 2023-12-12 11:22:36.108027 osu-wiki-tools-2.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-02-26 14:18:44.000000 osu-wiki-tools-2.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-12-12 11:22:36.105978 osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/
--rw-rw-rw-   0        0        0     1059 2023-12-12 11:22:36.000000 osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1286 2023-12-12 11:22:36.000000 osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-12 11:22:36.000000 osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-12-12 11:22:36.000000 osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2023-12-12 11:22:36.000000 osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-12-12 11:22:36.000000 osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-12 11:22:36.110074 osu-wiki-tools-2.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1186 2023-11-23 02:37:57.000000 osu-wiki-tools-2.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-12 11:22:36.069480 osu-wiki-tools-2.2.1/tests/
--rw-rw-rw-   0        0        0    12105 2023-02-26 14:18:44.000000 osu-wiki-tools-2.2.1/tests/test_article_parser.py
--rw-rw-rw-   0        0        0     3883 2023-02-26 14:18:44.000000 osu-wiki-tools-2.2.1/tests/test_check_links.py
--rw-rw-rw-   0        0        0    21144 2023-02-26 14:18:34.000000 osu-wiki-tools-2.2.1/tests/test_check_outdated_articles.py
--rw-rw-rw-   0        0        0     2354 2022-04-16 18:18:34.000000 osu-wiki-tools-2.2.1/tests/test_code_block_parser.py
--rw-rw-rw-   0        0        0     1492 2022-04-16 18:18:34.000000 osu-wiki-tools-2.2.1/tests/test_comment_parser.py
--rw-rw-rw-   0        0        0     4419 2023-11-22 11:03:10.000000 osu-wiki-tools-2.2.1/tests/test_file_utils.py
--rw-rw-rw-   0        0        0     4893 2023-12-12 11:21:56.000000 osu-wiki-tools-2.2.1/tests/test_identifier_parser.py
--rw-rw-rw-   0        0        0    39635 2023-11-30 22:08:53.000000 osu-wiki-tools-2.2.1/tests/test_link_checker.py
--rw-rw-rw-   0        0        0     9219 2022-07-31 07:21:51.000000 osu-wiki-tools-2.2.1/tests/test_link_parser.py
--rw-rw-rw-   0        0        0     1143 2023-11-23 15:54:03.000000 osu-wiki-tools-2.2.1/tests/test_redirect_parser.py
--rw-rw-rw-   0        0        0     2747 2022-04-14 00:20:54.000000 osu-wiki-tools-2.2.1/tests/test_reference_parser.py
--rw-rw-rw-   0        0        0      694 2023-11-22 22:07:45.000000 osu-wiki-tools-2.2.1/tests/test_visual_tests.py
--rw-rw-rw-   0        0        0     4223 2023-11-22 11:03:10.000000 osu-wiki-tools-2.2.1/tests/test_yaml_rules.py
-drwxrwxrwx   0        0        0        0 2023-12-12 11:22:36.088364 osu-wiki-tools-2.2.1/wikitools/
--rw-rw-rw-   0        0        0        0 2022-04-14 00:20:54.000000 osu-wiki-tools-2.2.1/wikitools/__init__.py
--rw-rw-rw-   0        0        0     6547 2023-11-22 11:03:10.000000 osu-wiki-tools-2.2.1/wikitools/article_parser.py
--rw-rw-rw-   0        0        0     3449 2022-04-16 18:18:34.000000 osu-wiki-tools-2.2.1/wikitools/code_block_parser.py
--rw-rw-rw-   0        0        0     3029 2022-04-16 18:18:34.000000 osu-wiki-tools-2.2.1/wikitools/comment_parser.py
--rw-rw-rw-   0        0        0      258 2022-05-06 12:30:44.000000 osu-wiki-tools-2.2.1/wikitools/console.py
--rw-rw-rw-   0        0        0     3815 2023-11-30 09:42:19.000000 osu-wiki-tools-2.2.1/wikitools/errors.py
--rw-rw-rw-   0        0        0     5381 2023-11-30 22:21:16.000000 osu-wiki-tools-2.2.1/wikitools/file_utils.py
--rw-rw-rw-   0        0        0     1314 2022-07-31 07:21:51.000000 osu-wiki-tools-2.2.1/wikitools/git_utils.py
--rw-rw-rw-   0        0        0     3259 2023-12-12 11:21:56.000000 osu-wiki-tools-2.2.1/wikitools/identifier_parser.py
--rw-rw-rw-   0        0        0    11885 2023-11-30 22:24:52.000000 osu-wiki-tools-2.2.1/wikitools/link_checker.py
--rw-rw-rw-   0        0        0     7826 2023-11-30 07:44:55.000000 osu-wiki-tools-2.2.1/wikitools/link_parser.py
--rw-rw-rw-   0        0        0      750 2023-11-23 15:56:44.000000 osu-wiki-tools-2.2.1/wikitools/redirect_parser.py
--rw-rw-rw-   0        0        0     2536 2022-04-14 08:51:50.000000 osu-wiki-tools-2.2.1/wikitools/reference_parser.py
--rw-rw-rw-   0        0        0     5436 2023-11-30 07:44:54.000000 osu-wiki-tools-2.2.1/wikitools/yaml_rules.py
-drwxrwxrwx   0        0        0        0 2023-12-12 11:22:36.099362 osu-wiki-tools-2.2.1/wikitools_cli/
--rw-rw-rw-   0        0        0       19 2023-12-12 11:21:56.000000 osu-wiki-tools-2.2.1/wikitools_cli/VERSION.py
--rw-rw-rw-   0        0        0        0 2022-06-05 22:05:02.000000 osu-wiki-tools-2.2.1/wikitools_cli/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-12 11:22:36.104975 osu-wiki-tools-2.2.1/wikitools_cli/commands/
--rw-rw-rw-   0        0        0        0 2022-07-31 07:21:51.000000 osu-wiki-tools-2.2.1/wikitools_cli/commands/__init__.py
--rw-rw-rw-   0        0        0     7117 2023-11-30 08:43:07.000000 osu-wiki-tools-2.2.1/wikitools_cli/commands/check_links.py
--rw-rw-rw-   0        0        0    10201 2023-12-01 07:48:55.000000 osu-wiki-tools-2.2.1/wikitools_cli/commands/check_outdated_articles.py
--rw-rw-rw-   0        0        0     3766 2023-02-26 14:18:44.000000 osu-wiki-tools-2.2.1/wikitools_cli/commands/check_yaml.py
--rw-rw-rw-   0        0        0     2270 2023-11-22 11:03:10.000000 osu-wiki-tools-2.2.1/wikitools_cli/osu_wiki_tools.py
--rw-rw-rw-   0        0        0     1728 2022-06-20 03:50:12.000000 osu-wiki-tools-2.2.1/wikitools_cli/update_tournament_countries.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:05:48.275408 osu_wiki_tools-2.3.0/
+-rw-rw-rw-   0        0        0     1083 2022-06-05 22:05:02.000000 osu_wiki_tools-2.3.0/LICENCE.md
+-rw-rw-rw-   0        0        0     1065 2024-05-22 13:05:48.275408 osu_wiki_tools-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2024-02-20 18:59:03.000000 osu_wiki_tools-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 13:05:48.274423 osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/
+-rw-rw-rw-   0        0        0     1065 2024-05-22 13:05:47.000000 osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1286 2024-05-22 13:05:47.000000 osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:05:47.000000 osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2024-05-22 13:05:47.000000 osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       55 2024-05-22 13:05:47.000000 osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-22 13:05:47.000000 osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 13:05:48.276408 osu_wiki_tools-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1192 2024-02-20 18:55:57.000000 osu_wiki_tools-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:05:48.100640 osu_wiki_tools-2.3.0/tests/
+-rw-rw-rw-   0        0        0    12105 2023-02-26 14:18:44.000000 osu_wiki_tools-2.3.0/tests/test_article_parser.py
+-rw-rw-rw-   0        0        0     3883 2023-02-26 14:18:44.000000 osu_wiki_tools-2.3.0/tests/test_check_links.py
+-rw-rw-rw-   0        0        0    21713 2024-02-20 16:04:41.000000 osu_wiki_tools-2.3.0/tests/test_check_outdated_articles.py
+-rw-rw-rw-   0        0        0     2354 2022-04-16 18:18:34.000000 osu_wiki_tools-2.3.0/tests/test_code_block_parser.py
+-rw-rw-rw-   0        0        0     1492 2022-04-16 18:18:34.000000 osu_wiki_tools-2.3.0/tests/test_comment_parser.py
+-rw-rw-rw-   0        0        0     4419 2023-11-22 11:03:10.000000 osu_wiki_tools-2.3.0/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     4893 2024-02-20 16:04:34.000000 osu_wiki_tools-2.3.0/tests/test_identifier_parser.py
+-rw-rw-rw-   0        0        0    39635 2023-11-30 22:08:53.000000 osu_wiki_tools-2.3.0/tests/test_link_checker.py
+-rw-rw-rw-   0        0        0     9219 2022-07-31 07:21:51.000000 osu_wiki_tools-2.3.0/tests/test_link_parser.py
+-rw-rw-rw-   0        0        0     1143 2023-11-23 15:54:03.000000 osu_wiki_tools-2.3.0/tests/test_redirect_parser.py
+-rw-rw-rw-   0        0        0     2747 2022-04-14 00:20:54.000000 osu_wiki_tools-2.3.0/tests/test_reference_parser.py
+-rw-rw-rw-   0        0        0      694 2023-11-22 22:07:45.000000 osu_wiki_tools-2.3.0/tests/test_visual_tests.py
+-rw-rw-rw-   0        0        0     4223 2023-11-22 11:03:10.000000 osu_wiki_tools-2.3.0/tests/test_yaml_rules.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:05:48.208522 osu_wiki_tools-2.3.0/wikitools/
+-rw-rw-rw-   0        0        0        0 2022-04-14 00:20:54.000000 osu_wiki_tools-2.3.0/wikitools/__init__.py
+-rw-rw-rw-   0        0        0     6547 2023-11-22 11:03:10.000000 osu_wiki_tools-2.3.0/wikitools/article_parser.py
+-rw-rw-rw-   0        0        0     3449 2022-04-16 18:18:34.000000 osu_wiki_tools-2.3.0/wikitools/code_block_parser.py
+-rw-rw-rw-   0        0        0     3029 2022-04-16 18:18:34.000000 osu_wiki_tools-2.3.0/wikitools/comment_parser.py
+-rw-rw-rw-   0        0        0      258 2022-05-06 12:30:44.000000 osu_wiki_tools-2.3.0/wikitools/console.py
+-rw-rw-rw-   0        0        0     3815 2023-11-30 09:42:19.000000 osu_wiki_tools-2.3.0/wikitools/errors.py
+-rw-rw-rw-   0        0        0     5381 2023-11-30 22:21:16.000000 osu_wiki_tools-2.3.0/wikitools/file_utils.py
+-rw-rw-rw-   0        0        0     1308 2024-02-20 16:04:41.000000 osu_wiki_tools-2.3.0/wikitools/git_utils.py
+-rw-rw-rw-   0        0        0     3259 2024-02-20 16:04:34.000000 osu_wiki_tools-2.3.0/wikitools/identifier_parser.py
+-rw-rw-rw-   0        0        0    11885 2023-11-30 22:24:52.000000 osu_wiki_tools-2.3.0/wikitools/link_checker.py
+-rw-rw-rw-   0        0        0     7826 2023-11-30 07:44:55.000000 osu_wiki_tools-2.3.0/wikitools/link_parser.py
+-rw-rw-rw-   0        0        0      750 2023-11-23 15:56:44.000000 osu_wiki_tools-2.3.0/wikitools/redirect_parser.py
+-rw-rw-rw-   0        0        0     2536 2022-04-14 08:51:50.000000 osu_wiki_tools-2.3.0/wikitools/reference_parser.py
+-rw-rw-rw-   0        0        0     5451 2024-05-22 12:57:51.000000 osu_wiki_tools-2.3.0/wikitools/yaml_rules.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:05:48.236856 osu_wiki_tools-2.3.0/wikitools_cli/
+-rw-rw-rw-   0        0        0       19 2024-05-22 12:57:51.000000 osu_wiki_tools-2.3.0/wikitools_cli/VERSION.py
+-rw-rw-rw-   0        0        0        0 2022-06-05 22:05:02.000000 osu_wiki_tools-2.3.0/wikitools_cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:05:48.273412 osu_wiki_tools-2.3.0/wikitools_cli/commands/
+-rw-rw-rw-   0        0        0        0 2022-07-31 07:21:51.000000 osu_wiki_tools-2.3.0/wikitools_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0     7117 2023-11-30 08:43:07.000000 osu_wiki_tools-2.3.0/wikitools_cli/commands/check_links.py
+-rw-rw-rw-   0        0        0    10161 2024-02-20 16:04:41.000000 osu_wiki_tools-2.3.0/wikitools_cli/commands/check_outdated_articles.py
+-rw-rw-rw-   0        0        0     3766 2023-02-26 14:18:44.000000 osu_wiki_tools-2.3.0/wikitools_cli/commands/check_yaml.py
+-rw-rw-rw-   0        0        0     2270 2024-05-22 12:57:48.000000 osu_wiki_tools-2.3.0/wikitools_cli/osu_wiki_tools.py
+-rw-rw-rw-   0        0        0     1728 2022-06-20 03:50:12.000000 osu_wiki_tools-2.3.0/wikitools_cli/update_tournament_countries.py
```

### Comparing `osu-wiki-tools-2.2.1/LICENCE.md` & `osu_wiki_tools-2.3.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/PKG-INFO` & `osu_wiki_tools-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: osu-wiki-tools
-Version: 2.2.1
+Version: 2.3.0
 Summary: Various tools for osu! wiki contributors
 Home-page: https://github.com/Walavouchey/osu-wiki-tools
 Author: Walavouchey
 Author-email: wala@yui.tv
 Project-URL: Bug Tracker, https://github.com/Walavouchey/osu-wiki-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
-Requires-Dist: PyYAML==6.0
-Requires-Dist: types-PyYAML==6.0.6
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: types-PyYAML==6.0.12.12
 Requires-Dist: yamllint==1.33.0
 
 # osu! wiki tools
 
 A collection of various tools that may be useful for [osu! wiki](https://osu.ppy.sh/wiki/) contributors
 
 ## Installation
```

### Comparing `osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/PKG-INFO` & `osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: osu-wiki-tools
-Version: 2.2.1
+Version: 2.3.0
 Summary: Various tools for osu! wiki contributors
 Home-page: https://github.com/Walavouchey/osu-wiki-tools
 Author: Walavouchey
 Author-email: wala@yui.tv
 Project-URL: Bug Tracker, https://github.com/Walavouchey/osu-wiki-tools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENCE.md
-Requires-Dist: PyYAML==6.0
-Requires-Dist: types-PyYAML==6.0.6
+Requires-Dist: PyYAML==6.0.1
+Requires-Dist: types-PyYAML==6.0.12.12
 Requires-Dist: yamllint==1.33.0
 
 # osu! wiki tools
 
 A collection of various tools that may be useful for [osu! wiki](https://osu.ppy.sh/wiki/) contributors
 
 ## Installation
```

### Comparing `osu-wiki-tools-2.2.1/osu_wiki_tools.egg-info/SOURCES.txt` & `osu_wiki_tools-2.3.0/osu_wiki_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/setup.py` & `osu_wiki_tools-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,12 +28,12 @@
     entry_points={
         "console_scripts": [
             "osu-wiki-tools=wikitools_cli.osu_wiki_tools:console_main",
         ],
     },
     python_requires=">=3.11",
     install_requires=[
-        "PyYAML==6.0",
-        "types-PyYAML==6.0.6",
+        "PyYAML==6.0.1",
+        "types-PyYAML==6.0.12.12",
         "yamllint==1.33.0",
     ],
 )
```

### Comparing `osu-wiki-tools-2.2.1/tests/test_article_parser.py` & `osu_wiki_tools-2.3.0/tests/test_article_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_check_links.py` & `osu_wiki_tools-2.3.0/tests/test_check_links.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_check_outdated_articles.py` & `osu_wiki_tools-2.3.0/tests/test_check_outdated_articles.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,29 +33,26 @@
         ]
 
         utils.create_files(root, *((path, '') for path in article_paths))
         utils.stage_all_and_commit("initial commit")
 
         utils.create_files(root, *((path, '# Article') for path in article_paths))
         utils.stage_all_and_commit("add article title")
-        commit_hash = utils.get_last_commit_hash()
 
-        # note that at least two existing commits are necessary to get a diff using `revision^`
-        modified_translations = outdater.list_modified_translations(commit_hash)
+        modified_translations = outdater.list_modified_translations("HEAD^")
 
         assert multiset(modified_translations) == multiset(utils.remove(article_paths, "en.md", "TEMPLATE.md"))
 
         utils.create_files(root,
             *((path, '# Article\n\nCeci est un article en français.') for path in
             utils.take(article_paths, "fr.md"))
         )
         utils.stage_all_and_commit("add article content")
-        commit_hash = utils.get_last_commit_hash()
 
-        modified_translations = outdater.list_modified_translations(commit_hash)
+        modified_translations = outdater.list_modified_translations("HEAD^")
 
         assert multiset(modified_translations) == multiset(utils.take(article_paths, "fr.md"))
 
     def test__list_modified_originals(self, root):
         utils.set_up_dummy_repo()
         article_paths = [
             'wiki/Article/en.md',
@@ -66,24 +63,22 @@
             'wiki/Article2/pt-br.md',
             'wiki/Article/zh-tw.md',
             'wiki/Article2/zh-tw.md',
         ]
 
         utils.create_files(root, *((path, '# Article') for path in article_paths))
         utils.stage_all_and_commit("add some articles")
-        commit_hash = utils.get_last_commit_hash()
 
         utils.create_files(root, *zip(article_paths[0:2], [
             '# Article\n\nThis is an article in English.',
             '# Article\n\nThis is another article in English.',
         ]))
         utils.stage_all_and_commit("add article content")
-        commit_hash = utils.get_last_commit_hash()
 
-        modified_originals = outdater.list_modified_originals(commit_hash)
+        modified_originals = outdater.list_modified_originals("HEAD^")
         assert multiset(modified_originals) == multiset(utils.take(article_paths, "en.md"))
 
     def test__list_outdated_translations(self, root):
         utils.set_up_dummy_repo()
         article_paths = [
             'wiki/Article/en.md',
             'wiki/Article2/en.md',
@@ -219,15 +214,15 @@
         utils.create_files(root, *(
             (article_path, '# Article\n\nThis is an article in English.') for article_path in
             utils.take(article_paths, "en.md")
         ))
         utils.stage_all_and_commit("modify english articles")
         commit_hash_2 = utils.get_last_commit_hash()
 
-        exit_code = outdater.main("--base-commit", commit_hash_2, f"{outdater.AUTOFIX_FLAG}")
+        exit_code = outdater.main("--base-commit", "HEAD^", "--outdated-since", commit_hash_2, f"{outdater.AUTOFIX_FLAG}")
 
         assert exit_code == 0
 
         outdated_translations = utils.get_changed_files()
 
         non_chinese_translations = utils.remove(article_paths, "en.md", "zh-tw.md")
 
@@ -296,25 +291,23 @@
         utils.create_files(root, *(
             (article_path, '# Article\n\nThis is an article in English.') for article_path in
             utils.take(article_paths, "en.md")
         ))
         utils.stage_all_and_commit("modify english articles")
         commit_hash_2 = utils.get_last_commit_hash()
 
-        exit_code = outdater.main("--base-commit", commit_hash_2, f"{outdater.AUTOFIX_FLAG}", f"{outdater.AUTOCOMMIT_FLAG}")
+        exit_code = outdater.main("--base-commit", "HEAD^", "--outdated-since", commit_hash_2, f"{outdater.AUTOFIX_FLAG}", f"{outdater.AUTOCOMMIT_FLAG}")
 
         assert exit_code == 0
 
-        commit_hash_3 = utils.get_last_commit_hash()
-
-        assert commit_hash_3 != commit_hash_2
+        assert commit_hash_2 != utils.get_last_commit_hash()
 
         assert utils.get_changed_files() == []
 
-        outdated_translations = outdater.list_modified_translations(commit_hash_3)
+        outdated_translations = outdater.list_modified_translations("HEAD^")
 
         non_chinese_translations = utils.remove(article_paths, "en.md", "zh-tw.md")
 
         assert multiset(outdated_translations) == multiset(non_chinese_translations)
 
         expected_content = textwrap.dedent('''
             ---
@@ -380,15 +373,15 @@
             (article_path, '# Article\n\nThis is an article in English.') for article_path in
             utils.take(article_paths, "en.md")
         ))
         utils.stage_all_and_commit("modify english articles")
         commit_hash_2 = utils.get_last_commit_hash()
 
         cd = file_utils.ChangeDirectory("wiki")
-        exit_code = outdater.main("--root", "..", "--base-commit", commit_hash_2, f"{outdater.AUTOFIX_FLAG}")
+        exit_code = outdater.main("--root", "..", "--base-commit", "HEAD^", "--outdated-since", commit_hash_2, f"{outdater.AUTOFIX_FLAG}")
         del cd
 
         assert exit_code == 0
 
         outdated_translations = utils.get_changed_files()
 
         non_chinese_translations = utils.remove(article_paths, "en.md", "zh-tw.md")
@@ -459,26 +452,24 @@
             (article_path, '# Article\n\nThis is an article in English.') for article_path in
             utils.take(article_paths, "en.md")
         ))
         utils.stage_all_and_commit("modify english articles")
         commit_hash_2 = utils.get_last_commit_hash()
 
         cd = file_utils.ChangeDirectory("wiki")
-        exit_code = outdater.main("--root", "..", "--base-commit", commit_hash_2, f"{outdater.AUTOFIX_FLAG}", f"{outdater.AUTOCOMMIT_FLAG}")
+        exit_code = outdater.main("--root", "..", "--base-commit", "HEAD^", "--outdated-since", commit_hash_2, f"{outdater.AUTOFIX_FLAG}", f"{outdater.AUTOCOMMIT_FLAG}")
         del cd
 
         assert exit_code == 0
 
-        commit_hash_3 = utils.get_last_commit_hash()
-
-        assert commit_hash_3 != commit_hash_2
+        assert commit_hash_2 != utils.get_last_commit_hash()
 
         assert utils.get_changed_files() == []
 
-        outdated_translations = outdater.list_modified_translations(commit_hash_3)
+        outdated_translations = outdater.list_modified_translations("HEAD^")
 
         non_chinese_translations = utils.remove(article_paths, "en.md", "zh-tw.md")
 
         assert multiset(outdated_translations) == multiset(non_chinese_translations)
 
         expected_content = textwrap.dedent('''
             ---
@@ -506,7 +497,31 @@
                 content = fd.read()
 
             assert content == '# Article\n\nThis is an article in English.'
 
         log = git_utils.git("--no-pager", "log", "--pretty=oneline").splitlines()
 
         assert len(log) == 4
+
+    def test__full_autofix_flow_with_invalid_outdated_since(self, root):
+        utils.set_up_dummy_repo()
+        article_paths = [
+            'wiki/Article/en.md',
+            'wiki/Article/fr.md',
+            'wiki/Article/pt-br.md',
+            'wiki/Article/zh-tw.md',
+        ]
+
+        utils.create_files(root, *((path, '# Article') for path in article_paths))
+        utils.stage_all_and_commit("add articles")
+
+        utils.create_files(root, *(
+            (article_path, '# Article\n\nThis is an article in English.') for article_path in
+            utils.take(article_paths, "en.md")
+        ))
+        utils.stage_all_and_commit("modify english articles")
+
+        exit_code = outdater.main("--base-commit", "HEAD^", f"{outdater.AUTOFIX_FLAG}")
+
+        assert exit_code == 1
+
+        assert utils.get_changed_files() == []
```

### Comparing `osu-wiki-tools-2.2.1/tests/test_code_block_parser.py` & `osu_wiki_tools-2.3.0/tests/test_code_block_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_comment_parser.py` & `osu_wiki_tools-2.3.0/tests/test_comment_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_file_utils.py` & `osu_wiki_tools-2.3.0/tests/test_file_utils.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_identifier_parser.py` & `osu_wiki_tools-2.3.0/tests/test_identifier_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_link_checker.py` & `osu_wiki_tools-2.3.0/tests/test_link_checker.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_link_parser.py` & `osu_wiki_tools-2.3.0/tests/test_link_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_redirect_parser.py` & `osu_wiki_tools-2.3.0/tests/test_redirect_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_reference_parser.py` & `osu_wiki_tools-2.3.0/tests/test_reference_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_visual_tests.py` & `osu_wiki_tools-2.3.0/tests/test_visual_tests.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/tests/test_yaml_rules.py` & `osu_wiki_tools-2.3.0/tests/test_yaml_rules.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/article_parser.py` & `osu_wiki_tools-2.3.0/wikitools/article_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/code_block_parser.py` & `osu_wiki_tools-2.3.0/wikitools/code_block_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/comment_parser.py` & `osu_wiki_tools-2.3.0/wikitools/comment_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/errors.py` & `osu_wiki_tools-2.3.0/wikitools/errors.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/file_utils.py` & `osu_wiki_tools-2.3.0/wikitools/file_utils.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/git_utils.py` & `osu_wiki_tools-2.3.0/wikitools/git_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
                 cmd, proc.returncode, out, err
             )
         )
     return out
 
 
 def git_diff(*file_paths, base_commit=""):
-    res = git("diff", "--diff-filter=d", "--name-only", f"{base_commit}^", "--", *file_paths)
+    res = git("diff", "--diff-filter=d", "--name-only", base_commit, "--", *file_paths)
     return res.splitlines()
 
 
 def get_first_branch_commit():
     """
     Gets the first commit of the current branch where it diverges from master.
```

### Comparing `osu-wiki-tools-2.2.1/wikitools/identifier_parser.py` & `osu_wiki_tools-2.3.0/wikitools/identifier_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/link_checker.py` & `osu_wiki_tools-2.3.0/wikitools/link_checker.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/link_parser.py` & `osu_wiki_tools-2.3.0/wikitools/link_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/redirect_parser.py` & `osu_wiki_tools-2.3.0/wikitools/redirect_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/reference_parser.py` & `osu_wiki_tools-2.3.0/wikitools/reference_parser.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools/yaml_rules.py` & `osu_wiki_tools-2.3.0/wikitools/yaml_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     "no_native_review",
     "no_native_review_since",
 
     # Newspost tags
     "date",
     "layout",
     "title",
+    "series",
     "tumblr_url",
 })
 
 
 class _JunkMatcher:
     def match_file(self, p: str):
         return not p.endswith(".md")
```

### Comparing `osu-wiki-tools-2.2.1/wikitools_cli/commands/check_links.py` & `osu_wiki_tools-2.3.0/wikitools_cli/commands/check_links.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools_cli/commands/check_outdated_articles.py` & `osu_wiki_tools-2.3.0/wikitools_cli/commands/check_outdated_articles.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,16 @@
         )
     )
     print("\n".join(console.red(f"* {filename}") for filename in filenames))
 
 
 def parse_args(args):
     parser = argparse.ArgumentParser(description=__doc__, formatter_class=argparse.RawTextHelpFormatter, usage="%(prog)s check-outdated-articles [options]")
-    parser.add_argument("-b", "--base-commit", help="commit since which to look for changes")
-    parser.add_argument("-o", "--outdated-since", default="", help=f"commit hash for the {OUTDATED_HASH_TAG} tag, uses the value of --base-commit if unspecified")
+    parser.add_argument("-b", "--base-commit", default="master", help="commit since which to look for changes")
+    parser.add_argument("-o", "--outdated-since", help=f"commit hash for the {OUTDATED_HASH_TAG} tag, uses the first commit where HEAD diverged from master if unspecified")
     parser.add_argument("-a", "--all", default=False, action="store_true", help="look for incorrect hashes in all outdated articles")
     parser.add_argument(f"{AUTOFIX_FLAG_SHORT}", f"{AUTOFIX_FLAG}", default=False, action="store_true", help=f"automatically add `{OUTDATED_HASH_TAG}: {{hash}}` to outdated articles")
     parser.add_argument(f"{AUTOCOMMIT_FLAG_SHORT}", f"{AUTOCOMMIT_FLAG}", default=False, action="store_true", help=f"automatically commit changes")
     parser.add_argument("-r", "--root", help="specify repository root, current working directory assumed otherwise")
     parser.add_argument("--no-recommend-autofix", action='store_true', help=f"don't recommend rerunning the script with {AUTOFIX_FLAG}")
     return parser.parse_args(args)
 
@@ -102,15 +102,15 @@
     return filter(file_utils.is_translation, git_utils.git_diff('wiki/**/*.md', base_commit=base_commit))
 
 
 def list_modified_originals(base_commit):
     return git_utils.git_diff('wiki/**/en.md', base_commit=base_commit)
 
 
-def outdate_translations(*translations, outdated_hash=""):
+def outdate_translations(*translations, outdated_hash):
     """
     Write outdated hash and marker to several translations at once.
     """
 
     for article_file in translations:
         with open(article_file, "r", encoding='utf-8') as fd:
             front_matter = article_parser.load_front_matter(fd)
@@ -147,70 +147,64 @@
 def main(*args):
     args = parse_args(args)
     exit_code = 0
 
     if args.root:
         changed_cwd = file_utils.ChangeDirectory(args.root)
 
-    base_commit = args.base_commit or git_utils.get_first_branch_commit()
-
-    if not base_commit and not args.all:
-        print(f"{console.red('Error:')} neither --base-commit (unable to obtain automatically) nor --all were specified; nothing to do.")
-        exit_code = 1
-        if args.root:
-            del changed_cwd
-        return exit_code
-
     modified_translations = set()
     with_bad_hashes = list()
 
-    if not args.all and base_commit:
-        modified_translations = set(list_modified_translations(base_commit))
-        with_bad_hashes = list(check_commit_hashes(modified_translations))
-    elif args.all:
+    if args.all:
         all_translations = file_utils.list_all_translations(file_utils.list_all_article_dirs())
         with_bad_hashes = list(check_commit_hashes(all_translations))
+    else:
+        modified_translations = set(list_modified_translations(args.base_commit))
+        with_bad_hashes = list(check_commit_hashes(modified_translations))
+
+    outdated_hash = None
 
     if with_bad_hashes:
-        print_bad_hash_error(*with_bad_hashes, outdated_hash=args.outdated_since or base_commit)
+        outdated_hash = args.outdated_since or git_utils.get_first_branch_commit()
+        print_bad_hash_error(*with_bad_hashes, outdated_hash=outdated_hash)
         print()
         exit_code = 1
 
-    if not base_commit:
-        if args.root:
-            del changed_cwd
-        return exit_code
-
-    modified_originals = list_modified_originals(base_commit)
+    modified_originals = list_modified_originals(args.base_commit)
     if modified_originals:
         all_translations = file_utils.list_all_translations(sorted(os.path.dirname(tl) for tl in modified_originals))
         translations_to_outdate = list(list_outdated_translations(all_translations, modified_translations))
         if translations_to_outdate:
-            outdated_hash = args.outdated_since or base_commit
+            outdated_hash = outdated_hash or args.outdated_since or git_utils.get_first_branch_commit()
 
             should_autofix = getattr(args, AUTOFIX_FLAG[2:], False)
             should_autocommit = getattr(args, AUTOCOMMIT_FLAG[2:], False)
             if should_autofix:
                 print(console.green('{} specified, outdating translations...'.format(AUTOFIX_FLAG)))
-                outdate_translations(*translations_to_outdate, outdated_hash=outdated_hash)
-                if not should_autocommit:
-                    print(console.green('Done! To commit the changes, run:'))
-                    print(console.green('\tgit add {}; git commit -m "outdate translations"'.format(
-                        " ".join(translations_to_outdate)
-                    )))
+
+                if outdated_hash:
+                    outdate_translations(*translations_to_outdate, outdated_hash=outdated_hash)
+                    if not should_autocommit:
+                        print(console.green('Done! To commit the changes, run:'))
+                        print(console.green('\tgit add {}; git commit -m "outdate translations"'.format(
+                            " ".join(translations_to_outdate)
+                        )))
+                    else:
+                        print(console.green('{} specified, committing changes...'.format(AUTOCOMMIT_FLAG)))
+                        git_utils.git("add", *translations_to_outdate)
+                        git_utils.git("commit", "-m", "outdate translations")
+                        print(console.green('Done! The changes have been committed for you.'))
+                        print()
+                        print(git_utils.git("show", "HEAD", "--no-patch"))
+                        print("Changed files:")
+                        for file_path in translations_to_outdate:
+                            print(console.green(f"* {file_path}"))
                 else:
-                    print(console.green('{} specified, committing changes...'.format(AUTOCOMMIT_FLAG)))
-                    git_utils.git("add", *translations_to_outdate)
-                    git_utils.git("commit", "-m", "outdate translations")
-                    print(console.green('Done! The changes have been committed for you.'))
-                    print()
-                    print(git_utils.git("show", "HEAD", "--no-patch"))
-                    print("Changed files:")
-                    for file_path in translations_to_outdate:
-                        print(console.green(f"* {file_path}"))
+                    print(f"{console.red('Error:')} --outdated-since was not specified and HEAD has not diverged from master.")
+                    exit_code = 1
             else:
                 print_translations_to_outdate(*translations_to_outdate, outdated_hash=outdated_hash, no_recommend_autofix=args.no_recommend_autofix)
                 exit_code = 1
 
         else:
             print(f"{console.grey('Notice:')} all unedited translations are properly outdated.")
```

### Comparing `osu-wiki-tools-2.2.1/wikitools_cli/commands/check_yaml.py` & `osu_wiki_tools-2.3.0/wikitools_cli/commands/check_yaml.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools_cli/osu_wiki_tools.py` & `osu_wiki_tools-2.3.0/wikitools_cli/osu_wiki_tools.py`

 * *Files identical despite different names*

### Comparing `osu-wiki-tools-2.2.1/wikitools_cli/update_tournament_countries.py` & `osu_wiki_tools-2.3.0/wikitools_cli/update_tournament_countries.py`

 * *Files identical despite different names*

