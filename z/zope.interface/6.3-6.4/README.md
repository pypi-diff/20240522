# Comparing `tmp/zope.interface-6.3.tar.gz` & `tmp/zope_interface-6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.interface-6.3.tar", last modified: Fri Apr 12 15:13:37 2024, max compression
+gzip compressed data, was "zope_interface-6.4.tar", last modified: Wed May 15 20:23:10 2024, max compression
```

## Comparing `zope.interface-6.3.tar` & `zope_interface-6.4.tar`

### file list

```diff
@@ -1,134 +1,133 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.232517 zope.interface-6.3/
--rw-r--r--   0 jens       (501) staff       (20)      588 2024-04-12 14:44:49.000000 zope.interface-6.3/.coveragerc
--rwxr-xr-x   0 jens       (501) staff       (20)     2259 2024-04-12 14:44:49.000000 zope.interface-6.3/.manylinux-install.sh
--rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-04-12 14:44:49.000000 zope.interface-6.3/.manylinux.sh
--rw-r--r--   0 jens       (501) staff       (20)      664 2024-04-12 14:44:49.000000 zope.interface-6.3/.readthedocs.yaml
--rw-r--r--   0 jens       (501) staff       (20)    38966 2024-04-12 14:52:40.000000 zope.interface-6.3/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      799 2024-04-12 14:44:49.000000 zope.interface-6.3/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       32 2023-01-03 12:44:50.000000 zope.interface-6.3/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     2070 2023-01-03 12:44:50.000000 zope.interface-6.3/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      579 2024-04-12 14:51:36.000000 zope.interface-6.3/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    42016 2024-04-12 15:13:37.232439 zope.interface-6.3/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     1353 2023-01-03 12:44:50.000000 zope.interface-6.3/README.rst
--rw-r--r--   0 jens       (501) staff       (20)     1971 2024-04-12 14:51:59.000000 zope.interface-6.3/appveyor.yml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.220392 zope.interface-6.3/benchmarks/
--rw-r--r--   0 jens       (501) staff       (20)     8497 2023-01-03 12:44:50.000000 zope.interface-6.3/benchmarks/micro.py
--rw-r--r--   0 jens       (501) staff       (20)      838 2023-01-03 12:44:50.000000 zope.interface-6.3/build.cmd
--rw-r--r--   0 jens       (501) staff       (20)      215 2023-01-03 12:44:50.000000 zope.interface-6.3/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.222163 zope.interface-6.3/docs/
--rw-r--r--   0 jens       (501) staff       (20)     5592 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/Makefile
--rw-r--r--   0 jens       (501) staff       (20)    41051 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/README.rst
--rw-r--r--   0 jens       (501) staff       (20)    33998 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/README.ru.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.218221 zope.interface-6.3/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.222253 zope.interface-6.3/docs/_build/doctest/
--rw-r--r--   0 jens       (501) staff       (20)     1292 2024-04-12 14:47:42.000000 zope.interface-6.3/docs/_build/doctest/output.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.218262 zope.interface-6.3/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.223447 zope.interface-6.3/docs/_build/html/_sources/
--rw-r--r--   0 jens       (501) staff       (20)    41051 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/README.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    33998 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/README.ru.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    18817 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/adapter.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    21169 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/adapter.ru.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.224182 zope.interface-6.3/docs/_build/html/_sources/api/
--rw-r--r--   0 jens       (501) staff       (20)      691 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/adapters.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1283 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/common.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     2465 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/components.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    21746 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/declarations.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      165 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      687 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/ro.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     9948 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/api/specifications.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/changes.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1742 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/foodforthought.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     9509 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/hacking.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     6537 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/human.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    10681 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/human.ru.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    10222 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/_build/html/_sources/verify.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    18817 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/adapter.rst
--rw-r--r--   0 jens       (501) staff       (20)    21169 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/adapter.ru.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.224931 zope.interface-6.3/docs/api/
--rw-r--r--   0 jens       (501) staff       (20)      691 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/adapters.rst
--rw-r--r--   0 jens       (501) staff       (20)     1283 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/common.rst
--rw-r--r--   0 jens       (501) staff       (20)     2465 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/components.rst
--rw-r--r--   0 jens       (501) staff       (20)    21746 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/declarations.rst
--rw-r--r--   0 jens       (501) staff       (20)      165 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/index.rst
--rw-r--r--   0 jens       (501) staff       (20)      687 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/ro.rst
--rw-r--r--   0 jens       (501) staff       (20)     9948 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/api/specifications.rst
--rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/changes.rst
--rw-r--r--   0 jens       (501) staff       (20)     9130 2024-04-12 14:41:20.000000 zope.interface-6.3/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)     1742 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/foodforthought.rst
--rw-r--r--   0 jens       (501) staff       (20)     9509 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/hacking.rst
--rw-r--r--   0 jens       (501) staff       (20)     6537 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/human.rst
--rw-r--r--   0 jens       (501) staff       (20)    10681 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/human.ru.rst
--rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     5110 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/make.bat
--rw-r--r--   0 jens       (501) staff       (20)       68 2023-10-05 10:12:16.000000 zope.interface-6.3/docs/requirements.txt
--rw-r--r--   0 jens       (501) staff       (20)    10222 2023-01-03 12:44:50.000000 zope.interface-6.3/docs/verify.rst
--rw-r--r--   0 jens       (501) staff       (20)      599 2024-04-12 15:13:37.233159 zope.interface-6.3/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     5014 2024-04-12 14:52:58.000000 zope.interface-6.3/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.218506 zope.interface-6.3/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.225032 zope.interface-6.3/src/zope/
--rw-r--r--   0 jens       (501) staff       (20)       56 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/__init__.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.227583 zope.interface-6.3/src/zope/interface/
--rw-r--r--   0 jens       (501) staff       (20)     3460 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     4369 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/_compat.py
--rw-r--r--   0 jens       (501) staff       (20)     1057 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/_flatten.py
--rw-r--r--   0 jens       (501) staff       (20)    57205 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/_zope_interface_coptimizations.c
--rw-r--r--   0 jens       (501) staff       (20)    36218 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/adapter.py
--rw-r--r--   0 jens       (501) staff       (20)     3892 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/advice.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.228631 zope.interface-6.3/src/zope/interface/common/
--rw-r--r--   0 jens       (501) staff       (20)    10462 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     3027 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/builtins.py
--rw-r--r--   0 jens       (501) staff       (20)     6792 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/collections.py
--rw-r--r--   0 jens       (501) staff       (20)    20964 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/idatetime.py
--rw-r--r--   0 jens       (501) staff       (20)     5368 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     1242 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/io.py
--rw-r--r--   0 jens       (501) staff       (20)     4678 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/mapping.py
--rw-r--r--   0 jens       (501) staff       (20)     1682 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/common/numbers.py
--rw-r--r--   0 jens       (501) staff       (20)     5526 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/sequence.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.229436 zope.interface-6.3/src/zope/interface/common/tests/
--rw-r--r--   0 jens       (501) staff       (20)     5309 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     3907 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/basemapping.py
--rw-r--r--   0 jens       (501) staff       (20)     1345 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/common/tests/test_builtins.py
--rw-r--r--   0 jens       (501) staff       (20)     5718 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_collections.py
--rw-r--r--   0 jens       (501) staff       (20)     1923 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_idatetime.py
--rw-r--r--   0 jens       (501) staff       (20)      813 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_import_interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     1597 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_io.py
--rw-r--r--   0 jens       (501) staff       (20)     1394 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/common/tests/test_numbers.py
--rw-r--r--   0 jens       (501) staff       (20)    43007 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/declarations.py
--rw-r--r--   0 jens       (501) staff       (20)     4068 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/document.py
--rw-r--r--   0 jens       (501) staff       (20)     8636 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/exceptions.py
--rw-r--r--   0 jens       (501) staff       (20)    39260 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/interface.py
--rw-r--r--   0 jens       (501) staff       (20)    50126 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)    25829 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/registry.py
--rw-r--r--   0 jens       (501) staff       (20)    24157 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/ro.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.231755 zope.interface-6.3/src/zope/interface/tests/
--rw-r--r--   0 jens       (501) staff       (20)     3961 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)      898 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/advisory_testing.py
--rw-r--r--   0 jens       (501) staff       (20)      912 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/dummy.py
--rw-r--r--   0 jens       (501) staff       (20)      890 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/idummy.py
--rw-r--r--   0 jens       (501) staff       (20)      839 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/m1.py
--rw-r--r--   0 jens       (501) staff       (20)     3015 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/tests/odd.py
--rw-r--r--   0 jens       (501) staff       (20)    79479 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_adapter.py
--rw-r--r--   0 jens       (501) staff       (20)     5962 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_advice.py
--rw-r--r--   0 jens       (501) staff       (20)     1290 2023-01-03 12:44:50.000000 zope.interface-6.3/src/zope/interface/tests/test_compile_flags.py
--rw-r--r--   0 jens       (501) staff       (20)    82140 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_declarations.py
--rw-r--r--   0 jens       (501) staff       (20)    17164 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_document.py
--rw-r--r--   0 jens       (501) staff       (20)     1120 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_element.py
--rw-r--r--   0 jens       (501) staff       (20)     6412 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_exceptions.py
--rw-r--r--   0 jens       (501) staff       (20)    92312 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_interface.py
--rw-r--r--   0 jens       (501) staff       (20)     4377 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     7566 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_odd_declarations.py
--rw-r--r--   0 jens       (501) staff       (20)   112910 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_registry.py
--rw-r--r--   0 jens       (501) staff       (20)    14124 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_ro.py
--rw-r--r--   0 jens       (501) staff       (20)     1934 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_sorting.py
--rw-r--r--   0 jens       (501) staff       (20)    19191 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/tests/test_verify.py
--rw-r--r--   0 jens       (501) staff       (20)     7226 2024-04-12 14:41:20.000000 zope.interface-6.3/src/zope/interface/verify.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-04-12 15:13:37.231920 zope.interface-6.3/src/zope.interface.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    42016 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     3783 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/namespace_packages.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-03 13:57:16.000000 zope.interface-6.3/src/zope.interface.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      170 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2024-04-12 15:13:37.000000 zope.interface-6.3/src/zope.interface.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     2045 2024-04-12 14:51:36.000000 zope.interface-6.3/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.738219 zope_interface-6.4/
+-rw-r--r--   0 jens       (501) staff       (20)      588 2024-05-13 12:30:38.000000 zope_interface-6.4/.coveragerc
+-rwxr-xr-x   0 jens       (501) staff       (20)     2259 2024-05-13 12:30:38.000000 zope_interface-6.4/.manylinux-install.sh
+-rwxr-xr-x   0 jens       (501) staff       (20)      509 2024-05-13 12:30:38.000000 zope_interface-6.4/.manylinux.sh
+-rw-r--r--   0 jens       (501) staff       (20)      664 2024-05-13 12:30:38.000000 zope_interface-6.4/.readthedocs.yaml
+-rw-r--r--   0 jens       (501) staff       (20)    39159 2024-05-15 20:12:06.000000 zope_interface-6.4/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      799 2024-05-13 12:30:38.000000 zope_interface-6.4/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       32 2023-01-03 12:44:50.000000 zope_interface-6.4/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2023-01-03 12:44:50.000000 zope_interface-6.4/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      558 2024-05-13 12:30:38.000000 zope_interface-6.4/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    42209 2024-05-15 20:23:10.738130 zope_interface-6.4/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1353 2023-01-03 12:44:50.000000 zope_interface-6.4/README.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.713046 zope_interface-6.4/benchmarks/
+-rw-r--r--   0 jens       (501) staff       (20)     8497 2023-01-03 12:44:50.000000 zope_interface-6.4/benchmarks/micro.py
+-rw-r--r--   0 jens       (501) staff       (20)      838 2023-01-03 12:44:50.000000 zope_interface-6.4/build.cmd
+-rw-r--r--   0 jens       (501) staff       (20)      215 2023-01-03 12:44:50.000000 zope_interface-6.4/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.717054 zope_interface-6.4/docs/
+-rw-r--r--   0 jens       (501) staff       (20)     5592 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/Makefile
+-rw-r--r--   0 jens       (501) staff       (20)    41051 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)    33998 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/README.ru.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.707262 zope_interface-6.4/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.717330 zope_interface-6.4/docs/_build/doctest/
+-rw-r--r--   0 jens       (501) staff       (20)     1292 2024-05-14 09:54:19.000000 zope_interface-6.4/docs/_build/doctest/output.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.707308 zope_interface-6.4/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.721435 zope_interface-6.4/docs/_build/html/_sources/
+-rw-r--r--   0 jens       (501) staff       (20)    41051 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/README.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    33998 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/README.ru.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    18817 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/adapter.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    21169 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/adapter.ru.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.722457 zope_interface-6.4/docs/_build/html/_sources/api/
+-rw-r--r--   0 jens       (501) staff       (20)      691 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/adapters.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1283 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/common.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2465 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/components.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    21746 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/declarations.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      165 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      687 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/ro.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     9948 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/api/specifications.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/changes.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1742 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/foodforthought.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     9509 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/hacking.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     6537 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/human.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10681 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/human.ru.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10222 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/_build/html/_sources/verify.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    18817 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/adapter.rst
+-rw-r--r--   0 jens       (501) staff       (20)    21169 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/adapter.ru.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.723830 zope_interface-6.4/docs/api/
+-rw-r--r--   0 jens       (501) staff       (20)      691 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/adapters.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1283 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/common.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2465 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/components.rst
+-rw-r--r--   0 jens       (501) staff       (20)    21746 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/declarations.rst
+-rw-r--r--   0 jens       (501) staff       (20)      165 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)      687 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/ro.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9948 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/api/specifications.rst
+-rw-r--r--   0 jens       (501) staff       (20)       28 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/changes.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9130 2024-04-12 14:41:20.000000 zope_interface-6.4/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)     1742 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/foodforthought.rst
+-rw-r--r--   0 jens       (501) staff       (20)     9509 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/hacking.rst
+-rw-r--r--   0 jens       (501) staff       (20)     6537 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/human.rst
+-rw-r--r--   0 jens       (501) staff       (20)    10681 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/human.ru.rst
+-rw-r--r--   0 jens       (501) staff       (20)      639 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5110 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/make.bat
+-rw-r--r--   0 jens       (501) staff       (20)       68 2023-10-05 10:12:16.000000 zope_interface-6.4/docs/requirements.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10222 2023-01-03 12:44:50.000000 zope_interface-6.4/docs/verify.rst
+-rw-r--r--   0 jens       (501) staff       (20)      570 2024-05-15 20:23:10.738424 zope_interface-6.4/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     5014 2024-05-15 20:12:24.000000 zope_interface-6.4/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.707549 zope_interface-6.4/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.723986 zope_interface-6.4/src/zope/
+-rw-r--r--   0 jens       (501) staff       (20)       56 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/__init__.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.728593 zope_interface-6.4/src/zope/interface/
+-rw-r--r--   0 jens       (501) staff       (20)     3460 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     4369 2024-05-15 13:08:06.000000 zope_interface-6.4/src/zope/interface/_compat.py
+-rw-r--r--   0 jens       (501) staff       (20)     1057 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/_flatten.py
+-rw-r--r--   0 jens       (501) staff       (20)    57205 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/_zope_interface_coptimizations.c
+-rw-r--r--   0 jens       (501) staff       (20)    36218 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/adapter.py
+-rw-r--r--   0 jens       (501) staff       (20)     3892 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/advice.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.730860 zope_interface-6.4/src/zope/interface/common/
+-rw-r--r--   0 jens       (501) staff       (20)    10462 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     3027 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/builtins.py
+-rw-r--r--   0 jens       (501) staff       (20)     6792 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/collections.py
+-rw-r--r--   0 jens       (501) staff       (20)    20964 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/idatetime.py
+-rw-r--r--   0 jens       (501) staff       (20)     5368 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     1242 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/io.py
+-rw-r--r--   0 jens       (501) staff       (20)     4678 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/mapping.py
+-rw-r--r--   0 jens       (501) staff       (20)     1682 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/common/numbers.py
+-rw-r--r--   0 jens       (501) staff       (20)     5526 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/sequence.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.732600 zope_interface-6.4/src/zope/interface/common/tests/
+-rw-r--r--   0 jens       (501) staff       (20)     5476 2024-05-13 12:27:59.000000 zope_interface-6.4/src/zope/interface/common/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     3907 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/basemapping.py
+-rw-r--r--   0 jens       (501) staff       (20)     1345 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/common/tests/test_builtins.py
+-rw-r--r--   0 jens       (501) staff       (20)     5718 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/test_collections.py
+-rw-r--r--   0 jens       (501) staff       (20)     1923 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/test_idatetime.py
+-rw-r--r--   0 jens       (501) staff       (20)      813 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/test_import_interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     1663 2024-05-13 12:27:59.000000 zope_interface-6.4/src/zope/interface/common/tests/test_io.py
+-rw-r--r--   0 jens       (501) staff       (20)     1394 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/common/tests/test_numbers.py
+-rw-r--r--   0 jens       (501) staff       (20)    43007 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/declarations.py
+-rw-r--r--   0 jens       (501) staff       (20)     4068 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/document.py
+-rw-r--r--   0 jens       (501) staff       (20)     8636 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/exceptions.py
+-rw-r--r--   0 jens       (501) staff       (20)    39409 2024-05-15 20:11:48.000000 zope_interface-6.4/src/zope/interface/interface.py
+-rw-r--r--   0 jens       (501) staff       (20)    50126 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)    25829 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/registry.py
+-rw-r--r--   0 jens       (501) staff       (20)    24157 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/ro.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.737229 zope_interface-6.4/src/zope/interface/tests/
+-rw-r--r--   0 jens       (501) staff       (20)     3961 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)      898 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/advisory_testing.py
+-rw-r--r--   0 jens       (501) staff       (20)      912 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/dummy.py
+-rw-r--r--   0 jens       (501) staff       (20)      890 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/idummy.py
+-rw-r--r--   0 jens       (501) staff       (20)      839 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/m1.py
+-rw-r--r--   0 jens       (501) staff       (20)     3015 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/tests/odd.py
+-rw-r--r--   0 jens       (501) staff       (20)    79479 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_adapter.py
+-rw-r--r--   0 jens       (501) staff       (20)     6040 2024-05-15 20:11:48.000000 zope_interface-6.4/src/zope/interface/tests/test_advice.py
+-rw-r--r--   0 jens       (501) staff       (20)     1290 2023-01-03 12:44:50.000000 zope_interface-6.4/src/zope/interface/tests/test_compile_flags.py
+-rw-r--r--   0 jens       (501) staff       (20)    82140 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_declarations.py
+-rw-r--r--   0 jens       (501) staff       (20)    17164 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_document.py
+-rw-r--r--   0 jens       (501) staff       (20)     1120 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_element.py
+-rw-r--r--   0 jens       (501) staff       (20)     6412 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_exceptions.py
+-rw-r--r--   0 jens       (501) staff       (20)    92312 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_interface.py
+-rw-r--r--   0 jens       (501) staff       (20)     4377 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     7566 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_odd_declarations.py
+-rw-r--r--   0 jens       (501) staff       (20)   112910 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_registry.py
+-rw-r--r--   0 jens       (501) staff       (20)    14124 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_ro.py
+-rw-r--r--   0 jens       (501) staff       (20)     1934 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_sorting.py
+-rw-r--r--   0 jens       (501) staff       (20)    19191 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/tests/test_verify.py
+-rw-r--r--   0 jens       (501) staff       (20)     7226 2024-04-12 14:41:20.000000 zope_interface-6.4/src/zope/interface/verify.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2024-05-15 20:23:10.737610 zope_interface-6.4/src/zope.interface.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    42209 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     3770 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/namespace_packages.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-01-03 13:57:16.000000 zope_interface-6.4/src/zope.interface.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      170 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2024-05-15 20:23:10.000000 zope_interface-6.4/src/zope.interface.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2132 2024-05-13 12:30:38.000000 zope_interface-6.4/tox.ini
```

### Comparing `zope.interface-6.3/.coveragerc` & `zope_interface-6.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/.manylinux-install.sh` & `zope_interface-6.4/.manylinux-install.sh`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/.readthedocs.yaml` & `zope_interface-6.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/CHANGES.rst` & `zope_interface-6.4/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 =========
  Changes
 =========
 
+6.4 (2024-05-15)
+================
+
+- Adjust for incompatible changes in Python 3.13b1.
+  (`#292 <https://github.com/zopefoundation/zope.interface/issues/292>`)
+
+- Build windows wheels on GHA.
+
 6.3 (2024-04-12)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a6.
 
 
 6.2 (2024-02-16)
```

### Comparing `zope.interface-6.3/CONTRIBUTING.md` & `zope_interface-6.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/LICENSE.txt` & `zope_interface-6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/MANIFEST.in` & `zope_interface-6.4/MANIFEST.in`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated from:
 # https://github.com/zopefoundation/meta/tree/master/config/c-code
 include *.md
 include *.rst
 include *.txt
 include buildout.cfg
 include tox.ini
-include appveyor.yml
 include .coveragerc
 
 recursive-include docs *.py
 recursive-include docs *.rst
 recursive-include docs *.txt
 recursive-include docs Makefile
```

### Comparing `zope.interface-6.3/PKG-INFO` & `zope_interface-6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.3
+Version: 6.4
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,14 +71,22 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.4 (2024-05-15)
+================
+
+- Adjust for incompatible changes in Python 3.13b1.
+  (`#292 <https://github.com/zopefoundation/zope.interface/issues/292>`)
+
+- Build windows wheels on GHA.
+
 6.3 (2024-04-12)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a6.
 
 
 6.2 (2024-02-16)
```

### Comparing `zope.interface-6.3/README.rst` & `zope_interface-6.4/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/benchmarks/micro.py` & `zope_interface-6.4/benchmarks/micro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/build.cmd` & `zope_interface-6.4/build.cmd`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/Makefile` & `zope_interface-6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/README.rst` & `zope_interface-6.4/docs/README.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/README.ru.rst` & `zope_interface-6.4/docs/README.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/doctest/output.txt` & `zope_interface-6.4/docs/_build/doctest/output.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Results of doctest builder run on 2024-04-12 09:47:41
+Results of doctest builder run on 2024-05-14 11:54:18
 =====================================================
 
+Document: verify
+----------------
+1 items passed all tests:
+  78 tests in default
+78 tests in 1 items.
+78 passed and 0 failed.
+Test passed.
+
 Document: foodforthought
 ------------------------
 1 items passed all tests:
   25 tests in default
 25 tests in 1 items.
 25 passed and 0 failed.
 Test passed.
 
-Document: README
-----------------
+Document: api/declarations
+--------------------------
 1 items passed all tests:
- 218 tests in default
-218 tests in 1 items.
-218 passed and 0 failed.
+ 302 tests in default
+302 tests in 1 items.
+302 passed and 0 failed.
 Test passed.
 
 Document: adapter
 -----------------
 1 items passed all tests:
  164 tests in default
 164 tests in 1 items.
 164 passed and 0 failed.
 Test passed.
 
-Document: human
----------------
-1 items passed all tests:
-  18 tests in default
-18 tests in 1 items.
-18 passed and 0 failed.
-Test passed.
-
 Document: api/specifications
 ----------------------------
 1 items passed all tests:
  109 tests in default
 109 tests in 1 items.
 109 passed and 0 failed.
 Test passed.
 
-Document: api/declarations
---------------------------
+Document: human
+---------------
 1 items passed all tests:
- 302 tests in default
-302 tests in 1 items.
-302 passed and 0 failed.
+  18 tests in default
+18 tests in 1 items.
+18 passed and 0 failed.
 Test passed.
 
-Document: verify
+Document: README
 ----------------
 1 items passed all tests:
-  78 tests in default
-78 tests in 1 items.
-78 passed and 0 failed.
+ 218 tests in default
+218 tests in 1 items.
+218 passed and 0 failed.
 Test passed.
 
 Doctest summary
 ===============
   914 tests
     0 failures in tests
     0 failures in setup code
```

### Comparing `zope.interface-6.3/docs/_build/html/_sources/README.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/README.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/README.ru.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/README.ru.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/adapter.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/adapter.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/adapter.ru.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/adapter.ru.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/api/adapters.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/api/adapters.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/api/common.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/api/common.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/api/components.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/api/components.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/api/declarations.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/api/declarations.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/api/ro.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/api/ro.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/api/specifications.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/api/specifications.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/foodforthought.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/foodforthought.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/hacking.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/hacking.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/human.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/human.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/human.ru.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/human.ru.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/index.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/_build/html/_sources/verify.rst.txt` & `zope_interface-6.4/docs/_build/html/_sources/verify.rst.txt`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/adapter.rst` & `zope_interface-6.4/docs/adapter.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/adapter.ru.rst` & `zope_interface-6.4/docs/adapter.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/api/adapters.rst` & `zope_interface-6.4/docs/api/adapters.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/api/common.rst` & `zope_interface-6.4/docs/api/common.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/api/components.rst` & `zope_interface-6.4/docs/api/components.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/api/declarations.rst` & `zope_interface-6.4/docs/api/declarations.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/api/ro.rst` & `zope_interface-6.4/docs/api/ro.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/api/specifications.rst` & `zope_interface-6.4/docs/api/specifications.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/conf.py` & `zope_interface-6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/foodforthought.rst` & `zope_interface-6.4/docs/foodforthought.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/hacking.rst` & `zope_interface-6.4/docs/hacking.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/human.rst` & `zope_interface-6.4/docs/human.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/human.ru.rst` & `zope_interface-6.4/docs/human.ru.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/index.rst` & `zope_interface-6.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/make.bat` & `zope_interface-6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/docs/verify.rst` & `zope_interface-6.4/docs/verify.rst`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/setup.cfg` & `zope_interface-6.4/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-[bdist_wheel]
-universal = 0
-
 [zest.releaser]
 create-wheel = no
 
 [flake8]
 doctests = 1
 
 [check-manifest]
```

### Comparing `zope.interface-6.3/setup.py` & `zope_interface-6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 long_description = (
         read('README.rst')
         + '\n' +
         read('CHANGES.rst')
         )
 
 setup(name='zope.interface',
-      version='6.3',
+      version='6.4',
       url='https://github.com/zopefoundation/zope.interface',
       license='ZPL 2.1',
       description='Interfaces for Python',
       author='Zope Foundation and Contributors',
       author_email='zope-dev@zope.org',
       long_description=long_description,
       classifiers=[
```

### Comparing `zope.interface-6.3/src/zope/interface/__init__.py` & `zope_interface-6.4/src/zope/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/_compat.py` & `zope_interface-6.4/src/zope/interface/_compat.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/_flatten.py` & `zope_interface-6.4/src/zope/interface/_flatten.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/_zope_interface_coptimizations.c` & `zope_interface-6.4/src/zope/interface/_zope_interface_coptimizations.c`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/adapter.py` & `zope_interface-6.4/src/zope/interface/adapter.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/advice.py` & `zope_interface-6.4/src/zope/interface/advice.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/__init__.py` & `zope_interface-6.4/src/zope/interface/common/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/builtins.py` & `zope_interface-6.4/src/zope/interface/common/builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/collections.py` & `zope_interface-6.4/src/zope/interface/common/collections.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/idatetime.py` & `zope_interface-6.4/src/zope/interface/common/idatetime.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/interfaces.py` & `zope_interface-6.4/src/zope/interface/common/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/io.py` & `zope_interface-6.4/src/zope/interface/common/io.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/mapping.py` & `zope_interface-6.4/src/zope/interface/common/mapping.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/numbers.py` & `zope_interface-6.4/src/zope/interface/common/numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/sequence.py` & `zope_interface-6.4/src/zope/interface/common/sequence.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/tests/__init__.py` & `zope_interface-6.4/src/zope/interface/common/tests/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -125,11 +125,15 @@
         if not constructor:
             constructor = self.CONSTRUCTORS.get(x.__name__)
         if not constructor:
             constructor = x
         if constructor is unittest.SkipTest:
             self.skipTest("Cannot create " + str(x))
 
-        result = constructor()
+        try:
+            result = constructor()
+        except Exception as e:  # pragma: no cover
+            raise TypeError(
+                f'Failed to create instance of {constructor}') from e
         if hasattr(result, 'close'):
             self.addCleanup(result.close)
         return result
```

### Comparing `zope.interface-6.3/src/zope/interface/common/tests/basemapping.py` & `zope_interface-6.4/src/zope/interface/common/tests/basemapping.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/tests/test_builtins.py` & `zope_interface-6.4/src/zope/interface/common/tests/test_builtins.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/tests/test_collections.py` & `zope_interface-6.4/src/zope/interface/common/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/tests/test_idatetime.py` & `zope_interface-6.4/src/zope/interface/common/tests/test_idatetime.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/tests/test_import_interfaces.py` & `zope_interface-6.4/src/zope/interface/common/tests/test_import_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/common/tests/test_io.py` & `zope_interface-6.4/src/zope/interface/common/tests/test_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,8 +35,9 @@
         abc.BufferedWriter: lambda: abc.BufferedWriter(abc.StringIO()),
         abc.BufferedReader: lambda: abc.BufferedReader(abc.StringIO()),
         abc.TextIOWrapper: lambda: abc.TextIOWrapper(abc.BytesIO()),
         abc.BufferedRandom: lambda: abc.BufferedRandom(abc.BytesIO()),
         abc.BufferedRWPair: lambda: abc.BufferedRWPair(abc.BytesIO(), abc.BytesIO()),
         abc.FileIO: lambda: abc.FileIO(__file__),
         '_WindowsConsoleIO': unittest.SkipTest,
+        'WinConsoleIO': unittest.SkipTest,  # breaks on PyPy-3.10
     }
```

### Comparing `zope.interface-6.3/src/zope/interface/common/tests/test_numbers.py` & `zope_interface-6.4/src/zope/interface/common/tests/test_numbers.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/declarations.py` & `zope_interface-6.4/src/zope/interface/declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/document.py` & `zope_interface-6.4/src/zope/interface/document.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/exceptions.py` & `zope_interface-6.4/src/zope/interface/exceptions.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/interface.py` & `zope_interface-6.4/src/zope/interface/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -798,14 +798,17 @@
                 # __qualname__: PEP 3155 (Python 3.3+)
                 '__qualname__',
                 # __annotations__: PEP 3107 (Python 3.0+)
                 '__annotations__',
                 # __static_attributes__: Python 3.13a6+
                 # https://github.com/python/cpython/pull/115913
                 '__static_attributes__',
+                # __firstlineno__: Python 3.13b1+
+                # https://github.com/python/cpython/pull/118475
+                '__firstlineno__',
             )
             and aval is not _decorator_non_return
         }
 
     def interfaces(self):
         """Return an iterator for the interfaces in the specification.
         """
```

### Comparing `zope.interface-6.3/src/zope/interface/interfaces.py` & `zope_interface-6.4/src/zope/interface/interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/registry.py` & `zope_interface-6.4/src/zope/interface/registry.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/ro.py` & `zope_interface-6.4/src/zope/interface/ro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/__init__.py` & `zope_interface-6.4/src/zope/interface/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/advisory_testing.py` & `zope_interface-6.4/src/zope/interface/tests/advisory_testing.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/dummy.py` & `zope_interface-6.4/src/zope/interface/tests/dummy.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/idummy.py` & `zope_interface-6.4/src/zope/interface/tests/idummy.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/m1.py` & `zope_interface-6.4/src/zope/interface/tests/m1.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/odd.py` & `zope_interface-6.4/src/zope/interface/tests/odd.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_adapter.py` & `zope_interface-6.4/src/zope/interface/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_advice.py` & `zope_interface-6.4/src/zope/interface/tests/test_advice.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,19 @@
         for d in module.__dict__, f_globals:
             self.assertTrue(d is advisory_testing.my_globals)
 
     def test_inside_function_call(self):
         from zope.interface.advice import getFrameInfo
         kind, module, f_locals, f_globals = getFrameInfo(sys._getframe())
         self.assertEqual(kind, "function call")
-        self.assertTrue(f_locals is locals()) # ???
+
+        frame = sys._getframe()
+        self.assertEqual(f_locals, frame.f_locals)
+        self.assertEqual(f_locals, locals())
+
         for d in module.__dict__, f_globals:
             self.assertTrue(d is globals())
 
     def test_inside_exec(self):
         from zope.interface.advice import getFrameInfo
         _globals = {'getFrameInfo': getFrameInfo}
         _locals = {}
```

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_compile_flags.py` & `zope_interface-6.4/src/zope/interface/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_declarations.py` & `zope_interface-6.4/src/zope/interface/tests/test_declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_document.py` & `zope_interface-6.4/src/zope/interface/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_element.py` & `zope_interface-6.4/src/zope/interface/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_exceptions.py` & `zope_interface-6.4/src/zope/interface/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_interface.py` & `zope_interface-6.4/src/zope/interface/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_interfaces.py` & `zope_interface-6.4/src/zope/interface/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_odd_declarations.py` & `zope_interface-6.4/src/zope/interface/tests/test_odd_declarations.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_registry.py` & `zope_interface-6.4/src/zope/interface/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_ro.py` & `zope_interface-6.4/src/zope/interface/tests/test_ro.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_sorting.py` & `zope_interface-6.4/src/zope/interface/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/tests/test_verify.py` & `zope_interface-6.4/src/zope/interface/tests/test_verify.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope/interface/verify.py` & `zope_interface-6.4/src/zope/interface/verify.py`

 * *Files identical despite different names*

### Comparing `zope.interface-6.3/src/zope.interface.egg-info/PKG-INFO` & `zope_interface-6.4/src/zope.interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.interface
-Version: 6.3
+Version: 6.4
 Summary: Interfaces for Python
 Home-page: https://github.com/zopefoundation/zope.interface
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.org
 License: ZPL 2.1
 Keywords: interface,components,plugins
 Classifier: Development Status :: 5 - Production/Stable
@@ -71,14 +71,22 @@
 
 For detailed documentation, please see https://zopeinterface.readthedocs.io/en/latest/
 
 =========
  Changes
 =========
 
+6.4 (2024-05-15)
+================
+
+- Adjust for incompatible changes in Python 3.13b1.
+  (`#292 <https://github.com/zopefoundation/zope.interface/issues/292>`)
+
+- Build windows wheels on GHA.
+
 6.3 (2024-04-12)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a6.
 
 
 6.2 (2024-02-16)
```

### Comparing `zope.interface-6.3/src/zope.interface.egg-info/SOURCES.txt` & `zope_interface-6.4/src/zope.interface.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 .readthedocs.yaml
 CHANGES.rst
 CONTRIBUTING.md
 COPYRIGHT.txt
 LICENSE.txt
 MANIFEST.in
 README.rst
-appveyor.yml
 build.cmd
 buildout.cfg
 setup.cfg
 setup.py
 tox.ini
 benchmarks/micro.py
 docs/Makefile
```

### Comparing `zope.interface-6.3/tox.ini` & `zope_interface-6.4/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -59,25 +59,27 @@
     build
     check-manifest
     check-python-versions >= 0.20.0
     wheel
 commands_pre =
 commands =
     check-manifest
-    check-python-versions
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
     python -m build --sdist --no-isolation
     twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
 deps =
     isort
+    flake8
 commands =
     isort --check-only --diff {toxinidir}/src {toxinidir}/setup.py
+    flake8 src setup.py
 
 [testenv:isort-apply]
 basepython = python3
 skip_install = true
 commands_pre =
 deps =
     isort
```

