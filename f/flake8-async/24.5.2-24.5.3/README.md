# Comparing `tmp/flake8_async-24.5.2.tar.gz` & `tmp/flake8_async-24.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_async-24.5.2.tar", last modified: Mon May 13 17:19:49 2024, max compression
+gzip compressed data, was "flake8_async-24.5.3.tar", last modified: Wed May 22 10:54:56 2024, max compression
```

## Comparing `flake8_async-24.5.2.tar` & `flake8_async-24.5.3.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:49.933717 flake8_async-24.5.2/
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-13 17:19:42.000000 flake8_async-24.5.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-13 17:19:42.000000 flake8_async-24.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-13 17:19:42.000000 flake8_async-24.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 17:19:42.000000 flake8_async-24.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23495 2024-05-13 17:19:49.933717 flake8_async-24.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-13 17:19:47.000000 flake8_async-24.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:49.913718 flake8_async-24.5.2/flake8_async/
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:49.917718 flake8_async-24.5.2/flake8_async/visitors/
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/flake8asyncvisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15294 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor101.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor102.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor103_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor105.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor111.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor118.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor2xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    36306 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor91x.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitor_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-05-13 17:19:42.000000 flake8_async-24.5.2/flake8_async/visitors/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:49.933717 flake8_async-24.5.2/flake8_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23495 2024-05-13 17:19:49.000000 flake8_async-24.5.2/flake8_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-13 17:19:49.000000 flake8_async-24.5.2/flake8_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:19:49.000000 flake8_async-24.5.2/flake8_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 17:19:49.000000 flake8_async-24.5.2/flake8_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:19:49.000000 flake8_async-24.5.2/flake8_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 17:19:49.000000 flake8_async-24.5.2/flake8_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 17:19:49.000000 flake8_async-24.5.2/flake8_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-13 17:19:42.000000 flake8_async-24.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:19:49.933717 flake8_async-24.5.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-05-13 17:19:42.000000 flake8_async-24.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:49.917718 flake8_async-24.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:49.921718 flake8_async-24.5.2/tests/autofix_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/autofix_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/autofix_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/autofix_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/autofix_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/autofix_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/autofix_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/autofix_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/autofix_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:49.933717 flake8_async-24.5.2/tests/eval_files/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/anyio_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async100_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async101.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async101_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async101_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async101_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async102.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async102_aclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async102_aclose_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async102_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async102_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async102_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async103.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async103_all_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async103_both_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async103_no_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async103_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async104.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async104_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async104_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async105.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async105_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async106.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async109.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async110.py
--rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async111.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async111_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async111_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async112.py
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async112_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async112_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async113.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async113_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async113_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async114.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async115.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async116.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async118.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async119.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async210.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async211.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async212.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async22x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async22x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async232.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async232_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async23x.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async23x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async240.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async250.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async250_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async251.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async251_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async900.py
--rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async912.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async912_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/async91x_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/no_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/noqa_no_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/eval_files/trio_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/test_all_visitors_imported.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/test_changelog_and_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/test_config_and_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/test_exception_on_invalid_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    29840 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/test_flake8_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/test_formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/test_messages_documented.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tests/trio_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-13 17:19:42.000000 flake8_async-24.5.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.600402 flake8_async-24.5.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 10:54:47.000000 flake8_async-24.5.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-22 10:54:47.000000 flake8_async-24.5.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-22 10:54:47.000000 flake8_async-24.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 10:54:47.000000 flake8_async-24.5.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-22 10:54:56.600402 flake8_async-24.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-22 10:54:47.000000 flake8_async-24.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.580402 flake8_async-24.5.3/flake8_async/
+-rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.584402 flake8_async-24.5.3/flake8_async/visitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/flake8asyncvisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15294 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor102.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor103_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor105.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor118.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor2xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36306 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor91x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitor_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-05-22 10:54:47.000000 flake8_async-24.5.3/flake8_async/visitors/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.600402 flake8_async-24.5.3/flake8_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 10:54:56.000000 flake8_async-24.5.3/flake8_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-22 10:54:47.000000 flake8_async-24.5.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:54:56.600402 flake8_async-24.5.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2204 2024-05-22 10:54:47.000000 flake8_async-24.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.588402 flake8_async-24.5.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.588402 flake8_async-24.5.3/tests/autofix_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/autofix_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:54:56.600402 flake8_async-24.5.3/tests/eval_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/anyio_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async100_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async101.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async101_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async101_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async101_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_aclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_aclose_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async102_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103_all_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103_both_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103_no_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async103_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async104.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async104_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async104_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async105_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async106.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async109.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async111_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async111_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async112_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async112_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async113_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4874 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async113_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async115.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async116.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async118.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async119.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async210.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async211.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async212.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async22x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async22x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async232_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async23x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async23x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async250.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async250_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async251.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async251_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async900.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async912.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async912_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/async91x_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/no_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/noqa_no_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/eval_files/trio_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_all_visitors_imported.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3807 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_changelog_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12695 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_config_and_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_exception_on_invalid_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29840 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_flake8_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3425 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/test_messages_documented.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tests/trio_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-22 10:54:47.000000 flake8_async-24.5.3/tox.ini
```

### Comparing `flake8_async-24.5.2/LICENSE` & `flake8_async-24.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/__init__.py` & `flake8_async-24.5.3/flake8_async/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import ast
 import functools
 import keyword
 import os
 import subprocess
 import sys
 import tokenize
+import warnings
 from argparse import ArgumentParser, ArgumentTypeError, Namespace
 from typing import TYPE_CHECKING
 
 import libcst as cst
 
 from .base import Options, error_has_subidentifier
 from .runner import Flake8AsyncRunner, Flake8AsyncRunner_cst
@@ -33,15 +34,15 @@
 
     from flake8.options.manager import OptionManager
 
     from .base import Error
 
 
 # CalVer: YY.month.patch, e.g. first release of July 2022 == "22.7.1"
-__version__ = "24.5.2"
+__version__ = "24.5.3"
 
 
 # taken from https://github.com/Zac-HD/shed
 @functools.lru_cache
 def _get_git_repo_root(cwd: str | None = None) -> str:
     return subprocess.run(
         ["git", "rev-parse", "--show-toplevel"],
@@ -258,29 +259,40 @@
                 "Decorators can be dotted or not, as well as support * as a wildcard. "
                 "For example, ``--no-checkpoint-warning-decorators=app.route,"
                 "mydecorator,mypackage.mydecorators.*``"
             ),
         )
         add_argument(
             "--startable-in-context-manager",
-            type=parse_trio114_identifiers,
+            type=parse_async114_identifiers,
             default="",
             required=False,
             help=(
                 "Comma-separated list of method calls to additionally enable ASYNC113 "
                 "warnings for. Will also check for the pattern inside function calls. "
                 "Methods must be valid identifiers as per `str.isidientifier()` and "
                 "not reserved keywords. "
                 "For example, ``--startable-in-context-manager=worker_serve,"
                 "myfunction``"
             ),
         )
         add_argument(
             "--trio200-blocking-calls",
-            type=parse_trio200_dict,
+            type=parse_async200_dict,
+            default={},
+            required=False,
+            help=(
+                "Comma-separated list of key->value pairs, where key is a [dotted] "
+                "function that if found inside an async function will raise ASYNC200, "
+                "suggesting it be replaced with {value}"
+            ),
+        )
+        add_argument(
+            "--async200-blocking-calls",
+            type=parse_async200_dict,
             default={},
             required=False,
             help=(
                 "Comma-separated list of key->value pairs, where key is a [dotted] "
                 "function that if found inside an async function will raise ASYNC200, "
                 "suggesting it be replaced with {value}"
             ),
@@ -344,40 +356,54 @@
 
         # if disable has default value, re-enable explicitly enabled codes
         if options.disable == ["ASYNC9"]:
             enabled_codes.update(
                 code for code in options.enable if not error_has_subidentifier(code)
             )
 
+        # we do not use DeprecationWarning, since that is silenced when run as standalone
+        # or should maybe just print on stderr
+        if options.trio200_blocking_calls:
+            warnings.warn(
+                "trio200-blocking-calls has been deprecated in favor "
+                "of async200-blocking-calls",
+                stacklevel=1,
+            )
+            assert not options.async200_blocking_calls, (
+                "You cannot specify both trio200-blocking-calls and "
+                "async200-blocking-calls. You should only use the latter."
+            )
+            options.async200_blocking_calls = options.trio200_blocking_calls
+
         Plugin._options = Options(
             enabled_codes=enabled_codes,
             autofix_codes=autofix_codes,
             error_on_autofix=options.error_on_autofix,
             no_checkpoint_warning_decorators=options.no_checkpoint_warning_decorators,
             startable_in_context_manager=options.startable_in_context_manager,
-            trio200_blocking_calls=options.trio200_blocking_calls,
+            async200_blocking_calls=options.async200_blocking_calls,
             anyio=options.anyio,
             asyncio=options.asyncio,
             disable_noqa=options.disable_noqa,
         )
 
 
 def comma_separated_list(raw_value: str) -> list[str]:
     return [s.strip() for s in raw_value.split(",") if s.strip()]
 
 
-def parse_trio114_identifiers(raw_value: str) -> list[str]:
+def parse_async114_identifiers(raw_value: str) -> list[str]:
     values = comma_separated_list(raw_value)
     for value in values:
         if keyword.iskeyword(value) or not value.isidentifier():
             raise ArgumentTypeError(f"{value!r} is not a valid method identifier")
     return values
 
 
-def parse_trio200_dict(raw_value: str) -> dict[str, str]:
+def parse_async200_dict(raw_value: str) -> dict[str, str]:
     res: dict[str, str] = {}
     splitter = "->"  # avoid ":" because it's part of .ini file syntax
     values = [s.strip() for s in raw_value.split(",") if s.strip()]
 
     for value in values:
         split_values = list(map(str.strip, value.split(splitter)))
         if len(split_values) != 2:
```

### Comparing `flake8_async-24.5.2/flake8_async/base.py` & `flake8_async-24.5.3/flake8_async/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     enabled_codes: set[str]
     # error codes to autofix
     autofix_codes: set[str]
     # whether to print an error message even when autofixed
     error_on_autofix: bool
     no_checkpoint_warning_decorators: Collection[str]
     startable_in_context_manager: Collection[str]
-    trio200_blocking_calls: dict[str, str]
+    async200_blocking_calls: dict[str, str]
     anyio: bool
     asyncio: bool
     disable_noqa: bool
 
 
 class Statement(NamedTuple):
     name: str
```

### Comparing `flake8_async-24.5.2/flake8_async/runner.py` & `flake8_async-24.5.3/flake8_async/runner.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/__init__.py` & `flake8_async-24.5.3/flake8_async/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/flake8asyncvisitor.py` & `flake8_async-24.5.3/flake8_async/visitors/flake8asyncvisitor.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/helpers.py` & `flake8_async-24.5.3/flake8_async/visitors/helpers.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor101.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor101.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor102.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor102.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor103_104.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor103_104.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor105.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor105.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor111.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor111.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor118.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor118.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor2xx.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor2xx.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     visit_Lambda = visit_AsyncFunctionDef
 
     def visit_Call(self, node: ast.Call):
         if self.async_function and not getattr(node, "awaited", False):
             self.visit_blocking_call(node)
 
     def visit_blocking_call(self, node: ast.Call):
-        blocking_calls = self.options.trio200_blocking_calls
+        blocking_calls = self.options.async200_blocking_calls
         if key := fnmatch_qualified_name([node.func], *blocking_calls):
             self.error(node, key, blocking_calls[key])
 
 
 # used by Visitor212 and Visitor232 - ??
```

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor91x.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor91x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitor_utility.py` & `flake8_async-24.5.3/flake8_async/visitors/visitor_utility.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async/visitors/visitors.py` & `flake8_async-24.5.3/flake8_async/visitors/visitors.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/flake8_async.egg-info/SOURCES.txt` & `flake8_async-24.5.3/flake8_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/pyproject.toml` & `flake8_async-24.5.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/setup.py` & `flake8_async-24.5.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,15 +21,19 @@
 
 setup(
     name="flake8-async",
     version=__version__,
     author="Zac Hatfield-Dodds, John Litborn, and Contributors",
     author_email="zac@zhd.dev",
     packages=find_packages(include=["flake8_async", "flake8_async.*"]),
-    url="https://github.com/python-trio/flake8-async",
+    project_urls={
+        "Homepage": "https://github.com/python-trio/flake8-async",
+        "Documentation": "https://flake8-async.readthedocs.io/",
+        "Changelog": "https://flake8-async.readthedocs.io/en/latest/changelog.html",
+    },
     license="MIT",
     description="A highly opinionated flake8 plugin for Trio-related problems.",
     zip_safe=False,
     install_requires=["flake8>=6", "libcst>=1.0.1"],
     python_requires=">=3.9",
     classifiers=[
         "Development Status :: 3 - Alpha",
@@ -40,19 +44,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
     ],
-    long_description=(
-        local_file("README.md").open().read()
-        + "\n\n"
-        + local_file("CHANGELOG.md").open().read()
-    ),
+    long_description=(local_file("README.md").open().read()),
     long_description_content_type="text/markdown",
     entry_points={
         # You're not allowed to register error codes longer than 3 characters. But flake8
         # doesn't enforce anything about the characters trailing the code, so we can say
         # the code is ASY and then just always happen to print NCxxx directly after it.
         "flake8.extension": ["ASY = flake8_async:Plugin"],
         "console_scripts": ["flake8-async=flake8_async:main"],
```

### Comparing `flake8_async-24.5.2/tests/autofix_files/async100.py` & `flake8_async-24.5.3/tests/autofix_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/autofix_files/async100_simple_autofix.py` & `flake8_async-24.5.3/tests/autofix_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/autofix_files/async910.py` & `flake8_async-24.5.3/tests/autofix_files/async910.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/autofix_files/async911.py` & `flake8_async-24.5.3/tests/autofix_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/autofix_files/async91x_autofix.py` & `flake8_async-24.5.3/tests/autofix_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/autofix_files/noqa.py` & `flake8_async-24.5.3/tests/autofix_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/conftest.py` & `flake8_async-24.5.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async100.py` & `flake8_async-24.5.3/tests/eval_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async100_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async100_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async100_noautofix.py` & `flake8_async-24.5.3/tests/eval_files/async100_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async100_simple_autofix.py` & `flake8_async-24.5.3/tests/eval_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async101.py` & `flake8_async-24.5.3/tests/eval_files/async101.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async101_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async101_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async102.py` & `flake8_async-24.5.3/tests/eval_files/async102.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async102_aclose.py` & `flake8_async-24.5.3/tests/eval_files/async102_aclose.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async102_aclose_args.py` & `flake8_async-24.5.3/tests/eval_files/async102_aclose_args.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async102_anyio.py` & `flake8_async-24.5.3/tests/eval_files/async102_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async102_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async102_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async102_trio.py` & `flake8_async-24.5.3/tests/eval_files/async102_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async103.py` & `flake8_async-24.5.3/tests/eval_files/async103.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async103_all_imported.py` & `flake8_async-24.5.3/tests/eval_files/async103_all_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async103_both_imported.py` & `flake8_async-24.5.3/tests/eval_files/async103_both_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async103_trio.py` & `flake8_async-24.5.3/tests/eval_files/async103_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async104.py` & `flake8_async-24.5.3/tests/eval_files/async104.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async104_anyio.py` & `flake8_async-24.5.3/tests/eval_files/async104_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async105.py` & `flake8_async-24.5.3/tests/eval_files/async105.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async106.py` & `flake8_async-24.5.3/tests/eval_files/async106.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async109.py` & `flake8_async-24.5.3/tests/eval_files/async109.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async110.py` & `flake8_async-24.5.3/tests/eval_files/async110.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async111.py` & `flake8_async-24.5.3/tests/eval_files/async111.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async111_anyio.py` & `flake8_async-24.5.3/tests/eval_files/async111_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async111_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async111_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async112.py` & `flake8_async-24.5.3/tests/eval_files/async112.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async112_anyio.py` & `flake8_async-24.5.3/tests/eval_files/async112_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async112_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async112_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async113.py` & `flake8_async-24.5.3/tests/eval_files/async113.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async113_trio.py` & `flake8_async-24.5.3/tests/eval_files/async113_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async114.py` & `flake8_async-24.5.3/tests/eval_files/async114.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async115.py` & `flake8_async-24.5.3/tests/eval_files/async115.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async116.py` & `flake8_async-24.5.3/tests/eval_files/async116.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async118.py` & `flake8_async-24.5.3/tests/eval_files/async118.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async119.py` & `flake8_async-24.5.3/tests/eval_files/async119.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async200.py` & `flake8_async-24.5.3/tests/eval_files/async200.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # type: ignore
 # specify command-line arguments to be used when testing this file.
 # Test spaces in options, and trailing comma
 # Cannot test newlines, since argparse splits on those if passed on the CLI
-# ARG --trio200-blocking-calls=bar -> BAR, bee-> SHOULD_NOT_BE_PRINTED,bonnet ->SHOULD_NOT_BE_PRINTED,bee.bonnet->BEEBONNET,*.postwild->POSTWILD,prewild.*->PREWILD,*.*.*->TRIPLEDOT,
+# ARG --async200-blocking-calls=bar -> BAR, bee-> SHOULD_NOT_BE_PRINTED,bonnet ->SHOULD_NOT_BE_PRINTED,bee.bonnet->BEEBONNET,*.postwild->POSTWILD,prewild.*->PREWILD,*.*.*->TRIPLEDOT,
 
 
 # don't error in sync function
 def bar():
     bar()
     bee.bonnet()
```

### Comparing `flake8_async-24.5.2/tests/eval_files/async210.py` & `flake8_async-24.5.3/tests/eval_files/async210.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async211.py` & `flake8_async-24.5.3/tests/eval_files/async211.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async212.py` & `flake8_async-24.5.3/tests/eval_files/async212.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async22x.py` & `flake8_async-24.5.3/tests/eval_files/async22x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async22x_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async22x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async232.py` & `flake8_async-24.5.3/tests/eval_files/async232.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async232_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async232_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async23x.py` & `flake8_async-24.5.3/tests/eval_files/async23x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async23x_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async23x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async240.py` & `flake8_async-24.5.3/tests/eval_files/async240.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async900.py` & `flake8_async-24.5.3/tests/eval_files/async900.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async910.py` & `flake8_async-24.5.3/tests/eval_files/async910.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async911.py` & `flake8_async-24.5.3/tests/eval_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async912.py` & `flake8_async-24.5.3/tests/eval_files/async912.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async912_asyncio.py` & `flake8_async-24.5.3/tests/eval_files/async912_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async91x_autofix.py` & `flake8_async-24.5.3/tests/eval_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/async91x_noautofix.py` & `flake8_async-24.5.3/tests/eval_files/async91x_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/eval_files/noqa.py` & `flake8_async-24.5.3/tests/eval_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/test_all_visitors_imported.py` & `flake8_async-24.5.3/tests/test_all_visitors_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/test_changelog_and_version.py` & `flake8_async-24.5.3/tests/test_changelog_and_version.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from pathlib import Path
 from typing import TYPE_CHECKING, NamedTuple, TypeVar
 
 if TYPE_CHECKING:
     from collections.abc import Iterable
 
 ROOT_PATH = Path(__file__).parent.parent
-CHANGELOG = ROOT_PATH / "CHANGELOG.md"
+CHANGELOG = ROOT_PATH / "docs" / "changelog.rst"
 README = ROOT_PATH / "README.md"
 INIT_FILE = ROOT_PATH / "flake8_async" / "__init__.py"
 
 T = TypeVar("T", bound="Version")
 
 
 class Version(NamedTuple):
@@ -37,29 +37,34 @@
         VERSION = Version.from_string(m.groups()[0])
         break
 else:
     raise RuntimeError("No version detected.")
 
 
 def get_releases() -> Iterable[Version]:
-    valid_pattern = re.compile(r"^## (\d\d\.\d?\d\.\d?\d)$")
-    invalid_pattern = re.compile(r"^## ")
+    valid_pattern = re.compile(r"^(\d\d\.\d?\d\.\d?\d)$")
+    header_pattern = re.compile(r"^=+$")
+    last_line_was_date = False
     with open(CHANGELOG, encoding="utf-8") as f:
         lines = f.readlines()
     for line in lines:
         version_match = valid_pattern.match(line)
-        if version_match:
+        if last_line_was_date:
+            assert header_pattern.match(line)
+            last_line_was_date = False
+        elif version_match:
             yield Version.from_string(version_match.group(1))
+            last_line_was_date = True
         else:
-            # stop lines such as `## Future` making it through to main/
-            assert not invalid_pattern.match(line)
+            # stop lines such as `Future\n=====` making it through to main/
+            assert not header_pattern.match(line), line
 
 
 def test_last_release_against_changelog() -> None:
-    """Ensure we have the latest version covered in 'CHANGELOG.md'."""
+    """Ensure we have the latest version covered in 'changelog.rst'."""
     latest_release = next(iter(get_releases()))
     assert latest_release == VERSION
 
 
 def test_version_increments_are_correct() -> None:
     versions = list(get_releases())
     for prev, current in zip(versions[1:], versions):
```

### Comparing `flake8_async-24.5.2/tests/test_config_and_args.py` & `flake8_async-24.5.3/tests/test_config_and_args.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         assert f"{arg!r} is not a valid method identifier" in err
 
 
 def test_200_options(capsys: pytest.CaptureFixture[str]):
     plugin = Plugin(ast.AST(), [])
     for i, arg in (0, "foo"), (2, "foo->->bar"), (2, "foo->bar->fee"):
         with pytest.raises(SystemExit):
-            initialize_options(plugin, args=[f"--trio200-blocking-calls={arg}"])
+            initialize_options(plugin, args=[f"--async200-blocking-calls={arg}"])
         out, err = capsys.readouterr()
         assert not out, out
         assert all(word in err for word in (str(i), arg, "->"))
 
 
 def test_anyio_from_config(tmp_path: Path, capsys: pytest.CaptureFixture[str]):
     assert tmp_path.joinpath(".flake8").write_text(
@@ -198,19 +198,20 @@
     )
     out, err = capsys.readouterr()
     assert not err
     assert expected == out
     assert returnvalue == 1
 
 
-def _test_trio200_from_config_common(tmp_path: Path) -> str:
+# `code` parameter temporarily introduced to test deprecation of trio200-blocking-calls
+def _test_async200_from_config_common(tmp_path: Path, code: str = "async200") -> str:
     assert tmp_path.joinpath(".flake8").write_text(
-        """
+        f"""
 [flake8]
-trio200-blocking-calls =
+{code}-blocking-calls =
   other -> async,
   sync_fns.* -> the_async_equivalent,
 select = ASYNC200
 extend-ignore = E
 """
     )
     assert tmp_path.joinpath("example.py").write_text(
@@ -230,15 +231,15 @@
 def test_200_from_config_flake8_internals(
     tmp_path: Path, capsys: pytest.CaptureFixture[str]
 ):
     # abuse flake8 internals to avoid having to use subprocess
     # which breaks breakpoints and hinders debugging
     # TODO: fixture (?) to change working directory
 
-    EXAMPLE_PY_TEXT = _test_trio200_from_config_common(tmp_path)
+    EXAMPLE_PY_TEXT = _test_async200_from_config_common(tmp_path)
     # replace ./ with tmp_path/
     err_msg = str(tmp_path) + EXAMPLE_PY_TEXT[1:]
 
     from flake8.main.cli import main
 
     returnvalue = main(
         argv=[
@@ -250,21 +251,32 @@
     out, err = capsys.readouterr()
     assert returnvalue == 1
     assert not err
     assert err_msg == out
 
 
 def test_200_from_config_subprocess(tmp_path: Path):
-    err_msg = _test_trio200_from_config_common(tmp_path)
+    err_msg = _test_async200_from_config_common(tmp_path)
     res = subprocess.run(["flake8"], cwd=tmp_path, capture_output=True, check=False)
     assert res.returncode == 1
     assert not res.stderr
     assert res.stdout == err_msg.encode("ascii")
 
 
+def test_trio200_from_config_subprocess(tmp_path: Path):
+    err_msg = _test_async200_from_config_common(tmp_path, code="trio200")
+    res = subprocess.run(["flake8"], cwd=tmp_path, capture_output=True, check=False)
+    assert res.returncode == 1
+    assert res.stderr.endswith(
+        b"UserWarning: trio200-blocking-calls has been deprecated in favor of "
+        b"async200-blocking-calls\n  warnings.warn(\n"
+    )
+    assert res.stdout == err_msg.encode("ascii")
+
+
 def test_900_default_off(capsys: pytest.CaptureFixture[str]):
     from flake8.main.cli import main
 
     returnvalue = main(
         argv=[
             "tests/trio900.py",
         ]
@@ -420,15 +432,15 @@
     assert not res.stderr
     assert res.returncode == 0
 
 
 # but make sure we can disable selected codes
 def test_config_disable_error_code(tmp_path: Path) -> None:
     # select ASYNC200 and create file that induces ASYNC200
-    _test_trio200_from_config_common(tmp_path)
+    _test_async200_from_config_common(tmp_path)
     # disable ASYNC200
     with open(tmp_path.joinpath(".flake8"), "a", encoding="utf-8") as file:
         file.write("disable = ASYNC200")
 
     # it now returns no errors
     res = subprocess.run(["flake8"], cwd=tmp_path, capture_output=True, check=True)
     assert not res.stdout
```

### Comparing `flake8_async-24.5.2/tests/test_decorator.py` & `flake8_async-24.5.3/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/test_exception_on_invalid_code.py` & `flake8_async-24.5.3/tests/test_exception_on_invalid_code.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/test_flake8_async.py` & `flake8_async-24.5.3/tests/test_flake8_async.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.5.2/tests/test_messages_documented.py` & `flake8_async-24.5.3/tests/test_messages_documented.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 import re
 from pathlib import Path
 from typing import cast
 
 from .test_flake8_async import ERROR_CODES
 
 ROOT_PATH = Path(__file__).parent.parent
-CHANGELOG = ROOT_PATH / "CHANGELOG.md"
-README = CHANGELOG.parent / "README.md"
+CHANGELOG = ROOT_PATH / "docs" / "changelog.rst"
+RULES_DOC = ROOT_PATH / "docs" / "rules.rst"
 
 # 107, 108 & 117 are removed (but still mentioned in changelog & readme)
 # ASYNCxxx_* are fake codes to get different error messages for the same code
 IGNORED_CODES_REGEX = r"(TRIO|ASYNC)(107|108|117)|ASYNC\d\d\d_.*"
 
 
 # temp function for eval files
 # less sure what to do with the changelog
 def rename_trio_to_async(s: str) -> str:
     return re.sub("TRIO", "ASYNC", s)
 
 
 def test_messages_documented():
     documented_errors: dict[str, set[str]] = {}
-    for path in (CHANGELOG, README):
+    for path in (CHANGELOG, RULES_DOC):
         with open(path, encoding="utf-8") as f:
             lines = f.readlines()
         filename = path.name
         documented_errors[filename] = set()
         for line in lines:
             for error_msg in re.findall(r"TRIO\d\d\d|ASYNC\d\d\d", line):
                 documented_errors[filename].add(rename_trio_to_async(error_msg))
```

### Comparing `flake8_async-24.5.2/tox.ini` & `flake8_async-24.5.3/tox.ini`

 * *Files identical despite different names*

