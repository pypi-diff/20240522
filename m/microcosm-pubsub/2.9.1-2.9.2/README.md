# Comparing `tmp/microcosm-pubsub-2.9.1.tar.gz` & `tmp/microcosm-pubsub-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microcosm-pubsub-2.9.1.tar", last modified: Fri Jan  3 13:31:50 2020, max compression
+gzip compressed data, was "dist/microcosm-pubsub-2.9.2.tar", last modified: Mon Jan  6 22:45:15 2020, max compression
```

## Comparing `microcosm-pubsub-2.9.1.tar` & `microcosm-pubsub-2.9.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      324 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4275 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/README.md
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1951 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/backoff.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/batch.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2536 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/chain.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2199 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3853 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/context_decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1392 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      394 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/exceptions.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2690 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/assign.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1863 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/call.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      330 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/case.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/for_each.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1621 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/switch.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1145 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/try_chain.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      973 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/when.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2417 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/codecs.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5580 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/consumer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/context.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      819 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      673 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/lifecycle.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2212 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/messages.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1538 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/naming.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3089 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/daemon.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      961 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/decorators.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6101 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/dispatcher.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6775 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/envelope.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      952 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/fields.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      266 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4475 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/base.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1027 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/chain_handlers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      968 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/publish_batch_message.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3250 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/uri_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3197 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/main.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/matchers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      837 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/matchers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3347 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/matchers/message.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1650 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/matchers/publishing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1502 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/message.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4036 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/metrics.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12396 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/producer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/reader.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5204 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/registry.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4319 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/microcosm_pubsub/result.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      324 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1942 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-01-03 13:31:49.000000 microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      219 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2020-01-03 13:31:50.000000 microcosm-pubsub-2.9.1/setup.cfg
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2351 2020-01-03 13:29:43.000000 microcosm-pubsub-2.9.1/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/MANIFEST.in
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      324 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4275 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/README.md
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1951 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/backoff.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      830 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/batch.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      329 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2536 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/chain.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2199 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/context.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3853 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/context_decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1392 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      394 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/exceptions.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      510 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2690 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/assign.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1863 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/call.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      330 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/case.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1499 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/for_each.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1621 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/switch.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1145 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/try_chain.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      973 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/when.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2417 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/codecs.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      133 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/constants.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5580 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/consumer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1440 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/context.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      819 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      673 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/lifecycle.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2212 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/messages.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1538 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/naming.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3089 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/daemon.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      961 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/decorators.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6101 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/dispatcher.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6775 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/envelope.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1419 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      952 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/fields.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      266 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4475 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/base.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1027 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/chain_handlers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      968 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/publish_batch_message.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3250 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/uri_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3197 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/main.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/matchers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      837 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/matchers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3347 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/matchers/message.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1650 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/matchers/publishing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1502 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/message.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4086 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/metrics.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    12396 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/producer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1539 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/reader.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5204 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/registry.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4319 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/microcosm_pubsub/result.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      324 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1942 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      988 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2020-01-06 22:45:14.000000 microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      219 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      463 2020-01-06 22:45:15.000000 microcosm-pubsub-2.9.2/setup.cfg
+-rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2351 2020-01-06 22:43:19.000000 microcosm-pubsub-2.9.2/setup.py
```

### Comparing `microcosm-pubsub-2.9.1/README.md` & `microcosm-pubsub-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/backoff.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/backoff.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/batch.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/batch.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/chain.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/chain.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/context.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/context.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/context_decorators.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/context_decorators.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/decorators.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/decorators.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/assign.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/assign.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/call.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/call.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/for_each.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/for_each.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/switch.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/switch.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/try_chain.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/try_chain.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/chain/statements/when.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/chain/statements/when.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/codecs.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/codecs.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/consumer.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/consumer.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/context.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/context.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/__init__.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/__init__.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/lifecycle.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/lifecycle.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/messages.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/messages.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/conventions/naming.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/conventions/naming.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/daemon.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/daemon.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/decorators.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/decorators.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/dispatcher.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/dispatcher.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/envelope.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/envelope.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/errors.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/errors.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/fields.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/fields.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/base.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/base.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/chain_handlers.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/chain_handlers.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/publish_batch_message.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/publish_batch_message.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/handlers/uri_handler.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/handlers/uri_handler.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/main.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/main.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/matchers/__init__.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/matchers/message.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/matchers/message.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/matchers/publishing.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/matchers/publishing.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/message.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/message.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/metrics.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
         """
         if not self.enabled:
             return
 
         tags = [
             "source:microcosm-pubsub",
             f"publish_result:{publish_result}",
+            f"media_type:{kwargs['media_type']}",
         ]
 
         self.metrics.histogram(
             "sns_producer",
             elapsed_time,
             tags=tags,
         )
```

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/producer.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/producer.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/reader.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/reader.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/registry.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/registry.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub/result.py` & `microcosm-pubsub-2.9.2/microcosm_pubsub/result.py`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/SOURCES.txt` & `microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/microcosm_pubsub.egg-info/entry_points.txt` & `microcosm-pubsub-2.9.2/microcosm_pubsub.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `microcosm-pubsub-2.9.1/setup.py` & `microcosm-pubsub-2.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 
 project = "microcosm-pubsub"
-version = "2.9.1"
+version = "2.9.2"
 
 setup(
     name=project,
     version=version,
     description="PubSub with SNS/SQS",
     author="Globality Engineering",
     author_email="engineering@globality.com",
```

