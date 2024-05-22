# Comparing `tmp/slate-nlp-1.1.1.tar.gz` & `tmp/slate_nlp-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slate-nlp-1.1.1.tar", last modified: Fri Apr 14 03:42:01 2023, max compression
+gzip compressed data, was "slate_nlp-1.1.2.tar", last modified: Wed May 22 01:12:47 2024, max compression
```

## Comparing `slate-nlp-1.1.1.tar` & `slate_nlp-1.1.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.241189 slate-nlp-1.1.1/
--rw-r--r--   0 jkum0593   (503) staff       (20)      121 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/.gitignore
--rw-r--r--   0 jkum0593   (503) staff       (20)      780 2023-04-14 03:03:02.000000 slate-nlp-1.1.1/LICENSE.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)    22691 2023-04-14 03:42:01.241028 slate-nlp-1.1.1/PKG-INFO
--rw-r--r--   0 jkum0593   (503) staff       (20)    20942 2023-04-10 11:28:24.000000 slate-nlp-1.1.1/README.md
--rw-r--r--   0 jkum0593   (503) staff       (20)      213 2022-10-24 01:09:40.000000 slate-nlp-1.1.1/_config.yml
-drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.228370 slate-nlp-1.1.1/_includes/
--rw-r--r--   0 jkum0593   (503) staff       (20)      399 2022-10-24 01:08:59.000000 slate-nlp-1.1.1/_includes/head-custom-google-analytics.html
--rw-r--r--   0 jkum0593   (503) staff       (20)     3596 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/ideas-for-improvement.md
--rw-r--r--   0 jkum0593   (503) staff       (20)     3854 2023-04-10 06:01:14.000000 slate-nlp-1.1.1/ner-book.config
-drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.231468 slate-nlp-1.1.1/paper/
--rw-r--r--   0 jkum0593   (503) staff       (20)    12450 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/acl19slate.bib
--rw-r--r--   0 jkum0593   (503) staff       (20)   447789 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/acl19slate.pdf
--rw-r--r--   0 jkum0593   (503) staff       (20)    22052 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/acl19slate.sty
--rw-r--r--   0 jkum0593   (503) staff       (20)    24066 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/acl19slate.tex
--rw-r--r--   0 jkum0593   (503) staff       (20)     2244 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/comparison.tex
--rw-r--r--   0 jkum0593   (503) staff       (20)      434 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/makefile
--rw-r--r--   0 jkum0593   (503) staff       (20)     4356 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/post-publish-supp.tex
--rw-r--r--   0 jkum0593   (503) staff       (20)   342538 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/screenshot-adjudicate.png
--rw-r--r--   0 jkum0593   (503) staff       (20)   198920 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/paper/screenshot.png
--rw-r--r--   0 jkum0593   (503) staff       (20)     1095 2023-04-14 03:41:56.000000 slate-nlp-1.1.1/pyproject.toml
--rw-r--r--   0 jkum0593   (503) staff       (20)       38 2023-04-14 03:42:01.241231 slate-nlp-1.1.1/setup.cfg
-drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.236742 slate-nlp-1.1.1/slate/
--rw-r--r--   0 jkum0593   (503) staff       (20)       15 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/slate/__init__.py
--rw-r--r--   0 jkum0593   (503) staff       (20)       66 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/slate/__main__.py
--rw-r--r--   0 jkum0593   (503) staff       (20)    19913 2023-04-10 11:27:42.000000 slate-nlp-1.1.1/slate/annotate.py
--rw-r--r--   0 jkum0593   (503) staff       (20)     9207 2023-04-07 01:20:03.000000 slate-nlp-1.1.1/slate/config.py
--rw-r--r--   0 jkum0593   (503) staff       (20)    38565 2023-04-10 11:29:42.000000 slate-nlp-1.1.1/slate/data.py
--rw-r--r--   0 jkum0593   (503) staff       (20)    21415 2023-04-10 06:31:20.000000 slate-nlp-1.1.1/slate/view.py
--rwxr-xr-x   0 jkum0593   (503) staff       (20)       95 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/slate.py
-drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.237748 slate-nlp-1.1.1/slate_nlp.egg-info/
--rw-r--r--   0 jkum0593   (503) staff       (20)    22691 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/PKG-INFO
--rw-r--r--   0 jkum0593   (503) staff       (20)     1291 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)        1 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)       46 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/entry_points.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)        6 2023-04-14 03:42:01.000000 slate-nlp-1.1.1/slate_nlp.egg-info/top_level.txt
-drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.238489 slate-nlp-1.1.1/tutorial/
--rw-r--r--   0 jkum0593   (503) staff       (20)    17655 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/config-example.txt
-drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2023-04-14 03:42:01.240660 slate-nlp-1.1.1/tutorial/data/
--rw-r--r--   0 jkum0593   (503) staff       (20)    12086 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)       55 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.category.annotations0
--rw-r--r--   0 jkum0593   (503) staff       (20)       87 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.category.annotations1
--rw-r--r--   0 jkum0593   (503) staff       (20)      166 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.category.annotations2
--rw-r--r--   0 jkum0593   (503) staff       (20)      220 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.category.annotations3
--rw-r--r--   0 jkum0593   (503) staff       (20)        6 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.link.annotations0
--rw-r--r--   0 jkum0593   (503) staff       (20)       12 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.link.annotations1
--rw-r--r--   0 jkum0593   (503) staff       (20)       18 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.link.annotations2
--rw-r--r--   0 jkum0593   (503) staff       (20)       24 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data0.txt.link.annotations3
--rw-r--r--   0 jkum0593   (503) staff       (20)    14560 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_data1.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)       32 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/input_file_list.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)      220 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/list_with_disagreements.category.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)      198 2022-10-24 01:03:43.000000 slate-nlp-1.1.1/tutorial/data/list_with_disagreements.link.txt
--rw-r--r--   0 jkum0593   (503) staff       (20)     2318 2023-04-10 11:28:10.000000 slate-nlp-1.1.1/tutorial/label.md
--rw-r--r--   0 jkum0593   (503) staff       (20)     2417 2023-04-10 11:28:14.000000 slate-nlp-1.1.1/tutorial/link.md
--rw-r--r--   0 jkum0593   (503) staff       (20)     4628 2023-04-10 06:25:50.000000 slate-nlp-1.1.1/tutorial/ner.md
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2024-05-22 01:12:47.176037 slate_nlp-1.1.2/
+-rw-r--r--   0 jkum0593   (503) staff       (20)      121 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/.gitignore
+-rw-r--r--   0 jkum0593   (503) staff       (20)      780 2023-04-14 03:03:02.000000 slate_nlp-1.1.2/LICENSE.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)    24911 2024-05-22 01:12:47.175577 slate_nlp-1.1.2/PKG-INFO
+-rw-r--r--   0 jkum0593   (503) staff       (20)    23162 2023-05-07 10:34:19.000000 slate_nlp-1.1.2/README.md
+-rw-r--r--   0 jkum0593   (503) staff       (20)      213 2022-10-24 01:09:40.000000 slate_nlp-1.1.2/_config.yml
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2024-05-22 01:12:47.152379 slate_nlp-1.1.2/_includes/
+-rw-r--r--   0 jkum0593   (503) staff       (20)      399 2022-10-24 01:08:59.000000 slate_nlp-1.1.2/_includes/head-custom-google-analytics.html
+-rw-r--r--   0 jkum0593   (503) staff       (20)     3596 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/ideas-for-improvement.md
+-rw-r--r--   0 jkum0593   (503) staff       (20)    10565 2024-05-22 01:11:51.000000 slate_nlp-1.1.2/ner-book.config
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2024-05-22 01:12:47.157899 slate_nlp-1.1.2/paper/
+-rw-r--r--   0 jkum0593   (503) staff       (20)    12450 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/acl19slate.bib
+-rw-r--r--   0 jkum0593   (503) staff       (20)   447789 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/acl19slate.pdf
+-rw-r--r--   0 jkum0593   (503) staff       (20)    22052 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/acl19slate.sty
+-rw-r--r--   0 jkum0593   (503) staff       (20)    24066 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/acl19slate.tex
+-rw-r--r--   0 jkum0593   (503) staff       (20)     2244 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/comparison.tex
+-rw-r--r--   0 jkum0593   (503) staff       (20)      434 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/makefile
+-rw-r--r--   0 jkum0593   (503) staff       (20)     4356 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/post-publish-supp.tex
+-rw-r--r--   0 jkum0593   (503) staff       (20)   342538 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/screenshot-adjudicate.png
+-rw-r--r--   0 jkum0593   (503) staff       (20)   198920 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/paper/screenshot.png
+-rw-r--r--   0 jkum0593   (503) staff       (20)     1095 2024-05-22 01:07:11.000000 slate_nlp-1.1.2/pyproject.toml
+-rw-r--r--   0 jkum0593   (503) staff       (20)       38 2024-05-22 01:12:47.176083 slate_nlp-1.1.2/setup.cfg
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2024-05-22 01:12:47.165507 slate_nlp-1.1.2/slate/
+-rw-r--r--   0 jkum0593   (503) staff       (20)       15 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/slate/__init__.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)       66 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/slate/__main__.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)    19913 2024-01-25 06:25:43.000000 slate_nlp-1.1.2/slate/annotate.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)     9207 2023-04-07 01:20:03.000000 slate_nlp-1.1.2/slate/config.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)    39630 2023-06-10 04:40:47.000000 slate_nlp-1.1.2/slate/data.py
+-rw-r--r--   0 jkum0593   (503) staff       (20)    21415 2023-04-14 03:57:58.000000 slate_nlp-1.1.2/slate/view.py
+-rwxr-xr-x   0 jkum0593   (503) staff       (20)       95 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/slate.py
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2024-05-22 01:12:47.175001 slate_nlp-1.1.2/slate_nlp.egg-info/
+-rw-r--r--   0 jkum0593   (503) staff       (20)    24911 2024-05-22 01:12:47.000000 slate_nlp-1.1.2/slate_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 jkum0593   (503) staff       (20)     1291 2024-05-22 01:12:47.000000 slate_nlp-1.1.2/slate_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)        1 2024-05-22 01:12:47.000000 slate_nlp-1.1.2/slate_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)       46 2024-05-22 01:12:47.000000 slate_nlp-1.1.2/slate_nlp.egg-info/entry_points.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)        6 2024-05-22 01:12:47.000000 slate_nlp-1.1.2/slate_nlp.egg-info/top_level.txt
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2024-05-22 01:12:47.169225 slate_nlp-1.1.2/tutorial/
+-rw-r--r--   0 jkum0593   (503) staff       (20)    17655 2023-05-13 04:43:54.000000 slate_nlp-1.1.2/tutorial/config-example.txt
+drwxr-xr-x   0 jkum0593   (503) staff       (20)        0 2024-05-22 01:12:47.174568 slate_nlp-1.1.2/tutorial/data/
+-rw-r--r--   0 jkum0593   (503) staff       (20)    12086 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)       55 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt.category.annotations0
+-rw-r--r--   0 jkum0593   (503) staff       (20)       87 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt.category.annotations1
+-rw-r--r--   0 jkum0593   (503) staff       (20)      166 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt.category.annotations2
+-rw-r--r--   0 jkum0593   (503) staff       (20)      220 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt.category.annotations3
+-rw-r--r--   0 jkum0593   (503) staff       (20)        6 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt.link.annotations0
+-rw-r--r--   0 jkum0593   (503) staff       (20)       12 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt.link.annotations1
+-rw-r--r--   0 jkum0593   (503) staff       (20)       18 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt.link.annotations2
+-rw-r--r--   0 jkum0593   (503) staff       (20)       24 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data0.txt.link.annotations3
+-rw-r--r--   0 jkum0593   (503) staff       (20)    14560 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_data1.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)       32 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/input_file_list.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)      220 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/list_with_disagreements.category.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)      198 2022-10-24 01:03:43.000000 slate_nlp-1.1.2/tutorial/data/list_with_disagreements.link.txt
+-rw-r--r--   0 jkum0593   (503) staff       (20)     2318 2023-04-14 03:57:58.000000 slate_nlp-1.1.2/tutorial/label.md
+-rw-r--r--   0 jkum0593   (503) staff       (20)     2417 2023-04-14 03:57:58.000000 slate_nlp-1.1.2/tutorial/link.md
+-rw-r--r--   0 jkum0593   (503) staff       (20)     4847 2023-04-25 13:03:16.000000 slate_nlp-1.1.2/tutorial/ner.md
```

### Comparing `slate-nlp-1.1.1/LICENSE.txt` & `slate_nlp-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/PKG-INFO` & `slate_nlp-1.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: slate-nlp
-Version: 1.1.1
-Summary: A terminal-based text annotation tool
-Author-email: "Jonathan K. Kummerfeld" <jonathan.kummerfeld@sydney.edu.au>
-License: Copyright (c) 2016-2023 Jonathan K Kummerfeld <jonathan.kummerfeld@sydney.edu.au>
-        
-        Permission to use, copy, modify, and/or distribute this software for any
-        purpose with or without fee is hereby granted, provided that the above
-        copyright notice and this permission notice appear in all copies.
-        
-        THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-        REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-        FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
-        INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
-        LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
-        OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
-        PERFORMANCE OF THIS SOFTWARE.
-        
-Project-URL: Homepage, https://jkk.name/slate/
-Project-URL: Bug Tracker, https://github.com/jkkummerfeld/slate/issues
-Keywords: nlp,annotation,labeling,natural-language-processing,text-annotation
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: !=3.0.*,!=3.1.*,!=3.2.*,<4,>=2.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 This is a tool for labeling text documents.
 Slate supports annotation at different scales (spans of characters, tokens, and lines, or a document) and of different types (free text, labels, and links).
 This covers a range of tasks, such as Part-of-Speech tagging, Named Entity Recognition, Text Classification (including Sentiment Analysis), Discourse Structure, and more.
 
 Why use this tool over the range of other text annotation tools out there?
 
 - Fast
@@ -171,37 +138,74 @@
 
 - Create a repository containing (1) the annotation guide, (2) the data to be annotated divided into user-specific folders.
 - Each annotator downloaded slate and used it to do their annotations and commit the files to the repository.
 - Either the whole group or the project leader went through files that were annotated by multiple people, using the adjudication mode in the tool.
 
 ### Comparing Annotations
 
-To use adjudication mode, create a file, `example.txt`, similar to the following (you can have as many annotators as you like):
+The tool supports displaying annotations for the purpose of adjudicating disagreements.
+There are two steps involved.
+Specifically, you can request that a set of other annotation files be read.
+Then, whenever one of those annotation files includes something that your current adjudication does not, the text is shown in red.
+
+#### Data list file creation
+A  data list file contains a series of lines in the format:
 
 ```
-raw-text0 adjudicated-anno0 ((1000,),(1000,)) anno0.1 anno0.2 anno0.3
-raw-text1 adjudicated-anno1 ((1000,),(1000,)) anno1.1 anno1.2
-raw-text2 adjudicated-anno2 ((1000,),(1000,)) anno2.1 anno2.2 anno2.3 anno2.4
+raw_file [output_file [cur_position [other_annotations]]]
 ```
 
-To save time, it is best to initialise `adjudicated-annoN` with the lines everyone agreed on:
+For example, this line says there is a raw text file `my-book.txt`, that the adjudications should be saved in `annotations-adjudicated.txt`, that annotation should start at the very start of `my-book.txt` and that there are three existing annotations to be compared:
+
+```
+my-book.txt annotations-adjudicated.txt ((0, 0), (0, 0)) my-book.txt.annotations1 my-book.txt.annotations2 my-book.txt.annotations3
+```
+
+Note: you can have as many "other_annotation" files as you want.
+
+#### Run slate with the data list file
+Now run slate as follows:
 
 ```
-for i in 0 1 2 ; do
-  count=`ls anno${i}.* | wc -l`
-  cat anno${i}.* | sort | uniq -c | awk -v count=$count '$1 == count' | sed 's/^ *[0-9]* *//' > matching
-done
+python slate.py -d data-list-file [any other arguments]
 ```
 
-Then run the tool as if you are annotating, for example for linking lines:
+#### Example
+
+The tutorial folder contains two example data list files:
+
+- `tutorial/data/list_with_disagreements.category.txt`
+- `tutorial/data/list_with_disagreements.link.txt`
+
+You can use them as follows:
 
 ```
-python ../learn-anno/slate/slate.py -d example.txt -pf -t link -s line -o -l log.adj.txt --do-not-show-linked
+cd tutorial/data
+python ../../slate.py -d list_with_disagreements.category.txt -t categorical -s token
 ```
 
+#### Efficiency Tip
+
+You can save time by putting annotations that all annotators agreed on into the `annotations-adjudicated.txt` file.
+This bash pipeline will do that if you replace:
+
+- `ANNOTATION_FILES` with the names of all of your annotation files, separated by spaces
+- `N_FILES` with the number of annotation files you have
+
+```
+cat ANNOTATION_FILES | sort | uniq -c | awk -v count=N_FILES '$1 == count' | sed 's/^ *[0-9]* *//' > annotations-adjudicated.txt
+```
+
+Breaking this down, it does the following:
+- `cat ANNOTATION_FILES `, print the annotation files in the terminal
+- `sort `, sort their contents together
+- `uniq -c `, where there are consecutive lines that are the same, only keep one, and also indicate how many times each line occurred
+- `awk -v count=N_FILES '$1 == count' `, only keep lines where the number at the start matches `N_FILES`
+- `sed 's/^ *[0-9]* *//' > annotations-adjudicated.txt`, remove the number at the start of the line (placed there by the `uniq` command)
+
 ## Detailed Usage Instructions
 
 ### Invocation options
 
 ```
 usage: slate.py [-h] [-d DATA_LIST [DATA_LIST ...]] [-t {categorical,link}]
                 [-s {character,token,line,document}] [-c CONFIG_FILE] [-l LOG_PREFIX] [-ld]
@@ -247,15 +251,17 @@
 
 ```bash
 python slate.py @arguments.txt
 ```
 
 ### Keybindings
 
-The tool shows files one at a time in plain text. Default commands are:
+The tool shows files one at a time in plain text. Default commands are shown below.
+
+Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
 
 Type                        | Key                                                       | Labelling Affect                 | Linking Affect
 --------------------------- | --------------------------------------------------------- | -------------------------------- | ---------------------
 Movement                    | <kbd>j</kbd> or <kbd>&larr;</kbd>                         | move to the left                 | move selected item to the left
 &nbsp;                      | <kbd>i</kbd> or <kbd>&uarr;</kbd>                         | move up a line                   | move selected item up a line
 &nbsp;                      | <kbd>o</kbd> or <kbd>&darr;</kbd>                         | move down a line                 | move selected item down a line
 &nbsp;                      | <kbd>;</kbd> or <kbd>&rarr;</kbd>                         | move to the right                | move selected item to the right
@@ -304,16 +310,14 @@
 &nbsp;                      | Normal | <kbd>h</kbd>                                    | toggle help info (default on)    
 &nbsp;                      | Normal | <kbd>{</kbd> or <kbd>PAGE-UP</kbd>              | shift view up 5 lines
 &nbsp;                      | Normal | <kbd>}</kbd> or <kbd>PAGE-DOWN</kbd>            | shift view down 5 lines
 &nbsp;                      | Normal | <kbd>></kbd> then <kbd>p</kbd>                  | toggle showing progress through files
 &nbsp;                      | Normal | <kbd>></kbd> then <kbd>l</kbd>                  | toggle showing legend for labels
 &nbsp;                      | Normal | <kbd>></kbd> then <kbd>m</kbd>                  | toggle showing the mark on the current item
 
-Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
-
 ### Misc
 
 To annotate multiple files, specify more than one as an argument.
 For greater control, provide a list of files in a file specified with `--data-list` / `-d`.
 The list should be formatted as follows, where [] indicate optional values:
 
 ```
@@ -332,14 +336,29 @@
 Note, the `-o` flag is added so it will allow you to edit the annotations you have already created.
 Otherwise the system will complain that you are overwriting existing annotation files.
 
 When the `additional_annotation_files` are included it activates an adjudication mode.
 By default, all annotations that appear in all additional files are added to the current annotations.
 Disagreements are coloured in the text, but will disappear once a decision is made (using the normal annotation commands).
 
+### Running in Windows
+
+Users have reported a range of issues when trying to run slate:
+
+- Underlining, which is used to show the currently selected text, does not work.
+- Shift keys do not work
+
+Here are a few things to try that others have found helpful:
+
+- Use the Windows Subsystem for Linux (WSL) with Ubuntu
+- Reinstall ncurses, or install windows-curses
+- If you hit an encoding issue, try converting your raw text file to ASCII
+- Try powershell
+- Use a config file with different keybindings, to avoid needing shift
+
 ## Customisation
 
 Colours and keys are customisable. For labelling, the default is:
 
  - Underlined, current selected item
  - Green on black, 'a' items
  - Blue on black, 's' items
@@ -396,14 +415,16 @@
 Label:          O                         SPACE_a green
 Label:          LOC                       SPACE_s blue
 Label:          PER                       SPACE_d red
 Label:          ORG                       SPACE_f yellow
 Label:          MISC                      SPACE_v magenta
 ```
 
+For an example of a custom config file, see [ner-book.config](ner-book.config)
+
 The current set of available colours is: [green, blue, white, cyan, magenta, red, yellow].
 Note that by default white is used for regular text and cyan is used for cases where multiple labels apply to the same content.
 
 To define more colours, edit the top of `slate/config.py`.
 By varying both the text colour (foreground) and background colour you can achieve quite a range of variations.
 You can also define any RGB colour you want using the curses [init_color](https://docs.python.org/3/library/curses.html#curses.init_color) function and the [init_pair](https://docs.python.org/3/library/curses.html#curses.init_pair) function.
```

### Comparing `slate-nlp-1.1.1/ideas-for-improvement.md` & `slate_nlp-1.1.2/ideas-for-improvement.md`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/paper/acl19slate.bib` & `slate_nlp-1.1.2/paper/acl19slate.bib`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/paper/acl19slate.pdf` & `slate_nlp-1.1.2/paper/acl19slate.pdf`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/paper/acl19slate.sty` & `slate_nlp-1.1.2/paper/acl19slate.sty`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/paper/acl19slate.tex` & `slate_nlp-1.1.2/paper/acl19slate.tex`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/paper/comparison.tex` & `slate_nlp-1.1.2/paper/comparison.tex`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/paper/post-publish-supp.tex` & `slate_nlp-1.1.2/paper/post-publish-supp.tex`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/paper/screenshot-adjudicate.png` & `slate_nlp-1.1.2/paper/screenshot-adjudicate.png`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/paper/screenshot.png` & `slate_nlp-1.1.2/paper/screenshot.png`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/pyproject.toml` & `slate_nlp-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slate-nlp"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   {name="Jonathan K. Kummerfeld", email="jonathan.kummerfeld@sydney.edu.au"},
 ]
 description = "A terminal-based text annotation tool"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 requires-python = '>=2.6, !=3.0.*, !=3.1.*, !=3.2.*, <4'
```

### Comparing `slate-nlp-1.1.1/slate/annotate.py` & `slate_nlp-1.1.2/slate/annotate.py`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/slate/config.py` & `slate_nlp-1.1.2/slate/config.py`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/slate/data.py` & `slate_nlp-1.1.2/slate/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
                 position_text.append(parts[next_part])
                 first = False
                 next_part += 1
             position_text = ' '.join(position_text)
 
             span = eval(position_text)
             position = Span(config.annotation, d, span)
+            if (not position.doc.valid_pos(position.start)) or (not position.doc.valid_pos(position.end)):
+                raise Exception("Invalid starting location in data list file.")
 
         # Additional annotations (used when comparing annotations)
         annotations = []
         if len(parts) > next_part:
             annotations = parts[next_part:]
         filenames.append((raw_file, position, output_file, annotations))
 
@@ -90,14 +92,35 @@
             for token in line.strip().split():
                 if self.first_char is None:
                     self.first_char = (len(self.tokens) - 1, 0, 0)
                 self.last_char = (len(self.tokens) - 1, len(cur), len(token) - 1)
                 cur.append(token)
         assert self.first_char is not None, "Empty document: {}".format(filename)
 
+    def valid_pos(self, pos):
+        if len(pos) == 0:
+            return True
+        # Check line
+        line = pos[0]
+        if line < 0 or line >= len(self.tokens):
+            return False
+        if len(self.tokens[line]) == 0:
+            return False
+        # Check token
+        if len(pos) >= 2:
+            tok = pos[1]
+            if tok < 0 or tok >= len(self.tokens[line]):
+                return False
+            # Check character
+            if len(pos) == 3:
+                char = pos[2]
+                if char < 0 or char >= len(self.tokens[line][tok]):
+                    return False
+        return True
+
     def get_3tuple(self, partial, start):
         if len(partial) == 3:
             return partial
         elif len(partial) == 0:
             if start: return self.first_char
             else: return self.last_char
         else:
@@ -138,27 +161,28 @@
                                 ctoken += 1
                                 cchar = 0
                             else:
                                 cchar += 1
         return self.search_cache[text]
 
     def get_moved_pos(self, pos, right=0, down=0, maxjump=False, skip_blank=True):
-        """Calculate a shifted version of  a given a position in this document.
+        """Calculate a shifted version of a given position in this document.
 
         Co-ordinates are (line number, token number, character number), with
         (0,0, 0) as the top left, tokens increasing left to right and lines
         increasing top to bottom.
         """
         if len(pos) == 0: # This is the whole document, can't move
             return pos
         elif len(pos) == 1: # This is a line
             npos = pos[0]
             # Interpret left/right as also being up/down for lines
             if down == 0 and right != 0:
                 down = right
+
             if maxjump:
                 if down < 0: npos = self.first_char[0]
                 elif down > 0: npos = self.last_char[0]
             else:
                 # Shift incrementally so we can optionally only count lines
                 # that have tokens.
                 shift = down
@@ -612,15 +636,27 @@
         self.labels = set()
         if type(init_label) == set:
             self.labels.update(init_label)
         elif init_label is not None:
             self.labels.add(init_label)
 
     def __eq__(self, other):
-        return self.spans == other.spans and self.labels == other.labels and self.doc == other.doc
+        if self.doc != other.doc:
+            return False
+
+        if self.labels != other.labels:
+            return False
+
+        if len(self.spans) != len(other.spans):
+            return False
+        else:
+            for span in self.spans:
+                if span not in other.spans:
+                    return False
+        return True
 
     def __str__(self):
         labels = []
         for label in self.labels:
             labels.append(str(label))
         labels = ' '.join(labels)
```

### Comparing `slate-nlp-1.1.1/slate/view.py` & `slate_nlp-1.1.2/slate/view.py`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/slate_nlp.egg-info/PKG-INFO` & `slate_nlp-1.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slate-nlp
-Version: 1.1.1
+Version: 1.1.2
 Summary: A terminal-based text annotation tool
 Author-email: "Jonathan K. Kummerfeld" <jonathan.kummerfeld@sydney.edu.au>
 License: Copyright (c) 2016-2023 Jonathan K Kummerfeld <jonathan.kummerfeld@sydney.edu.au>
         
         Permission to use, copy, modify, and/or distribute this software for any
         purpose with or without fee is hereby granted, provided that the above
         copyright notice and this permission notice appear in all copies.
@@ -171,37 +171,74 @@
 
 - Create a repository containing (1) the annotation guide, (2) the data to be annotated divided into user-specific folders.
 - Each annotator downloaded slate and used it to do their annotations and commit the files to the repository.
 - Either the whole group or the project leader went through files that were annotated by multiple people, using the adjudication mode in the tool.
 
 ### Comparing Annotations
 
-To use adjudication mode, create a file, `example.txt`, similar to the following (you can have as many annotators as you like):
+The tool supports displaying annotations for the purpose of adjudicating disagreements.
+There are two steps involved.
+Specifically, you can request that a set of other annotation files be read.
+Then, whenever one of those annotation files includes something that your current adjudication does not, the text is shown in red.
 
+#### Data list file creation
+A  data list file contains a series of lines in the format:
+
+```
+raw_file [output_file [cur_position [other_annotations]]]
 ```
-raw-text0 adjudicated-anno0 ((1000,),(1000,)) anno0.1 anno0.2 anno0.3
-raw-text1 adjudicated-anno1 ((1000,),(1000,)) anno1.1 anno1.2
-raw-text2 adjudicated-anno2 ((1000,),(1000,)) anno2.1 anno2.2 anno2.3 anno2.4
+
+For example, this line says there is a raw text file `my-book.txt`, that the adjudications should be saved in `annotations-adjudicated.txt`, that annotation should start at the very start of `my-book.txt` and that there are three existing annotations to be compared:
+
 ```
+my-book.txt annotations-adjudicated.txt ((0, 0), (0, 0)) my-book.txt.annotations1 my-book.txt.annotations2 my-book.txt.annotations3
+```
+
+Note: you can have as many "other_annotation" files as you want.
+
+#### Run slate with the data list file
+Now run slate as follows:
+
+```
+python slate.py -d data-list-file [any other arguments]
+```
+
+#### Example
+
+The tutorial folder contains two example data list files:
+
+- `tutorial/data/list_with_disagreements.category.txt`
+- `tutorial/data/list_with_disagreements.link.txt`
 
-To save time, it is best to initialise `adjudicated-annoN` with the lines everyone agreed on:
+You can use them as follows:
 
 ```
-for i in 0 1 2 ; do
-  count=`ls anno${i}.* | wc -l`
-  cat anno${i}.* | sort | uniq -c | awk -v count=$count '$1 == count' | sed 's/^ *[0-9]* *//' > matching
-done
+cd tutorial/data
+python ../../slate.py -d list_with_disagreements.category.txt -t categorical -s token
 ```
 
-Then run the tool as if you are annotating, for example for linking lines:
+#### Efficiency Tip
+
+You can save time by putting annotations that all annotators agreed on into the `annotations-adjudicated.txt` file.
+This bash pipeline will do that if you replace:
+
+- `ANNOTATION_FILES` with the names of all of your annotation files, separated by spaces
+- `N_FILES` with the number of annotation files you have
 
 ```
-python ../learn-anno/slate/slate.py -d example.txt -pf -t link -s line -o -l log.adj.txt --do-not-show-linked
+cat ANNOTATION_FILES | sort | uniq -c | awk -v count=N_FILES '$1 == count' | sed 's/^ *[0-9]* *//' > annotations-adjudicated.txt
 ```
 
+Breaking this down, it does the following:
+- `cat ANNOTATION_FILES `, print the annotation files in the terminal
+- `sort `, sort their contents together
+- `uniq -c `, where there are consecutive lines that are the same, only keep one, and also indicate how many times each line occurred
+- `awk -v count=N_FILES '$1 == count' `, only keep lines where the number at the start matches `N_FILES`
+- `sed 's/^ *[0-9]* *//' > annotations-adjudicated.txt`, remove the number at the start of the line (placed there by the `uniq` command)
+
 ## Detailed Usage Instructions
 
 ### Invocation options
 
 ```
 usage: slate.py [-h] [-d DATA_LIST [DATA_LIST ...]] [-t {categorical,link}]
                 [-s {character,token,line,document}] [-c CONFIG_FILE] [-l LOG_PREFIX] [-ld]
@@ -247,15 +284,17 @@
 
 ```bash
 python slate.py @arguments.txt
 ```
 
 ### Keybindings
 
-The tool shows files one at a time in plain text. Default commands are:
+The tool shows files one at a time in plain text. Default commands are shown below.
+
+Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
 
 Type                        | Key                                                       | Labelling Affect                 | Linking Affect
 --------------------------- | --------------------------------------------------------- | -------------------------------- | ---------------------
 Movement                    | <kbd>j</kbd> or <kbd>&larr;</kbd>                         | move to the left                 | move selected item to the left
 &nbsp;                      | <kbd>i</kbd> or <kbd>&uarr;</kbd>                         | move up a line                   | move selected item up a line
 &nbsp;                      | <kbd>o</kbd> or <kbd>&darr;</kbd>                         | move down a line                 | move selected item down a line
 &nbsp;                      | <kbd>;</kbd> or <kbd>&rarr;</kbd>                         | move to the right                | move selected item to the right
@@ -304,16 +343,14 @@
 &nbsp;                      | Normal | <kbd>h</kbd>                                    | toggle help info (default on)    
 &nbsp;                      | Normal | <kbd>{</kbd> or <kbd>PAGE-UP</kbd>              | shift view up 5 lines
 &nbsp;                      | Normal | <kbd>}</kbd> or <kbd>PAGE-DOWN</kbd>            | shift view down 5 lines
 &nbsp;                      | Normal | <kbd>></kbd> then <kbd>p</kbd>                  | toggle showing progress through files
 &nbsp;                      | Normal | <kbd>></kbd> then <kbd>l</kbd>                  | toggle showing legend for labels
 &nbsp;                      | Normal | <kbd>></kbd> then <kbd>m</kbd>                  | toggle showing the mark on the current item
 
-Note: special keys such as `ENTER` and `BACKSPACE` may not work on non-OS-X operating systems. That is why in all places where they are used we have an alternative as well.
-
 ### Misc
 
 To annotate multiple files, specify more than one as an argument.
 For greater control, provide a list of files in a file specified with `--data-list` / `-d`.
 The list should be formatted as follows, where [] indicate optional values:
 
 ```
@@ -332,14 +369,29 @@
 Note, the `-o` flag is added so it will allow you to edit the annotations you have already created.
 Otherwise the system will complain that you are overwriting existing annotation files.
 
 When the `additional_annotation_files` are included it activates an adjudication mode.
 By default, all annotations that appear in all additional files are added to the current annotations.
 Disagreements are coloured in the text, but will disappear once a decision is made (using the normal annotation commands).
 
+### Running in Windows
+
+Users have reported a range of issues when trying to run slate:
+
+- Underlining, which is used to show the currently selected text, does not work.
+- Shift keys do not work
+
+Here are a few things to try that others have found helpful:
+
+- Use the Windows Subsystem for Linux (WSL) with Ubuntu
+- Reinstall ncurses, or install windows-curses
+- If you hit an encoding issue, try converting your raw text file to ASCII
+- Try powershell
+- Use a config file with different keybindings, to avoid needing shift
+
 ## Customisation
 
 Colours and keys are customisable. For labelling, the default is:
 
  - Underlined, current selected item
  - Green on black, 'a' items
  - Blue on black, 's' items
@@ -396,14 +448,16 @@
 Label:          O                         SPACE_a green
 Label:          LOC                       SPACE_s blue
 Label:          PER                       SPACE_d red
 Label:          ORG                       SPACE_f yellow
 Label:          MISC                      SPACE_v magenta
 ```
 
+For an example of a custom config file, see [ner-book.config](ner-book.config)
+
 The current set of available colours is: [green, blue, white, cyan, magenta, red, yellow].
 Note that by default white is used for regular text and cyan is used for cases where multiple labels apply to the same content.
 
 To define more colours, edit the top of `slate/config.py`.
 By varying both the text colour (foreground) and background colour you can achieve quite a range of variations.
 You can also define any RGB colour you want using the curses [init_color](https://docs.python.org/3/library/curses.html#curses.init_color) function and the [init_pair](https://docs.python.org/3/library/curses.html#curses.init_pair) function.
```

### Comparing `slate-nlp-1.1.1/slate_nlp.egg-info/SOURCES.txt` & `slate_nlp-1.1.2/slate_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/tutorial/config-example.txt` & `slate_nlp-1.1.2/tutorial/config-example.txt`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/tutorial/data/input_data0.txt` & `slate_nlp-1.1.2/tutorial/data/input_data0.txt`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/tutorial/data/input_data1.txt` & `slate_nlp-1.1.2/tutorial/data/input_data1.txt`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/tutorial/label.md` & `slate_nlp-1.1.2/tutorial/label.md`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/tutorial/link.md` & `slate_nlp-1.1.2/tutorial/link.md`

 * *Files identical despite different names*

### Comparing `slate-nlp-1.1.1/tutorial/ner.md` & `slate_nlp-1.1.2/tutorial/ner.md`

 * *Files 4% similar despite different names*

```diff
@@ -91,14 +91,16 @@
 
 Run this command to start annotating, now with information about the existing annotations:
 
 ```
 python slate.py -d anno-file-list.txt -t categorical -s token -o -c ner-book.config -l log.tutorial.ner.txt -sl -sm
 ```
 
+Note - if this crashes with a `list index out of range` error then you need to change the `(1,0)` part of the line above because your data has a blank second line. Change the first number to be a line that does exist.
+
 You will see that:
 
  - Any annotation in `example.annotations.adjudicated.txt` appears as a normal annotation.
  - Any annotation that is consistent across the different sets of annotations appears as a normal annotation.
  - Any tokens that have a disagreement in annotation appear in red.
 
 You can now go through, assigning labels wherever you see red, resolving the disagreements between the annotations and creating one consistent set of annotations.
```

