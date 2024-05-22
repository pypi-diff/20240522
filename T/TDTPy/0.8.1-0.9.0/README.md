# Comparing `tmp/TDTPy-0.8.1.tar.gz` & `tmp/TDTPy-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TDTPy-0.8.1.tar", last modified: Tue Mar 10 17:03:54 2020, max compression
+gzip compressed data, was "C:\Users\bburan\projects\open-source\tdtpy\dist\tmpp7qd3k_d\TDTPy-0.9.0.tar", last modified: Thu Aug 11 19:37:26 2022, max compression
```

## Comparing `TDTPy-0.8.1.tar` & `TDTPy-0.9.0.tar`

### file list

```diff
@@ -1,70 +1,59 @@
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/
--rw-rw-r--   0 bburan    (1000) bburan    (1000)       41 2020-03-09 19:22:45.000000 TDTPy-0.8.1/CHANGES.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     1545 2020-03-09 19:22:45.000000 TDTPy-0.8.1/LICENSE.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      130 2020-03-09 19:22:45.000000 TDTPy-0.8.1/MANIFEST.in
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     4035 2020-03-10 17:03:54.000000 TDTPy-0.8.1/PKG-INFO
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     2931 2020-03-09 19:22:45.000000 TDTPy-0.8.1/README.rst
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/TDTPy.egg-info/
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     4035 2020-03-10 17:03:54.000000 TDTPy-0.8.1/TDTPy.egg-info/PKG-INFO
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     1492 2020-03-10 17:03:54.000000 TDTPy-0.8.1/TDTPy.egg-info/SOURCES.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)        1 2020-03-10 17:03:54.000000 TDTPy-0.8.1/TDTPy.egg-info/dependency_links.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)       20 2020-03-10 17:03:54.000000 TDTPy-0.8.1/TDTPy.egg-info/requires.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)        4 2020-03-10 17:03:54.000000 TDTPy-0.8.1/TDTPy.egg-info/top_level.txt
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/docs/
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/docs/_build/
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/docs/_build/html/
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/docs/_build/html/_sources/
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      470 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/_build/html/_sources/api.rst.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     8903 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/_build/html/_sources/code_examples.rst.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     2503 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/_build/html/_sources/converting.rst.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    12257 2020-03-09 20:13:29.000000 TDTPy-0.8.1/docs/_build/html/_sources/dsp_buffer.rst.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     6479 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/_build/html/_sources/dsp_circuit.rst.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      579 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/_build/html/_sources/getting_started.rst.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     5546 2020-03-09 20:21:14.000000 TDTPy-0.8.1/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     5843 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/_build/html/_sources/server_api.rst.txt
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      470 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/api.rst
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     8903 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/code_examples.rst
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     2503 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/converting.rst
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    12257 2020-03-09 20:13:29.000000 TDTPy-0.8.1/docs/dsp_buffer.rst
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     6479 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/dsp_circuit.rst
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      579 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/getting_started.rst
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     5546 2020-03-09 20:21:14.000000 TDTPy-0.8.1/docs/index.rst
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     5843 2020-03-09 19:22:45.000000 TDTPy-0.8.1/docs/server_api.rst
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      243 2020-03-10 17:03:54.000000 TDTPy-0.8.1/setup.cfg
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     1815 2020-03-10 17:03:49.000000 TDTPy-0.8.1/setup.py
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/tdt/
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      581 2020-03-10 17:02:48.000000 TDTPy-0.8.1/tdt/__init__.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     5859 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/abstract_ring_buffer.py
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/tdt/actxobjects/
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     4309 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/PA5x.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    13772 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/RPcoX.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     7525 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/TDevAccX.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    14476 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/TTank.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    14476 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/TTankEng.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    34923 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/TTankInterfaces.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    26012 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/TTankX.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     5462 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/ZBUSx.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     1158 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/actxobjects/__init__.py
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/tdt/components/
--rw-rw-r--   0 bburan    (1000) bburan    (1000)        0 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/components/__init__.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)   276469 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/components/data_reduction.rcx
--rw-rw-r--   0 bburan    (1000) bburan    (1000)   229077 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/components/test_RZ6_audio_out.rcx
--rw-rw-r--   0 bburan    (1000) bburan    (1000)   570843 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/components/test_physiology_RZ5.rcx
--rw-rw-r--   0 bburan    (1000) bburan    (1000)   580333 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/components/test_physiology_RZ6.rcx
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    46497 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/components/test_read.rcx
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      939 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/constants.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     2979 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/convert.py
-drwxrwxr-x   0 bburan    (1000) bburan    (1000)        0 2020-03-10 17:03:54.000000 TDTPy-0.8.1/tdt/device/
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     4666 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/device/RZ6.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)        0 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/device/__init__.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    17928 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/dsp_buffer.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    16902 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/dsp_circuit.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)      207 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/dsp_error.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    14050 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/dsp_process.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     3190 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/dsp_project.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)    13353 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/dsp_server.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     4010 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/shared_ring_buffer.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     1725 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/test_io_speed.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     2112 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/test_process.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     8826 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/tests.py
--rw-rw-r--   0 bburan    (1000) bburan    (1000)     8955 2020-03-09 19:22:45.000000 TDTPy-0.8.1/tdt/util.py
+drwxrwxrwx   0        0        0        0 2022-08-11 19:37:26.000000 TDTPy-0.9.0/
+-rw-rw-rw-   0        0        0      385 2022-08-11 19:35:22.000000 TDTPy-0.9.0/CHANGES.txt
+-rw-rw-rw-   0        0        0     1545 2022-08-11 19:29:57.000000 TDTPy-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      130 2022-08-11 19:29:57.000000 TDTPy-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3583 2022-08-11 19:37:26.000000 TDTPy-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2922 2022-08-11 19:29:57.000000 TDTPy-0.9.0/README.rst
+drwxrwxrwx   0        0        0        0 2022-08-11 19:37:26.000000 TDTPy-0.9.0/TDTPy.egg-info/
+-rw-rw-rw-   0        0        0     3583 2022-08-11 19:37:26.000000 TDTPy-0.9.0/TDTPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1135 2022-08-11 19:37:26.000000 TDTPy-0.9.0/TDTPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-11 19:37:26.000000 TDTPy-0.9.0/TDTPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2022-08-11 19:37:26.000000 TDTPy-0.9.0/TDTPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2022-08-11 19:37:26.000000 TDTPy-0.9.0/TDTPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-08-11 19:37:26.000000 TDTPy-0.9.0/docs/
+-rw-rw-rw-   0        0        0      470 2022-08-11 19:29:57.000000 TDTPy-0.9.0/docs/api.rst
+-rw-rw-rw-   0        0        0     8903 2022-08-11 19:29:57.000000 TDTPy-0.9.0/docs/code_examples.rst
+-rw-rw-rw-   0        0        0     2503 2022-08-11 19:29:57.000000 TDTPy-0.9.0/docs/converting.rst
+-rw-rw-rw-   0        0        0    12555 2022-08-11 19:29:57.000000 TDTPy-0.9.0/docs/dsp_buffer.rst
+-rw-rw-rw-   0        0        0     6479 2022-08-11 19:29:57.000000 TDTPy-0.9.0/docs/dsp_circuit.rst
+-rw-rw-rw-   0        0        0      579 2022-08-11 19:29:57.000000 TDTPy-0.9.0/docs/getting_started.rst
+-rw-rw-rw-   0        0        0     5673 2022-08-11 19:29:57.000000 TDTPy-0.9.0/docs/index.rst
+-rw-rw-rw-   0        0        0     5843 2022-08-11 19:29:57.000000 TDTPy-0.9.0/docs/server_api.rst
+-rw-rw-rw-   0        0        0      259 2022-08-11 19:37:26.000000 TDTPy-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1867 2022-08-11 19:29:57.000000 TDTPy-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-11 19:37:26.000000 TDTPy-0.9.0/tdt/
+-rw-rw-rw-   0        0        0      304 2022-08-11 19:30:19.000000 TDTPy-0.9.0/tdt/__init__.py
+-rw-rw-rw-   0        0        0     5859 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/abstract_ring_buffer.py
+drwxrwxrwx   0        0        0        0 2022-08-11 19:37:26.000000 TDTPy-0.9.0/tdt/actxobjects/
+-rw-rw-rw-   0        0        0     4309 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/PA5x.py
+-rw-rw-rw-   0        0        0    13772 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/RPcoX.py
+-rw-rw-rw-   0        0        0     7738 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/TDevAccX.py
+-rw-rw-rw-   0        0        0    14663 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/TTank.py
+-rw-rw-rw-   0        0        0    14663 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/TTankEng.py
+-rw-rw-rw-   0        0        0    35535 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/TTankInterfaces.py
+-rw-rw-rw-   0        0        0    26630 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/TTankX.py
+-rw-rw-rw-   0        0        0     5462 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/ZBUSx.py
+-rw-rw-rw-   0        0        0     1158 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/actxobjects/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-11 19:37:26.000000 TDTPy-0.9.0/tdt/components/
+-rw-rw-rw-   0        0        0        0 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/components/__init__.py
+-rw-rw-rw-   0        0        0   276469 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/components/data_reduction.rcx
+-rw-rw-rw-   0        0        0   229077 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/components/test_RZ6_audio_out.rcx
+-rw-rw-rw-   0        0        0   570843 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/components/test_physiology_RZ5.rcx
+-rw-rw-rw-   0        0        0   580333 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/components/test_physiology_RZ6.rcx
+-rw-rw-rw-   0        0        0    46497 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/components/test_read.rcx
+-rw-rw-rw-   0        0        0      939 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/constants.py
+-rw-rw-rw-   0        0        0     3104 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/convert.py
+drwxrwxrwx   0        0        0        0 2022-08-11 19:37:26.000000 TDTPy-0.9.0/tdt/device/
+-rw-rw-rw-   0        0        0     4666 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/device/RZ6.py
+-rw-rw-rw-   0        0        0        0 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/device/__init__.py
+-rw-rw-rw-   0        0        0    19130 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/dsp_buffer.py
+-rw-rw-rw-   0        0        0    16902 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/dsp_circuit.py
+-rw-rw-rw-   0        0        0      207 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/dsp_error.py
+-rw-rw-rw-   0        0        0    14050 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/dsp_process.py
+-rw-rw-rw-   0        0        0     3190 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/dsp_project.py
+-rw-rw-rw-   0        0        0    13329 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/dsp_server.py
+-rw-rw-rw-   0        0        0     4010 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/shared_ring_buffer.py
+-rw-rw-rw-   0        0        0     1725 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/test_io_speed.py
+-rw-rw-rw-   0        0        0     2112 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/test_process.py
+-rw-rw-rw-   0        0        0     8826 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/tests.py
+-rw-rw-rw-   0        0        0     8955 2022-08-11 19:29:57.000000 TDTPy-0.9.0/tdt/util.py
```

### Comparing `TDTPy-0.8.1/LICENSE.txt` & `TDTPy-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/PKG-INFO` & `TDTPy-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-Metadata-Version: 1.1
-Name: TDTPy
-Version: 0.8.1
-Summary: Module for communicating with TDT's System 3 hardware
-Home-page: http://tdtpy.readthedocs.org
-Author: The TDTPy development team
-Author-email: bburan@alum.mit.edu
-License: BSD (3-clause)
-Description: =====
-        TDTPy
-        =====
-        
-        .. image:: https://zenodo.org/badge/doi/10.5281/zenodo.17651.svg   
-           :target: http://dx.doi.org/10.5281/zenodo.17651
-        
-        TDTPy is a Python wrapper around `Tucker-Davis Technologies`_ `ActiveX library`_
-        [PDF link] (known as RPcoX) for communicating with their System 3 hardware (e.g.
-        the RP2.1, RX6, RZ6, etc.).
-        
-        In addition to the standard operations (loading
-        circuits, configuring tags and reading/writing to hardware buffers), TDTPy
-        offers a number of high-level features that are not included in the ActiveX
-        library:
-        
-        * **Handling type conversion** between analog and digital units (e.g. converting
-          seconds to number of DSP cycles based on the CPU frequency of the hardware).
-        * **Remote procedure call (RPC) server** for allowing multiple processes and/or programs
-          to communicate with the hardware across the same connection. The drivers
-          provided by TDT do not handle concurrency issues. To handle these issues, we
-          have created a RPC server that handles concurrency issues, allowing multiple
-          programs to talk to the hardware simultaneously. The programs can either run
-          on the same computer or on a separate computer.
-        * If you use the RPC server, your client code can run on **any platform** (e.g. Mac
-          OSX, Unix, Solaris, etc); however, the server must run on a Windows-based
-          computer.
-        * **Simple reads and writes.** The hardware buffers are implemented as "ring
-          buffers" with various features such as multichannel storage and data
-          compression. TDTPy automatically detects the configuration of the hardware
-          buffer and returns a buffer object (`DSPBuffer`) that you can read/write
-          to without having to deal with the intricacies of the hardware buffer itself.
-        * **Robust error handling.** Some methods in the ActiveX library will fail silently
-          (e.g. if you try to access a nonexistent tag, attempt to write more data than
-          the hardware buffer can hold, or wire up a tag to a static port). When the
-          RPvds circuit is first loaded to the hardware, TDTPy will inspect the
-          microcode (i.e. the RPvds circuit) and store some information about the tags
-          and buffers available. All subsequent operations are validated against this
-          metadata before being passed to the ActiveX library. If an invalid operation
-          is attempted, a DSPError is raised with the appropriate message.
-        
-        .. _Tucker-Davis Technologies: http://www.tdt.com
-        .. _System 3: http://www.tdt.com/products.htm 
-        .. _ActiveX library: http://www.tdt.com/T2Download/manuals/ActiveX_User_Reference.pdf
-        
-        The minimum required dependencies to run the software are:
-        
-          - Python >= 2.7
-          - NumPy >= 1.8
-          - pywin32
-          - six
-        
-        -------
-        License
-        -------
-        TDTPy is distributed under the BSD license.
-        
-        ------------
-        Contributors
-        ------------
-        * Brad Buran (New York University, Oregon Health & Science University)
-        * Eric Larson (University of Washington)
-        * Decibel Therapeutics, Inc.
-        
-        Source code: http://github.com/LABSN/tdtpy
-        
-        Documentation: http://tdtpy.readthedocs.org
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved
+Metadata-Version: 2.1
+Name: TDTPy
+Version: 0.9.0
+Summary: Module for communicating with TDT's System 3 hardware
+Home-page: http://tdtpy.readthedocs.org
+Author: The TDTPy development team
+Author-email: bburan@alum.mit.edu
+License: BSD (3-clause)
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Classifier: License :: OSI Approved
+Provides-Extra: test
+License-File: LICENSE.txt
+
+=====
+TDTPy
+=====
+
+.. image:: https://zenodo.org/badge/doi/10.5281/zenodo.17651.svg   
+   :target: http://dx.doi.org/10.5281/zenodo.17651
+
+TDTPy is a Python wrapper around `Tucker-Davis Technologies`_ `ActiveX library`_
+[PDF link] (known as RPcoX) for communicating with their System 3 hardware (e.g.
+the RP2.1, RX6, RZ6, etc.).
+
+In addition to the standard operations (loading
+circuits, configuring tags and reading/writing to hardware buffers), TDTPy
+offers a number of high-level features that are not included in the ActiveX
+library:
+
+* **Handling type conversion** between analog and digital units (e.g. converting
+  seconds to number of DSP cycles based on the CPU frequency of the hardware).
+* **Remote procedure call (RPC) server** for allowing multiple processes and/or programs
+  to communicate with the hardware across the same connection. The drivers
+  provided by TDT do not handle concurrency issues. To handle these issues, we
+  have created a RPC server that handles concurrency issues, allowing multiple
+  programs to talk to the hardware simultaneously. The programs can either run
+  on the same computer or on a separate computer.
+* If you use the RPC server, your client code can run on **any platform** (e.g. Mac
+  OSX, Unix, Solaris, etc); however, the server must run on a Windows-based
+  computer.
+* **Simple reads and writes.** The hardware buffers are implemented as "ring
+  buffers" with various features such as multichannel storage and data
+  compression. TDTPy automatically detects the configuration of the hardware
+  buffer and returns a buffer object (`DSPBuffer`) that you can read/write
+  to without having to deal with the intricacies of the hardware buffer itself.
+* **Robust error handling.** Some methods in the ActiveX library will fail silently
+  (e.g. if you try to access a nonexistent tag, attempt to write more data than
+  the hardware buffer can hold, or wire up a tag to a static port). When the
+  RPvds circuit is first loaded to the hardware, TDTPy will inspect the
+  microcode (i.e. the RPvds circuit) and store some information about the tags
+  and buffers available. All subsequent operations are validated against this
+  metadata before being passed to the ActiveX library. If an invalid operation
+  is attempted, a DSPError is raised with the appropriate message.
+
+.. _Tucker-Davis Technologies: http://www.tdt.com
+.. _System 3: http://www.tdt.com/products.htm 
+.. _ActiveX library: http://www.tdt.com/T2Download/manuals/ActiveX_User_Reference.pdf
+
+The minimum required dependencies to run the software are:
+
+  - Python >= 3.7
+  - NumPy >= 1.8
+  - pywin32
+
+-------
+License
+-------
+TDTPy is distributed under the BSD license.
+
+------------
+Contributors
+------------
+* Brad Buran (New York University, Oregon Health & Science University)
+* Eric Larson (University of Washington)
+* Decibel Therapeutics, Inc.
+
+Source code: http://github.com/LABSN/tdtpy
+
+Documentation: http://tdtpy.readthedocs.org
+
```

### Comparing `TDTPy-0.8.1/README.rst` & `TDTPy-0.9.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -41,18 +41,17 @@
 
 .. _Tucker-Davis Technologies: http://www.tdt.com
 .. _System 3: http://www.tdt.com/products.htm 
 .. _ActiveX library: http://www.tdt.com/T2Download/manuals/ActiveX_User_Reference.pdf
 
 The minimum required dependencies to run the software are:
 
-  - Python >= 2.7
+  - Python >= 3.7
   - NumPy >= 1.8
   - pywin32
-  - six
 
 -------
 License
 -------
 TDTPy is distributed under the BSD license.
 
 ------------
```

### Comparing `TDTPy-0.8.1/TDTPy.egg-info/PKG-INFO` & `TDTPy-0.9.0/TDTPy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-Metadata-Version: 1.1
-Name: TDTPy
-Version: 0.8.1
-Summary: Module for communicating with TDT's System 3 hardware
-Home-page: http://tdtpy.readthedocs.org
-Author: The TDTPy development team
-Author-email: bburan@alum.mit.edu
-License: BSD (3-clause)
-Description: =====
-        TDTPy
-        =====
-        
-        .. image:: https://zenodo.org/badge/doi/10.5281/zenodo.17651.svg   
-           :target: http://dx.doi.org/10.5281/zenodo.17651
-        
-        TDTPy is a Python wrapper around `Tucker-Davis Technologies`_ `ActiveX library`_
-        [PDF link] (known as RPcoX) for communicating with their System 3 hardware (e.g.
-        the RP2.1, RX6, RZ6, etc.).
-        
-        In addition to the standard operations (loading
-        circuits, configuring tags and reading/writing to hardware buffers), TDTPy
-        offers a number of high-level features that are not included in the ActiveX
-        library:
-        
-        * **Handling type conversion** between analog and digital units (e.g. converting
-          seconds to number of DSP cycles based on the CPU frequency of the hardware).
-        * **Remote procedure call (RPC) server** for allowing multiple processes and/or programs
-          to communicate with the hardware across the same connection. The drivers
-          provided by TDT do not handle concurrency issues. To handle these issues, we
-          have created a RPC server that handles concurrency issues, allowing multiple
-          programs to talk to the hardware simultaneously. The programs can either run
-          on the same computer or on a separate computer.
-        * If you use the RPC server, your client code can run on **any platform** (e.g. Mac
-          OSX, Unix, Solaris, etc); however, the server must run on a Windows-based
-          computer.
-        * **Simple reads and writes.** The hardware buffers are implemented as "ring
-          buffers" with various features such as multichannel storage and data
-          compression. TDTPy automatically detects the configuration of the hardware
-          buffer and returns a buffer object (`DSPBuffer`) that you can read/write
-          to without having to deal with the intricacies of the hardware buffer itself.
-        * **Robust error handling.** Some methods in the ActiveX library will fail silently
-          (e.g. if you try to access a nonexistent tag, attempt to write more data than
-          the hardware buffer can hold, or wire up a tag to a static port). When the
-          RPvds circuit is first loaded to the hardware, TDTPy will inspect the
-          microcode (i.e. the RPvds circuit) and store some information about the tags
-          and buffers available. All subsequent operations are validated against this
-          metadata before being passed to the ActiveX library. If an invalid operation
-          is attempted, a DSPError is raised with the appropriate message.
-        
-        .. _Tucker-Davis Technologies: http://www.tdt.com
-        .. _System 3: http://www.tdt.com/products.htm 
-        .. _ActiveX library: http://www.tdt.com/T2Download/manuals/ActiveX_User_Reference.pdf
-        
-        The minimum required dependencies to run the software are:
-        
-          - Python >= 2.7
-          - NumPy >= 1.8
-          - pywin32
-          - six
-        
-        -------
-        License
-        -------
-        TDTPy is distributed under the BSD license.
-        
-        ------------
-        Contributors
-        ------------
-        * Brad Buran (New York University, Oregon Health & Science University)
-        * Eric Larson (University of Washington)
-        * Decibel Therapeutics, Inc.
-        
-        Source code: http://github.com/LABSN/tdtpy
-        
-        Documentation: http://tdtpy.readthedocs.org
-        
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: System :: Hardware
-Classifier: License :: OSI Approved
+Metadata-Version: 2.1
+Name: TDTPy
+Version: 0.9.0
+Summary: Module for communicating with TDT's System 3 hardware
+Home-page: http://tdtpy.readthedocs.org
+Author: The TDTPy development team
+Author-email: bburan@alum.mit.edu
+License: BSD (3-clause)
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: System :: Hardware
+Classifier: License :: OSI Approved
+Provides-Extra: test
+License-File: LICENSE.txt
+
+=====
+TDTPy
+=====
+
+.. image:: https://zenodo.org/badge/doi/10.5281/zenodo.17651.svg   
+   :target: http://dx.doi.org/10.5281/zenodo.17651
+
+TDTPy is a Python wrapper around `Tucker-Davis Technologies`_ `ActiveX library`_
+[PDF link] (known as RPcoX) for communicating with their System 3 hardware (e.g.
+the RP2.1, RX6, RZ6, etc.).
+
+In addition to the standard operations (loading
+circuits, configuring tags and reading/writing to hardware buffers), TDTPy
+offers a number of high-level features that are not included in the ActiveX
+library:
+
+* **Handling type conversion** between analog and digital units (e.g. converting
+  seconds to number of DSP cycles based on the CPU frequency of the hardware).
+* **Remote procedure call (RPC) server** for allowing multiple processes and/or programs
+  to communicate with the hardware across the same connection. The drivers
+  provided by TDT do not handle concurrency issues. To handle these issues, we
+  have created a RPC server that handles concurrency issues, allowing multiple
+  programs to talk to the hardware simultaneously. The programs can either run
+  on the same computer or on a separate computer.
+* If you use the RPC server, your client code can run on **any platform** (e.g. Mac
+  OSX, Unix, Solaris, etc); however, the server must run on a Windows-based
+  computer.
+* **Simple reads and writes.** The hardware buffers are implemented as "ring
+  buffers" with various features such as multichannel storage and data
+  compression. TDTPy automatically detects the configuration of the hardware
+  buffer and returns a buffer object (`DSPBuffer`) that you can read/write
+  to without having to deal with the intricacies of the hardware buffer itself.
+* **Robust error handling.** Some methods in the ActiveX library will fail silently
+  (e.g. if you try to access a nonexistent tag, attempt to write more data than
+  the hardware buffer can hold, or wire up a tag to a static port). When the
+  RPvds circuit is first loaded to the hardware, TDTPy will inspect the
+  microcode (i.e. the RPvds circuit) and store some information about the tags
+  and buffers available. All subsequent operations are validated against this
+  metadata before being passed to the ActiveX library. If an invalid operation
+  is attempted, a DSPError is raised with the appropriate message.
+
+.. _Tucker-Davis Technologies: http://www.tdt.com
+.. _System 3: http://www.tdt.com/products.htm 
+.. _ActiveX library: http://www.tdt.com/T2Download/manuals/ActiveX_User_Reference.pdf
+
+The minimum required dependencies to run the software are:
+
+  - Python >= 3.7
+  - NumPy >= 1.8
+  - pywin32
+
+-------
+License
+-------
+TDTPy is distributed under the BSD license.
+
+------------
+Contributors
+------------
+* Brad Buran (New York University, Oregon Health & Science University)
+* Eric Larson (University of Washington)
+* Decibel Therapeutics, Inc.
+
+Source code: http://github.com/LABSN/tdtpy
+
+Documentation: http://tdtpy.readthedocs.org
+
```

### Comparing `TDTPy-0.8.1/docs/_build/html/_sources/code_examples.rst.txt` & `TDTPy-0.9.0/docs/code_examples.rst`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/docs/_build/html/_sources/converting.rst.txt` & `TDTPy-0.9.0/docs/converting.rst`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/docs/_build/html/_sources/dsp_buffer.rst.txt` & `TDTPy-0.9.0/docs/dsp_buffer.rst`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,298 +1,298 @@
-:class:`tdt.DSPBuffer` -- Wrapper for RPvds buffer objects
-==========================================================
-
-Each buffer requires tags linked to the data and index parameters of the buffer
-component.  All other tags described below are optional, but will be used if
-present.  The data tag and supporting tags can have any name; however, the
-recommended approach is to use the data tag plus one of the following prefixes
-indicating the purpose of the supporting tag.
-
-    i
-        index tag (idx_tag)
-    n
-        size tag (size_tag)
-    sf
-        scaling factor tag (sf_tag)
-    c
-        cycle tag (cycle_tag)
-    d
-        downsampling tag (dec_tag)
-
-If no value is provided for a tag, the default extension is added to the value
-for the data_tag and the circuit is checked to see if the tag exists.  For
-example, if you have `spikes`, `spikes_i`, and `spikes_n` tags in your RPvds
-circuit, you can simply initialize the class by passing only the name of the
-data tag (`spikes`) and it will automatically use `spikes_i` and `spikes_n` as
-the index and size tags, respectively::
-
-   >>> buffer = circuit.get_buffer('spikes', 'r')
-
-If a required tag cannot be found (either by explicitly defining the tag name or
-automatically by adding the default extension to the data tag name), an error is
-raised.
-
-.. image:: example_buffer.*
-
-In the above code, there is a singlue buffer named `contact` with three
-supporting tags (`contact_d`, `contact_sf` and `contact_i`) that assist the
-:mod:`tdt.DSPBuffer` class in reading data stored in `contact`.  For example, we
-know that, due to the fact that we are applying a scaling factor of 127 to the
-floating-point data stored in the contact buffer, we are only saving the data
-with a resolution of 0.00787::
-
-    >>> contact_buffer = circuit.get_buffer('contact', 'r', src_type='int8')
-    >>> print contact_buffer.resolution
-    0.00787
-
-Because we specified that the data is stored in 8-bit format, four samples are
-being compressed into a single 32-bit slot::
-
-    >>> print contact_buffer.compression
-    4
-
-Since `contact_d` is set to 80 (i.e. acquire and save a sample every 80 cycles),
-we know the sampling frequency of the contact data is only 1/80th of the
-sampling rate of the DSP::
-
-    >>> print circuit.fs
-    97656.25
-    >>> print contact_buffer.fs
-    1220.703125
-
-.. note::
-
-    This buffer uses the enable and reset hops to control data acquisition,
-    consistent with the coding guidelines described in dsp_buffer.rst.
-
-.. note::
-
-    Currently TDTPy does not support changing sampling rate on-the-fly (you can
-    do it, but you need to reload the buffer).
-
-Writing single channel data
----------------------------
-
-If you are using epoch-based outputs (where you upload a waveform of fixed size
-and halt playout once the buffer is complete), then you can use the
-`WriteableDSPBuffer.set` method::
-
-   >>> speaker_buffer = circuit.get_buffer('speaker', 'w')
-   >>> speaker_buffer.set(tone_pip)
-
-If you are using continuous output (e.g., where you need to update the stream
-as the experiment progresses)::
-
-TODO
-
-TDTPy has not been tested with writing multi-channel data (mainly because we
-currently do not have a use-case for it). 
-
-Reading single and multichannel data
-------------------------------------
-TODO
-
-Tags
-----
-data_tag : string (required)
-    Tag to read data from
-idx_tag : defaults to data_tag_i (required)
-    Tag indicating current index of buffer.  For buffer reads this tag
-    serves as a "handshake" (i.e. when the index changes, new data is
-    available).
-size_tag : defaults to data_tag_n (optional)
-    Tag indicating current size of buffer.
-sf_tag : defaults to data_tag_sf (optional)
-    Tag indicating scaling factor applied to data before it is stored in the
-    buffer.
-cycle_tag : defaults to data_tag_c (optional)
-    Tag indicating number of times buffer has wrapped around to beginning.
-    Used to ensure no data is lost.
-dec_tag : defaults to data_tag_d (optional)
-    Tag indicating decimation factor.  Used to compute sampling frequency of
-    data stored in buffer: e.g. if circuit runs at 100 kHz, but you only
-    sample every 25 cycles, the actual sampling frequency is 4 kHz.  
-    
-Additional Parameters
-----------------------
-circuit : instance of `tdt.DSPCircuit`
-    Circuit object the buffer is attached to
-block_size : int
-    Coerce data read/write to multiple of the block size.  Must be a
-    multiple of the channel number.
-src_type : str or numpy dtype
-    Type of data in buffer (can be a string or numpy dtype).  Valid data
-    formats are float32, int32, int16 and int8.
-dest_type : str or numpy dtype
-    Type to convert data to
-channels : int
-    Number of channels stored in buffer
-
-Available attributes
---------------------
-
-When the buffer is first loaded, there is some "introspection" of the circuit to
-determine key properties of the buffer (e.g. what is the format of the data
-stored in the DSP buffer, how much data can be stored before the buffer fills
-up, etc.).
-
-data_tag, idx_tag, size_tag, sf_tag, cycle_tag, dec_tag : str
-    Names of supporting tags present in the circuit (both the names provided
-    when the b uffer was loaded as well as the ones automatically discovered
-    when the buffer is created.  None if the tag is not present.
-src_type 
-    Numpy dtype of the data stored on the device.  Defaults to float32.
-dest_type
-    Numpy dtype of array returned when data is read from the device
-compression
-    Number of samples stored in a single 32-bit "slot" on the device.  For
-    example, if you are using the MCFloat2Int8 component to convert four samples
-    of data into 8-bit integers and storing these four samples as a single
-    32-bit work, the compression factor is 4.
-sf
-    Scaling factor of the data.  If you are not using compression, the scaling
-    factor is almost certainly one.
-resolution
-    If data is being compressed, computes the actual resolution of the
-    acquired data given the scaling factor.  For example, if you are
-    compressing data into an 8-bit integer using a scaling factor of 10,
-    then the resolution of the acquired data will be 0.1 since numbers will
-    get rounded to the nearest tenth (e.g. 0.183 will get rounded to 0.2).
-dec_factor
-    Also called the "downsampling rate".  Indicates the number of device
-    cycles before a sample is stored in the buffer.  If 1 (default), a sample is
-    acquired on every cycle.  If 2, a sample is acquired on every other cycle.
-fs
-    Sampling frequency of data stored in buffer.  This is basically the
-    sampling frequency of the device divided by the decimation factor
-    (dec_factor): e.g. if a sample is acquired only on every other cycle,
-    then the sampling frequency of the buffer is effectively half of the
-    device clock rate.
-channels
-    Number of channels
-block_size
-    Coerce read size to multiples of this value (can be overridden if needed)
-
-Buffer size attributes
-----------------------
-
-There are three ways to think about the buffer size.  First, how many 32-bit
-words can the buffer hold?  All buffer components in a RPvds circuit store data
-in 32-bit word segments.  However, we can store two 16-bit values or four 8-bit
-values into a single word.  Even if a buffer can only hold 1000 32-bit words, it
-may actually hold 2000 or 4000 samples if we are compressing two or four samples
-of data into a single buffer "slot".  Now, if we are storing multiple channels
-of data in a single buffer, then the buffer will fill up more quickly than an
-identically-sized buffer storing only a single channel of data.  By reporting
-buffer size as the number of samples per channel, we can get a sense for how
-quickly the buffer will fill up.
-
->>> buffer = circuit.get_buffer('spikes', 'r', channels=16)
->>> print buffer.compression    # number of samples in each buffer slot
-2
->>> print buffer.n_slots        # number of slots
-4000
->>> print buffer.n_samples      # number of samples
-8000
->>> print buffer.size           # number of samples per channel
-500
->>> print buffer.fs             # sampling frequency of buffer data
-12207.03125
->>> print buffer.sample_time    # time (in seconds) to fill up the buffer
-0.04096
-
-In the above example, we know that even though the buffer can hold 8,000
-samples of data, it will fill up after only 500 samples of 16-channel data are
-collected.  At a sampling frequency of 12 kHz, this means the buffer can only
-hold 41 msec of 16-channel data.  This provides a useful metric for knowing
-whether we have set the buffer size appropriately.
-
-n_slots
-    Size in number of 32-bit words (the buffer's atomic unit of of storage)
-n_samples
-    Size in number of samples (data points) that can be stored in the buffer.
-    The size will be either 1x, 2x or 4x the size of n_slots depending on how
-    many samples are stored in each slot.
-size
-    Size in number of samples (data points) per channel.
-sample_time
-    How many seconds before the buffer is full?
-
-It is also possible to resize buffers in the RPvds circuit if a size_tag is
-present.  The above attributes reflect the current size of the buffer, which may
-be smaller than the maximum possible size allocated.
-
-n_slots_max
-    Maximum size in number of 32-bit words
-n_samples_max
-    Maximum size in number of samples
-size_max
-    Maximum size in number of channels
-
-Acquiring segments of data
---------------------------
-
-Two utility methods, `DSPBuffer.acquire` and `DSPBuffer.acquire_samples` are
-provided to facilitate the common task of acquiring a segment of data in
-response to some stimulus.  They both fire a trigger then continuously download
-data from the buffer until a certain end condition is met.  This end condition
-can either be the number of samples acquired or the value of a tag in th RPvds
-circuit.
-
-The `DSPBuffer.acquire` method takes three arguments: 
-
-* The trigger to fire, initiating data acquisition.  If None, no trigger is
-  fired and acquire begins spooling data immediately.
-* The tag on the DSP to monitor.  
-* The value of the monitor tag that indicates data acquisition is done.  If not
-  provided, the initial value of the tag will be retrieved before firing the
-  trigger.  In this situation, the end condition is met when the value of the
-  tag changes from its initial value.
-
-Fire trigger 1 and continuously acquire data until ``running`` tag is False::
-
-    microphone_buffer.acquire(1, 'recording', False)
-
-Fire trigger 1 and continuously acquire data until ``complete`` tag is True::
-
-    microphone_buffer.acquire(1, 'complete', True)
-
-Get the initial value of ``toggle``, fire trigger 1, then continuously acquire
-data until the value of ``toggle`` changes::
-
-    microphone_buffer.acquire(1, 'toggle')
-
-Continuously acquire until the value of the trial end timestamp, ``trial_end|``
-changes::
-
-    microphone_buffer.acquire(1, 'trial_end|')
-
-Fire trigger 1 and continuously acquire data until ``index`` tag is greater or
-equal to 10000::
-
-    microphone_buffer.acquire(1, 'index', lambda x: x >= 1000)
-
-Fire trigger 2 and acquire 100000 samples of data::
-
-    microphone_buffer.acquire_samples(2, 100000)
-
-.. note::
-
-    The acquire method continuously downloads data while monitoring the end
-    condition.  This allows you to acquire sets of data larger than the buffer
-    size without losing any data.  Just be sure that the poll interval is
-    short enough to grab new data before it gets overwritten.  To determine how
-    quickly your buffer will fill, check its `sample_time` attribute.
-
-.. note::
-
-    A very common mistake to make is setting the block size for the buffer to a
-    number that is not an integer divisor of the number of samples to be
-    acquired.  If you are acquiring 10000 samples of data and set the block size
-    to 1048, then both `DSPBuffer.acquire` and `DSPBuffer.acquire_samples` will
-    hang after acquiring 9432 samples since they are waiting for another 1048
-    samples to be acquired, but only 568 new samples are in the buffer.  If you
-    don't know in advance what the final length of the data will be, just leave
-    the block size at its default value of 1.
-
-    To prevent this from happening, a ValueError will be raised if you attempt
-    to acquire a number of samples that is not a multiple of block size.
+:class:`tdt.DSPBuffer` -- Wrapper for RPvds buffer objects
+==========================================================
+
+Each buffer requires tags linked to the data and index parameters of the buffer
+component.  All other tags described below are optional, but will be used if
+present.  The data tag and supporting tags can have any name; however, the
+recommended approach is to use the data tag plus one of the following prefixes
+indicating the purpose of the supporting tag.
+
+    i
+        index tag (idx_tag)
+    n
+        size tag (size_tag)
+    sf
+        scaling factor tag (sf_tag)
+    c
+        cycle tag (cycle_tag)
+    d
+        downsampling tag (dec_tag)
+
+If no value is provided for a tag, the default extension is added to the value
+for the data_tag and the circuit is checked to see if the tag exists.  For
+example, if you have `spikes`, `spikes_i`, and `spikes_n` tags in your RPvds
+circuit, you can simply initialize the class by passing only the name of the
+data tag (`spikes`) and it will automatically use `spikes_i` and `spikes_n` as
+the index and size tags, respectively::
+
+   >>> buffer = circuit.get_buffer('spikes', 'r')
+
+If a required tag cannot be found (either by explicitly defining the tag name or
+automatically by adding the default extension to the data tag name), an error is
+raised.
+
+.. image:: example_buffer.*
+
+In the above code, there is a singlue buffer named `contact` with three
+supporting tags (`contact_d`, `contact_sf` and `contact_i`) that assist the
+:mod:`tdt.DSPBuffer` class in reading data stored in `contact`.  For example, we
+know that, due to the fact that we are applying a scaling factor of 127 to the
+floating-point data stored in the contact buffer, we are only saving the data
+with a resolution of 0.00787::
+
+    >>> contact_buffer = circuit.get_buffer('contact', 'r', src_type='int8')
+    >>> print contact_buffer.resolution
+    0.00787
+
+Because we specified that the data is stored in 8-bit format, four samples are
+being compressed into a single 32-bit slot::
+
+    >>> print contact_buffer.compression
+    4
+
+Since `contact_d` is set to 80 (i.e. acquire and save a sample every 80 cycles),
+we know the sampling frequency of the contact data is only 1/80th of the
+sampling rate of the DSP::
+
+    >>> print circuit.fs
+    97656.25
+    >>> print contact_buffer.fs
+    1220.703125
+
+.. note::
+
+    This buffer uses the enable and reset hops to control data acquisition,
+    consistent with the coding guidelines described in dsp_buffer.rst.
+
+.. note::
+
+    Currently TDTPy does not support changing sampling rate on-the-fly (you can
+    do it, but you need to reload the buffer).
+
+Writing single channel data
+---------------------------
+
+If you are using epoch-based outputs (where you upload a waveform of fixed size
+and halt playout once the buffer is complete), then you can use the
+`WriteableDSPBuffer.set` method::
+
+   >>> speaker_buffer = circuit.get_buffer('speaker', 'w')
+   >>> speaker_buffer.set(tone_pip)
+
+If you are using continuous output (e.g., where you need to update the stream
+as the experiment progresses)::
+
+TODO
+
+TDTPy has not been tested with writing multi-channel data (mainly because we
+currently do not have a use-case for it). 
+
+Reading single and multichannel data
+------------------------------------
+TODO
+
+Tags
+----
+data_tag : string (required)
+    Tag to read data from
+idx_tag : defaults to data_tag_i (required)
+    Tag indicating current index of buffer.  For buffer reads this tag
+    serves as a "handshake" (i.e. when the index changes, new data is
+    available).
+size_tag : defaults to data_tag_n (optional)
+    Tag indicating current size of buffer.
+sf_tag : defaults to data_tag_sf (optional)
+    Tag indicating scaling factor applied to data before it is stored in the
+    buffer.
+cycle_tag : defaults to data_tag_c (optional)
+    Tag indicating number of times buffer has wrapped around to beginning.
+    Used to ensure no data is lost.
+dec_tag : defaults to data_tag_d (optional)
+    Tag indicating decimation factor.  Used to compute sampling frequency of
+    data stored in buffer: e.g. if circuit runs at 100 kHz, but you only
+    sample every 25 cycles, the actual sampling frequency is 4 kHz.  
+    
+Additional Parameters
+----------------------
+circuit : instance of `tdt.DSPCircuit`
+    Circuit object the buffer is attached to
+block_size : int
+    Coerce data read/write to multiple of the block size.  Must be a
+    multiple of the channel number.
+src_type : str or numpy dtype
+    Type of data in buffer (can be a string or numpy dtype).  Valid data
+    formats are float32, int32, int16 and int8.
+dest_type : str or numpy dtype
+    Type to convert data to
+channels : int
+    Number of channels stored in buffer
+
+Available attributes
+--------------------
+
+When the buffer is first loaded, there is some "introspection" of the circuit to
+determine key properties of the buffer (e.g. what is the format of the data
+stored in the DSP buffer, how much data can be stored before the buffer fills
+up, etc.).
+
+data_tag, idx_tag, size_tag, sf_tag, cycle_tag, dec_tag : str
+    Names of supporting tags present in the circuit (both the names provided
+    when the b uffer was loaded as well as the ones automatically discovered
+    when the buffer is created.  None if the tag is not present.
+src_type 
+    Numpy dtype of the data stored on the device.  Defaults to float32.
+dest_type
+    Numpy dtype of array returned when data is read from the device
+compression
+    Number of samples stored in a single 32-bit "slot" on the device.  For
+    example, if you are using the MCFloat2Int8 component to convert four samples
+    of data into 8-bit integers and storing these four samples as a single
+    32-bit work, the compression factor is 4.
+sf
+    Scaling factor of the data.  If you are not using compression, the scaling
+    factor is almost certainly one.
+resolution
+    If data is being compressed, computes the actual resolution of the
+    acquired data given the scaling factor.  For example, if you are
+    compressing data into an 8-bit integer using a scaling factor of 10,
+    then the resolution of the acquired data will be 0.1 since numbers will
+    get rounded to the nearest tenth (e.g. 0.183 will get rounded to 0.2).
+dec_factor
+    Also called the "downsampling rate".  Indicates the number of device
+    cycles before a sample is stored in the buffer.  If 1 (default), a sample is
+    acquired on every cycle.  If 2, a sample is acquired on every other cycle.
+fs
+    Sampling frequency of data stored in buffer.  This is basically the
+    sampling frequency of the device divided by the decimation factor
+    (dec_factor): e.g. if a sample is acquired only on every other cycle,
+    then the sampling frequency of the buffer is effectively half of the
+    device clock rate.
+channels
+    Number of channels
+block_size
+    Coerce read size to multiples of this value (can be overridden if needed)
+
+Buffer size attributes
+----------------------
+
+There are three ways to think about the buffer size.  First, how many 32-bit
+words can the buffer hold?  All buffer components in a RPvds circuit store data
+in 32-bit word segments.  However, we can store two 16-bit values or four 8-bit
+values into a single word.  Even if a buffer can only hold 1000 32-bit words, it
+may actually hold 2000 or 4000 samples if we are compressing two or four samples
+of data into a single buffer "slot".  Now, if we are storing multiple channels
+of data in a single buffer, then the buffer will fill up more quickly than an
+identically-sized buffer storing only a single channel of data.  By reporting
+buffer size as the number of samples per channel, we can get a sense for how
+quickly the buffer will fill up.
+
+>>> buffer = circuit.get_buffer('spikes', 'r', channels=16)
+>>> print buffer.compression    # number of samples in each buffer slot
+2
+>>> print buffer.n_slots        # number of slots
+4000
+>>> print buffer.n_samples      # number of samples
+8000
+>>> print buffer.size           # number of samples per channel
+500
+>>> print buffer.fs             # sampling frequency of buffer data
+12207.03125
+>>> print buffer.sample_time    # time (in seconds) to fill up the buffer
+0.04096
+
+In the above example, we know that even though the buffer can hold 8,000
+samples of data, it will fill up after only 500 samples of 16-channel data are
+collected.  At a sampling frequency of 12 kHz, this means the buffer can only
+hold 41 msec of 16-channel data.  This provides a useful metric for knowing
+whether we have set the buffer size appropriately.
+
+n_slots
+    Size in number of 32-bit words (the buffer's atomic unit of of storage)
+n_samples
+    Size in number of samples (data points) that can be stored in the buffer.
+    The size will be either 1x, 2x or 4x the size of n_slots depending on how
+    many samples are stored in each slot.
+size
+    Size in number of samples (data points) per channel.
+sample_time
+    How many seconds before the buffer is full?
+
+It is also possible to resize buffers in the RPvds circuit if a size_tag is
+present.  The above attributes reflect the current size of the buffer, which may
+be smaller than the maximum possible size allocated.
+
+n_slots_max
+    Maximum size in number of 32-bit words
+n_samples_max
+    Maximum size in number of samples
+size_max
+    Maximum size in number of channels
+
+Acquiring segments of data
+--------------------------
+
+Two utility methods, `DSPBuffer.acquire` and `DSPBuffer.acquire_samples` are
+provided to facilitate the common task of acquiring a segment of data in
+response to some stimulus.  They both fire a trigger then continuously download
+data from the buffer until a certain end condition is met.  This end condition
+can either be the number of samples acquired or the value of a tag in th RPvds
+circuit.
+
+The `DSPBuffer.acquire` method takes three arguments: 
+
+* The trigger to fire, initiating data acquisition.  If None, no trigger is
+  fired and acquire begins spooling data immediately.
+* The tag on the DSP to monitor.  
+* The value of the monitor tag that indicates data acquisition is done.  If not
+  provided, the initial value of the tag will be retrieved before firing the
+  trigger.  In this situation, the end condition is met when the value of the
+  tag changes from its initial value.
+
+Fire trigger 1 and continuously acquire data until ``running`` tag is False::
+
+    microphone_buffer.acquire(1, 'recording', False)
+
+Fire trigger 1 and continuously acquire data until ``complete`` tag is True::
+
+    microphone_buffer.acquire(1, 'complete', True)
+
+Get the initial value of ``toggle``, fire trigger 1, then continuously acquire
+data until the value of ``toggle`` changes::
+
+    microphone_buffer.acquire(1, 'toggle')
+
+Continuously acquire until the value of the trial end timestamp, ``trial_end|``
+changes::
+
+    microphone_buffer.acquire(1, 'trial_end|')
+
+Fire trigger 1 and continuously acquire data until ``index`` tag is greater or
+equal to 10000::
+
+    microphone_buffer.acquire(1, 'index', lambda x: x >= 1000)
+
+Fire trigger 2 and acquire 100000 samples of data::
+
+    microphone_buffer.acquire_samples(2, 100000)
+
+.. note::
+
+    The acquire method continuously downloads data while monitoring the end
+    condition.  This allows you to acquire sets of data larger than the buffer
+    size without losing any data.  Just be sure that the poll interval is
+    short enough to grab new data before it gets overwritten.  To determine how
+    quickly your buffer will fill, check its `sample_time` attribute.
+
+.. note::
+
+    A very common mistake to make is setting the block size for the buffer to a
+    number that is not an integer divisor of the number of samples to be
+    acquired.  If you are acquiring 10000 samples of data and set the block size
+    to 1048, then both `DSPBuffer.acquire` and `DSPBuffer.acquire_samples` will
+    hang after acquiring 9432 samples since they are waiting for another 1048
+    samples to be acquired, but only 568 new samples are in the buffer.  If you
+    don't know in advance what the final length of the data will be, just leave
+    the block size at its default value of 1.
+
+    To prevent this from happening, a ValueError will be raised if you attempt
+    to acquire a number of samples that is not a multiple of block size.
```

### Comparing `TDTPy-0.8.1/docs/_build/html/_sources/dsp_circuit.rst.txt` & `TDTPy-0.9.0/docs/dsp_circuit.rst`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/docs/_build/html/_sources/getting_started.rst.txt` & `TDTPy-0.9.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/docs/_build/html/_sources/index.rst.txt` & `TDTPy-0.9.0/docs/index.rst`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-TDTPy Documentation
-===================
-
-Python interface for TDT equipment
-----------------------------------
-
-**Contributors**
-
-* Brad Buran (New York University; Oregon Health & Science University)
-* Eric Larson (University of Washington)
-* Decibel Therapeutics, Inc.
-
-**Acknowledgements**
-
-Work on TDTPy was supported by grant DC009237 from the `National Institute on
-Deafness and other Communication Disorders`_.
-
-.. _National Institute on Deafness and other Communication Disorders: http://www.nidcd.nih.gov
-
-.. module:: tdt
-    :platform: Windows (requires proprietary ActiveX driver from TDT)
-.. moduleauthor:: Brad Buran <bburan@alum.mit.edu>
-
-.. note::
-
-    If you use the server provided by TDTPy to communicate with your hardware
-    your client code should be able to run on any platform including Unix, Linux
-    and OSX).  The server, however, requires the proprietary ActiveX drivers
-    provided by TDT which only run on Windows.
-
-Contents
---------
-
-.. toctree::
-    :maxdepth: 2
-
-    getting_started.rst
-    code_examples.rst
-    converting.rst
-    dsp_circuit.rst
-    dsp_buffer.rst
-    api.rst
-    server_api.rst
-
-.. include:: ../readme.rst
-
-Furthermore, TDTPy was as written as part of an initial progress towards a
-hardware abstraction layer.  Your experiment code should not care whether you're
-using Tucker Davis' `System 3`_ hardware, `National Instruments DAQ platform`_,
-a high-quality audio card, or some combination of different vendors' hardware.
-A key goal of TDTPy is to begin progress towards an application programming
-interface (API) that can be implemented by Python wrappers around other hardware
-vendors' libraries.  By building experiment code on top of TDTPy (rather than
-directly on top of TDT's ActiveX library), switching to another hardware
-platform should only require the following steps:
-
-* Identifying (or writing) a wrapper around the vendor's library that supports
-  the public API that TDTPy also supports.
-* Writing the underlying microcode (e.g. a LabVIEW VI if you are switching
-  to National Instruments' PXI) for the new hardware required to run the
-  experiment.
-* Changing your code to import from your new wrapper rather than TDTPy.
-
-We have already built two programs, Neurogen_ and NeuroBehavior_, on top of
-TDTPy with an eye towards ensuring that we can switch to a different hardware
-platform if needed.
-
-Key differences between TDTPy and OpenEx
-========================================
-
-Some people may note a number of similarities between the goals of the TDTPy and
-TDT's OpenEx platform.  Both platforms are designed to streamline the process of
-setting up and running experiments by providing high-level functionality.
-
-* TDTPy is open-source.  OpenEx (despite the name) is not.
-* Both OpenEx and TDTPy facilitate handling of buffer reads and writes provided
-  you follow certain conventions in setting up your RPvds circuit.  OpenEx
-  requires strict conventions (e.g. you must give your tag a four-letter name
-  with a special prefix).  TDTPy allows you to use whatever names you like.
-* Both TDTPy and OpenEx support running the hardware communication in a
-  subprocess.  However, OpenEx does not make the data immediately available.  At
-  best, there is a 10 second lag from the time the data is downloaded from the
-  hardware to the time it is availabile to your script for plotting and
-  analysis.  TDTPy makes the downloaded data available immediately.
-* OpenEx integrates with other components produced by TDT (OpenController,
-  OpenDeveloper, OpenWorkbench, etc.).  TDTPy currently does not offer the
-  functionality provided by these other components.
-* OpenEx requires the use of TDT's proprietary data format (TTank).  In addition
-  to being a proprietary, binary format, TTank imposes certain constraints on
-  how you can save your data to disk.  In contrast, TDTPy allows you to handle
-  saving the data (i.e. you can dump it to a HDF5, XML, ASCII, CSV or MAT
-  container).
-* Integrating OpenEx with your custom scripts is somewhat of a hack.  You must
-  launch OpenEx then launch your script.  TDTPy is part of your script.
-* TDTPy comes with robust error-checking that catches many common coding
-  mistakes (e.g. attempting to access a non-existent tag on the device) and a
-  test-suite you can use to ensure your hardware is performing to spec.
-
-Roadmap
-=======
-
-* In the write-test-debug routine of developing RPvds circuits, it would be very
-  useful to have a GUI that allows you to interactively monitor and manipulate
-  tag values well as visualize and manipulate data in the RPvds buffers.  We can
-  leverage Enthought's powerful Traits_, TraitsGUI_ and Chaco_ packages for this
-  purpose.
-* Support processing pipelines for uploaded and downloaded data.  This would be
-  especially useful when running TDTPy as a subprocess to offload much of the
-  processing overhead to a second CPU.
-* Support streaming data from RPvds buffers to disk so the main process does not
-  have to handle this step as well (requires a IO library that is thread/process
-  safe).
-
-.. _National Instruments DAQ platform: http://www.ni.com/dataacquisition/multifunction/
-.. _Neurogen: http://bradburan.com/programs-and-scripts/neurogen/
-.. _NeuroBehavior: http://bradburan.com/programs-and-scripts/neurobehavior/
-.. _Chaco: http://code.enthought.com/projects/chaco/ 
-.. _Traits: http://code.enthought.com/projects/traits/ 
-.. _TraitsGUI: http://code.enthought.com/projects/traits_gui/ 
-
-
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+TDTPy Documentation
+===================
+
+Python interface for TDT equipment
+----------------------------------
+
+**Contributors**
+
+* Brad Buran (New York University; Oregon Health & Science University)
+* Eric Larson (University of Washington)
+* Decibel Therapeutics, Inc.
+
+**Acknowledgements**
+
+Work on TDTPy was supported by grant DC009237 from the `National Institute on
+Deafness and other Communication Disorders`_.
+
+.. _National Institute on Deafness and other Communication Disorders: http://www.nidcd.nih.gov
+
+.. module:: tdt
+    :platform: Windows (requires proprietary ActiveX driver from TDT)
+.. moduleauthor:: Brad Buran <bburan@alum.mit.edu>
+
+.. note::
+
+    If you use the server provided by TDTPy to communicate with your hardware
+    your client code should be able to run on any platform including Unix, Linux
+    and OSX).  The server, however, requires the proprietary ActiveX drivers
+    provided by TDT which only run on Windows.
+
+Contents
+--------
+
+.. toctree::
+    :maxdepth: 2
+
+    getting_started.rst
+    code_examples.rst
+    converting.rst
+    dsp_circuit.rst
+    dsp_buffer.rst
+    api.rst
+    server_api.rst
+
+.. include:: ../readme.rst
+
+Furthermore, TDTPy was as written as part of an initial progress towards a
+hardware abstraction layer.  Your experiment code should not care whether you're
+using Tucker Davis' `System 3`_ hardware, `National Instruments DAQ platform`_,
+a high-quality audio card, or some combination of different vendors' hardware.
+A key goal of TDTPy is to begin progress towards an application programming
+interface (API) that can be implemented by Python wrappers around other hardware
+vendors' libraries.  By building experiment code on top of TDTPy (rather than
+directly on top of TDT's ActiveX library), switching to another hardware
+platform should only require the following steps:
+
+* Identifying (or writing) a wrapper around the vendor's library that supports
+  the public API that TDTPy also supports.
+* Writing the underlying microcode (e.g. a LabVIEW VI if you are switching
+  to National Instruments' PXI) for the new hardware required to run the
+  experiment.
+* Changing your code to import from your new wrapper rather than TDTPy.
+
+We have already built two programs, Neurogen_ and NeuroBehavior_, on top of
+TDTPy with an eye towards ensuring that we can switch to a different hardware
+platform if needed.
+
+Key differences between TDTPy and OpenEx
+========================================
+
+Some people may note a number of similarities between the goals of the TDTPy and
+TDT's OpenEx platform.  Both platforms are designed to streamline the process of
+setting up and running experiments by providing high-level functionality.
+
+* TDTPy is open-source.  OpenEx (despite the name) is not.
+* Both OpenEx and TDTPy facilitate handling of buffer reads and writes provided
+  you follow certain conventions in setting up your RPvds circuit.  OpenEx
+  requires strict conventions (e.g. you must give your tag a four-letter name
+  with a special prefix).  TDTPy allows you to use whatever names you like.
+* Both TDTPy and OpenEx support running the hardware communication in a
+  subprocess.  However, OpenEx does not make the data immediately available.  At
+  best, there is a 10 second lag from the time the data is downloaded from the
+  hardware to the time it is availabile to your script for plotting and
+  analysis.  TDTPy makes the downloaded data available immediately.
+* OpenEx integrates with other components produced by TDT (OpenController,
+  OpenDeveloper, OpenWorkbench, etc.).  TDTPy currently does not offer the
+  functionality provided by these other components.
+* OpenEx requires the use of TDT's proprietary data format (TTank).  In addition
+  to being a proprietary, binary format, TTank imposes certain constraints on
+  how you can save your data to disk.  In contrast, TDTPy allows you to handle
+  saving the data (i.e. you can dump it to a HDF5, XML, ASCII, CSV or MAT
+  container).
+* Integrating OpenEx with your custom scripts is somewhat of a hack.  You must
+  launch OpenEx then launch your script.  TDTPy is part of your script.
+* TDTPy comes with robust error-checking that catches many common coding
+  mistakes (e.g. attempting to access a non-existent tag on the device) and a
+  test-suite you can use to ensure your hardware is performing to spec.
+
+Roadmap
+=======
+
+* In the write-test-debug routine of developing RPvds circuits, it would be very
+  useful to have a GUI that allows you to interactively monitor and manipulate
+  tag values well as visualize and manipulate data in the RPvds buffers.  We can
+  leverage Enthought's powerful Traits_, TraitsGUI_ and Chaco_ packages for this
+  purpose.
+* Support processing pipelines for uploaded and downloaded data.  This would be
+  especially useful when running TDTPy as a subprocess to offload much of the
+  processing overhead to a second CPU.
+* Support streaming data from RPvds buffers to disk so the main process does not
+  have to handle this step as well (requires a IO library that is thread/process
+  safe).
+
+.. _National Instruments DAQ platform: http://www.ni.com/dataacquisition/multifunction/
+.. _Neurogen: http://bradburan.com/programs-and-scripts/neurogen/
+.. _NeuroBehavior: http://bradburan.com/programs-and-scripts/neurobehavior/
+.. _Chaco: http://code.enthought.com/projects/chaco/ 
+.. _Traits: http://code.enthought.com/projects/traits/ 
+.. _TraitsGUI: http://code.enthought.com/projects/traits_gui/ 
+
+
+Indices and tables
+==================
+
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
```

### Comparing `TDTPy-0.8.1/docs/_build/html/_sources/server_api.rst.txt` & `TDTPy-0.9.0/docs/server_api.rst`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/setup.py` & `TDTPy-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,18 @@
               'tdt.actxobjects',
               'tdt.components',
               'tdt.device'],
     url='http://tdtpy.readthedocs.org',
     license='BSD (3-clause)',
     description='Module for communicating with TDT\'s System 3 hardware',
     long_description=long_description,
-    install_requires=['six', 'pypiwin32', 'numpy'],
+    install_requires=['pypiwin32', 'numpy'],
+    extras_require={
+        'test': ['pytest'],
+    },
     package_data={'tdt': ['components/*.rcx']},
     classifiers=CLASSIFIERS,
     command_options={
         'build_sphinx': {
             'project': ('setup.py', name),
             'version': ('setup.py', version),
             'release': ('setup.py', version),
```

### Comparing `TDTPy-0.8.1/tdt/abstract_ring_buffer.py` & `TDTPy-0.9.0/tdt/abstract_ring_buffer.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/actxobjects/PA5x.py` & `TDTPy-0.9.0/tdt/actxobjects/PA5x.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/actxobjects/RPcoX.py` & `TDTPy-0.9.0/tdt/actxobjects/RPcoX.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/actxobjects/TDevAccX.py` & `TDTPy-0.9.0/tdt/actxobjects/TDevAccX.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,213 +1,213 @@
-# -*- coding: utf-8 -*-
-# Created by makepy.py version 0.5.00
-# By python version 2.6.6 |EPD 6.3-1 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
-# From type library 'TDevAccX.ocx'
-# On Mon Nov 22 10:28:02 2010
-"""TDevAccX ActiveX Control module"""
-makepy_version = '0.5.00'
-python_version = 0x20606f0
-
-import win32com.client.CLSIDToClass, pythoncom, pywintypes
-import win32com.client.util
-from pywintypes import IID
-from win32com.client import Dispatch
-
-# The following 3 lines may need tweaking for the particular server
-# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
-defaultNamedOptArg=pythoncom.Empty
-defaultNamedNotOptArg=pythoncom.Empty
-defaultUnnamedArg=pythoncom.Empty
-
-CLSID = IID('{735FF2F5-CC9A-4D67-BFC1-FD5FA6742027}')
-MajorVersion = 1
-MinorVersion = 0
-LibraryFlags = 10
-LCID = 0x0
-
-from win32com.client import DispatchBaseClass
-class _DTDevAccX(DispatchBaseClass):
-	"""Dispatch interface for TDevAccX Control"""
-	CLSID = IID('{F04FC131-D33B-45B7-BC22-CF58B06CA5CB}')
-	coclass_clsid = IID('{09EFA19D-3AD0-49A8-8232-18D6F7512CE8}')
-
-	def AboutBox(self):
-		return self._oleobj_.InvokeTypes(-552, LCID, 1, (24, 0), (),)
-
-	def CheckServerConnection(self):
-		return self._oleobj_.InvokeTypes(2, LCID, 1, (3, 0), (),)
-
-	def CloseConnection(self):
-		return self._oleobj_.InvokeTypes(3, LCID, 1, (24, 0), (),)
-
-	def ConnectServer(self, ServerName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(1, LCID, 1, (3, 0), ((8, 0),),ServerName
-			)
-
-	def GetDeviceName(self, Index=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(17, LCID, 1, (8, 0), ((3, 0),),Index
-			)
-
-	def GetDeviceRCO(self, DeviceName=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(19, LCID, 1, (8, 0), ((8, 0),),DeviceName
-			)
-
-	def GetDeviceSF(self, Target=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(10, LCID, 1, (4, 0), ((8, 0),),Target
-			)
-
-	def GetDeviceStatus(self, Target=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(14, LCID, 1, (3, 0), ((8, 0),),Target
-			)
-
-	def GetDeviceType(self, DeviceName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(18, LCID, 1, (3, 0), ((8, 0),),DeviceName
-			)
-
-	def GetNextTag(self, DeviceName=defaultNamedNotOptArg, ReqType=defaultNamedNotOptArg, DoFirst=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(20, LCID, 1, (8, 0), ((8, 0), (3, 0), (3, 0)),DeviceName
-			, ReqType, DoFirst)
-
-	def GetSysMode(self):
-		return self._oleobj_.InvokeTypes(16, LCID, 1, (3, 0), (),)
-
-	def GetTankName(self):
-		"""method GetTankName"""
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(23, LCID, 1, (8, 0), (),)
-
-	def GetTargetClass(self, Target=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(8, LCID, 1, (3, 0), ((8, 0),),Target
-			)
-
-	def GetTargetSize(self, Target=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(11, LCID, 1, (3, 0), ((8, 0),),Target
-			)
-
-	def GetTargetType(self, Target=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(15, LCID, 1, (3, 0), ((8, 0),),Target
-			)
-
-	def GetTargetVal(self, Target=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(12, LCID, 1, (5, 0), ((8, 0),),Target
-			)
-
-	def ReadTarget(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, nWords=defaultNamedNotOptArg, pData=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(6, LCID, 1, (3, 0), ((8, 0), (3, 0), (3, 0), (16388, 0)),Target
-			, nOS, nWords, pData)
-
-	def ReadTargetV(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, nWords=defaultNamedNotOptArg):
-		return self._ApplyTypes_(7, 1, (12, 0), ((8, 0), (3, 0), (3, 0)), u'ReadTargetV', None,Target
-			, nOS, nWords)
-
-	def ReadTargetVEX(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, nWords=defaultNamedNotOptArg, SrcType=defaultNamedNotOptArg
-			, DstType=defaultNamedNotOptArg):
-		return self._ApplyTypes_(24, 1, (12, 0), ((8, 0), (3, 0), (3, 0), (8, 0), (8, 0)), u'ReadTargetVEX', None,Target
-			, nOS, nWords, SrcType, DstType)
-
-	def SetSysMode(self, NewMode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(21, LCID, 1, (3, 0), ((3, 0),),NewMode
-			)
-
-	def SetTankName(self, TankName=defaultNamedNotOptArg):
-		"""method SetTankName"""
-		return self._oleobj_.InvokeTypes(22, LCID, 1, (3, 0), ((8, 0),),TankName
-			)
-
-	def SetTargetVal(self, Target=defaultNamedNotOptArg, Val=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(13, LCID, 1, (3, 0), ((8, 0), (5, 0)),Target
-			, Val)
-
-	def WriteTarget(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, nWords=defaultNamedNotOptArg, pData=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(4, LCID, 1, (3, 0), ((8, 0), (3, 0), (3, 0), (16388, 0)),Target
-			, nOS, nWords, pData)
-
-	def WriteTargetV(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, vData=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(5, LCID, 1, (3, 0), ((8, 0), (3, 0), (12, 0)),Target
-			, nOS, vData)
-
-	def WriteTargetVEX(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, DstType=defaultNamedNotOptArg, Buf=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(25, LCID, 1, (3, 0), ((8, 0), (3, 0), (8, 0), (12, 0)),Target
-			, nOS, DstType, Buf)
-
-	def ZeroTarget(self, Target=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(9, LCID, 1, (24, 0), ((8, 0),),Target
-			)
-
-	_prop_map_get_ = {
-	}
-	_prop_map_put_ = {
-	}
-
-class _DTDevAccXEvents:
-	"""Event interface for TDevAccX Control"""
-	CLSID = CLSID_Sink = IID('{64E8C018-79F7-4C72-9244-6CAE7315BA4F}')
-	coclass_clsid = IID('{09EFA19D-3AD0-49A8-8232-18D6F7512CE8}')
-	_public_methods_ = [] # For COM Server support
-	_dispid_to_func_ = {
-		}
-
-	def __init__(self, oobj = None):
-		if oobj is None:
-			self._olecp = None
-		else:
-			import win32com.server.util
-			from win32com.server.policy import EventHandlerPolicy
-			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
-			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
-			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
-			self._olecp,self._olecp_cookie = cp,cookie
-	def __del__(self):
-		try:
-			self.close()
-		except pythoncom.com_error:
-			pass
-	def close(self):
-		if self._olecp is not None:
-			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
-			cp.Unadvise(cookie)
-	def _query_interface_(self, iid):
-		import win32com.server.util
-		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
-
-	# Event Handlers
-	# If you create handlers, they should have the following prototypes:
-
-
-from win32com.client import CoClassBaseClass
-# This CoClass is known by the name 'TDevAcc.X'
-class TDevAccX(CoClassBaseClass): # A CoClass
-	# TDevAccX Control
-	CLSID = IID('{09EFA19D-3AD0-49A8-8232-18D6F7512CE8}')
-	coclass_sources = [
-		_DTDevAccXEvents,
-	]
-	default_source = _DTDevAccXEvents
-	coclass_interfaces = [
-		_DTDevAccX,
-	]
-	default_interface = _DTDevAccX
-
-RecordMap = {
-}
-
-CLSIDToClassMap = {
-	'{F04FC131-D33B-45B7-BC22-CF58B06CA5CB}' : _DTDevAccX,
-	'{64E8C018-79F7-4C72-9244-6CAE7315BA4F}' : _DTDevAccXEvents,
-	'{09EFA19D-3AD0-49A8-8232-18D6F7512CE8}' : TDevAccX,
-}
-CLSIDToPackageMap = {}
-win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
-VTablesToPackageMap = {}
-VTablesToClassMap = {
-}
-
-
-NamesToIIDMap = {
-	'_DTDevAccXEvents' : '{64E8C018-79F7-4C72-9244-6CAE7315BA4F}',
-	'_DTDevAccX' : '{F04FC131-D33B-45B7-BC22-CF58B06CA5CB}',
-}
-
-
+# -*- coding: utf-8 -*-
+# Created by makepy.py version 0.5.00
+# By python version 2.6.6 |EPD 6.3-1 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
+# From type library 'TDevAccX.ocx'
+# On Mon Nov 22 10:28:02 2010
+"""TDevAccX ActiveX Control module"""
+makepy_version = '0.5.00'
+python_version = 0x20606f0
+
+import win32com.client.CLSIDToClass, pythoncom, pywintypes
+import win32com.client.util
+from pywintypes import IID
+from win32com.client import Dispatch
+
+# The following 3 lines may need tweaking for the particular server
+# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
+defaultNamedOptArg=pythoncom.Empty
+defaultNamedNotOptArg=pythoncom.Empty
+defaultUnnamedArg=pythoncom.Empty
+
+CLSID = IID('{735FF2F5-CC9A-4D67-BFC1-FD5FA6742027}')
+MajorVersion = 1
+MinorVersion = 0
+LibraryFlags = 10
+LCID = 0x0
+
+from win32com.client import DispatchBaseClass
+class _DTDevAccX(DispatchBaseClass):
+	"""Dispatch interface for TDevAccX Control"""
+	CLSID = IID('{F04FC131-D33B-45B7-BC22-CF58B06CA5CB}')
+	coclass_clsid = IID('{09EFA19D-3AD0-49A8-8232-18D6F7512CE8}')
+
+	def AboutBox(self):
+		return self._oleobj_.InvokeTypes(-552, LCID, 1, (24, 0), (),)
+
+	def CheckServerConnection(self):
+		return self._oleobj_.InvokeTypes(2, LCID, 1, (3, 0), (),)
+
+	def CloseConnection(self):
+		return self._oleobj_.InvokeTypes(3, LCID, 1, (24, 0), (),)
+
+	def ConnectServer(self, ServerName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(1, LCID, 1, (3, 0), ((8, 0),),ServerName
+			)
+
+	def GetDeviceName(self, Index=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(17, LCID, 1, (8, 0), ((3, 0),),Index
+			)
+
+	def GetDeviceRCO(self, DeviceName=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(19, LCID, 1, (8, 0), ((8, 0),),DeviceName
+			)
+
+	def GetDeviceSF(self, Target=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(10, LCID, 1, (4, 0), ((8, 0),),Target
+			)
+
+	def GetDeviceStatus(self, Target=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(14, LCID, 1, (3, 0), ((8, 0),),Target
+			)
+
+	def GetDeviceType(self, DeviceName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(18, LCID, 1, (3, 0), ((8, 0),),DeviceName
+			)
+
+	def GetNextTag(self, DeviceName=defaultNamedNotOptArg, ReqType=defaultNamedNotOptArg, DoFirst=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(20, LCID, 1, (8, 0), ((8, 0), (3, 0), (3, 0)),DeviceName
+			, ReqType, DoFirst)
+
+	def GetSysMode(self):
+		return self._oleobj_.InvokeTypes(16, LCID, 1, (3, 0), (),)
+
+	def GetTankName(self):
+		"""method GetTankName"""
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(23, LCID, 1, (8, 0), (),)
+
+	def GetTargetClass(self, Target=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(8, LCID, 1, (3, 0), ((8, 0),),Target
+			)
+
+	def GetTargetSize(self, Target=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(11, LCID, 1, (3, 0), ((8, 0),),Target
+			)
+
+	def GetTargetType(self, Target=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(15, LCID, 1, (3, 0), ((8, 0),),Target
+			)
+
+	def GetTargetVal(self, Target=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(12, LCID, 1, (5, 0), ((8, 0),),Target
+			)
+
+	def ReadTarget(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, nWords=defaultNamedNotOptArg, pData=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(6, LCID, 1, (3, 0), ((8, 0), (3, 0), (3, 0), (16388, 0)),Target
+			, nOS, nWords, pData)
+
+	def ReadTargetV(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, nWords=defaultNamedNotOptArg):
+		return self._ApplyTypes_(7, 1, (12, 0), ((8, 0), (3, 0), (3, 0)), u'ReadTargetV', None,Target
+			, nOS, nWords)
+
+	def ReadTargetVEX(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, nWords=defaultNamedNotOptArg, SrcType=defaultNamedNotOptArg
+			, DstType=defaultNamedNotOptArg):
+		return self._ApplyTypes_(24, 1, (12, 0), ((8, 0), (3, 0), (3, 0), (8, 0), (8, 0)), u'ReadTargetVEX', None,Target
+			, nOS, nWords, SrcType, DstType)
+
+	def SetSysMode(self, NewMode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(21, LCID, 1, (3, 0), ((3, 0),),NewMode
+			)
+
+	def SetTankName(self, TankName=defaultNamedNotOptArg):
+		"""method SetTankName"""
+		return self._oleobj_.InvokeTypes(22, LCID, 1, (3, 0), ((8, 0),),TankName
+			)
+
+	def SetTargetVal(self, Target=defaultNamedNotOptArg, Val=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(13, LCID, 1, (3, 0), ((8, 0), (5, 0)),Target
+			, Val)
+
+	def WriteTarget(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, nWords=defaultNamedNotOptArg, pData=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(4, LCID, 1, (3, 0), ((8, 0), (3, 0), (3, 0), (16388, 0)),Target
+			, nOS, nWords, pData)
+
+	def WriteTargetV(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, vData=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(5, LCID, 1, (3, 0), ((8, 0), (3, 0), (12, 0)),Target
+			, nOS, vData)
+
+	def WriteTargetVEX(self, Target=defaultNamedNotOptArg, nOS=defaultNamedNotOptArg, DstType=defaultNamedNotOptArg, Buf=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(25, LCID, 1, (3, 0), ((8, 0), (3, 0), (8, 0), (12, 0)),Target
+			, nOS, DstType, Buf)
+
+	def ZeroTarget(self, Target=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(9, LCID, 1, (24, 0), ((8, 0),),Target
+			)
+
+	_prop_map_get_ = {
+	}
+	_prop_map_put_ = {
+	}
+
+class _DTDevAccXEvents:
+	"""Event interface for TDevAccX Control"""
+	CLSID = CLSID_Sink = IID('{64E8C018-79F7-4C72-9244-6CAE7315BA4F}')
+	coclass_clsid = IID('{09EFA19D-3AD0-49A8-8232-18D6F7512CE8}')
+	_public_methods_ = [] # For COM Server support
+	_dispid_to_func_ = {
+		}
+
+	def __init__(self, oobj = None):
+		if oobj is None:
+			self._olecp = None
+		else:
+			import win32com.server.util
+			from win32com.server.policy import EventHandlerPolicy
+			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
+			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
+			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
+			self._olecp,self._olecp_cookie = cp,cookie
+	def __del__(self):
+		try:
+			self.close()
+		except pythoncom.com_error:
+			pass
+	def close(self):
+		if self._olecp is not None:
+			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
+			cp.Unadvise(cookie)
+	def _query_interface_(self, iid):
+		import win32com.server.util
+		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
+
+	# Event Handlers
+	# If you create handlers, they should have the following prototypes:
+
+
+from win32com.client import CoClassBaseClass
+# This CoClass is known by the name 'TDevAcc.X'
+class TDevAccX(CoClassBaseClass): # A CoClass
+	# TDevAccX Control
+	CLSID = IID('{09EFA19D-3AD0-49A8-8232-18D6F7512CE8}')
+	coclass_sources = [
+		_DTDevAccXEvents,
+	]
+	default_source = _DTDevAccXEvents
+	coclass_interfaces = [
+		_DTDevAccX,
+	]
+	default_interface = _DTDevAccX
+
+RecordMap = {
+}
+
+CLSIDToClassMap = {
+	'{F04FC131-D33B-45B7-BC22-CF58B06CA5CB}' : _DTDevAccX,
+	'{64E8C018-79F7-4C72-9244-6CAE7315BA4F}' : _DTDevAccXEvents,
+	'{09EFA19D-3AD0-49A8-8232-18D6F7512CE8}' : TDevAccX,
+}
+CLSIDToPackageMap = {}
+win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
+VTablesToPackageMap = {}
+VTablesToClassMap = {
+}
+
+
+NamesToIIDMap = {
+	'_DTDevAccXEvents' : '{64E8C018-79F7-4C72-9244-6CAE7315BA4F}',
+	'_DTDevAccX' : '{F04FC131-D33B-45B7-BC22-CF58B06CA5CB}',
+}
+
+
```

### Comparing `TDTPy-0.8.1/tdt/actxobjects/TTank.py` & `TDTPy-0.9.0/tdt/actxobjects/TTank.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-# -*- coding: utf-8 -*-
-# Created by makepy.py version 0.5.00
-# By python version 2.6.6 |EPD 6.3-1 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
-# From type library 'TTankEng.exe'
-# On Mon Nov 22 10:28:59 2010
-"""TTankEng 1.0 Type Library"""
-makepy_version = '0.5.00'
-python_version = 0x20606f0
-
-import win32com.client.CLSIDToClass, pythoncom, pywintypes
-import win32com.client.util
-from pywintypes import IID
-from win32com.client import Dispatch
-
-# The following 3 lines may need tweaking for the particular server
-# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
-defaultNamedOptArg=pythoncom.Empty
-defaultNamedNotOptArg=pythoncom.Empty
-defaultUnnamedArg=pythoncom.Empty
-
-CLSID = IID('{BBA11881-D2C7-4FDB-873D-A474560D7394}')
-MajorVersion = 1
-MinorVersion = 0
-LibraryFlags = 8
-LCID = 0x0
-
-from win32com.client import CoClassBaseClass
-# This CoClass is known by the name 'TTankEng.TankServer.1'
-class TankServer(CoClassBaseClass): # A CoClass
-	# TankServer Class
-	CLSID = IID('{23ADF218-986A-4FE1-8C7E-0CBB5D8EF70F}')
-	coclass_sources = [
-	]
-	coclass_interfaces = [
-	]
-
-ITankServer_vtables_dispatch_ = 0
-ITankServer_vtables_ = [
-	(( u'AddClient' , u'ClientName' , ), 1610678272, (1610678272, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 12 , (3, 0, None, None) , 0 , )),
-	(( u'AddTank' , u'TankName' , u'FilePath' , ), 1610678273, (1610678273, (), [ (8, 1, None, None) , 
-			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 16 , (3, 0, None, None) , 0 , )),
-	(( u'CloseTank' , u'CID' , ), 1610678274, (1610678274, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 20 , (3, 0, None, None) , 0 , )),
-	(( u'DeleteClient' , u'CID' , ), 1610678275, (1610678275, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 24 , (3, 0, None, None) , 0 , )),
-	(( u'RemoveTank' , u'TankName' , ), 1610678276, (1610678276, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 28 , (3, 0, None, None) , 0 , )),
-	(( u'GetBlockInfo' , u'CID' , u'Name' , u'Owner' , u'Memo' , 
-			u'StartTime' , u'StopTime' , u'Notes' , ), 1610678277, (1610678277, (), [ (3, 1, None, None) , 
-			(16392, 2, None, None) , (16392, 2, None, None) , (16392, 2, None, None) , (16389, 2, None, None) , (16389, 2, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 32 , (3, 0, None, None) , 0 , )),
-	(( u'GetError' , u'CID' , u'ErrMess' , ), 1610678278, (1610678278, (), [ (3, 1, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 36 , (3, 0, None, None) , 0 , )),
-	(( u'GetEvents' , u'CID' , u'pvEV' , u'MaxEv' , u'CodeID' , 
-			u'ChanNo' , u'SortCode' , u'T1' , u'T2' , u'Options' , 
-			), 1610678279, (1610678279, (), [ (3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 40 , (3, 0, None, None) , 0 , )),
-	(( u'GetStatus' , u'CID' , u'StatCode' , ), 1610678280, (1610678280, (), [ (3, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 44 , (3, 0, None, None) , 0 , )),
-	(( u'InitializeTank' , u'TankName' , ), 1610678281, (1610678281, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 48 , (3, 0, None, None) , 0 , )),
-	(( u'OpenTank' , u'CID' , u'TankName' , u'Mode' , ), 1610678282, (1610678282, (), [ 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 52 , (3, 0, None, None) , 0 , )),
-	(( u'SaveEvents' , u'CID' , u'pvEV' , ), 1610678283, (1610678283, (), [ (3, 1, None, None) , 
-			(16396, 1, None, None) , ], 1 , 1 , 4 , 0 , 56 , (3, 0, None, None) , 0 , )),
-	(( u'SelectBlock' , u'CID' , u'Name' , ), 1610678284, (1610678284, (), [ (3, 1, None, None) , 
-			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 60 , (3, 0, None, None) , 0 , )),
-	(( u'SetReadOffset' , u'CID' , u'OSTime' , ), 1610678285, (1610678285, (), [ (3, 1, None, None) , 
-			(5, 1, None, None) , ], 1 , 1 , 4 , 0 , 64 , (3, 0, None, None) , 0 , )),
-	(( u'StartRecord' , u'CID' , u'BlockName' , ), 1610678286, (1610678286, (), [ (3, 1, None, None) , 
-			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 68 , (3, 0, None, None) , 0 , )),
-	(( u'StopRecord' , u'CID' , ), 1610678287, (1610678287, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 72 , (3, 0, None, None) , 0 , )),
-	(( u'GetSeqEvents' , u'pvEV' , u'MaxRead' , u'Reset' , ), 1610678288, (1610678288, (), [ 
-			(16396, 2, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 76 , (3, 0, None, None) , 0 , )),
-	(( u'SetOSTime' , u'CID' , u'OSTime' , ), 1610678289, (1610678289, (), [ (3, 1, None, None) , 
-			(5, 1, None, None) , ], 1 , 1 , 4 , 0 , 80 , (3, 0, None, None) , 0 , )),
-	(( u'QueryBlockName' , u'CID' , u'n' , u'pName' , ), 1610678290, (1610678290, (), [ 
-			(3, 1, None, None) , (3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 84 , (3, 0, None, None) , 0 , )),
-	(( u'GetEventCodes' , u'CID' , u'pvCL' , u'evtype' , ), 1610678291, (1610678291, (), [ 
-			(3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 88 , (3, 0, None, None) , 0 , )),
-	(( u'ResetTank' , u'TankName' , ), 1610678292, (1610678292, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 92 , (3, 0, None, None) , 0 , )),
-	(( u'CheckTank' , u'TankName' , ), 1610678293, (1610678293, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 96 , (3, 0, None, None) , 0 , )),
-	(( u'GetEnumTank' , u'nTank' , u'TankName' , ), 1610678294, (1610678294, (), [ (3, 1, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 100 , (3, 0, None, None) , 0 , )),
-	(( u'GetTankDebug' , u'TankName' , u'DebugMess' , ), 1610678295, (1610678295, (), [ (8, 1, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 104 , (3, 0, None, None) , 0 , )),
-	(( u'EnabTankDebug' , u'TankName' , u'enab' , ), 1610678296, (1610678296, (), [ (8, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 108 , (3, 0, None, None) , 0 , )),
-	(( u'GetTankItem' , u'Name' , u'ItemCode' , u'RetVal' , ), 1610678297, (1610678297, (), [ 
-			(8, 1, None, None) , (8, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 112 , (3, 0, None, None) , 0 , )),
-	(( u'RemoveEvents' , u'CID' , u'BlockName' , u'RelTime1' , u'RelTime2' , 
-			), 1610678298, (1610678298, (), [ (3, 1, None, None) , (8, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , ], 1 , 1 , 4 , 0 , 116 , (3, 0, None, None) , 0 , )),
-	(( u'GetHotBlock' , u'CID' , u'pName' , ), 1610678299, (1610678299, (), [ (3, 1, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 120 , (3, 0, None, None) , 0 , )),
-	(( u'GetNumOf' , u'CID' , u'ItemCode' , ), 1610678300, (1610678300, (), [ (3, 1, None, None) , 
-			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 124 , (3, 0, None, None) , 0 , )),
-	(( u'GetEpocCodes' , u'CID' , u'pvCL' , ), 1610678301, (1610678301, (), [ (3, 1, None, None) , 
-			(16396, 2, None, None) , ], 1 , 1 , 4 , 0 , 128 , (3, 0, None, None) , 0 , )),
-	(( u'GetEpocs' , u'CID' , u'pvEP' , u'TankCode' , u'T1' , 
-			u'T2' , u'MaxEpocs' , ), 1610678302, (1610678302, (), [ (3, 1, None, None) , (16396, 2, None, None) , 
-			(3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 132 , (3, 0, None, None) , 0 , )),
-	(( u'SetFilter' , u'CID' , u'TankCode' , u'TestCode' , u'V1' , 
-			u'V2' , ), 1610678303, (1610678303, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(5, 1, None, None) , (5, 1, None, None) , ], 1 , 1 , 4 , 0 , 136 , (3, 0, None, None) , 0 , )),
-	(( u'QryEpocAt' , u'CID' , u'TankCode' , u'rTime' , u'ReqItem' , 
-			u'pRV' , ), 1610678304, (1610678304, (), [ (3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , 
-			(3, 1, None, None) , (16389, 2, None, None) , ], 1 , 1 , 4 , 0 , 140 , (3, 0, None, None) , 0 , )),
-	(( u'CreateEpocIndexing' , u'CID' , ), 1610678305, (1610678305, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 144 , (3, 0, None, None) , 0 , )),
-	(( u'ClearIndexing' , u'CID' , ), 1610678306, (1610678306, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 148 , (3, 0, None, None) , 0 , )),
-	(( u'IndexEvent' , u'CID' , u'TankCode' , u'Channel' , u'SortCode' , 
-			), 1610678307, (1610678307, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 152 , (3, 0, None, None) , 0 , )),
-	(( u'SetBlockInfo' , u'CID' , u'BlockName' , u'ItemCode' , u'sVal' , 
-			), 1610678308, (1610678308, (), [ (3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 156 , (3, 0, None, None) , 0 , )),
-	(( u'QryEpocAtIdx' , u'CID' , u'TankCode' , u'Idx' , u'ReqItem' , 
-			u'pRV' , ), 1610678309, (1610678309, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (16389, 2, None, None) , ], 1 , 1 , 4 , 0 , 160 , (3, 0, None, None) , 0 , )),
-	(( u'LosenFactor' , u'CID' , u'pVal' , ), 1610678310, (1610678310, (), [ (3, 0, None, None) , 
-			(16389, 10, None, None) , ], 1 , 2 , 4 , 0 , 164 , (3, 0, None, None) , 0 , )),
-	(( u'LosenFactor' , u'CID' , u'pVal' , ), 1610678310, (1610678310, (), [ (3, 0, None, None) , 
-			(5, 1, None, None) , ], 1 , 4 , 4 , 0 , 168 , (3, 0, None, None) , 0 , )),
-	(( u'SetFilterEx' , u'CID' , u'TankCode' , u'TestCode' , u'V1' , 
-			u'V2' , u'dimension' , u'filterIdx' , ), 1610678312, (1610678312, (), [ (3, 1, None, None) , 
-			(3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 172 , (3, 0, None, None) , 0 , )),
-	(( u'CacheDalay' , u'CID' , u'pVal' , ), 1610678313, (1610678313, (), [ (3, 1, None, None) , 
-			(16389, 10, None, None) , ], 1 , 2 , 4 , 0 , 176 , (3, 0, None, None) , 0 , )),
-	(( u'CacheDalay' , u'CID' , u'pVal' , ), 1610678313, (1610678313, (), [ (3, 1, None, None) , 
-			(5, 1, None, None) , ], 1 , 4 , 4 , 0 , 180 , (3, 0, None, None) , 0 , )),
-	(( u'SetQueryCondition' , u'CID' , u'strQuery' , u'RespectDuration' , ), 1610678315, (1610678315, (), [ 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 184 , (3, 0, None, None) , 0 , )),
-	(( u'SetFilterWithDimension' , u'CID' , u'dimension' , u'ID' , u'strQuery' , 
-			u'IsExclusive' , u'RecpectDuration' , ), 1610678316, (1610678316, (), [ (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 188 , (3, 0, None, None) , 0 , )),
-	(( u'SetEpocTimeFilter' , u'CID' , u'EpocCode' , u'T1' , u'T2' , 
-			u'RefOnset' , ), 1610678317, (1610678317, (), [ (3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , 
-			(5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 192 , (3, 0, None, None) , 0 , )),
-	(( u'SetTimeRefEpoc' , u'CID' , u'EpocCode' , u'RefOnset' , ), 1610678318, (1610678318, (), [ 
-			(3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 196 , (3, 0, None, None) , 0 , )),
-	(( u'GetEpocsEx' , u'CID' , u'pvEP' , u'TankCode' , u'T1' , 
-			u'T2' , u'MaxEpocs' , u'Mode' , ), 1610678319, (1610678319, (), [ (3, 1, None, None) , 
-			(16396, 2, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 200 , (3, 0, None, None) , 0 , )),
-	(( u'GetValidTimeRanges' , u'CID' , u'pvEP' , u'T1' , u'T2' , 
-			u'MaxRanges' , ), 1610678320, (1610678320, (), [ (3, 1, None, None) , (16396, 2, None, None) , (5, 1, None, None) , 
-			(5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 204 , (3, 0, None, None) , 0 , )),
-	(( u'QryEpocAtEx' , u'CID' , u'pvEP' , u'TankCode' , u'rTime' , 
-			u'RespectDuration' , ), 1610678321, (1610678321, (), [ (3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , 
-			(5, 1, None, None) , (3, 0, None, None) , ], 1 , 1 , 4 , 0 , 208 , (3, 0, None, None) , 0 , )),
-	(( u'StartRecordEx' , u'CID' , u'BlockName' , u'SupplementString' , ), 1610678322, (1610678322, (), [ 
-			(3, 1, None, None) , (8, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 212 , (3, 0, None, None) , 0 , )),
-	(( u'SetUseSortName' , u'CID' , u'SortName' , u'option' , ), 1610678323, (1610678323, (), [ 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 216 , (3, 0, None, None) , 0 , )),
-	(( u'SaveSortCode' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
-			u'sortCodeArray' , u'sortCondition' , u'option' , ), 1610678324, (1610678324, (), [ (3, 1, None, None) , 
-			(3, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , (12, 1, None, None) , (8, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 220 , (3, 0, None, None) , 0 , )),
-	(( u'GetSortInfoList' , u'CID' , u'codeName' , u'option1' , u'option2' , 
-			u'pInfoArray' , ), 1610678325, (1610678325, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (16396, 2, None, None) , ], 1 , 1 , 4 , 0 , 224 , (3, 0, None, None) , 0 , )),
-	(( u'GetSortCondition' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
-			u'option' , u'pSortCondition' , ), 1610678326, (1610678326, (), [ (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 228 , (3, 0, None, None) , 0 , )),
-	(( u'DeleteSortCode' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
-			u'option' , ), 1610678327, (1610678327, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 232 , (3, 0, None, None) , 0 , )),
-	(( u'GetSortChanMap' , u'CID' , u'codeName' , u'SortName' , u'option' , 
-			u'pChanMap' , ), 1610678328, (1610678328, (), [ (3, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , 
-			(3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 236 , (3, 0, None, None) , 0 , )),
-	(( u'SetRecordOption' , u'CID' , u'refTime' , u'option' , u'bufOption' , 
-			), 1610678329, (1610678329, (), [ (3, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 240 , (3, 0, None, None) , 0 , )),
-]
-
-RecordMap = {
-}
-
-CLSIDToClassMap = {
-	'{23ADF218-986A-4FE1-8C7E-0CBB5D8EF70F}' : TankServer,
-}
-CLSIDToPackageMap = {}
-win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
-VTablesToPackageMap = {}
-VTablesToClassMap = {
-	'{3E7319F1-2220-41D1-A76A-0A30C45AA03F}' : 'ITankServer',
-}
-
-
-NamesToIIDMap = {
-	'ITankServer' : '{3E7319F1-2220-41D1-A76A-0A30C45AA03F}',
-}
-
-
+# -*- coding: utf-8 -*-
+# Created by makepy.py version 0.5.00
+# By python version 2.6.6 |EPD 6.3-1 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
+# From type library 'TTankEng.exe'
+# On Mon Nov 22 10:28:59 2010
+"""TTankEng 1.0 Type Library"""
+makepy_version = '0.5.00'
+python_version = 0x20606f0
+
+import win32com.client.CLSIDToClass, pythoncom, pywintypes
+import win32com.client.util
+from pywintypes import IID
+from win32com.client import Dispatch
+
+# The following 3 lines may need tweaking for the particular server
+# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
+defaultNamedOptArg=pythoncom.Empty
+defaultNamedNotOptArg=pythoncom.Empty
+defaultUnnamedArg=pythoncom.Empty
+
+CLSID = IID('{BBA11881-D2C7-4FDB-873D-A474560D7394}')
+MajorVersion = 1
+MinorVersion = 0
+LibraryFlags = 8
+LCID = 0x0
+
+from win32com.client import CoClassBaseClass
+# This CoClass is known by the name 'TTankEng.TankServer.1'
+class TankServer(CoClassBaseClass): # A CoClass
+	# TankServer Class
+	CLSID = IID('{23ADF218-986A-4FE1-8C7E-0CBB5D8EF70F}')
+	coclass_sources = [
+	]
+	coclass_interfaces = [
+	]
+
+ITankServer_vtables_dispatch_ = 0
+ITankServer_vtables_ = [
+	(( u'AddClient' , u'ClientName' , ), 1610678272, (1610678272, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 12 , (3, 0, None, None) , 0 , )),
+	(( u'AddTank' , u'TankName' , u'FilePath' , ), 1610678273, (1610678273, (), [ (8, 1, None, None) , 
+			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 16 , (3, 0, None, None) , 0 , )),
+	(( u'CloseTank' , u'CID' , ), 1610678274, (1610678274, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 20 , (3, 0, None, None) , 0 , )),
+	(( u'DeleteClient' , u'CID' , ), 1610678275, (1610678275, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 24 , (3, 0, None, None) , 0 , )),
+	(( u'RemoveTank' , u'TankName' , ), 1610678276, (1610678276, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 28 , (3, 0, None, None) , 0 , )),
+	(( u'GetBlockInfo' , u'CID' , u'Name' , u'Owner' , u'Memo' , 
+			u'StartTime' , u'StopTime' , u'Notes' , ), 1610678277, (1610678277, (), [ (3, 1, None, None) , 
+			(16392, 2, None, None) , (16392, 2, None, None) , (16392, 2, None, None) , (16389, 2, None, None) , (16389, 2, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 32 , (3, 0, None, None) , 0 , )),
+	(( u'GetError' , u'CID' , u'ErrMess' , ), 1610678278, (1610678278, (), [ (3, 1, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 36 , (3, 0, None, None) , 0 , )),
+	(( u'GetEvents' , u'CID' , u'pvEV' , u'MaxEv' , u'CodeID' , 
+			u'ChanNo' , u'SortCode' , u'T1' , u'T2' , u'Options' , 
+			), 1610678279, (1610678279, (), [ (3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 40 , (3, 0, None, None) , 0 , )),
+	(( u'GetStatus' , u'CID' , u'StatCode' , ), 1610678280, (1610678280, (), [ (3, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 44 , (3, 0, None, None) , 0 , )),
+	(( u'InitializeTank' , u'TankName' , ), 1610678281, (1610678281, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 48 , (3, 0, None, None) , 0 , )),
+	(( u'OpenTank' , u'CID' , u'TankName' , u'Mode' , ), 1610678282, (1610678282, (), [ 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 52 , (3, 0, None, None) , 0 , )),
+	(( u'SaveEvents' , u'CID' , u'pvEV' , ), 1610678283, (1610678283, (), [ (3, 1, None, None) , 
+			(16396, 1, None, None) , ], 1 , 1 , 4 , 0 , 56 , (3, 0, None, None) , 0 , )),
+	(( u'SelectBlock' , u'CID' , u'Name' , ), 1610678284, (1610678284, (), [ (3, 1, None, None) , 
+			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 60 , (3, 0, None, None) , 0 , )),
+	(( u'SetReadOffset' , u'CID' , u'OSTime' , ), 1610678285, (1610678285, (), [ (3, 1, None, None) , 
+			(5, 1, None, None) , ], 1 , 1 , 4 , 0 , 64 , (3, 0, None, None) , 0 , )),
+	(( u'StartRecord' , u'CID' , u'BlockName' , ), 1610678286, (1610678286, (), [ (3, 1, None, None) , 
+			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 68 , (3, 0, None, None) , 0 , )),
+	(( u'StopRecord' , u'CID' , ), 1610678287, (1610678287, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 72 , (3, 0, None, None) , 0 , )),
+	(( u'GetSeqEvents' , u'pvEV' , u'MaxRead' , u'Reset' , ), 1610678288, (1610678288, (), [ 
+			(16396, 2, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 76 , (3, 0, None, None) , 0 , )),
+	(( u'SetOSTime' , u'CID' , u'OSTime' , ), 1610678289, (1610678289, (), [ (3, 1, None, None) , 
+			(5, 1, None, None) , ], 1 , 1 , 4 , 0 , 80 , (3, 0, None, None) , 0 , )),
+	(( u'QueryBlockName' , u'CID' , u'n' , u'pName' , ), 1610678290, (1610678290, (), [ 
+			(3, 1, None, None) , (3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 84 , (3, 0, None, None) , 0 , )),
+	(( u'GetEventCodes' , u'CID' , u'pvCL' , u'evtype' , ), 1610678291, (1610678291, (), [ 
+			(3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 88 , (3, 0, None, None) , 0 , )),
+	(( u'ResetTank' , u'TankName' , ), 1610678292, (1610678292, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 92 , (3, 0, None, None) , 0 , )),
+	(( u'CheckTank' , u'TankName' , ), 1610678293, (1610678293, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 96 , (3, 0, None, None) , 0 , )),
+	(( u'GetEnumTank' , u'nTank' , u'TankName' , ), 1610678294, (1610678294, (), [ (3, 1, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 100 , (3, 0, None, None) , 0 , )),
+	(( u'GetTankDebug' , u'TankName' , u'DebugMess' , ), 1610678295, (1610678295, (), [ (8, 1, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 104 , (3, 0, None, None) , 0 , )),
+	(( u'EnabTankDebug' , u'TankName' , u'enab' , ), 1610678296, (1610678296, (), [ (8, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 108 , (3, 0, None, None) , 0 , )),
+	(( u'GetTankItem' , u'Name' , u'ItemCode' , u'RetVal' , ), 1610678297, (1610678297, (), [ 
+			(8, 1, None, None) , (8, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 112 , (3, 0, None, None) , 0 , )),
+	(( u'RemoveEvents' , u'CID' , u'BlockName' , u'RelTime1' , u'RelTime2' , 
+			), 1610678298, (1610678298, (), [ (3, 1, None, None) , (8, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , ], 1 , 1 , 4 , 0 , 116 , (3, 0, None, None) , 0 , )),
+	(( u'GetHotBlock' , u'CID' , u'pName' , ), 1610678299, (1610678299, (), [ (3, 1, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 120 , (3, 0, None, None) , 0 , )),
+	(( u'GetNumOf' , u'CID' , u'ItemCode' , ), 1610678300, (1610678300, (), [ (3, 1, None, None) , 
+			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 124 , (3, 0, None, None) , 0 , )),
+	(( u'GetEpocCodes' , u'CID' , u'pvCL' , ), 1610678301, (1610678301, (), [ (3, 1, None, None) , 
+			(16396, 2, None, None) , ], 1 , 1 , 4 , 0 , 128 , (3, 0, None, None) , 0 , )),
+	(( u'GetEpocs' , u'CID' , u'pvEP' , u'TankCode' , u'T1' , 
+			u'T2' , u'MaxEpocs' , ), 1610678302, (1610678302, (), [ (3, 1, None, None) , (16396, 2, None, None) , 
+			(3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 132 , (3, 0, None, None) , 0 , )),
+	(( u'SetFilter' , u'CID' , u'TankCode' , u'TestCode' , u'V1' , 
+			u'V2' , ), 1610678303, (1610678303, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(5, 1, None, None) , (5, 1, None, None) , ], 1 , 1 , 4 , 0 , 136 , (3, 0, None, None) , 0 , )),
+	(( u'QryEpocAt' , u'CID' , u'TankCode' , u'rTime' , u'ReqItem' , 
+			u'pRV' , ), 1610678304, (1610678304, (), [ (3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , 
+			(3, 1, None, None) , (16389, 2, None, None) , ], 1 , 1 , 4 , 0 , 140 , (3, 0, None, None) , 0 , )),
+	(( u'CreateEpocIndexing' , u'CID' , ), 1610678305, (1610678305, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 144 , (3, 0, None, None) , 0 , )),
+	(( u'ClearIndexing' , u'CID' , ), 1610678306, (1610678306, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 148 , (3, 0, None, None) , 0 , )),
+	(( u'IndexEvent' , u'CID' , u'TankCode' , u'Channel' , u'SortCode' , 
+			), 1610678307, (1610678307, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 152 , (3, 0, None, None) , 0 , )),
+	(( u'SetBlockInfo' , u'CID' , u'BlockName' , u'ItemCode' , u'sVal' , 
+			), 1610678308, (1610678308, (), [ (3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 156 , (3, 0, None, None) , 0 , )),
+	(( u'QryEpocAtIdx' , u'CID' , u'TankCode' , u'Idx' , u'ReqItem' , 
+			u'pRV' , ), 1610678309, (1610678309, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (16389, 2, None, None) , ], 1 , 1 , 4 , 0 , 160 , (3, 0, None, None) , 0 , )),
+	(( u'LosenFactor' , u'CID' , u'pVal' , ), 1610678310, (1610678310, (), [ (3, 0, None, None) , 
+			(16389, 10, None, None) , ], 1 , 2 , 4 , 0 , 164 , (3, 0, None, None) , 0 , )),
+	(( u'LosenFactor' , u'CID' , u'pVal' , ), 1610678310, (1610678310, (), [ (3, 0, None, None) , 
+			(5, 1, None, None) , ], 1 , 4 , 4 , 0 , 168 , (3, 0, None, None) , 0 , )),
+	(( u'SetFilterEx' , u'CID' , u'TankCode' , u'TestCode' , u'V1' , 
+			u'V2' , u'dimension' , u'filterIdx' , ), 1610678312, (1610678312, (), [ (3, 1, None, None) , 
+			(3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 172 , (3, 0, None, None) , 0 , )),
+	(( u'CacheDalay' , u'CID' , u'pVal' , ), 1610678313, (1610678313, (), [ (3, 1, None, None) , 
+			(16389, 10, None, None) , ], 1 , 2 , 4 , 0 , 176 , (3, 0, None, None) , 0 , )),
+	(( u'CacheDalay' , u'CID' , u'pVal' , ), 1610678313, (1610678313, (), [ (3, 1, None, None) , 
+			(5, 1, None, None) , ], 1 , 4 , 4 , 0 , 180 , (3, 0, None, None) , 0 , )),
+	(( u'SetQueryCondition' , u'CID' , u'strQuery' , u'RespectDuration' , ), 1610678315, (1610678315, (), [ 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 184 , (3, 0, None, None) , 0 , )),
+	(( u'SetFilterWithDimension' , u'CID' , u'dimension' , u'ID' , u'strQuery' , 
+			u'IsExclusive' , u'RecpectDuration' , ), 1610678316, (1610678316, (), [ (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 188 , (3, 0, None, None) , 0 , )),
+	(( u'SetEpocTimeFilter' , u'CID' , u'EpocCode' , u'T1' , u'T2' , 
+			u'RefOnset' , ), 1610678317, (1610678317, (), [ (3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , 
+			(5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 192 , (3, 0, None, None) , 0 , )),
+	(( u'SetTimeRefEpoc' , u'CID' , u'EpocCode' , u'RefOnset' , ), 1610678318, (1610678318, (), [ 
+			(3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 196 , (3, 0, None, None) , 0 , )),
+	(( u'GetEpocsEx' , u'CID' , u'pvEP' , u'TankCode' , u'T1' , 
+			u'T2' , u'MaxEpocs' , u'Mode' , ), 1610678319, (1610678319, (), [ (3, 1, None, None) , 
+			(16396, 2, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 200 , (3, 0, None, None) , 0 , )),
+	(( u'GetValidTimeRanges' , u'CID' , u'pvEP' , u'T1' , u'T2' , 
+			u'MaxRanges' , ), 1610678320, (1610678320, (), [ (3, 1, None, None) , (16396, 2, None, None) , (5, 1, None, None) , 
+			(5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 204 , (3, 0, None, None) , 0 , )),
+	(( u'QryEpocAtEx' , u'CID' , u'pvEP' , u'TankCode' , u'rTime' , 
+			u'RespectDuration' , ), 1610678321, (1610678321, (), [ (3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , 
+			(5, 1, None, None) , (3, 0, None, None) , ], 1 , 1 , 4 , 0 , 208 , (3, 0, None, None) , 0 , )),
+	(( u'StartRecordEx' , u'CID' , u'BlockName' , u'SupplementString' , ), 1610678322, (1610678322, (), [ 
+			(3, 1, None, None) , (8, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 212 , (3, 0, None, None) , 0 , )),
+	(( u'SetUseSortName' , u'CID' , u'SortName' , u'option' , ), 1610678323, (1610678323, (), [ 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 216 , (3, 0, None, None) , 0 , )),
+	(( u'SaveSortCode' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
+			u'sortCodeArray' , u'sortCondition' , u'option' , ), 1610678324, (1610678324, (), [ (3, 1, None, None) , 
+			(3, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , (12, 1, None, None) , (8, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 220 , (3, 0, None, None) , 0 , )),
+	(( u'GetSortInfoList' , u'CID' , u'codeName' , u'option1' , u'option2' , 
+			u'pInfoArray' , ), 1610678325, (1610678325, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (16396, 2, None, None) , ], 1 , 1 , 4 , 0 , 224 , (3, 0, None, None) , 0 , )),
+	(( u'GetSortCondition' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
+			u'option' , u'pSortCondition' , ), 1610678326, (1610678326, (), [ (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 228 , (3, 0, None, None) , 0 , )),
+	(( u'DeleteSortCode' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
+			u'option' , ), 1610678327, (1610678327, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 232 , (3, 0, None, None) , 0 , )),
+	(( u'GetSortChanMap' , u'CID' , u'codeName' , u'SortName' , u'option' , 
+			u'pChanMap' , ), 1610678328, (1610678328, (), [ (3, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , 
+			(3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 236 , (3, 0, None, None) , 0 , )),
+	(( u'SetRecordOption' , u'CID' , u'refTime' , u'option' , u'bufOption' , 
+			), 1610678329, (1610678329, (), [ (3, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 240 , (3, 0, None, None) , 0 , )),
+]
+
+RecordMap = {
+}
+
+CLSIDToClassMap = {
+	'{23ADF218-986A-4FE1-8C7E-0CBB5D8EF70F}' : TankServer,
+}
+CLSIDToPackageMap = {}
+win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
+VTablesToPackageMap = {}
+VTablesToClassMap = {
+	'{3E7319F1-2220-41D1-A76A-0A30C45AA03F}' : 'ITankServer',
+}
+
+
+NamesToIIDMap = {
+	'ITankServer' : '{3E7319F1-2220-41D1-A76A-0A30C45AA03F}',
+}
+
+
```

### Comparing `TDTPy-0.8.1/tdt/actxobjects/TTankEng.py` & `TDTPy-0.9.0/tdt/actxobjects/TTankEng.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-# -*- coding: utf-8 -*-
-# Created by makepy.py version 0.5.00
-# By python version 2.6.6 |EPD 6.3-2 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
-# From type library 'TTankEng.exe'
-# On Thu Dec 02 20:59:59 2010
-"""TTankEng 1.0 Type Library"""
-makepy_version = '0.5.00'
-python_version = 0x20606f0
-
-import win32com.client.CLSIDToClass, pythoncom, pywintypes
-import win32com.client.util
-from pywintypes import IID
-from win32com.client import Dispatch
-
-# The following 3 lines may need tweaking for the particular server
-# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
-defaultNamedOptArg=pythoncom.Empty
-defaultNamedNotOptArg=pythoncom.Empty
-defaultUnnamedArg=pythoncom.Empty
-
-CLSID = IID('{BBA11881-D2C7-4FDB-873D-A474560D7394}')
-MajorVersion = 1
-MinorVersion = 0
-LibraryFlags = 8
-LCID = 0x0
-
-from win32com.client import CoClassBaseClass
-# This CoClass is known by the name 'TTankEng.TankServer.1'
-class TankServer(CoClassBaseClass): # A CoClass
-	# TankServer Class
-	CLSID = IID('{23ADF218-986A-4FE1-8C7E-0CBB5D8EF70F}')
-	coclass_sources = [
-	]
-	coclass_interfaces = [
-	]
-
-ITankServer_vtables_dispatch_ = 0
-ITankServer_vtables_ = [
-	(( u'AddClient' , u'ClientName' , ), 1610678272, (1610678272, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 12 , (3, 0, None, None) , 0 , )),
-	(( u'AddTank' , u'TankName' , u'FilePath' , ), 1610678273, (1610678273, (), [ (8, 1, None, None) , 
-			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 16 , (3, 0, None, None) , 0 , )),
-	(( u'CloseTank' , u'CID' , ), 1610678274, (1610678274, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 20 , (3, 0, None, None) , 0 , )),
-	(( u'DeleteClient' , u'CID' , ), 1610678275, (1610678275, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 24 , (3, 0, None, None) , 0 , )),
-	(( u'RemoveTank' , u'TankName' , ), 1610678276, (1610678276, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 28 , (3, 0, None, None) , 0 , )),
-	(( u'GetBlockInfo' , u'CID' , u'Name' , u'Owner' , u'Memo' , 
-			u'StartTime' , u'StopTime' , u'Notes' , ), 1610678277, (1610678277, (), [ (3, 1, None, None) , 
-			(16392, 2, None, None) , (16392, 2, None, None) , (16392, 2, None, None) , (16389, 2, None, None) , (16389, 2, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 32 , (3, 0, None, None) , 0 , )),
-	(( u'GetError' , u'CID' , u'ErrMess' , ), 1610678278, (1610678278, (), [ (3, 1, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 36 , (3, 0, None, None) , 0 , )),
-	(( u'GetEvents' , u'CID' , u'pvEV' , u'MaxEv' , u'CodeID' , 
-			u'ChanNo' , u'SortCode' , u'T1' , u'T2' , u'Options' , 
-			), 1610678279, (1610678279, (), [ (3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 40 , (3, 0, None, None) , 0 , )),
-	(( u'GetStatus' , u'CID' , u'StatCode' , ), 1610678280, (1610678280, (), [ (3, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 44 , (3, 0, None, None) , 0 , )),
-	(( u'InitializeTank' , u'TankName' , ), 1610678281, (1610678281, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 48 , (3, 0, None, None) , 0 , )),
-	(( u'OpenTank' , u'CID' , u'TankName' , u'Mode' , ), 1610678282, (1610678282, (), [ 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 52 , (3, 0, None, None) , 0 , )),
-	(( u'SaveEvents' , u'CID' , u'pvEV' , ), 1610678283, (1610678283, (), [ (3, 1, None, None) , 
-			(16396, 1, None, None) , ], 1 , 1 , 4 , 0 , 56 , (3, 0, None, None) , 0 , )),
-	(( u'SelectBlock' , u'CID' , u'Name' , ), 1610678284, (1610678284, (), [ (3, 1, None, None) , 
-			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 60 , (3, 0, None, None) , 0 , )),
-	(( u'SetReadOffset' , u'CID' , u'OSTime' , ), 1610678285, (1610678285, (), [ (3, 1, None, None) , 
-			(5, 1, None, None) , ], 1 , 1 , 4 , 0 , 64 , (3, 0, None, None) , 0 , )),
-	(( u'StartRecord' , u'CID' , u'BlockName' , ), 1610678286, (1610678286, (), [ (3, 1, None, None) , 
-			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 68 , (3, 0, None, None) , 0 , )),
-	(( u'StopRecord' , u'CID' , ), 1610678287, (1610678287, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 72 , (3, 0, None, None) , 0 , )),
-	(( u'GetSeqEvents' , u'pvEV' , u'MaxRead' , u'Reset' , ), 1610678288, (1610678288, (), [ 
-			(16396, 2, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 76 , (3, 0, None, None) , 0 , )),
-	(( u'SetOSTime' , u'CID' , u'OSTime' , ), 1610678289, (1610678289, (), [ (3, 1, None, None) , 
-			(5, 1, None, None) , ], 1 , 1 , 4 , 0 , 80 , (3, 0, None, None) , 0 , )),
-	(( u'QueryBlockName' , u'CID' , u'n' , u'pName' , ), 1610678290, (1610678290, (), [ 
-			(3, 1, None, None) , (3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 84 , (3, 0, None, None) , 0 , )),
-	(( u'GetEventCodes' , u'CID' , u'pvCL' , u'evtype' , ), 1610678291, (1610678291, (), [ 
-			(3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 88 , (3, 0, None, None) , 0 , )),
-	(( u'ResetTank' , u'TankName' , ), 1610678292, (1610678292, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 92 , (3, 0, None, None) , 0 , )),
-	(( u'CheckTank' , u'TankName' , ), 1610678293, (1610678293, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 96 , (3, 0, None, None) , 0 , )),
-	(( u'GetEnumTank' , u'nTank' , u'TankName' , ), 1610678294, (1610678294, (), [ (3, 1, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 100 , (3, 0, None, None) , 0 , )),
-	(( u'GetTankDebug' , u'TankName' , u'DebugMess' , ), 1610678295, (1610678295, (), [ (8, 1, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 104 , (3, 0, None, None) , 0 , )),
-	(( u'EnabTankDebug' , u'TankName' , u'enab' , ), 1610678296, (1610678296, (), [ (8, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 108 , (3, 0, None, None) , 0 , )),
-	(( u'GetTankItem' , u'Name' , u'ItemCode' , u'RetVal' , ), 1610678297, (1610678297, (), [ 
-			(8, 1, None, None) , (8, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 112 , (3, 0, None, None) , 0 , )),
-	(( u'RemoveEvents' , u'CID' , u'BlockName' , u'RelTime1' , u'RelTime2' , 
-			), 1610678298, (1610678298, (), [ (3, 1, None, None) , (8, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , ], 1 , 1 , 4 , 0 , 116 , (3, 0, None, None) , 0 , )),
-	(( u'GetHotBlock' , u'CID' , u'pName' , ), 1610678299, (1610678299, (), [ (3, 1, None, None) , 
-			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 120 , (3, 0, None, None) , 0 , )),
-	(( u'GetNumOf' , u'CID' , u'ItemCode' , ), 1610678300, (1610678300, (), [ (3, 1, None, None) , 
-			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 124 , (3, 0, None, None) , 0 , )),
-	(( u'GetEpocCodes' , u'CID' , u'pvCL' , ), 1610678301, (1610678301, (), [ (3, 1, None, None) , 
-			(16396, 2, None, None) , ], 1 , 1 , 4 , 0 , 128 , (3, 0, None, None) , 0 , )),
-	(( u'GetEpocs' , u'CID' , u'pvEP' , u'TankCode' , u'T1' , 
-			u'T2' , u'MaxEpocs' , ), 1610678302, (1610678302, (), [ (3, 1, None, None) , (16396, 2, None, None) , 
-			(3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 132 , (3, 0, None, None) , 0 , )),
-	(( u'SetFilter' , u'CID' , u'TankCode' , u'TestCode' , u'V1' , 
-			u'V2' , ), 1610678303, (1610678303, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(5, 1, None, None) , (5, 1, None, None) , ], 1 , 1 , 4 , 0 , 136 , (3, 0, None, None) , 0 , )),
-	(( u'QryEpocAt' , u'CID' , u'TankCode' , u'rTime' , u'ReqItem' , 
-			u'pRV' , ), 1610678304, (1610678304, (), [ (3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , 
-			(3, 1, None, None) , (16389, 2, None, None) , ], 1 , 1 , 4 , 0 , 140 , (3, 0, None, None) , 0 , )),
-	(( u'CreateEpocIndexing' , u'CID' , ), 1610678305, (1610678305, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 144 , (3, 0, None, None) , 0 , )),
-	(( u'ClearIndexing' , u'CID' , ), 1610678306, (1610678306, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 148 , (3, 0, None, None) , 0 , )),
-	(( u'IndexEvent' , u'CID' , u'TankCode' , u'Channel' , u'SortCode' , 
-			), 1610678307, (1610678307, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 152 , (3, 0, None, None) , 0 , )),
-	(( u'SetBlockInfo' , u'CID' , u'BlockName' , u'ItemCode' , u'sVal' , 
-			), 1610678308, (1610678308, (), [ (3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 156 , (3, 0, None, None) , 0 , )),
-	(( u'QryEpocAtIdx' , u'CID' , u'TankCode' , u'Idx' , u'ReqItem' , 
-			u'pRV' , ), 1610678309, (1610678309, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (16389, 2, None, None) , ], 1 , 1 , 4 , 0 , 160 , (3, 0, None, None) , 0 , )),
-	(( u'LosenFactor' , u'CID' , u'pVal' , ), 1610678310, (1610678310, (), [ (3, 0, None, None) , 
-			(16389, 10, None, None) , ], 1 , 2 , 4 , 0 , 164 , (3, 0, None, None) , 0 , )),
-	(( u'LosenFactor' , u'CID' , u'pVal' , ), 1610678310, (1610678310, (), [ (3, 0, None, None) , 
-			(5, 1, None, None) , ], 1 , 4 , 4 , 0 , 168 , (3, 0, None, None) , 0 , )),
-	(( u'SetFilterEx' , u'CID' , u'TankCode' , u'TestCode' , u'V1' , 
-			u'V2' , u'dimension' , u'filterIdx' , ), 1610678312, (1610678312, (), [ (3, 1, None, None) , 
-			(3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 172 , (3, 0, None, None) , 0 , )),
-	(( u'CacheDalay' , u'CID' , u'pVal' , ), 1610678313, (1610678313, (), [ (3, 1, None, None) , 
-			(16389, 10, None, None) , ], 1 , 2 , 4 , 0 , 176 , (3, 0, None, None) , 0 , )),
-	(( u'CacheDalay' , u'CID' , u'pVal' , ), 1610678313, (1610678313, (), [ (3, 1, None, None) , 
-			(5, 1, None, None) , ], 1 , 4 , 4 , 0 , 180 , (3, 0, None, None) , 0 , )),
-	(( u'SetQueryCondition' , u'CID' , u'strQuery' , u'RespectDuration' , ), 1610678315, (1610678315, (), [ 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 184 , (3, 0, None, None) , 0 , )),
-	(( u'SetFilterWithDimension' , u'CID' , u'dimension' , u'ID' , u'strQuery' , 
-			u'IsExclusive' , u'RecpectDuration' , ), 1610678316, (1610678316, (), [ (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 188 , (3, 0, None, None) , 0 , )),
-	(( u'SetEpocTimeFilter' , u'CID' , u'EpocCode' , u'T1' , u'T2' , 
-			u'RefOnset' , ), 1610678317, (1610678317, (), [ (3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , 
-			(5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 192 , (3, 0, None, None) , 0 , )),
-	(( u'SetTimeRefEpoc' , u'CID' , u'EpocCode' , u'RefOnset' , ), 1610678318, (1610678318, (), [ 
-			(3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 196 , (3, 0, None, None) , 0 , )),
-	(( u'GetEpocsEx' , u'CID' , u'pvEP' , u'TankCode' , u'T1' , 
-			u'T2' , u'MaxEpocs' , u'Mode' , ), 1610678319, (1610678319, (), [ (3, 1, None, None) , 
-			(16396, 2, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 200 , (3, 0, None, None) , 0 , )),
-	(( u'GetValidTimeRanges' , u'CID' , u'pvEP' , u'T1' , u'T2' , 
-			u'MaxRanges' , ), 1610678320, (1610678320, (), [ (3, 1, None, None) , (16396, 2, None, None) , (5, 1, None, None) , 
-			(5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 204 , (3, 0, None, None) , 0 , )),
-	(( u'QryEpocAtEx' , u'CID' , u'pvEP' , u'TankCode' , u'rTime' , 
-			u'RespectDuration' , ), 1610678321, (1610678321, (), [ (3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , 
-			(5, 1, None, None) , (3, 0, None, None) , ], 1 , 1 , 4 , 0 , 208 , (3, 0, None, None) , 0 , )),
-	(( u'StartRecordEx' , u'CID' , u'BlockName' , u'SupplementString' , ), 1610678322, (1610678322, (), [ 
-			(3, 1, None, None) , (8, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 212 , (3, 0, None, None) , 0 , )),
-	(( u'SetUseSortName' , u'CID' , u'SortName' , u'option' , ), 1610678323, (1610678323, (), [ 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 216 , (3, 0, None, None) , 0 , )),
-	(( u'SaveSortCode' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
-			u'sortCodeArray' , u'sortCondition' , u'option' , ), 1610678324, (1610678324, (), [ (3, 1, None, None) , 
-			(3, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , (12, 1, None, None) , (8, 1, None, None) , 
-			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 220 , (3, 0, None, None) , 0 , )),
-	(( u'GetSortInfoList' , u'CID' , u'codeName' , u'option1' , u'option2' , 
-			u'pInfoArray' , ), 1610678325, (1610678325, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (16396, 2, None, None) , ], 1 , 1 , 4 , 0 , 224 , (3, 0, None, None) , 0 , )),
-	(( u'GetSortCondition' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
-			u'option' , u'pSortCondition' , ), 1610678326, (1610678326, (), [ (3, 1, None, None) , (3, 1, None, None) , 
-			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 228 , (3, 0, None, None) , 0 , )),
-	(( u'DeleteSortCode' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
-			u'option' , ), 1610678327, (1610678327, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
-			(8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 232 , (3, 0, None, None) , 0 , )),
-	(( u'GetSortChanMap' , u'CID' , u'codeName' , u'SortName' , u'option' , 
-			u'pChanMap' , ), 1610678328, (1610678328, (), [ (3, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , 
-			(3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 236 , (3, 0, None, None) , 0 , )),
-	(( u'SetRecordOption' , u'CID' , u'refTime' , u'option' , u'bufOption' , 
-			), 1610678329, (1610678329, (), [ (3, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 240 , (3, 0, None, None) , 0 , )),
-]
-
-RecordMap = {
-}
-
-CLSIDToClassMap = {
-	'{23ADF218-986A-4FE1-8C7E-0CBB5D8EF70F}' : TankServer,
-}
-CLSIDToPackageMap = {}
-win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
-VTablesToPackageMap = {}
-VTablesToClassMap = {
-	'{3E7319F1-2220-41D1-A76A-0A30C45AA03F}' : 'ITankServer',
-}
-
-
-NamesToIIDMap = {
-	'ITankServer' : '{3E7319F1-2220-41D1-A76A-0A30C45AA03F}',
-}
-
-
+# -*- coding: utf-8 -*-
+# Created by makepy.py version 0.5.00
+# By python version 2.6.6 |EPD 6.3-2 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
+# From type library 'TTankEng.exe'
+# On Thu Dec 02 20:59:59 2010
+"""TTankEng 1.0 Type Library"""
+makepy_version = '0.5.00'
+python_version = 0x20606f0
+
+import win32com.client.CLSIDToClass, pythoncom, pywintypes
+import win32com.client.util
+from pywintypes import IID
+from win32com.client import Dispatch
+
+# The following 3 lines may need tweaking for the particular server
+# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
+defaultNamedOptArg=pythoncom.Empty
+defaultNamedNotOptArg=pythoncom.Empty
+defaultUnnamedArg=pythoncom.Empty
+
+CLSID = IID('{BBA11881-D2C7-4FDB-873D-A474560D7394}')
+MajorVersion = 1
+MinorVersion = 0
+LibraryFlags = 8
+LCID = 0x0
+
+from win32com.client import CoClassBaseClass
+# This CoClass is known by the name 'TTankEng.TankServer.1'
+class TankServer(CoClassBaseClass): # A CoClass
+	# TankServer Class
+	CLSID = IID('{23ADF218-986A-4FE1-8C7E-0CBB5D8EF70F}')
+	coclass_sources = [
+	]
+	coclass_interfaces = [
+	]
+
+ITankServer_vtables_dispatch_ = 0
+ITankServer_vtables_ = [
+	(( u'AddClient' , u'ClientName' , ), 1610678272, (1610678272, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 12 , (3, 0, None, None) , 0 , )),
+	(( u'AddTank' , u'TankName' , u'FilePath' , ), 1610678273, (1610678273, (), [ (8, 1, None, None) , 
+			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 16 , (3, 0, None, None) , 0 , )),
+	(( u'CloseTank' , u'CID' , ), 1610678274, (1610678274, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 20 , (3, 0, None, None) , 0 , )),
+	(( u'DeleteClient' , u'CID' , ), 1610678275, (1610678275, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 24 , (3, 0, None, None) , 0 , )),
+	(( u'RemoveTank' , u'TankName' , ), 1610678276, (1610678276, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 28 , (3, 0, None, None) , 0 , )),
+	(( u'GetBlockInfo' , u'CID' , u'Name' , u'Owner' , u'Memo' , 
+			u'StartTime' , u'StopTime' , u'Notes' , ), 1610678277, (1610678277, (), [ (3, 1, None, None) , 
+			(16392, 2, None, None) , (16392, 2, None, None) , (16392, 2, None, None) , (16389, 2, None, None) , (16389, 2, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 32 , (3, 0, None, None) , 0 , )),
+	(( u'GetError' , u'CID' , u'ErrMess' , ), 1610678278, (1610678278, (), [ (3, 1, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 36 , (3, 0, None, None) , 0 , )),
+	(( u'GetEvents' , u'CID' , u'pvEV' , u'MaxEv' , u'CodeID' , 
+			u'ChanNo' , u'SortCode' , u'T1' , u'T2' , u'Options' , 
+			), 1610678279, (1610678279, (), [ (3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 40 , (3, 0, None, None) , 0 , )),
+	(( u'GetStatus' , u'CID' , u'StatCode' , ), 1610678280, (1610678280, (), [ (3, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 44 , (3, 0, None, None) , 0 , )),
+	(( u'InitializeTank' , u'TankName' , ), 1610678281, (1610678281, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 48 , (3, 0, None, None) , 0 , )),
+	(( u'OpenTank' , u'CID' , u'TankName' , u'Mode' , ), 1610678282, (1610678282, (), [ 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 52 , (3, 0, None, None) , 0 , )),
+	(( u'SaveEvents' , u'CID' , u'pvEV' , ), 1610678283, (1610678283, (), [ (3, 1, None, None) , 
+			(16396, 1, None, None) , ], 1 , 1 , 4 , 0 , 56 , (3, 0, None, None) , 0 , )),
+	(( u'SelectBlock' , u'CID' , u'Name' , ), 1610678284, (1610678284, (), [ (3, 1, None, None) , 
+			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 60 , (3, 0, None, None) , 0 , )),
+	(( u'SetReadOffset' , u'CID' , u'OSTime' , ), 1610678285, (1610678285, (), [ (3, 1, None, None) , 
+			(5, 1, None, None) , ], 1 , 1 , 4 , 0 , 64 , (3, 0, None, None) , 0 , )),
+	(( u'StartRecord' , u'CID' , u'BlockName' , ), 1610678286, (1610678286, (), [ (3, 1, None, None) , 
+			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 68 , (3, 0, None, None) , 0 , )),
+	(( u'StopRecord' , u'CID' , ), 1610678287, (1610678287, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 72 , (3, 0, None, None) , 0 , )),
+	(( u'GetSeqEvents' , u'pvEV' , u'MaxRead' , u'Reset' , ), 1610678288, (1610678288, (), [ 
+			(16396, 2, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 76 , (3, 0, None, None) , 0 , )),
+	(( u'SetOSTime' , u'CID' , u'OSTime' , ), 1610678289, (1610678289, (), [ (3, 1, None, None) , 
+			(5, 1, None, None) , ], 1 , 1 , 4 , 0 , 80 , (3, 0, None, None) , 0 , )),
+	(( u'QueryBlockName' , u'CID' , u'n' , u'pName' , ), 1610678290, (1610678290, (), [ 
+			(3, 1, None, None) , (3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 84 , (3, 0, None, None) , 0 , )),
+	(( u'GetEventCodes' , u'CID' , u'pvCL' , u'evtype' , ), 1610678291, (1610678291, (), [ 
+			(3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 88 , (3, 0, None, None) , 0 , )),
+	(( u'ResetTank' , u'TankName' , ), 1610678292, (1610678292, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 92 , (3, 0, None, None) , 0 , )),
+	(( u'CheckTank' , u'TankName' , ), 1610678293, (1610678293, (), [ (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 96 , (3, 0, None, None) , 0 , )),
+	(( u'GetEnumTank' , u'nTank' , u'TankName' , ), 1610678294, (1610678294, (), [ (3, 1, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 100 , (3, 0, None, None) , 0 , )),
+	(( u'GetTankDebug' , u'TankName' , u'DebugMess' , ), 1610678295, (1610678295, (), [ (8, 1, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 104 , (3, 0, None, None) , 0 , )),
+	(( u'EnabTankDebug' , u'TankName' , u'enab' , ), 1610678296, (1610678296, (), [ (8, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 108 , (3, 0, None, None) , 0 , )),
+	(( u'GetTankItem' , u'Name' , u'ItemCode' , u'RetVal' , ), 1610678297, (1610678297, (), [ 
+			(8, 1, None, None) , (8, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 112 , (3, 0, None, None) , 0 , )),
+	(( u'RemoveEvents' , u'CID' , u'BlockName' , u'RelTime1' , u'RelTime2' , 
+			), 1610678298, (1610678298, (), [ (3, 1, None, None) , (8, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , ], 1 , 1 , 4 , 0 , 116 , (3, 0, None, None) , 0 , )),
+	(( u'GetHotBlock' , u'CID' , u'pName' , ), 1610678299, (1610678299, (), [ (3, 1, None, None) , 
+			(16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 120 , (3, 0, None, None) , 0 , )),
+	(( u'GetNumOf' , u'CID' , u'ItemCode' , ), 1610678300, (1610678300, (), [ (3, 1, None, None) , 
+			(8, 1, None, None) , ], 1 , 1 , 4 , 0 , 124 , (3, 0, None, None) , 0 , )),
+	(( u'GetEpocCodes' , u'CID' , u'pvCL' , ), 1610678301, (1610678301, (), [ (3, 1, None, None) , 
+			(16396, 2, None, None) , ], 1 , 1 , 4 , 0 , 128 , (3, 0, None, None) , 0 , )),
+	(( u'GetEpocs' , u'CID' , u'pvEP' , u'TankCode' , u'T1' , 
+			u'T2' , u'MaxEpocs' , ), 1610678302, (1610678302, (), [ (3, 1, None, None) , (16396, 2, None, None) , 
+			(3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 132 , (3, 0, None, None) , 0 , )),
+	(( u'SetFilter' , u'CID' , u'TankCode' , u'TestCode' , u'V1' , 
+			u'V2' , ), 1610678303, (1610678303, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(5, 1, None, None) , (5, 1, None, None) , ], 1 , 1 , 4 , 0 , 136 , (3, 0, None, None) , 0 , )),
+	(( u'QryEpocAt' , u'CID' , u'TankCode' , u'rTime' , u'ReqItem' , 
+			u'pRV' , ), 1610678304, (1610678304, (), [ (3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , 
+			(3, 1, None, None) , (16389, 2, None, None) , ], 1 , 1 , 4 , 0 , 140 , (3, 0, None, None) , 0 , )),
+	(( u'CreateEpocIndexing' , u'CID' , ), 1610678305, (1610678305, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 144 , (3, 0, None, None) , 0 , )),
+	(( u'ClearIndexing' , u'CID' , ), 1610678306, (1610678306, (), [ (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 148 , (3, 0, None, None) , 0 , )),
+	(( u'IndexEvent' , u'CID' , u'TankCode' , u'Channel' , u'SortCode' , 
+			), 1610678307, (1610678307, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 152 , (3, 0, None, None) , 0 , )),
+	(( u'SetBlockInfo' , u'CID' , u'BlockName' , u'ItemCode' , u'sVal' , 
+			), 1610678308, (1610678308, (), [ (3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 156 , (3, 0, None, None) , 0 , )),
+	(( u'QryEpocAtIdx' , u'CID' , u'TankCode' , u'Idx' , u'ReqItem' , 
+			u'pRV' , ), 1610678309, (1610678309, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (16389, 2, None, None) , ], 1 , 1 , 4 , 0 , 160 , (3, 0, None, None) , 0 , )),
+	(( u'LosenFactor' , u'CID' , u'pVal' , ), 1610678310, (1610678310, (), [ (3, 0, None, None) , 
+			(16389, 10, None, None) , ], 1 , 2 , 4 , 0 , 164 , (3, 0, None, None) , 0 , )),
+	(( u'LosenFactor' , u'CID' , u'pVal' , ), 1610678310, (1610678310, (), [ (3, 0, None, None) , 
+			(5, 1, None, None) , ], 1 , 4 , 4 , 0 , 168 , (3, 0, None, None) , 0 , )),
+	(( u'SetFilterEx' , u'CID' , u'TankCode' , u'TestCode' , u'V1' , 
+			u'V2' , u'dimension' , u'filterIdx' , ), 1610678312, (1610678312, (), [ (3, 1, None, None) , 
+			(3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 172 , (3, 0, None, None) , 0 , )),
+	(( u'CacheDalay' , u'CID' , u'pVal' , ), 1610678313, (1610678313, (), [ (3, 1, None, None) , 
+			(16389, 10, None, None) , ], 1 , 2 , 4 , 0 , 176 , (3, 0, None, None) , 0 , )),
+	(( u'CacheDalay' , u'CID' , u'pVal' , ), 1610678313, (1610678313, (), [ (3, 1, None, None) , 
+			(5, 1, None, None) , ], 1 , 4 , 4 , 0 , 180 , (3, 0, None, None) , 0 , )),
+	(( u'SetQueryCondition' , u'CID' , u'strQuery' , u'RespectDuration' , ), 1610678315, (1610678315, (), [ 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 184 , (3, 0, None, None) , 0 , )),
+	(( u'SetFilterWithDimension' , u'CID' , u'dimension' , u'ID' , u'strQuery' , 
+			u'IsExclusive' , u'RecpectDuration' , ), 1610678316, (1610678316, (), [ (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 188 , (3, 0, None, None) , 0 , )),
+	(( u'SetEpocTimeFilter' , u'CID' , u'EpocCode' , u'T1' , u'T2' , 
+			u'RefOnset' , ), 1610678317, (1610678317, (), [ (3, 1, None, None) , (3, 1, None, None) , (5, 1, None, None) , 
+			(5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 192 , (3, 0, None, None) , 0 , )),
+	(( u'SetTimeRefEpoc' , u'CID' , u'EpocCode' , u'RefOnset' , ), 1610678318, (1610678318, (), [ 
+			(3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 196 , (3, 0, None, None) , 0 , )),
+	(( u'GetEpocsEx' , u'CID' , u'pvEP' , u'TankCode' , u'T1' , 
+			u'T2' , u'MaxEpocs' , u'Mode' , ), 1610678319, (1610678319, (), [ (3, 1, None, None) , 
+			(16396, 2, None, None) , (3, 1, None, None) , (5, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 200 , (3, 0, None, None) , 0 , )),
+	(( u'GetValidTimeRanges' , u'CID' , u'pvEP' , u'T1' , u'T2' , 
+			u'MaxRanges' , ), 1610678320, (1610678320, (), [ (3, 1, None, None) , (16396, 2, None, None) , (5, 1, None, None) , 
+			(5, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 204 , (3, 0, None, None) , 0 , )),
+	(( u'QryEpocAtEx' , u'CID' , u'pvEP' , u'TankCode' , u'rTime' , 
+			u'RespectDuration' , ), 1610678321, (1610678321, (), [ (3, 1, None, None) , (16396, 2, None, None) , (3, 1, None, None) , 
+			(5, 1, None, None) , (3, 0, None, None) , ], 1 , 1 , 4 , 0 , 208 , (3, 0, None, None) , 0 , )),
+	(( u'StartRecordEx' , u'CID' , u'BlockName' , u'SupplementString' , ), 1610678322, (1610678322, (), [ 
+			(3, 1, None, None) , (8, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 212 , (3, 0, None, None) , 0 , )),
+	(( u'SetUseSortName' , u'CID' , u'SortName' , u'option' , ), 1610678323, (1610678323, (), [ 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 216 , (3, 0, None, None) , 0 , )),
+	(( u'SaveSortCode' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
+			u'sortCodeArray' , u'sortCondition' , u'option' , ), 1610678324, (1610678324, (), [ (3, 1, None, None) , 
+			(3, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , (12, 1, None, None) , (8, 1, None, None) , 
+			(3, 1, None, None) , ], 1 , 1 , 4 , 0 , 220 , (3, 0, None, None) , 0 , )),
+	(( u'GetSortInfoList' , u'CID' , u'codeName' , u'option1' , u'option2' , 
+			u'pInfoArray' , ), 1610678325, (1610678325, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (16396, 2, None, None) , ], 1 , 1 , 4 , 0 , 224 , (3, 0, None, None) , 0 , )),
+	(( u'GetSortCondition' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
+			u'option' , u'pSortCondition' , ), 1610678326, (1610678326, (), [ (3, 1, None, None) , (3, 1, None, None) , 
+			(3, 1, None, None) , (8, 1, None, None) , (3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 228 , (3, 0, None, None) , 0 , )),
+	(( u'DeleteSortCode' , u'CID' , u'codeName' , u'idxChan' , u'SortName' , 
+			u'option' , ), 1610678327, (1610678327, (), [ (3, 1, None, None) , (3, 1, None, None) , (3, 1, None, None) , 
+			(8, 1, None, None) , (3, 1, None, None) , ], 1 , 1 , 4 , 0 , 232 , (3, 0, None, None) , 0 , )),
+	(( u'GetSortChanMap' , u'CID' , u'codeName' , u'SortName' , u'option' , 
+			u'pChanMap' , ), 1610678328, (1610678328, (), [ (3, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , 
+			(3, 1, None, None) , (16392, 2, None, None) , ], 1 , 1 , 4 , 0 , 236 , (3, 0, None, None) , 0 , )),
+	(( u'SetRecordOption' , u'CID' , u'refTime' , u'option' , u'bufOption' , 
+			), 1610678329, (1610678329, (), [ (3, 1, None, None) , (5, 1, None, None) , (3, 1, None, None) , (8, 1, None, None) , ], 1 , 1 , 4 , 0 , 240 , (3, 0, None, None) , 0 , )),
+]
+
+RecordMap = {
+}
+
+CLSIDToClassMap = {
+	'{23ADF218-986A-4FE1-8C7E-0CBB5D8EF70F}' : TankServer,
+}
+CLSIDToPackageMap = {}
+win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
+VTablesToPackageMap = {}
+VTablesToClassMap = {
+	'{3E7319F1-2220-41D1-A76A-0A30C45AA03F}' : 'ITankServer',
+}
+
+
+NamesToIIDMap = {
+	'ITankServer' : '{3E7319F1-2220-41D1-A76A-0A30C45AA03F}',
+}
+
+
```

### Comparing `TDTPy-0.8.1/tdt/actxobjects/TTankInterfaces.py` & `TDTPy-0.9.0/tdt/actxobjects/TTankInterfaces.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,612 +1,612 @@
-# -*- coding: utf-8 -*-
-# Created by makepy.py version 0.5.00
-# By python version 2.6.6 |EPD 6.3-2 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
-# From type library 'TTankInterfaces.ocx'
-# On Thu Dec 02 21:00:50 2010
-"""TTankInterfaces"""
-makepy_version = '0.5.00'
-python_version = 0x20606f0
-
-import win32com.client.CLSIDToClass, pythoncom, pywintypes
-import win32com.client.util
-from pywintypes import IID
-from win32com.client import Dispatch
-
-# The following 3 lines may need tweaking for the particular server
-# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
-defaultNamedOptArg=pythoncom.Empty
-defaultNamedNotOptArg=pythoncom.Empty
-defaultUnnamedArg=pythoncom.Empty
-
-CLSID = IID('{831D8AF7-7E2B-426B-A430-18E670F56C12}')
-MajorVersion = 10
-MinorVersion = 9
-LibraryFlags = 10
-LCID = 0x0
-
-from win32com.client import DispatchBaseClass
-class _BlockSelect(DispatchBaseClass):
-	CLSID = IID('{C2F42E9B-86B7-4F21-889D-8B854B019640}')
-	coclass_clsid = IID('{CB81F5AF-7625-4F83-B629-54C37B55A203}')
-
-	def Refresh(self):
-		return self._oleobj_.InvokeTypes(1610809385, LCID, 1, (24, 0), (),)
-
-	_prop_map_get_ = {
-		"ActiveBlock": (1745027109, 2, (8, 0), (), "ActiveBlock", None),
-		"AllowDragDrop": (1745027114, 2, (11, 0), (), "AllowDragDrop", None),
-		"AllowPopup": (1745027115, 2, (11, 0), (), "AllowPopup", None),
-		"HideDetails": (1745027110, 2, (11, 0), (), "HideDetails", None),
-		"ShowDate": (1745027106, 2, (11, 0), (), "ShowDate", None),
-		"ShowDuration": (1745027103, 2, (11, 0), (), "ShowDuration", None),
-		"ShowMemo": (1745027101, 2, (11, 0), (), "ShowMemo", None),
-		"ShowOwner": (1745027102, 2, (11, 0), (), "ShowOwner", None),
-		"ShowServer": (1745027108, 2, (11, 0), (), "ShowServer", None),
-		"ShowStart": (1745027105, 2, (11, 0), (), "ShowStart", None),
-		"ShowStop": (1745027104, 2, (11, 0), (), "ShowStop", None),
-		"ShowTank": (1745027107, 2, (11, 0), (), "ShowTank", None),
-		"SingleClickSelect": (1745027100, 2, (11, 0), (), "SingleClickSelect", None),
-		"UseServer": (1745027112, 2, (8, 0), (), "UseServer", None),
-		"UseTank": (1745027111, 2, (8, 0), (), "UseTank", None),
-	}
-	_prop_map_put_ = {
-		"ActiveBlock": ((1745027109, LCID, 4, 0),()),
-		"AllowDragDrop": ((1745027114, LCID, 4, 0),()),
-		"AllowPopup": ((1745027115, LCID, 4, 0),()),
-		"HideDetails": ((1745027110, LCID, 4, 0),()),
-		"ShowDate": ((1745027106, LCID, 4, 0),()),
-		"ShowDuration": ((1745027103, LCID, 4, 0),()),
-		"ShowMemo": ((1745027101, LCID, 4, 0),()),
-		"ShowOwner": ((1745027102, LCID, 4, 0),()),
-		"ShowServer": ((1745027108, LCID, 4, 0),()),
-		"ShowStart": ((1745027105, LCID, 4, 0),()),
-		"ShowStop": ((1745027104, LCID, 4, 0),()),
-		"ShowTank": ((1745027107, LCID, 4, 0),()),
-		"SingleClickSelect": ((1745027100, LCID, 4, 0),()),
-		"UseServer": ((1745027112, LCID, 4, 0),()),
-		"UseTank": ((1745027111, LCID, 4, 0),()),
-	}
-
-class _EventSelect(DispatchBaseClass):
-	CLSID = IID('{CBA421AC-7EB7-40BA-AA2C-81CC652B2EEF}')
-	coclass_clsid = IID('{01B10737-93FA-4FB2-B1F1-0C59793EBCAA}')
-
-	def ClearChecks(self, CheckState=defaultNamedNotOptArg):
-		return self._ApplyTypes_(1610809454, 1, (24, 0), ((16395, 3),), u'ClearChecks', None,CheckState
-			)
-
-	def GetChecked(self, EvName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(1610809451, LCID, 1, (11, 0), ((8, 1),),EvName
-			)
-
-	def GetEvName(self, Index=defaultNamedNotOptArg):
-		return self._ApplyTypes_(1610809453, 1, (8, 0), ((16387, 3),), u'GetEvName', None,Index
-			)
-
-	def Refresh(self):
-		return self._oleobj_.InvokeTypes(1610809449, LCID, 1, (24, 0), (),)
-
-	def SetChecked(self, EvName=defaultNamedNotOptArg, CheckState=defaultNamedNotOptArg):
-		return self._ApplyTypes_(1610809452, 1, (24, 0), ((8, 1), (16395, 3)), u'SetChecked', None,EvName
-			, CheckState)
-
-	_prop_map_get_ = {
-		"ActiveEvent": (1745027145, 2, (8, 0), (), "ActiveEvent", None),
-		"AllowActive": (1745027143, 2, (11, 0), (), "AllowActive", None),
-		"AllowDragDrop": (1745027142, 2, (11, 0), (), "AllowDragDrop", None),
-		"HideDetails": (1745027158, 2, (11, 0), (), "HideDetails", None),
-		"ShowBlock": (1745027148, 2, (11, 0), (), "ShowBlock", None),
-		"ShowChecks": (1745027146, 2, (11, 0), (), "ShowChecks", None),
-		"ShowDataFormat": (1745027153, 2, (11, 0), (), "ShowDataFormat", None),
-		"ShowDefaultEvent": (1745027183, 2, (11, 0), (), "ShowDefaultEvent", None),
-		"ShowFirstTime": (1745027151, 2, (11, 0), (), "ShowFirstTime", None),
-		"ShowSampleFreq": (1745027152, 2, (11, 0), (), "ShowSampleFreq", None),
-		"ShowServer": (1745027150, 2, (11, 0), (), "ShowServer", None),
-		"ShowSize": (1745027147, 2, (11, 0), (), "ShowSize", None),
-		"ShowStrbOff": (1745027184, 2, (11, 0), (), "ShowStrbOff", None),
-		"ShowTank": (1745027149, 2, (11, 0), (), "ShowTank", None),
-		"ShowType": (1745027154, 2, (11, 0), (), "ShowType", None),
-		"SingleClickSelect": (1745027144, 2, (11, 0), (), "SingleClickSelect", None),
-		"UseBlock": (1745027155, 2, (8, 0), (), "UseBlock", None),
-		"UseServer": (1745027157, 2, (8, 0), (), "UseServer", None),
-		"UseTank": (1745027156, 2, (8, 0), (), "UseTank", None),
-	}
-	_prop_map_put_ = {
-		"ActiveEvent": ((1745027145, LCID, 4, 0),()),
-		"AllowActive": ((1745027143, LCID, 4, 0),()),
-		"AllowDragDrop": ((1745027142, LCID, 4, 0),()),
-		"HideDetails": ((1745027158, LCID, 4, 0),()),
-		"ShowBlock": ((1745027148, LCID, 4, 0),()),
-		"ShowChecks": ((1745027146, LCID, 4, 0),()),
-		"ShowDataFormat": ((1745027153, LCID, 4, 0),()),
-		"ShowDefaultEvent": ((1745027183, LCID, 4, 0),()),
-		"ShowFirstTime": ((1745027151, LCID, 4, 0),()),
-		"ShowSampleFreq": ((1745027152, LCID, 4, 0),()),
-		"ShowServer": ((1745027150, LCID, 4, 0),()),
-		"ShowSize": ((1745027147, LCID, 4, 0),()),
-		"ShowStrbOff": ((1745027184, LCID, 4, 0),()),
-		"ShowTank": ((1745027149, LCID, 4, 0),()),
-		"ShowType": ((1745027154, LCID, 4, 0),()),
-		"SingleClickSelect": ((1745027144, LCID, 4, 0),()),
-		"UseBlock": ((1745027155, LCID, 4, 0),()),
-		"UseServer": ((1745027157, LCID, 4, 0),()),
-		"UseTank": ((1745027156, LCID, 4, 0),()),
-	}
-
-class _ServSelProps(DispatchBaseClass):
-	CLSID = IID('{91124062-FA58-4A43-962A-A3E90676DEC0}')
-	coclass_clsid = IID('{42EDA46E-842E-4131-9C40-1E47D6B8ABB1}')
-
-	_prop_map_get_ = {
-	}
-	_prop_map_put_ = {
-	}
-
-class _ServerSelect(DispatchBaseClass):
-	CLSID = IID('{7BE3D05E-A964-4EF6-A8E6-1E07AB181A98}')
-	coclass_clsid = IID('{A16140DD-AAA9-46C3-9565-6F1E8815D90A}')
-
-	def AddServer(self, ServName=defaultNamedNotOptArg, IPAddr=defaultNamedNotOptArg, Username=defaultNamedNotOptArg, Domain=defaultNamedNotOptArg
-			, Password=defaultNamedNotOptArg):
-		return self._ApplyTypes_(1610809405, 1, (11, 0), ((16392, 3), (16392, 3), (16392, 3), (16392, 3), (16392, 3)), u'AddServer', None,ServName
-			, IPAddr, Username, Domain, Password)
-
-	def DeleteServer(self, ServerName=defaultNamedNotOptArg):
-		return self._ApplyTypes_(1610809407, 1, (11, 0), ((16392, 3),), u'DeleteServer', None,ServerName
-			)
-
-	def ModifyServer(self, ServName=defaultNamedNotOptArg, IPAddr=defaultNamedNotOptArg, Username=defaultNamedNotOptArg, Domain=defaultNamedNotOptArg
-			, Password=defaultNamedNotOptArg):
-		return self._ApplyTypes_(1610809406, 1, (11, 0), ((16392, 3), (16392, 3), (16392, 3), (16392, 3), (16392, 3)), u'ModifyServer', None,ServName
-			, IPAddr, Username, Domain, Password)
-
-	def Refresh(self):
-		return self._oleobj_.InvokeTypes(1610809419, LCID, 1, (24, 0), (),)
-
-	_prop_map_get_ = {
-		"ActiveServer": (1745027118, 2, (8, 0), (), "ActiveServer", None),
-		"AllowDragDrop": (1745027148, 2, (11, 0), (), "AllowDragDrop", None),
-		"AllowEdit": (1745027119, 2, (11, 0), (), "AllowEdit", None),
-		"HideDetails": (1745027136, 2, (11, 0), (), "HideDetails", None),
-	}
-	_prop_map_put_ = {
-		"ActiveServer": ((1745027118, LCID, 4, 0),()),
-		"AllowDragDrop": ((1745027148, LCID, 4, 0),()),
-		"AllowEdit": ((1745027119, LCID, 4, 0),()),
-		"HideDetails": ((1745027136, LCID, 4, 0),()),
-	}
-
-class _TankSelect(DispatchBaseClass):
-	CLSID = IID('{2303C7E3-BC00-4B81-A550-D258167DC1C0}')
-	coclass_clsid = IID('{6BCC8D27-0166-441E-9441-8F55DB2779FB}')
-
-	def AddTank(self, path=defaultNamedNotOptArg, name=defaultNamedNotOptArg, quite=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(1610809446, LCID, 1, (11, 0), ((8, 1), (8, 1), (11, 1)),path
-			, name, quite)
-
-	def Refresh(self):
-		return self._oleobj_.InvokeTypes(1610809417, LCID, 1, (24, 0), (),)
-
-	_prop_map_get_ = {
-		"ActiveTank": (1745027119, 2, (8, 0), (), "ActiveTank", None),
-		"AllowDragDrop": (1745027146, 2, (11, 0), (), "AllowDragDrop", None),
-		"AllowPopup": (1745027124, 2, (11, 0), (), "AllowPopup", None),
-		"FileDialogInitPath": (1745027149, 2, (8, 0), (), "FileDialogInitPath", None),
-		"HideDetails": (1745027121, 2, (11, 0), (), "HideDetails", None),
-		"ShowOnlyPathString": (1745027147, 2, (8, 0), (), "ShowOnlyPathString", None),
-		"ShowServer": (1745027122, 2, (11, 0), (), "ShowServer", None),
-		"ShowSpecPathOnly": (1745027148, 2, (11, 0), (), "ShowSpecPathOnly", None),
-		"ShowTankNew": (1745027175, 2, (11, 0), (), "ShowTankNew", None),
-		"SingleClickSelect": (1745027120, 2, (11, 0), (), "SingleClickSelect", None),
-		"UseServer": (1745027123, 2, (8, 0), (), "UseServer", None),
-	}
-	_prop_map_put_ = {
-		"ActiveTank": ((1745027119, LCID, 4, 0),()),
-		"AllowDragDrop": ((1745027146, LCID, 4, 0),()),
-		"AllowPopup": ((1745027124, LCID, 4, 0),()),
-		"FileDialogInitPath": ((1745027149, LCID, 4, 0),()),
-		"HideDetails": ((1745027121, LCID, 4, 0),()),
-		"ShowOnlyPathString": ((1745027147, LCID, 4, 0),()),
-		"ShowServer": ((1745027122, LCID, 4, 0),()),
-		"ShowSpecPathOnly": ((1745027148, LCID, 4, 0),()),
-		"ShowTankNew": ((1745027175, LCID, 4, 0),()),
-		"SingleClickSelect": ((1745027120, LCID, 4, 0),()),
-		"UseServer": ((1745027123, LCID, 4, 0),()),
-	}
-
-class _BlockSelect_:
-	CLSID = CLSID_Sink = IID('{DC769221-9AD4-4CCD-B51A-FEC47ED63458}')
-	coclass_clsid = IID('{CB81F5AF-7625-4F83-B629-54C37B55A203}')
-	_public_methods_ = [] # For COM Server support
-	_dispid_to_func_ = {
-		        2 : "OnBeginDrag",
-		        1 : "OnBlockChanged",
-		}
-
-	def __init__(self, oobj = None):
-		if oobj is None:
-			self._olecp = None
-		else:
-			import win32com.server.util
-			from win32com.server.policy import EventHandlerPolicy
-			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
-			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
-			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
-			self._olecp,self._olecp_cookie = cp,cookie
-	def __del__(self):
-		try:
-			self.close()
-		except pythoncom.com_error:
-			pass
-	def close(self):
-		if self._olecp is not None:
-			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
-			cp.Unadvise(cookie)
-	def _query_interface_(self, iid):
-		import win32com.server.util
-		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
-
-	# Event Handlers
-	# If you create handlers, they should have the following prototypes:
-#	def OnBeginDrag(self, TDD=defaultNamedNotOptArg):
-#	def OnBlockChanged(self, ActBlock=defaultNamedNotOptArg, ActTank=defaultNamedNotOptArg, ActServer=defaultNamedNotOptArg):
-
-
-class _EventSelect_:
-	CLSID = CLSID_Sink = IID('{3F098EDA-4EFB-4923-9613-373BF08B3F5C}')
-	coclass_clsid = IID('{01B10737-93FA-4FB2-B1F1-0C59793EBCAA}')
-	_public_methods_ = [] # For COM Server support
-	_dispid_to_func_ = {
-		        2 : "OnBeginDrag",
-		        3 : "OnChangeCheck",
-		        5 : "OnEventDblClicked",
-		        4 : "OnEventClicked",
-		        1 : "OnActEventChanged",
-		}
-
-	def __init__(self, oobj = None):
-		if oobj is None:
-			self._olecp = None
-		else:
-			import win32com.server.util
-			from win32com.server.policy import EventHandlerPolicy
-			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
-			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
-			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
-			self._olecp,self._olecp_cookie = cp,cookie
-	def __del__(self):
-		try:
-			self.close()
-		except pythoncom.com_error:
-			pass
-	def close(self):
-		if self._olecp is not None:
-			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
-			cp.Unadvise(cookie)
-	def _query_interface_(self, iid):
-		import win32com.server.util
-		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
-
-	# Event Handlers
-	# If you create handlers, they should have the following prototypes:
-#	def OnBeginDrag(self, TDD=defaultNamedNotOptArg):
-#	def OnChangeCheck(self, EvName=defaultNamedNotOptArg):
-#	def OnEventDblClicked(self, EvName=defaultNamedNotOptArg):
-#	def OnEventClicked(self, EvName=defaultNamedNotOptArg):
-#	def OnActEventChanged(self, NewActEvent=defaultNamedNotOptArg):
-
-
-class _ServerSelect_:
-	CLSID = CLSID_Sink = IID('{75CA8D1D-4078-4EA7-8EC2-E2198C9CFA52}')
-	coclass_clsid = IID('{A16140DD-AAA9-46C3-9565-6F1E8815D90A}')
-	_public_methods_ = [] # For COM Server support
-	_dispid_to_func_ = {
-		        1 : "OnServerChanged",
-		}
-
-	def __init__(self, oobj = None):
-		if oobj is None:
-			self._olecp = None
-		else:
-			import win32com.server.util
-			from win32com.server.policy import EventHandlerPolicy
-			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
-			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
-			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
-			self._olecp,self._olecp_cookie = cp,cookie
-	def __del__(self):
-		try:
-			self.close()
-		except pythoncom.com_error:
-			pass
-	def close(self):
-		if self._olecp is not None:
-			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
-			cp.Unadvise(cookie)
-	def _query_interface_(self, iid):
-		import win32com.server.util
-		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
-
-	# Event Handlers
-	# If you create handlers, they should have the following prototypes:
-#	def OnServerChanged(self, NewServer=defaultNamedNotOptArg):
-
-
-class _TankSelect_:
-	CLSID = CLSID_Sink = IID('{58277ACF-7979-45F9-BBE7-0FB5D6B416F4}')
-	coclass_clsid = IID('{6BCC8D27-0166-441E-9441-8F55DB2779FB}')
-	_public_methods_ = [] # For COM Server support
-	_dispid_to_func_ = {
-		        1 : "OnTankChanged",
-		}
-
-	def __init__(self, oobj = None):
-		if oobj is None:
-			self._olecp = None
-		else:
-			import win32com.server.util
-			from win32com.server.policy import EventHandlerPolicy
-			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
-			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
-			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
-			self._olecp,self._olecp_cookie = cp,cookie
-	def __del__(self):
-		try:
-			self.close()
-		except pythoncom.com_error:
-			pass
-	def close(self):
-		if self._olecp is not None:
-			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
-			cp.Unadvise(cookie)
-	def _query_interface_(self, iid):
-		import win32com.server.util
-		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
-
-	# Event Handlers
-	# If you create handlers, they should have the following prototypes:
-#	def OnTankChanged(self, ActTank=defaultNamedNotOptArg, ActServer=defaultNamedNotOptArg):
-
-
-from win32com.client import CoClassBaseClass
-# This CoClass is known by the name 'TTankInterfaces.BlockSelect'
-class BlockSelect(CoClassBaseClass): # A CoClass
-	CLSID = IID('{CB81F5AF-7625-4F83-B629-54C37B55A203}')
-	coclass_sources = [
-		_BlockSelect_,
-	]
-	default_source = _BlockSelect_
-	coclass_interfaces = [
-		_BlockSelect,
-	]
-	default_interface = _BlockSelect
-
-# This CoClass is known by the name 'TTankInterfaces.EventSelect'
-class EventSelect(CoClassBaseClass): # A CoClass
-	CLSID = IID('{01B10737-93FA-4FB2-B1F1-0C59793EBCAA}')
-	coclass_sources = [
-		_EventSelect_,
-	]
-	default_source = _EventSelect_
-	coclass_interfaces = [
-		_EventSelect,
-	]
-	default_interface = _EventSelect
-
-class ServSelProps(CoClassBaseClass): # A CoClass
-	CLSID = IID('{42EDA46E-842E-4131-9C40-1E47D6B8ABB1}')
-	coclass_sources = [
-	]
-	coclass_interfaces = [
-		_ServSelProps,
-	]
-	default_interface = _ServSelProps
-
-# This CoClass is known by the name 'TTankInterfaces.ServerSelect'
-class ServerSelect(CoClassBaseClass): # A CoClass
-	CLSID = IID('{A16140DD-AAA9-46C3-9565-6F1E8815D90A}')
-	coclass_sources = [
-		_ServerSelect_,
-	]
-	default_source = _ServerSelect_
-	coclass_interfaces = [
-		_ServerSelect,
-	]
-	default_interface = _ServerSelect
-
-# This CoClass is known by the name 'TTankInterfaces.TankSelect'
-class TankSelect(CoClassBaseClass): # A CoClass
-	CLSID = IID('{6BCC8D27-0166-441E-9441-8F55DB2779FB}')
-	coclass_sources = [
-		_TankSelect_,
-	]
-	default_source = _TankSelect_
-	coclass_interfaces = [
-		_TankSelect,
-	]
-	default_interface = _TankSelect
-
-_BlockSelect_vtables_dispatch_ = 1
-_BlockSelect_vtables_ = [
-	(( u'Refresh' , ), 1610809385, (1610809385, (), [ ], 1 , 1 , 4 , 0 , 1956 , (3, 0, None, None) , 0 , )),
-	(( u'UseServer' , None , ), 1745027112, (1745027112, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1960 , (3, 0, None, None) , 0 , )),
-	(( u'UseServer' , None , ), 1745027112, (1745027112, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1964 , (3, 0, None, None) , 0 , )),
-	(( u'UseTank' , None , ), 1745027111, (1745027111, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1968 , (3, 0, None, None) , 0 , )),
-	(( u'UseTank' , None , ), 1745027111, (1745027111, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1972 , (3, 0, None, None) , 0 , )),
-	(( u'HideDetails' , None , ), 1745027110, (1745027110, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1976 , (3, 0, None, None) , 0 , )),
-	(( u'HideDetails' , None , ), 1745027110, (1745027110, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1980 , (3, 0, None, None) , 0 , )),
-	(( u'ActiveBlock' , None , ), 1745027109, (1745027109, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1984 , (3, 0, None, None) , 0 , )),
-	(( u'ActiveBlock' , None , ), 1745027109, (1745027109, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1988 , (3, 0, None, None) , 0 , )),
-	(( u'ShowServer' , None , ), 1745027108, (1745027108, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1992 , (3, 0, None, None) , 0 , )),
-	(( u'ShowServer' , None , ), 1745027108, (1745027108, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1996 , (3, 0, None, None) , 0 , )),
-	(( u'ShowTank' , None , ), 1745027107, (1745027107, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2000 , (3, 0, None, None) , 0 , )),
-	(( u'ShowTank' , None , ), 1745027107, (1745027107, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2004 , (3, 0, None, None) , 0 , )),
-	(( u'ShowDate' , None , ), 1745027106, (1745027106, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2008 , (3, 0, None, None) , 0 , )),
-	(( u'ShowDate' , None , ), 1745027106, (1745027106, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2012 , (3, 0, None, None) , 0 , )),
-	(( u'ShowStart' , None , ), 1745027105, (1745027105, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2016 , (3, 0, None, None) , 0 , )),
-	(( u'ShowStart' , None , ), 1745027105, (1745027105, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2020 , (3, 0, None, None) , 0 , )),
-	(( u'ShowStop' , None , ), 1745027104, (1745027104, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2024 , (3, 0, None, None) , 0 , )),
-	(( u'ShowStop' , None , ), 1745027104, (1745027104, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2028 , (3, 0, None, None) , 0 , )),
-	(( u'ShowDuration' , None , ), 1745027103, (1745027103, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2032 , (3, 0, None, None) , 0 , )),
-	(( u'ShowDuration' , None , ), 1745027103, (1745027103, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2036 , (3, 0, None, None) , 0 , )),
-	(( u'ShowOwner' , None , ), 1745027102, (1745027102, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2040 , (3, 0, None, None) , 0 , )),
-	(( u'ShowOwner' , None , ), 1745027102, (1745027102, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2044 , (3, 0, None, None) , 0 , )),
-	(( u'ShowMemo' , None , ), 1745027101, (1745027101, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2048 , (3, 0, None, None) , 0 , )),
-	(( u'ShowMemo' , None , ), 1745027101, (1745027101, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2052 , (3, 0, None, None) , 0 , )),
-	(( u'SingleClickSelect' , None , ), 1745027100, (1745027100, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2056 , (3, 0, None, None) , 0 , )),
-	(( u'SingleClickSelect' , None , ), 1745027100, (1745027100, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2060 , (3, 0, None, None) , 0 , )),
-	(( u'AllowDragDrop' , None , ), 1745027114, (1745027114, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2064 , (3, 0, None, None) , 0 , )),
-	(( u'AllowDragDrop' , None , ), 1745027114, (1745027114, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2068 , (3, 0, None, None) , 0 , )),
-	(( u'AllowPopup' , None , ), 1745027115, (1745027115, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2072 , (3, 0, None, None) , 0 , )),
-	(( u'AllowPopup' , None , ), 1745027115, (1745027115, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2076 , (3, 0, None, None) , 0 , )),
-]
-
-_EventSelect_vtables_dispatch_ = 1
-_EventSelect_vtables_ = [
-	(( u'HideDetails' , None , ), 1745027158, (1745027158, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1956 , (3, 0, None, None) , 0 , )),
-	(( u'HideDetails' , None , ), 1745027158, (1745027158, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1960 , (3, 0, None, None) , 0 , )),
-	(( u'UseServer' , None , ), 1745027157, (1745027157, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1964 , (3, 0, None, None) , 0 , )),
-	(( u'UseServer' , None , ), 1745027157, (1745027157, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1968 , (3, 0, None, None) , 0 , )),
-	(( u'UseTank' , None , ), 1745027156, (1745027156, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1972 , (3, 0, None, None) , 0 , )),
-	(( u'UseTank' , None , ), 1745027156, (1745027156, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1976 , (3, 0, None, None) , 0 , )),
-	(( u'UseBlock' , None , ), 1745027155, (1745027155, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1980 , (3, 0, None, None) , 0 , )),
-	(( u'UseBlock' , None , ), 1745027155, (1745027155, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1984 , (3, 0, None, None) , 0 , )),
-	(( u'Refresh' , ), 1610809449, (1610809449, (), [ ], 1 , 1 , 4 , 0 , 1988 , (3, 0, None, None) , 0 , )),
-	(( u'ShowType' , None , ), 1745027154, (1745027154, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1992 , (3, 0, None, None) , 0 , )),
-	(( u'ShowType' , None , ), 1745027154, (1745027154, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1996 , (3, 0, None, None) , 0 , )),
-	(( u'ShowDataFormat' , None , ), 1745027153, (1745027153, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2000 , (3, 0, None, None) , 0 , )),
-	(( u'ShowDataFormat' , None , ), 1745027153, (1745027153, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2004 , (3, 0, None, None) , 0 , )),
-	(( u'ShowSampleFreq' , None , ), 1745027152, (1745027152, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2008 , (3, 0, None, None) , 0 , )),
-	(( u'ShowSampleFreq' , None , ), 1745027152, (1745027152, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2012 , (3, 0, None, None) , 0 , )),
-	(( u'ShowFirstTime' , None , ), 1745027151, (1745027151, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2016 , (3, 0, None, None) , 0 , )),
-	(( u'ShowFirstTime' , None , ), 1745027151, (1745027151, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2020 , (3, 0, None, None) , 0 , )),
-	(( u'ShowServer' , None , ), 1745027150, (1745027150, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2024 , (3, 0, None, None) , 0 , )),
-	(( u'ShowServer' , None , ), 1745027150, (1745027150, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2028 , (3, 0, None, None) , 0 , )),
-	(( u'ShowTank' , None , ), 1745027149, (1745027149, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2032 , (3, 0, None, None) , 0 , )),
-	(( u'ShowTank' , None , ), 1745027149, (1745027149, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2036 , (3, 0, None, None) , 0 , )),
-	(( u'ShowBlock' , None , ), 1745027148, (1745027148, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2040 , (3, 0, None, None) , 0 , )),
-	(( u'ShowBlock' , None , ), 1745027148, (1745027148, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2044 , (3, 0, None, None) , 0 , )),
-	(( u'ShowSize' , None , ), 1745027147, (1745027147, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2048 , (3, 0, None, None) , 0 , )),
-	(( u'ShowSize' , None , ), 1745027147, (1745027147, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2052 , (3, 0, None, None) , 0 , )),
-	(( u'ShowChecks' , None , ), 1745027146, (1745027146, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2056 , (3, 0, None, None) , 0 , )),
-	(( u'ShowChecks' , None , ), 1745027146, (1745027146, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2060 , (3, 0, None, None) , 0 , )),
-	(( u'GetChecked' , u'EvName' , None , ), 1610809451, (1610809451, (), [ (8, 1, None, None) , 
-			(16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 2064 , (3, 0, None, None) , 0 , )),
-	(( u'SetChecked' , u'EvName' , u'CheckState' , ), 1610809452, (1610809452, (), [ (8, 1, None, None) , 
-			(16395, 3, None, None) , ], 1 , 1 , 4 , 0 , 2068 , (3, 0, None, None) , 0 , )),
-	(( u'GetEvName' , u'Index' , None , ), 1610809453, (1610809453, (), [ (16387, 3, None, None) , 
-			(16392, 10, None, None) , ], 1 , 1 , 4 , 0 , 2072 , (3, 0, None, None) , 0 , )),
-	(( u'ClearChecks' , u'CheckState' , ), 1610809454, (1610809454, (), [ (16395, 3, None, None) , ], 1 , 1 , 4 , 0 , 2076 , (3, 0, None, None) , 0 , )),
-	(( u'ActiveEvent' , None , ), 1745027145, (1745027145, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 2080 , (3, 0, None, None) , 0 , )),
-	(( u'ActiveEvent' , None , ), 1745027145, (1745027145, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 2084 , (3, 0, None, None) , 0 , )),
-	(( u'SingleClickSelect' , None , ), 1745027144, (1745027144, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2088 , (3, 0, None, None) , 0 , )),
-	(( u'SingleClickSelect' , None , ), 1745027144, (1745027144, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2092 , (3, 0, None, None) , 0 , )),
-	(( u'AllowActive' , None , ), 1745027143, (1745027143, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2096 , (3, 0, None, None) , 0 , )),
-	(( u'AllowActive' , None , ), 1745027143, (1745027143, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2100 , (3, 0, None, None) , 0 , )),
-	(( u'AllowDragDrop' , None , ), 1745027142, (1745027142, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2104 , (3, 0, None, None) , 0 , )),
-	(( u'AllowDragDrop' , None , ), 1745027142, (1745027142, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2108 , (3, 0, None, None) , 0 , )),
-	(( u'ShowDefaultEvent' , None , ), 1745027183, (1745027183, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2112 , (3, 0, None, None) , 0 , )),
-	(( u'ShowDefaultEvent' , None , ), 1745027183, (1745027183, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2116 , (3, 0, None, None) , 0 , )),
-	(( u'ShowStrbOff' , None , ), 1745027184, (1745027184, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2120 , (3, 0, None, None) , 0 , )),
-	(( u'ShowStrbOff' , None , ), 1745027184, (1745027184, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2124 , (3, 0, None, None) , 0 , )),
-]
-
-_ServSelProps_vtables_dispatch_ = 1
-_ServSelProps_vtables_ = [
-]
-
-_ServerSelect_vtables_dispatch_ = 1
-_ServerSelect_vtables_ = [
-	(( u'AllowEdit' , None , ), 1745027119, (1745027119, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1956 , (3, 0, None, None) , 0 , )),
-	(( u'AllowEdit' , None , ), 1745027119, (1745027119, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1960 , (3, 0, None, None) , 0 , )),
-	(( u'AddServer' , u'ServName' , u'IPAddr' , u'Username' , u'Domain' , 
-			u'Password' , None , ), 1610809405, (1610809405, (), [ (16392, 3, None, None) , (16392, 3, None, None) , 
-			(16392, 3, None, None) , (16392, 3, None, None) , (16392, 3, None, None) , (16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 1964 , (3, 0, None, None) , 0 , )),
-	(( u'ModifyServer' , u'ServName' , u'IPAddr' , u'Username' , u'Domain' , 
-			u'Password' , None , ), 1610809406, (1610809406, (), [ (16392, 3, None, None) , (16392, 3, None, None) , 
-			(16392, 3, None, None) , (16392, 3, None, None) , (16392, 3, None, None) , (16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 1968 , (3, 0, None, None) , 0 , )),
-	(( u'DeleteServer' , u'ServerName' , None , ), 1610809407, (1610809407, (), [ (16392, 3, None, None) , 
-			(16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 1972 , (3, 0, None, None) , 0 , )),
-	(( u'ActiveServer' , None , ), 1745027118, (1745027118, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1976 , (3, 0, None, None) , 0 , )),
-	(( u'ActiveServer' , None , ), 1745027118, (1745027118, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1980 , (3, 0, None, None) , 0 , )),
-	(( u'HideDetails' , None , ), 1745027136, (1745027136, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1984 , (3, 0, None, None) , 0 , )),
-	(( u'HideDetails' , None , ), 1745027136, (1745027136, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1988 , (3, 0, None, None) , 0 , )),
-	(( u'Refresh' , ), 1610809419, (1610809419, (), [ ], 1 , 1 , 4 , 0 , 1992 , (3, 0, None, None) , 0 , )),
-	(( u'AllowDragDrop' , None , ), 1745027148, (1745027148, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1996 , (3, 0, None, None) , 0 , )),
-	(( u'AllowDragDrop' , None , ), 1745027148, (1745027148, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2000 , (3, 0, None, None) , 0 , )),
-]
-
-_TankSelect_vtables_dispatch_ = 1
-_TankSelect_vtables_ = [
-	(( u'Refresh' , ), 1610809417, (1610809417, (), [ ], 1 , 1 , 4 , 0 , 1956 , (3, 0, None, None) , 0 , )),
-	(( u'AllowPopup' , None , ), 1745027124, (1745027124, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1960 , (3, 0, None, None) , 0 , )),
-	(( u'AllowPopup' , None , ), 1745027124, (1745027124, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1964 , (3, 0, None, None) , 0 , )),
-	(( u'UseServer' , None , ), 1745027123, (1745027123, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1968 , (3, 0, None, None) , 0 , )),
-	(( u'UseServer' , None , ), 1745027123, (1745027123, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1972 , (3, 0, None, None) , 0 , )),
-	(( u'ShowServer' , None , ), 1745027122, (1745027122, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1976 , (3, 0, None, None) , 0 , )),
-	(( u'ShowServer' , None , ), 1745027122, (1745027122, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1980 , (3, 0, None, None) , 0 , )),
-	(( u'HideDetails' , None , ), 1745027121, (1745027121, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1984 , (3, 0, None, None) , 0 , )),
-	(( u'HideDetails' , None , ), 1745027121, (1745027121, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1988 , (3, 0, None, None) , 0 , )),
-	(( u'SingleClickSelect' , None , ), 1745027120, (1745027120, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1992 , (3, 0, None, None) , 0 , )),
-	(( u'SingleClickSelect' , None , ), 1745027120, (1745027120, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1996 , (3, 0, None, None) , 0 , )),
-	(( u'ActiveTank' , None , ), 1745027119, (1745027119, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 2000 , (3, 0, None, None) , 0 , )),
-	(( u'ActiveTank' , None , ), 1745027119, (1745027119, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 2004 , (3, 0, None, None) , 0 , )),
-	(( u'AllowDragDrop' , None , ), 1745027146, (1745027146, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2008 , (3, 0, None, None) , 0 , )),
-	(( u'AllowDragDrop' , None , ), 1745027146, (1745027146, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2012 , (3, 0, None, None) , 0 , )),
-	(( u'ShowOnlyPathString' , None , ), 1745027147, (1745027147, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 2016 , (3, 0, None, None) , 0 , )),
-	(( u'ShowOnlyPathString' , None , ), 1745027147, (1745027147, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 2020 , (3, 0, None, None) , 0 , )),
-	(( u'ShowSpecPathOnly' , None , ), 1745027148, (1745027148, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2024 , (3, 0, None, None) , 0 , )),
-	(( u'ShowSpecPathOnly' , None , ), 1745027148, (1745027148, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2028 , (3, 0, None, None) , 0 , )),
-	(( u'FileDialogInitPath' , None , ), 1745027149, (1745027149, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 2032 , (3, 0, None, None) , 0 , )),
-	(( u'FileDialogInitPath' , None , ), 1745027149, (1745027149, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 2036 , (3, 0, None, None) , 0 , )),
-	(( u'AddTank' , u'path' , u'name' , u'quite' , None , 
-			), 1610809446, (1610809446, (), [ (8, 1, None, None) , (8, 1, None, None) , (11, 1, None, None) , (16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 2040 , (3, 0, None, None) , 0 , )),
-	(( u'ShowTankNew' , None , ), 1745027175, (1745027175, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2044 , (3, 0, None, None) , 0 , )),
-	(( u'ShowTankNew' , None , ), 1745027175, (1745027175, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2048 , (3, 0, None, None) , 0 , )),
-]
-
-RecordMap = {
-	u'TankInfo': '{A3EA7E81-5BF7-4FE4-9659-D797A6DD6A13}',
-}
-
-CLSIDToClassMap = {
-	'{A16140DD-AAA9-46C3-9565-6F1E8815D90A}' : ServerSelect,
-	'{C2F42E9B-86B7-4F21-889D-8B854B019640}' : _BlockSelect,
-	'{DC769221-9AD4-4CCD-B51A-FEC47ED63458}' : _BlockSelect_,
-	'{01B10737-93FA-4FB2-B1F1-0C59793EBCAA}' : EventSelect,
-	'{42EDA46E-842E-4131-9C40-1E47D6B8ABB1}' : ServSelProps,
-	'{75CA8D1D-4078-4EA7-8EC2-E2198C9CFA52}' : _ServerSelect_,
-	'{CBA421AC-7EB7-40BA-AA2C-81CC652B2EEF}' : _EventSelect,
-	'{7BE3D05E-A964-4EF6-A8E6-1E07AB181A98}' : _ServerSelect,
-	'{91124062-FA58-4A43-962A-A3E90676DEC0}' : _ServSelProps,
-	'{58277ACF-7979-45F9-BBE7-0FB5D6B416F4}' : _TankSelect_,
-	'{3F098EDA-4EFB-4923-9613-373BF08B3F5C}' : _EventSelect_,
-	'{6BCC8D27-0166-441E-9441-8F55DB2779FB}' : TankSelect,
-	'{2303C7E3-BC00-4B81-A550-D258167DC1C0}' : _TankSelect,
-	'{CB81F5AF-7625-4F83-B629-54C37B55A203}' : BlockSelect,
-}
-CLSIDToPackageMap = {}
-win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
-VTablesToPackageMap = {}
-VTablesToClassMap = {
-	'{CBA421AC-7EB7-40BA-AA2C-81CC652B2EEF}' : '_EventSelect',
-	'{91124062-FA58-4A43-962A-A3E90676DEC0}' : '_ServSelProps',
-	'{7BE3D05E-A964-4EF6-A8E6-1E07AB181A98}' : '_ServerSelect',
-	'{2303C7E3-BC00-4B81-A550-D258167DC1C0}' : '_TankSelect',
-	'{C2F42E9B-86B7-4F21-889D-8B854B019640}' : '_BlockSelect',
-}
-
-
-NamesToIIDMap = {
-	'_BlockSelect_' : '{DC769221-9AD4-4CCD-B51A-FEC47ED63458}',
-	'_EventSelect' : '{CBA421AC-7EB7-40BA-AA2C-81CC652B2EEF}',
-	'_BlockSelect' : '{C2F42E9B-86B7-4F21-889D-8B854B019640}',
-	'_ServSelProps' : '{91124062-FA58-4A43-962A-A3E90676DEC0}',
-	'_ServerSelect_' : '{75CA8D1D-4078-4EA7-8EC2-E2198C9CFA52}',
-	'_EventSelect_' : '{3F098EDA-4EFB-4923-9613-373BF08B3F5C}',
-	'_TankSelect' : '{2303C7E3-BC00-4B81-A550-D258167DC1C0}',
-	'_ServerSelect' : '{7BE3D05E-A964-4EF6-A8E6-1E07AB181A98}',
-	'_TankSelect_' : '{58277ACF-7979-45F9-BBE7-0FB5D6B416F4}',
-}
-
-
+# -*- coding: utf-8 -*-
+# Created by makepy.py version 0.5.00
+# By python version 2.6.6 |EPD 6.3-2 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
+# From type library 'TTankInterfaces.ocx'
+# On Thu Dec 02 21:00:50 2010
+"""TTankInterfaces"""
+makepy_version = '0.5.00'
+python_version = 0x20606f0
+
+import win32com.client.CLSIDToClass, pythoncom, pywintypes
+import win32com.client.util
+from pywintypes import IID
+from win32com.client import Dispatch
+
+# The following 3 lines may need tweaking for the particular server
+# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
+defaultNamedOptArg=pythoncom.Empty
+defaultNamedNotOptArg=pythoncom.Empty
+defaultUnnamedArg=pythoncom.Empty
+
+CLSID = IID('{831D8AF7-7E2B-426B-A430-18E670F56C12}')
+MajorVersion = 10
+MinorVersion = 9
+LibraryFlags = 10
+LCID = 0x0
+
+from win32com.client import DispatchBaseClass
+class _BlockSelect(DispatchBaseClass):
+	CLSID = IID('{C2F42E9B-86B7-4F21-889D-8B854B019640}')
+	coclass_clsid = IID('{CB81F5AF-7625-4F83-B629-54C37B55A203}')
+
+	def Refresh(self):
+		return self._oleobj_.InvokeTypes(1610809385, LCID, 1, (24, 0), (),)
+
+	_prop_map_get_ = {
+		"ActiveBlock": (1745027109, 2, (8, 0), (), "ActiveBlock", None),
+		"AllowDragDrop": (1745027114, 2, (11, 0), (), "AllowDragDrop", None),
+		"AllowPopup": (1745027115, 2, (11, 0), (), "AllowPopup", None),
+		"HideDetails": (1745027110, 2, (11, 0), (), "HideDetails", None),
+		"ShowDate": (1745027106, 2, (11, 0), (), "ShowDate", None),
+		"ShowDuration": (1745027103, 2, (11, 0), (), "ShowDuration", None),
+		"ShowMemo": (1745027101, 2, (11, 0), (), "ShowMemo", None),
+		"ShowOwner": (1745027102, 2, (11, 0), (), "ShowOwner", None),
+		"ShowServer": (1745027108, 2, (11, 0), (), "ShowServer", None),
+		"ShowStart": (1745027105, 2, (11, 0), (), "ShowStart", None),
+		"ShowStop": (1745027104, 2, (11, 0), (), "ShowStop", None),
+		"ShowTank": (1745027107, 2, (11, 0), (), "ShowTank", None),
+		"SingleClickSelect": (1745027100, 2, (11, 0), (), "SingleClickSelect", None),
+		"UseServer": (1745027112, 2, (8, 0), (), "UseServer", None),
+		"UseTank": (1745027111, 2, (8, 0), (), "UseTank", None),
+	}
+	_prop_map_put_ = {
+		"ActiveBlock": ((1745027109, LCID, 4, 0),()),
+		"AllowDragDrop": ((1745027114, LCID, 4, 0),()),
+		"AllowPopup": ((1745027115, LCID, 4, 0),()),
+		"HideDetails": ((1745027110, LCID, 4, 0),()),
+		"ShowDate": ((1745027106, LCID, 4, 0),()),
+		"ShowDuration": ((1745027103, LCID, 4, 0),()),
+		"ShowMemo": ((1745027101, LCID, 4, 0),()),
+		"ShowOwner": ((1745027102, LCID, 4, 0),()),
+		"ShowServer": ((1745027108, LCID, 4, 0),()),
+		"ShowStart": ((1745027105, LCID, 4, 0),()),
+		"ShowStop": ((1745027104, LCID, 4, 0),()),
+		"ShowTank": ((1745027107, LCID, 4, 0),()),
+		"SingleClickSelect": ((1745027100, LCID, 4, 0),()),
+		"UseServer": ((1745027112, LCID, 4, 0),()),
+		"UseTank": ((1745027111, LCID, 4, 0),()),
+	}
+
+class _EventSelect(DispatchBaseClass):
+	CLSID = IID('{CBA421AC-7EB7-40BA-AA2C-81CC652B2EEF}')
+	coclass_clsid = IID('{01B10737-93FA-4FB2-B1F1-0C59793EBCAA}')
+
+	def ClearChecks(self, CheckState=defaultNamedNotOptArg):
+		return self._ApplyTypes_(1610809454, 1, (24, 0), ((16395, 3),), u'ClearChecks', None,CheckState
+			)
+
+	def GetChecked(self, EvName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(1610809451, LCID, 1, (11, 0), ((8, 1),),EvName
+			)
+
+	def GetEvName(self, Index=defaultNamedNotOptArg):
+		return self._ApplyTypes_(1610809453, 1, (8, 0), ((16387, 3),), u'GetEvName', None,Index
+			)
+
+	def Refresh(self):
+		return self._oleobj_.InvokeTypes(1610809449, LCID, 1, (24, 0), (),)
+
+	def SetChecked(self, EvName=defaultNamedNotOptArg, CheckState=defaultNamedNotOptArg):
+		return self._ApplyTypes_(1610809452, 1, (24, 0), ((8, 1), (16395, 3)), u'SetChecked', None,EvName
+			, CheckState)
+
+	_prop_map_get_ = {
+		"ActiveEvent": (1745027145, 2, (8, 0), (), "ActiveEvent", None),
+		"AllowActive": (1745027143, 2, (11, 0), (), "AllowActive", None),
+		"AllowDragDrop": (1745027142, 2, (11, 0), (), "AllowDragDrop", None),
+		"HideDetails": (1745027158, 2, (11, 0), (), "HideDetails", None),
+		"ShowBlock": (1745027148, 2, (11, 0), (), "ShowBlock", None),
+		"ShowChecks": (1745027146, 2, (11, 0), (), "ShowChecks", None),
+		"ShowDataFormat": (1745027153, 2, (11, 0), (), "ShowDataFormat", None),
+		"ShowDefaultEvent": (1745027183, 2, (11, 0), (), "ShowDefaultEvent", None),
+		"ShowFirstTime": (1745027151, 2, (11, 0), (), "ShowFirstTime", None),
+		"ShowSampleFreq": (1745027152, 2, (11, 0), (), "ShowSampleFreq", None),
+		"ShowServer": (1745027150, 2, (11, 0), (), "ShowServer", None),
+		"ShowSize": (1745027147, 2, (11, 0), (), "ShowSize", None),
+		"ShowStrbOff": (1745027184, 2, (11, 0), (), "ShowStrbOff", None),
+		"ShowTank": (1745027149, 2, (11, 0), (), "ShowTank", None),
+		"ShowType": (1745027154, 2, (11, 0), (), "ShowType", None),
+		"SingleClickSelect": (1745027144, 2, (11, 0), (), "SingleClickSelect", None),
+		"UseBlock": (1745027155, 2, (8, 0), (), "UseBlock", None),
+		"UseServer": (1745027157, 2, (8, 0), (), "UseServer", None),
+		"UseTank": (1745027156, 2, (8, 0), (), "UseTank", None),
+	}
+	_prop_map_put_ = {
+		"ActiveEvent": ((1745027145, LCID, 4, 0),()),
+		"AllowActive": ((1745027143, LCID, 4, 0),()),
+		"AllowDragDrop": ((1745027142, LCID, 4, 0),()),
+		"HideDetails": ((1745027158, LCID, 4, 0),()),
+		"ShowBlock": ((1745027148, LCID, 4, 0),()),
+		"ShowChecks": ((1745027146, LCID, 4, 0),()),
+		"ShowDataFormat": ((1745027153, LCID, 4, 0),()),
+		"ShowDefaultEvent": ((1745027183, LCID, 4, 0),()),
+		"ShowFirstTime": ((1745027151, LCID, 4, 0),()),
+		"ShowSampleFreq": ((1745027152, LCID, 4, 0),()),
+		"ShowServer": ((1745027150, LCID, 4, 0),()),
+		"ShowSize": ((1745027147, LCID, 4, 0),()),
+		"ShowStrbOff": ((1745027184, LCID, 4, 0),()),
+		"ShowTank": ((1745027149, LCID, 4, 0),()),
+		"ShowType": ((1745027154, LCID, 4, 0),()),
+		"SingleClickSelect": ((1745027144, LCID, 4, 0),()),
+		"UseBlock": ((1745027155, LCID, 4, 0),()),
+		"UseServer": ((1745027157, LCID, 4, 0),()),
+		"UseTank": ((1745027156, LCID, 4, 0),()),
+	}
+
+class _ServSelProps(DispatchBaseClass):
+	CLSID = IID('{91124062-FA58-4A43-962A-A3E90676DEC0}')
+	coclass_clsid = IID('{42EDA46E-842E-4131-9C40-1E47D6B8ABB1}')
+
+	_prop_map_get_ = {
+	}
+	_prop_map_put_ = {
+	}
+
+class _ServerSelect(DispatchBaseClass):
+	CLSID = IID('{7BE3D05E-A964-4EF6-A8E6-1E07AB181A98}')
+	coclass_clsid = IID('{A16140DD-AAA9-46C3-9565-6F1E8815D90A}')
+
+	def AddServer(self, ServName=defaultNamedNotOptArg, IPAddr=defaultNamedNotOptArg, Username=defaultNamedNotOptArg, Domain=defaultNamedNotOptArg
+			, Password=defaultNamedNotOptArg):
+		return self._ApplyTypes_(1610809405, 1, (11, 0), ((16392, 3), (16392, 3), (16392, 3), (16392, 3), (16392, 3)), u'AddServer', None,ServName
+			, IPAddr, Username, Domain, Password)
+
+	def DeleteServer(self, ServerName=defaultNamedNotOptArg):
+		return self._ApplyTypes_(1610809407, 1, (11, 0), ((16392, 3),), u'DeleteServer', None,ServerName
+			)
+
+	def ModifyServer(self, ServName=defaultNamedNotOptArg, IPAddr=defaultNamedNotOptArg, Username=defaultNamedNotOptArg, Domain=defaultNamedNotOptArg
+			, Password=defaultNamedNotOptArg):
+		return self._ApplyTypes_(1610809406, 1, (11, 0), ((16392, 3), (16392, 3), (16392, 3), (16392, 3), (16392, 3)), u'ModifyServer', None,ServName
+			, IPAddr, Username, Domain, Password)
+
+	def Refresh(self):
+		return self._oleobj_.InvokeTypes(1610809419, LCID, 1, (24, 0), (),)
+
+	_prop_map_get_ = {
+		"ActiveServer": (1745027118, 2, (8, 0), (), "ActiveServer", None),
+		"AllowDragDrop": (1745027148, 2, (11, 0), (), "AllowDragDrop", None),
+		"AllowEdit": (1745027119, 2, (11, 0), (), "AllowEdit", None),
+		"HideDetails": (1745027136, 2, (11, 0), (), "HideDetails", None),
+	}
+	_prop_map_put_ = {
+		"ActiveServer": ((1745027118, LCID, 4, 0),()),
+		"AllowDragDrop": ((1745027148, LCID, 4, 0),()),
+		"AllowEdit": ((1745027119, LCID, 4, 0),()),
+		"HideDetails": ((1745027136, LCID, 4, 0),()),
+	}
+
+class _TankSelect(DispatchBaseClass):
+	CLSID = IID('{2303C7E3-BC00-4B81-A550-D258167DC1C0}')
+	coclass_clsid = IID('{6BCC8D27-0166-441E-9441-8F55DB2779FB}')
+
+	def AddTank(self, path=defaultNamedNotOptArg, name=defaultNamedNotOptArg, quite=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(1610809446, LCID, 1, (11, 0), ((8, 1), (8, 1), (11, 1)),path
+			, name, quite)
+
+	def Refresh(self):
+		return self._oleobj_.InvokeTypes(1610809417, LCID, 1, (24, 0), (),)
+
+	_prop_map_get_ = {
+		"ActiveTank": (1745027119, 2, (8, 0), (), "ActiveTank", None),
+		"AllowDragDrop": (1745027146, 2, (11, 0), (), "AllowDragDrop", None),
+		"AllowPopup": (1745027124, 2, (11, 0), (), "AllowPopup", None),
+		"FileDialogInitPath": (1745027149, 2, (8, 0), (), "FileDialogInitPath", None),
+		"HideDetails": (1745027121, 2, (11, 0), (), "HideDetails", None),
+		"ShowOnlyPathString": (1745027147, 2, (8, 0), (), "ShowOnlyPathString", None),
+		"ShowServer": (1745027122, 2, (11, 0), (), "ShowServer", None),
+		"ShowSpecPathOnly": (1745027148, 2, (11, 0), (), "ShowSpecPathOnly", None),
+		"ShowTankNew": (1745027175, 2, (11, 0), (), "ShowTankNew", None),
+		"SingleClickSelect": (1745027120, 2, (11, 0), (), "SingleClickSelect", None),
+		"UseServer": (1745027123, 2, (8, 0), (), "UseServer", None),
+	}
+	_prop_map_put_ = {
+		"ActiveTank": ((1745027119, LCID, 4, 0),()),
+		"AllowDragDrop": ((1745027146, LCID, 4, 0),()),
+		"AllowPopup": ((1745027124, LCID, 4, 0),()),
+		"FileDialogInitPath": ((1745027149, LCID, 4, 0),()),
+		"HideDetails": ((1745027121, LCID, 4, 0),()),
+		"ShowOnlyPathString": ((1745027147, LCID, 4, 0),()),
+		"ShowServer": ((1745027122, LCID, 4, 0),()),
+		"ShowSpecPathOnly": ((1745027148, LCID, 4, 0),()),
+		"ShowTankNew": ((1745027175, LCID, 4, 0),()),
+		"SingleClickSelect": ((1745027120, LCID, 4, 0),()),
+		"UseServer": ((1745027123, LCID, 4, 0),()),
+	}
+
+class _BlockSelect_:
+	CLSID = CLSID_Sink = IID('{DC769221-9AD4-4CCD-B51A-FEC47ED63458}')
+	coclass_clsid = IID('{CB81F5AF-7625-4F83-B629-54C37B55A203}')
+	_public_methods_ = [] # For COM Server support
+	_dispid_to_func_ = {
+		        2 : "OnBeginDrag",
+		        1 : "OnBlockChanged",
+		}
+
+	def __init__(self, oobj = None):
+		if oobj is None:
+			self._olecp = None
+		else:
+			import win32com.server.util
+			from win32com.server.policy import EventHandlerPolicy
+			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
+			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
+			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
+			self._olecp,self._olecp_cookie = cp,cookie
+	def __del__(self):
+		try:
+			self.close()
+		except pythoncom.com_error:
+			pass
+	def close(self):
+		if self._olecp is not None:
+			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
+			cp.Unadvise(cookie)
+	def _query_interface_(self, iid):
+		import win32com.server.util
+		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
+
+	# Event Handlers
+	# If you create handlers, they should have the following prototypes:
+#	def OnBeginDrag(self, TDD=defaultNamedNotOptArg):
+#	def OnBlockChanged(self, ActBlock=defaultNamedNotOptArg, ActTank=defaultNamedNotOptArg, ActServer=defaultNamedNotOptArg):
+
+
+class _EventSelect_:
+	CLSID = CLSID_Sink = IID('{3F098EDA-4EFB-4923-9613-373BF08B3F5C}')
+	coclass_clsid = IID('{01B10737-93FA-4FB2-B1F1-0C59793EBCAA}')
+	_public_methods_ = [] # For COM Server support
+	_dispid_to_func_ = {
+		        2 : "OnBeginDrag",
+		        3 : "OnChangeCheck",
+		        5 : "OnEventDblClicked",
+		        4 : "OnEventClicked",
+		        1 : "OnActEventChanged",
+		}
+
+	def __init__(self, oobj = None):
+		if oobj is None:
+			self._olecp = None
+		else:
+			import win32com.server.util
+			from win32com.server.policy import EventHandlerPolicy
+			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
+			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
+			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
+			self._olecp,self._olecp_cookie = cp,cookie
+	def __del__(self):
+		try:
+			self.close()
+		except pythoncom.com_error:
+			pass
+	def close(self):
+		if self._olecp is not None:
+			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
+			cp.Unadvise(cookie)
+	def _query_interface_(self, iid):
+		import win32com.server.util
+		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
+
+	# Event Handlers
+	# If you create handlers, they should have the following prototypes:
+#	def OnBeginDrag(self, TDD=defaultNamedNotOptArg):
+#	def OnChangeCheck(self, EvName=defaultNamedNotOptArg):
+#	def OnEventDblClicked(self, EvName=defaultNamedNotOptArg):
+#	def OnEventClicked(self, EvName=defaultNamedNotOptArg):
+#	def OnActEventChanged(self, NewActEvent=defaultNamedNotOptArg):
+
+
+class _ServerSelect_:
+	CLSID = CLSID_Sink = IID('{75CA8D1D-4078-4EA7-8EC2-E2198C9CFA52}')
+	coclass_clsid = IID('{A16140DD-AAA9-46C3-9565-6F1E8815D90A}')
+	_public_methods_ = [] # For COM Server support
+	_dispid_to_func_ = {
+		        1 : "OnServerChanged",
+		}
+
+	def __init__(self, oobj = None):
+		if oobj is None:
+			self._olecp = None
+		else:
+			import win32com.server.util
+			from win32com.server.policy import EventHandlerPolicy
+			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
+			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
+			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
+			self._olecp,self._olecp_cookie = cp,cookie
+	def __del__(self):
+		try:
+			self.close()
+		except pythoncom.com_error:
+			pass
+	def close(self):
+		if self._olecp is not None:
+			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
+			cp.Unadvise(cookie)
+	def _query_interface_(self, iid):
+		import win32com.server.util
+		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
+
+	# Event Handlers
+	# If you create handlers, they should have the following prototypes:
+#	def OnServerChanged(self, NewServer=defaultNamedNotOptArg):
+
+
+class _TankSelect_:
+	CLSID = CLSID_Sink = IID('{58277ACF-7979-45F9-BBE7-0FB5D6B416F4}')
+	coclass_clsid = IID('{6BCC8D27-0166-441E-9441-8F55DB2779FB}')
+	_public_methods_ = [] # For COM Server support
+	_dispid_to_func_ = {
+		        1 : "OnTankChanged",
+		}
+
+	def __init__(self, oobj = None):
+		if oobj is None:
+			self._olecp = None
+		else:
+			import win32com.server.util
+			from win32com.server.policy import EventHandlerPolicy
+			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
+			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
+			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
+			self._olecp,self._olecp_cookie = cp,cookie
+	def __del__(self):
+		try:
+			self.close()
+		except pythoncom.com_error:
+			pass
+	def close(self):
+		if self._olecp is not None:
+			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
+			cp.Unadvise(cookie)
+	def _query_interface_(self, iid):
+		import win32com.server.util
+		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
+
+	# Event Handlers
+	# If you create handlers, they should have the following prototypes:
+#	def OnTankChanged(self, ActTank=defaultNamedNotOptArg, ActServer=defaultNamedNotOptArg):
+
+
+from win32com.client import CoClassBaseClass
+# This CoClass is known by the name 'TTankInterfaces.BlockSelect'
+class BlockSelect(CoClassBaseClass): # A CoClass
+	CLSID = IID('{CB81F5AF-7625-4F83-B629-54C37B55A203}')
+	coclass_sources = [
+		_BlockSelect_,
+	]
+	default_source = _BlockSelect_
+	coclass_interfaces = [
+		_BlockSelect,
+	]
+	default_interface = _BlockSelect
+
+# This CoClass is known by the name 'TTankInterfaces.EventSelect'
+class EventSelect(CoClassBaseClass): # A CoClass
+	CLSID = IID('{01B10737-93FA-4FB2-B1F1-0C59793EBCAA}')
+	coclass_sources = [
+		_EventSelect_,
+	]
+	default_source = _EventSelect_
+	coclass_interfaces = [
+		_EventSelect,
+	]
+	default_interface = _EventSelect
+
+class ServSelProps(CoClassBaseClass): # A CoClass
+	CLSID = IID('{42EDA46E-842E-4131-9C40-1E47D6B8ABB1}')
+	coclass_sources = [
+	]
+	coclass_interfaces = [
+		_ServSelProps,
+	]
+	default_interface = _ServSelProps
+
+# This CoClass is known by the name 'TTankInterfaces.ServerSelect'
+class ServerSelect(CoClassBaseClass): # A CoClass
+	CLSID = IID('{A16140DD-AAA9-46C3-9565-6F1E8815D90A}')
+	coclass_sources = [
+		_ServerSelect_,
+	]
+	default_source = _ServerSelect_
+	coclass_interfaces = [
+		_ServerSelect,
+	]
+	default_interface = _ServerSelect
+
+# This CoClass is known by the name 'TTankInterfaces.TankSelect'
+class TankSelect(CoClassBaseClass): # A CoClass
+	CLSID = IID('{6BCC8D27-0166-441E-9441-8F55DB2779FB}')
+	coclass_sources = [
+		_TankSelect_,
+	]
+	default_source = _TankSelect_
+	coclass_interfaces = [
+		_TankSelect,
+	]
+	default_interface = _TankSelect
+
+_BlockSelect_vtables_dispatch_ = 1
+_BlockSelect_vtables_ = [
+	(( u'Refresh' , ), 1610809385, (1610809385, (), [ ], 1 , 1 , 4 , 0 , 1956 , (3, 0, None, None) , 0 , )),
+	(( u'UseServer' , None , ), 1745027112, (1745027112, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1960 , (3, 0, None, None) , 0 , )),
+	(( u'UseServer' , None , ), 1745027112, (1745027112, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1964 , (3, 0, None, None) , 0 , )),
+	(( u'UseTank' , None , ), 1745027111, (1745027111, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1968 , (3, 0, None, None) , 0 , )),
+	(( u'UseTank' , None , ), 1745027111, (1745027111, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1972 , (3, 0, None, None) , 0 , )),
+	(( u'HideDetails' , None , ), 1745027110, (1745027110, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1976 , (3, 0, None, None) , 0 , )),
+	(( u'HideDetails' , None , ), 1745027110, (1745027110, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1980 , (3, 0, None, None) , 0 , )),
+	(( u'ActiveBlock' , None , ), 1745027109, (1745027109, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1984 , (3, 0, None, None) , 0 , )),
+	(( u'ActiveBlock' , None , ), 1745027109, (1745027109, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1988 , (3, 0, None, None) , 0 , )),
+	(( u'ShowServer' , None , ), 1745027108, (1745027108, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1992 , (3, 0, None, None) , 0 , )),
+	(( u'ShowServer' , None , ), 1745027108, (1745027108, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1996 , (3, 0, None, None) , 0 , )),
+	(( u'ShowTank' , None , ), 1745027107, (1745027107, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2000 , (3, 0, None, None) , 0 , )),
+	(( u'ShowTank' , None , ), 1745027107, (1745027107, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2004 , (3, 0, None, None) , 0 , )),
+	(( u'ShowDate' , None , ), 1745027106, (1745027106, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2008 , (3, 0, None, None) , 0 , )),
+	(( u'ShowDate' , None , ), 1745027106, (1745027106, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2012 , (3, 0, None, None) , 0 , )),
+	(( u'ShowStart' , None , ), 1745027105, (1745027105, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2016 , (3, 0, None, None) , 0 , )),
+	(( u'ShowStart' , None , ), 1745027105, (1745027105, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2020 , (3, 0, None, None) , 0 , )),
+	(( u'ShowStop' , None , ), 1745027104, (1745027104, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2024 , (3, 0, None, None) , 0 , )),
+	(( u'ShowStop' , None , ), 1745027104, (1745027104, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2028 , (3, 0, None, None) , 0 , )),
+	(( u'ShowDuration' , None , ), 1745027103, (1745027103, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2032 , (3, 0, None, None) , 0 , )),
+	(( u'ShowDuration' , None , ), 1745027103, (1745027103, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2036 , (3, 0, None, None) , 0 , )),
+	(( u'ShowOwner' , None , ), 1745027102, (1745027102, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2040 , (3, 0, None, None) , 0 , )),
+	(( u'ShowOwner' , None , ), 1745027102, (1745027102, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2044 , (3, 0, None, None) , 0 , )),
+	(( u'ShowMemo' , None , ), 1745027101, (1745027101, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2048 , (3, 0, None, None) , 0 , )),
+	(( u'ShowMemo' , None , ), 1745027101, (1745027101, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2052 , (3, 0, None, None) , 0 , )),
+	(( u'SingleClickSelect' , None , ), 1745027100, (1745027100, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2056 , (3, 0, None, None) , 0 , )),
+	(( u'SingleClickSelect' , None , ), 1745027100, (1745027100, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2060 , (3, 0, None, None) , 0 , )),
+	(( u'AllowDragDrop' , None , ), 1745027114, (1745027114, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2064 , (3, 0, None, None) , 0 , )),
+	(( u'AllowDragDrop' , None , ), 1745027114, (1745027114, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2068 , (3, 0, None, None) , 0 , )),
+	(( u'AllowPopup' , None , ), 1745027115, (1745027115, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2072 , (3, 0, None, None) , 0 , )),
+	(( u'AllowPopup' , None , ), 1745027115, (1745027115, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2076 , (3, 0, None, None) , 0 , )),
+]
+
+_EventSelect_vtables_dispatch_ = 1
+_EventSelect_vtables_ = [
+	(( u'HideDetails' , None , ), 1745027158, (1745027158, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1956 , (3, 0, None, None) , 0 , )),
+	(( u'HideDetails' , None , ), 1745027158, (1745027158, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1960 , (3, 0, None, None) , 0 , )),
+	(( u'UseServer' , None , ), 1745027157, (1745027157, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1964 , (3, 0, None, None) , 0 , )),
+	(( u'UseServer' , None , ), 1745027157, (1745027157, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1968 , (3, 0, None, None) , 0 , )),
+	(( u'UseTank' , None , ), 1745027156, (1745027156, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1972 , (3, 0, None, None) , 0 , )),
+	(( u'UseTank' , None , ), 1745027156, (1745027156, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1976 , (3, 0, None, None) , 0 , )),
+	(( u'UseBlock' , None , ), 1745027155, (1745027155, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1980 , (3, 0, None, None) , 0 , )),
+	(( u'UseBlock' , None , ), 1745027155, (1745027155, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1984 , (3, 0, None, None) , 0 , )),
+	(( u'Refresh' , ), 1610809449, (1610809449, (), [ ], 1 , 1 , 4 , 0 , 1988 , (3, 0, None, None) , 0 , )),
+	(( u'ShowType' , None , ), 1745027154, (1745027154, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1992 , (3, 0, None, None) , 0 , )),
+	(( u'ShowType' , None , ), 1745027154, (1745027154, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1996 , (3, 0, None, None) , 0 , )),
+	(( u'ShowDataFormat' , None , ), 1745027153, (1745027153, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2000 , (3, 0, None, None) , 0 , )),
+	(( u'ShowDataFormat' , None , ), 1745027153, (1745027153, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2004 , (3, 0, None, None) , 0 , )),
+	(( u'ShowSampleFreq' , None , ), 1745027152, (1745027152, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2008 , (3, 0, None, None) , 0 , )),
+	(( u'ShowSampleFreq' , None , ), 1745027152, (1745027152, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2012 , (3, 0, None, None) , 0 , )),
+	(( u'ShowFirstTime' , None , ), 1745027151, (1745027151, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2016 , (3, 0, None, None) , 0 , )),
+	(( u'ShowFirstTime' , None , ), 1745027151, (1745027151, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2020 , (3, 0, None, None) , 0 , )),
+	(( u'ShowServer' , None , ), 1745027150, (1745027150, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2024 , (3, 0, None, None) , 0 , )),
+	(( u'ShowServer' , None , ), 1745027150, (1745027150, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2028 , (3, 0, None, None) , 0 , )),
+	(( u'ShowTank' , None , ), 1745027149, (1745027149, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2032 , (3, 0, None, None) , 0 , )),
+	(( u'ShowTank' , None , ), 1745027149, (1745027149, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2036 , (3, 0, None, None) , 0 , )),
+	(( u'ShowBlock' , None , ), 1745027148, (1745027148, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2040 , (3, 0, None, None) , 0 , )),
+	(( u'ShowBlock' , None , ), 1745027148, (1745027148, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2044 , (3, 0, None, None) , 0 , )),
+	(( u'ShowSize' , None , ), 1745027147, (1745027147, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2048 , (3, 0, None, None) , 0 , )),
+	(( u'ShowSize' , None , ), 1745027147, (1745027147, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2052 , (3, 0, None, None) , 0 , )),
+	(( u'ShowChecks' , None , ), 1745027146, (1745027146, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2056 , (3, 0, None, None) , 0 , )),
+	(( u'ShowChecks' , None , ), 1745027146, (1745027146, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2060 , (3, 0, None, None) , 0 , )),
+	(( u'GetChecked' , u'EvName' , None , ), 1610809451, (1610809451, (), [ (8, 1, None, None) , 
+			(16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 2064 , (3, 0, None, None) , 0 , )),
+	(( u'SetChecked' , u'EvName' , u'CheckState' , ), 1610809452, (1610809452, (), [ (8, 1, None, None) , 
+			(16395, 3, None, None) , ], 1 , 1 , 4 , 0 , 2068 , (3, 0, None, None) , 0 , )),
+	(( u'GetEvName' , u'Index' , None , ), 1610809453, (1610809453, (), [ (16387, 3, None, None) , 
+			(16392, 10, None, None) , ], 1 , 1 , 4 , 0 , 2072 , (3, 0, None, None) , 0 , )),
+	(( u'ClearChecks' , u'CheckState' , ), 1610809454, (1610809454, (), [ (16395, 3, None, None) , ], 1 , 1 , 4 , 0 , 2076 , (3, 0, None, None) , 0 , )),
+	(( u'ActiveEvent' , None , ), 1745027145, (1745027145, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 2080 , (3, 0, None, None) , 0 , )),
+	(( u'ActiveEvent' , None , ), 1745027145, (1745027145, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 2084 , (3, 0, None, None) , 0 , )),
+	(( u'SingleClickSelect' , None , ), 1745027144, (1745027144, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2088 , (3, 0, None, None) , 0 , )),
+	(( u'SingleClickSelect' , None , ), 1745027144, (1745027144, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2092 , (3, 0, None, None) , 0 , )),
+	(( u'AllowActive' , None , ), 1745027143, (1745027143, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2096 , (3, 0, None, None) , 0 , )),
+	(( u'AllowActive' , None , ), 1745027143, (1745027143, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2100 , (3, 0, None, None) , 0 , )),
+	(( u'AllowDragDrop' , None , ), 1745027142, (1745027142, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2104 , (3, 0, None, None) , 0 , )),
+	(( u'AllowDragDrop' , None , ), 1745027142, (1745027142, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2108 , (3, 0, None, None) , 0 , )),
+	(( u'ShowDefaultEvent' , None , ), 1745027183, (1745027183, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2112 , (3, 0, None, None) , 0 , )),
+	(( u'ShowDefaultEvent' , None , ), 1745027183, (1745027183, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2116 , (3, 0, None, None) , 0 , )),
+	(( u'ShowStrbOff' , None , ), 1745027184, (1745027184, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2120 , (3, 0, None, None) , 0 , )),
+	(( u'ShowStrbOff' , None , ), 1745027184, (1745027184, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2124 , (3, 0, None, None) , 0 , )),
+]
+
+_ServSelProps_vtables_dispatch_ = 1
+_ServSelProps_vtables_ = [
+]
+
+_ServerSelect_vtables_dispatch_ = 1
+_ServerSelect_vtables_ = [
+	(( u'AllowEdit' , None , ), 1745027119, (1745027119, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1956 , (3, 0, None, None) , 0 , )),
+	(( u'AllowEdit' , None , ), 1745027119, (1745027119, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1960 , (3, 0, None, None) , 0 , )),
+	(( u'AddServer' , u'ServName' , u'IPAddr' , u'Username' , u'Domain' , 
+			u'Password' , None , ), 1610809405, (1610809405, (), [ (16392, 3, None, None) , (16392, 3, None, None) , 
+			(16392, 3, None, None) , (16392, 3, None, None) , (16392, 3, None, None) , (16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 1964 , (3, 0, None, None) , 0 , )),
+	(( u'ModifyServer' , u'ServName' , u'IPAddr' , u'Username' , u'Domain' , 
+			u'Password' , None , ), 1610809406, (1610809406, (), [ (16392, 3, None, None) , (16392, 3, None, None) , 
+			(16392, 3, None, None) , (16392, 3, None, None) , (16392, 3, None, None) , (16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 1968 , (3, 0, None, None) , 0 , )),
+	(( u'DeleteServer' , u'ServerName' , None , ), 1610809407, (1610809407, (), [ (16392, 3, None, None) , 
+			(16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 1972 , (3, 0, None, None) , 0 , )),
+	(( u'ActiveServer' , None , ), 1745027118, (1745027118, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1976 , (3, 0, None, None) , 0 , )),
+	(( u'ActiveServer' , None , ), 1745027118, (1745027118, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1980 , (3, 0, None, None) , 0 , )),
+	(( u'HideDetails' , None , ), 1745027136, (1745027136, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1984 , (3, 0, None, None) , 0 , )),
+	(( u'HideDetails' , None , ), 1745027136, (1745027136, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1988 , (3, 0, None, None) , 0 , )),
+	(( u'Refresh' , ), 1610809419, (1610809419, (), [ ], 1 , 1 , 4 , 0 , 1992 , (3, 0, None, None) , 0 , )),
+	(( u'AllowDragDrop' , None , ), 1745027148, (1745027148, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1996 , (3, 0, None, None) , 0 , )),
+	(( u'AllowDragDrop' , None , ), 1745027148, (1745027148, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2000 , (3, 0, None, None) , 0 , )),
+]
+
+_TankSelect_vtables_dispatch_ = 1
+_TankSelect_vtables_ = [
+	(( u'Refresh' , ), 1610809417, (1610809417, (), [ ], 1 , 1 , 4 , 0 , 1956 , (3, 0, None, None) , 0 , )),
+	(( u'AllowPopup' , None , ), 1745027124, (1745027124, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1960 , (3, 0, None, None) , 0 , )),
+	(( u'AllowPopup' , None , ), 1745027124, (1745027124, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1964 , (3, 0, None, None) , 0 , )),
+	(( u'UseServer' , None , ), 1745027123, (1745027123, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 1968 , (3, 0, None, None) , 0 , )),
+	(( u'UseServer' , None , ), 1745027123, (1745027123, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 1972 , (3, 0, None, None) , 0 , )),
+	(( u'ShowServer' , None , ), 1745027122, (1745027122, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1976 , (3, 0, None, None) , 0 , )),
+	(( u'ShowServer' , None , ), 1745027122, (1745027122, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1980 , (3, 0, None, None) , 0 , )),
+	(( u'HideDetails' , None , ), 1745027121, (1745027121, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1984 , (3, 0, None, None) , 0 , )),
+	(( u'HideDetails' , None , ), 1745027121, (1745027121, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1988 , (3, 0, None, None) , 0 , )),
+	(( u'SingleClickSelect' , None , ), 1745027120, (1745027120, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 1992 , (3, 0, None, None) , 0 , )),
+	(( u'SingleClickSelect' , None , ), 1745027120, (1745027120, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 1996 , (3, 0, None, None) , 0 , )),
+	(( u'ActiveTank' , None , ), 1745027119, (1745027119, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 2000 , (3, 0, None, None) , 0 , )),
+	(( u'ActiveTank' , None , ), 1745027119, (1745027119, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 2004 , (3, 0, None, None) , 0 , )),
+	(( u'AllowDragDrop' , None , ), 1745027146, (1745027146, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2008 , (3, 0, None, None) , 0 , )),
+	(( u'AllowDragDrop' , None , ), 1745027146, (1745027146, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2012 , (3, 0, None, None) , 0 , )),
+	(( u'ShowOnlyPathString' , None , ), 1745027147, (1745027147, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 2016 , (3, 0, None, None) , 0 , )),
+	(( u'ShowOnlyPathString' , None , ), 1745027147, (1745027147, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 2020 , (3, 0, None, None) , 0 , )),
+	(( u'ShowSpecPathOnly' , None , ), 1745027148, (1745027148, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2024 , (3, 0, None, None) , 0 , )),
+	(( u'ShowSpecPathOnly' , None , ), 1745027148, (1745027148, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2028 , (3, 0, None, None) , 0 , )),
+	(( u'FileDialogInitPath' , None , ), 1745027149, (1745027149, (), [ (8, 1, None, None) , ], 1 , 4 , 4 , 0 , 2032 , (3, 0, None, None) , 0 , )),
+	(( u'FileDialogInitPath' , None , ), 1745027149, (1745027149, (), [ (16392, 10, None, None) , ], 1 , 2 , 4 , 0 , 2036 , (3, 0, None, None) , 0 , )),
+	(( u'AddTank' , u'path' , u'name' , u'quite' , None , 
+			), 1610809446, (1610809446, (), [ (8, 1, None, None) , (8, 1, None, None) , (11, 1, None, None) , (16395, 10, None, None) , ], 1 , 1 , 4 , 0 , 2040 , (3, 0, None, None) , 0 , )),
+	(( u'ShowTankNew' , None , ), 1745027175, (1745027175, (), [ (16395, 10, None, None) , ], 1 , 2 , 4 , 0 , 2044 , (3, 0, None, None) , 0 , )),
+	(( u'ShowTankNew' , None , ), 1745027175, (1745027175, (), [ (11, 1, None, None) , ], 1 , 4 , 4 , 0 , 2048 , (3, 0, None, None) , 0 , )),
+]
+
+RecordMap = {
+	u'TankInfo': '{A3EA7E81-5BF7-4FE4-9659-D797A6DD6A13}',
+}
+
+CLSIDToClassMap = {
+	'{A16140DD-AAA9-46C3-9565-6F1E8815D90A}' : ServerSelect,
+	'{C2F42E9B-86B7-4F21-889D-8B854B019640}' : _BlockSelect,
+	'{DC769221-9AD4-4CCD-B51A-FEC47ED63458}' : _BlockSelect_,
+	'{01B10737-93FA-4FB2-B1F1-0C59793EBCAA}' : EventSelect,
+	'{42EDA46E-842E-4131-9C40-1E47D6B8ABB1}' : ServSelProps,
+	'{75CA8D1D-4078-4EA7-8EC2-E2198C9CFA52}' : _ServerSelect_,
+	'{CBA421AC-7EB7-40BA-AA2C-81CC652B2EEF}' : _EventSelect,
+	'{7BE3D05E-A964-4EF6-A8E6-1E07AB181A98}' : _ServerSelect,
+	'{91124062-FA58-4A43-962A-A3E90676DEC0}' : _ServSelProps,
+	'{58277ACF-7979-45F9-BBE7-0FB5D6B416F4}' : _TankSelect_,
+	'{3F098EDA-4EFB-4923-9613-373BF08B3F5C}' : _EventSelect_,
+	'{6BCC8D27-0166-441E-9441-8F55DB2779FB}' : TankSelect,
+	'{2303C7E3-BC00-4B81-A550-D258167DC1C0}' : _TankSelect,
+	'{CB81F5AF-7625-4F83-B629-54C37B55A203}' : BlockSelect,
+}
+CLSIDToPackageMap = {}
+win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
+VTablesToPackageMap = {}
+VTablesToClassMap = {
+	'{CBA421AC-7EB7-40BA-AA2C-81CC652B2EEF}' : '_EventSelect',
+	'{91124062-FA58-4A43-962A-A3E90676DEC0}' : '_ServSelProps',
+	'{7BE3D05E-A964-4EF6-A8E6-1E07AB181A98}' : '_ServerSelect',
+	'{2303C7E3-BC00-4B81-A550-D258167DC1C0}' : '_TankSelect',
+	'{C2F42E9B-86B7-4F21-889D-8B854B019640}' : '_BlockSelect',
+}
+
+
+NamesToIIDMap = {
+	'_BlockSelect_' : '{DC769221-9AD4-4CCD-B51A-FEC47ED63458}',
+	'_EventSelect' : '{CBA421AC-7EB7-40BA-AA2C-81CC652B2EEF}',
+	'_BlockSelect' : '{C2F42E9B-86B7-4F21-889D-8B854B019640}',
+	'_ServSelProps' : '{91124062-FA58-4A43-962A-A3E90676DEC0}',
+	'_ServerSelect_' : '{75CA8D1D-4078-4EA7-8EC2-E2198C9CFA52}',
+	'_EventSelect_' : '{3F098EDA-4EFB-4923-9613-373BF08B3F5C}',
+	'_TankSelect' : '{2303C7E3-BC00-4B81-A550-D258167DC1C0}',
+	'_ServerSelect' : '{7BE3D05E-A964-4EF6-A8E6-1E07AB181A98}',
+	'_TankSelect_' : '{58277ACF-7979-45F9-BBE7-0FB5D6B416F4}',
+}
+
+
```

### Comparing `TDTPy-0.8.1/tdt/actxobjects/TTankX.py` & `TDTPy-0.9.0/tdt/actxobjects/TTankX.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,618 +1,618 @@
-# -*- coding: utf-8 -*-
-# Created by makepy.py version 0.5.00
-# By python version 2.6.6 |EPD 6.3-2 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
-# From type library 'TTankX.ocx'
-# On Thu Dec 02 21:01:19 2010
-"""TTankX ActiveX Control module"""
-makepy_version = '0.5.00'
-python_version = 0x20606f0
-
-import win32com.client.CLSIDToClass, pythoncom, pywintypes
-import win32com.client.util
-from pywintypes import IID
-from win32com.client import Dispatch
-
-# The following 3 lines may need tweaking for the particular server
-# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
-defaultNamedOptArg=pythoncom.Empty
-defaultNamedNotOptArg=pythoncom.Empty
-defaultUnnamedArg=pythoncom.Empty
-
-CLSID = IID('{3EABA0EF-2FBA-41F8-A970-3F238A4BAB01}')
-MajorVersion = 1
-MinorVersion = 0
-LibraryFlags = 10
-LCID = 0x0
-
-from win32com.client import DispatchBaseClass
-class _DTTankX(DispatchBaseClass):
-	"""Dispatch interface for TTankX Control"""
-	CLSID = IID('{BE6CAD3F-28F1-4EAC-B210-9CAA5CA8B5B8}')
-	coclass_clsid = IID('{670490CE-57D2-4176-8E74-80C4C6A47D88}')
-
-	def AboutBox(self):
-		return self._oleobj_.InvokeTypes(-552, LCID, 1, (24, 0), (),)
-
-	def AddClient(self, ClientName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(19, LCID, 1, (3, 0), ((8, 0),),ClientName
-			)
-
-	def AddServer(self, ServerName=defaultNamedNotOptArg, IPAddress=defaultNamedNotOptArg, Username=defaultNamedNotOptArg, Domain=defaultNamedNotOptArg
-			, Password=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(48, LCID, 1, (3, 0), ((8, 0), (8, 0), (8, 0), (8, 0), (8, 0)),ServerName
-			, IPAddress, Username, Domain, Password)
-
-	def AddTank(self, TankName=defaultNamedNotOptArg, FilePath=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(20, LCID, 1, (3, 0), ((8, 0), (8, 0)),TankName
-			, FilePath)
-
-	def BuildEpocEv(self, Index=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, Value=defaultNamedNotOptArg
-			, BuddyEpoc=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(69, LCID, 1, (3, 0), ((3, 0), (8, 0), (5, 0), (5, 0), (8, 0)),Index
-			, TankCode, TimeStamp, Value, BuddyEpoc)
-
-	def BuildFilterDesc(self, TankCode=defaultNamedNotOptArg, TestCode=defaultNamedNotOptArg, V1=defaultNamedNotOptArg, V2=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(81, LCID, 1, (8, 0), ((3, 0), (3, 0), (5, 0), (5, 0)),TankCode
-			, TestCode, V1, V2)
-
-	def BuildScalar(self, Index=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg
-			, Value=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(68, LCID, 1, (3, 0), ((3, 0), (8, 0), (3, 0), (5, 0), (5, 0)),Index
-			, TankCode, SortChan, TimeStamp, Value)
-
-	def BuildSnipEv(self, Index=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, HasSort=defaultNamedNotOptArg
-			, pData=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(71, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (3, 0), (16388, 0)),Index
-			, SortChan, TimeStamp, HasSort, pData)
-
-	def BuildSnipEvV(self, Index=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, HasSort=defaultNamedNotOptArg
-			, vData=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(73, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (3, 0), (16396, 0)),Index
-			, SortChan, TimeStamp, HasSort, vData)
-
-	def BuildStreamEv(self, Index=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, pData=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(72, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (16388, 0)),Index
-			, SortChan, TimeStamp, pData)
-
-	def BuildStreamEvV(self, Index=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, vData=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(74, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (12, 0)),Index
-			, SortChan, TimeStamp, vData)
-
-	def CheckTank(self, TankName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(21, LCID, 1, (3, 0), ((8, 0),),TankName
-			)
-
-	def ClearEpocIndexing(self):
-		return self._oleobj_.InvokeTypes(85, LCID, 1, (24, 0), (),)
-
-	def CloseTank(self):
-		return self._oleobj_.InvokeTypes(22, LCID, 1, (24, 0), (),)
-
-	def CodeToString(self, EvCode=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(23, LCID, 1, (8, 0), ((3, 0),),EvCode
-			)
-
-	def ConnectServer(self, ServerName=defaultNamedNotOptArg, ClientName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(18, LCID, 1, (3, 0), ((8, 0), (8, 0)),ServerName
-			, ClientName)
-
-	def CreateEpocIndexing(self):
-		return self._oleobj_.InvokeTypes(84, LCID, 1, (3, 0), (),)
-
-	def DFromToString(self, DFormCode=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(27, LCID, 1, (8, 0), ((3, 0),),DFormCode
-			)
-
-	def DeleteClient(self, ClientName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(24, LCID, 1, (24, 0), ((8, 0),),ClientName
-			)
-
-	def DeleteSortCode(self, sortName=defaultNamedNotOptArg, snipName=defaultNamedNotOptArg, idxChan=defaultNamedNotOptArg):
-		"""method DeleteSortCode"""
-		return self._oleobj_.InvokeTypes(125, LCID, 1, (3, 0), ((8, 0), (8, 0), (3, 0)),sortName
-			, snipName, idxChan)
-
-	def DisableTankDebug(self, TankName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(34, LCID, 1, (24, 0), ((8, 0),),TankName
-			)
-
-	def EnableTankDebug(self, TankName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(33, LCID, 1, (24, 0), ((8, 0),),TankName
-			)
-
-	def EvTypeToString(self, evTypeCode=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(26, LCID, 1, (8, 0), ((3, 0),),evTypeCode
-			)
-
-	def FancyTime(self, Time=defaultNamedNotOptArg, Format=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(44, LCID, 1, (8, 0), ((5, 0), (8, 0)),Time
-			, Format)
-
-	def FromTTD(self, TTD=defaultNamedNotOptArg, FieldCode=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(54, LCID, 1, (8, 0), ((8, 0), (8, 0)),TTD
-			, FieldCode)
-
-	def GetClientID(self, ClientName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(35, LCID, 1, (3, 0), ((8, 0),),ClientName
-			)
-
-	def GetCodeSpecs(self, EvCode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(36, LCID, 1, (3, 0), ((3, 0),),EvCode
-			)
-
-	def GetCodeSpecsLazy(self, EvCode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(111, LCID, 1, (3, 0), ((3, 0),),EvCode
-			)
-
-	def GetDebug(self, TankName=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(28, LCID, 1, (8, 0), ((8, 0),),TankName
-			)
-
-	def GetEnumServer(self, Index=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(51, LCID, 1, (8, 0), ((3, 0),),Index
-			)
-
-	def GetEnumTank(self, Index=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(47, LCID, 1, (8, 0), ((3, 0),),Index
-			)
-
-	def GetEpocCode(self, Index=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(58, LCID, 1, (8, 0), ((3, 0),),Index
-			)
-
-	def GetEpocs(self, pEPs=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, T1=defaultNamedNotOptArg, T2=defaultNamedNotOptArg
-			, MaxRet=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(60, LCID, 1, (3, 0), ((16389, 0), (3, 0), (5, 0), (5, 0), (3, 0)),pEPs
-			, TankCode, T1, T2, MaxRet)
-
-	def GetEpocsEx(self, pEPs=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, MaxReturn=defaultNamedNotOptArg, Mode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(94, LCID, 1, (3, 0), ((16389, 0), (3, 0), (3, 0), (3, 0)),pEPs
-			, TankCode, MaxReturn, Mode)
-
-	def GetEpocsExV(self, TankCode=defaultNamedNotOptArg, Mode=defaultNamedNotOptArg):
-		return self._ApplyTypes_(95, 1, (12, 0), ((8, 0), (3, 0)), u'GetEpocsExV', None,TankCode
-			, Mode)
-
-	def GetEpocsV(self, TankCode=defaultNamedNotOptArg, T1=defaultNamedNotOptArg, T2=defaultNamedNotOptArg, MaxEpocs=defaultNamedNotOptArg):
-		return self._ApplyTypes_(57, 1, (12, 0), ((8, 0), (5, 0), (5, 0), (3, 0)), u'GetEpocsV', None,TankCode
-			, T1, T2, MaxEpocs)
-
-	def GetError(self):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(29, LCID, 1, (8, 0), (),)
-
-	def GetEvTsqIdx(self):
-		"""method GetEvTsqIdx"""
-		return self._ApplyTypes_(122, 1, (12, 0), (), u'GetEvTsqIdx', None,)
-
-	def GetEventCodes(self, EvType=defaultNamedNotOptArg):
-		return self._ApplyTypes_(38, 1, (12, 0), ((3, 0),), u'GetEventCodes', None,EvType
-			)
-
-	def GetFilterTolerance(self):
-		return self._oleobj_.InvokeTypes(87, LCID, 1, (5, 0), (),)
-
-	def GetGlobal(self, code=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(106, LCID, 1, (5, 0), ((3, 0),),code
-			)
-
-	def GetGlobalB(self, name=defaultNamedNotOptArg):
-		"""method GetGlobalB"""
-		return self._oleobj_.InvokeTypes(119, LCID, 1, (5, 0), ((8, 0),),name
-			)
-
-	def GetGlobalStringB(self, name=defaultNamedNotOptArg):
-		"""method GetGlobalStringB"""
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(120, LCID, 1, (8, 0), ((8, 0),),name
-			)
-
-	def GetGlobalStringV(self, name=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(108, LCID, 1, (8, 0), ((31, 0),),name
-			)
-
-	def GetGlobalV(self, name=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(107, LCID, 1, (5, 0), ((31, 0),),name
-			)
-
-	def GetHotBlock(self):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(66, LCID, 1, (8, 0), (),)
-
-	def GetNPer(self, DForm=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(59, LCID, 1, (3, 0), ((3, 0),),DForm
-			)
-
-	def GetServerItem(self, ServerName=defaultNamedNotOptArg, ItemCode=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(50, LCID, 1, (8, 0), ((8, 0), (8, 0)),ServerName
-			, ItemCode)
-
-	def GetSortChanMap(self, sortName=defaultNamedNotOptArg, snipName=defaultNamedNotOptArg):
-		"""method GetSortChanMap"""
-		return self._ApplyTypes_(126, 1, (12, 0), ((8, 0), (8, 0)), u'GetSortChanMap', None,sortName
-			, snipName)
-
-	def GetSortCondition(self, sortName=defaultNamedNotOptArg, snipName=defaultNamedNotOptArg, idxChan=defaultNamedNotOptArg):
-		"""method GetSortCondition"""
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(124, LCID, 1, (8, 0), ((8, 0), (8, 0), (3, 0)),sortName
-			, snipName, idxChan)
-
-	def GetSortName(self, EventName=defaultNamedNotOptArg, idxSortID=defaultNamedNotOptArg):
-		"""method GetSortName"""
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(113, LCID, 1, (8, 0), ((8, 0), (3, 0)),EventName
-			, idxSortID)
-
-	def GetStatus(self, StatCode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(39, LCID, 1, (3, 0), ((3, 0),),StatCode
-			)
-
-	def GetTankItem(self, TankName=defaultNamedNotOptArg, ItemCode=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(52, LCID, 1, (8, 0), ((8, 0), (8, 0)),TankName
-			, ItemCode)
-
-	def GetValidTimeRanges(self, pRanges=defaultNamedNotOptArg, MaxReturn=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(99, LCID, 1, (3, 0), ((16389, 0), (3, 0)),pRanges
-			, MaxReturn)
-
-	def GetValidTimeRangesV(self):
-		return self._ApplyTypes_(100, 1, (12, 0), (), u'GetValidTimeRangesV', None,)
-
-	def IndexEvent(self, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg, SortCode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(83, LCID, 1, (3, 0), ((3, 0), (3, 0), (3, 0)),TankCode
-			, Channel, SortCode)
-
-	def InitializeTank(self, TankName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(40, LCID, 1, (3, 0), ((8, 0),),TankName
-			)
-
-	def OpenTank(self, TankName=defaultNamedNotOptArg, AccessMode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(30, LCID, 1, (3, 0), ((8, 0), (8, 0)),TankName
-			, AccessMode)
-
-	def ParseEv(self, RecIndex=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg, SortCode=defaultNamedNotOptArg
-			, Npts=defaultNamedNotOptArg, pData=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(75, LCID, 1, (3, 0), ((3, 0), (16389, 0), (16387, 0), (16387, 0), (16387, 0), (16388, 0)),RecIndex
-			, TimeStamp, Channel, SortCode, Npts, pData
-			)
-
-	def ParseEvInfoV(self, RecIndex=defaultNamedNotOptArg, nRecs=defaultNamedNotOptArg, nItem=defaultNamedNotOptArg):
-		return self._ApplyTypes_(77, 1, (12, 0), ((3, 0), (3, 0), (3, 0)), u'ParseEvInfoV', None,RecIndex
-			, nRecs, nItem)
-
-	def ParseEvV(self, RecIndex=defaultNamedNotOptArg, nRecs=defaultNamedNotOptArg):
-		return self._ApplyTypes_(76, 1, (12, 0), ((3, 0), (3, 0)), u'ParseEvV', None,RecIndex
-			, nRecs)
-
-	def ParseFilterDesc(self, FiltDesc=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, TestCode=defaultNamedNotOptArg, V1=defaultNamedNotOptArg
-			, V2=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(80, LCID, 1, (3, 0), ((8, 0), (16387, 0), (16387, 0), (16389, 0), (16389, 0)),FiltDesc
-			, TankCode, TestCode, V1, V2)
-
-	def QryEpocAt(self, TankCode=defaultNamedNotOptArg, rTime=defaultNamedNotOptArg, ReqItem=defaultNamedNotOptArg, RetVal=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(64, LCID, 1, (3, 0), ((3, 0), (5, 0), (3, 0), (16389, 0)),TankCode
-			, rTime, ReqItem, RetVal)
-
-	def QryEpocAtV(self, TankCode=defaultNamedNotOptArg, rTime=defaultNamedNotOptArg, ReqItem=defaultNamedNotOptArg):
-		return self._ApplyTypes_(65, 1, (12, 0), ((8, 0), (5, 0), (3, 0)), u'QryEpocAtV', None,TankCode
-			, rTime, ReqItem)
-
-	def QueryBlockName(self, BlockNumber=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(41, LCID, 1, (8, 0), ((3, 0),),BlockNumber
-			)
-
-	def ReadEvents(self, MaxRet=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg, SortCode=defaultNamedNotOptArg
-			, T1=defaultNamedNotOptArg, T2=defaultNamedNotOptArg, Options=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(62, LCID, 1, (3, 0), ((3, 0), (3, 0), (3, 0), (3, 0), (5, 0), (5, 0), (3, 0)),MaxRet
-			, TankCode, Channel, SortCode, T1, T2
-			, Options)
-
-	def ReadEventsSimple(self, EventName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(96, LCID, 1, (3, 0), ((8, 0),),EventName
-			)
-
-	def ReadEventsV(self, MaxRet=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg, SortCode=defaultNamedNotOptArg
-			, T1=defaultNamedNotOptArg, T2=defaultNamedNotOptArg, Options=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(63, LCID, 1, (3, 0), ((3, 0), (8, 0), (3, 0), (3, 0), (5, 0), (5, 0), (8, 0)),MaxRet
-			, TankCode, Channel, SortCode, T1, T2
-			, Options)
-
-	def ReadWaves(self, TankCode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(97, LCID, 1, (3, 0), ((3, 0),),TankCode
-			)
-
-	def ReadWavesOnTimeRange(self, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(101, LCID, 1, (3, 0), ((3, 0), (3, 0)),TankCode
-			, Channel)
-
-	def ReadWavesOnTimeRangeB(self, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg):
-		"""method ReadWavesOnTimeRangeB"""
-		return self._ApplyTypes_(116, 1, (12, 0), ((8, 0), (3, 0)), u'ReadWavesOnTimeRangeB', None,TankCode
-			, Channel)
-
-	def ReadWavesOnTimeRangeV(self, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg):
-		return self._ApplyTypes_(102, 1, (12, 0), ((31, 0), (3, 0)), u'ReadWavesOnTimeRangeV', None,TankCode
-			, Channel)
-
-	def ReadWavesV(self, TankCode=defaultNamedNotOptArg):
-		return self._ApplyTypes_(98, 1, (12, 0), ((8, 0),), u'ReadWavesV', None,TankCode
-			)
-
-	def ReleaseServer(self):
-		return self._oleobj_.InvokeTypes(42, LCID, 1, (24, 0), (),)
-
-	def RemoveBlock(self, BlockName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(56, LCID, 1, (3, 0), ((8, 0),),BlockName
-			)
-
-	def RemoveEvents(self, BlockName=defaultNamedNotOptArg, RelTime1=defaultNamedNotOptArg, RelTime2=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(55, LCID, 1, (3, 0), ((8, 0), (5, 0), (5, 0)),BlockName
-			, RelTime1, RelTime2)
-
-	def RemoveServer(self, ServerName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(49, LCID, 1, (3, 0), ((8, 0),),ServerName
-			)
-
-	def RemoveTank(self, TankName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(25, LCID, 1, (3, 0), ((8, 0),),TankName
-			)
-
-	def ResetFilters(self):
-		return self._oleobj_.InvokeTypes(82, LCID, 1, (24, 0), (),)
-
-	def ResetGlobals(self):
-		return self._oleobj_.InvokeTypes(110, LCID, 1, (24, 0), (),)
-
-	def ResetTank(self, TankName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(43, LCID, 1, (3, 0), ((8, 0),),TankName
-			)
-
-	def SaveSortCodes(self, sortName=defaultNamedNotOptArg, snipName=defaultNamedNotOptArg, idxChan=defaultNamedNotOptArg, sortCondition=defaultNamedNotOptArg
-			, sortCodeArray=defaultNamedNotOptArg):
-		"""method SaveSortCodes"""
-		return self._oleobj_.InvokeTypes(123, LCID, 1, (3, 0), ((8, 0), (8, 0), (3, 0), (8, 0), (12, 0)),sortName
-			, snipName, idxChan, sortCondition, sortCodeArray)
-
-	def SelectBlock(self, BlockName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(32, LCID, 1, (3, 0), ((8, 0),),BlockName
-			)
-
-	def SetBuildHead(self, TankCode=defaultNamedNotOptArg, DataForm=defaultNamedNotOptArg, SampFreq=defaultNamedNotOptArg, nNet=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(70, LCID, 1, (24, 0), ((8, 0), (3, 0), (5, 0), (3, 0)),TankCode
-			, DataForm, SampFreq, nNet)
-
-	def SetEpocTimeFilter(self, EpocCode=defaultNamedNotOptArg, Offset=defaultNamedNotOptArg, Dur=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(90, LCID, 1, (3, 0), ((3, 0), (5, 0), (5, 0)),EpocCode
-			, Offset, Dur)
-
-	def SetEpocTimeFilterB(self, EpocCode=defaultNamedNotOptArg, Offset=defaultNamedNotOptArg, Dur=defaultNamedNotOptArg):
-		"""method SetEpocTimeFilterB"""
-		return self._oleobj_.InvokeTypes(114, LCID, 1, (3, 0), ((8, 0), (5, 0), (5, 0)),EpocCode
-			, Offset, Dur)
-
-	def SetEpocTimeFilterV(self, EpocCode=defaultNamedNotOptArg, Offset=defaultNamedNotOptArg, Dur=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(91, LCID, 1, (3, 0), ((31, 0), (5, 0), (5, 0)),EpocCode
-			, Offset, Dur)
-
-	def SetFilter(self, TankCode=defaultNamedNotOptArg, TestCode=defaultNamedNotOptArg, V1=defaultNamedNotOptArg, V2=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(78, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (5, 0)),TankCode
-			, TestCode, V1, V2)
-
-	def SetFilterArray(self, Dim=defaultNamedNotOptArg, ID=defaultNamedNotOptArg, Filter=defaultNamedNotOptArg, Exclusive=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(89, LCID, 1, (3, 0), ((3, 0), (3, 0), (8, 0), (3, 0)),Dim
-			, ID, Filter, Exclusive)
-
-	def SetFilterTolerance(self, loosenFactor=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(86, LCID, 1, (3, 0), ((5, 0),),loosenFactor
-			)
-
-	def SetFilterWithDesc(self, FiltDesc=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(79, LCID, 1, (3, 0), ((8, 0),),FiltDesc
-			)
-
-	def SetFilterWithDescEx(self, Filter=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(88, LCID, 1, (3, 0), ((8, 0),),Filter
-			)
-
-	def SetGlobal(self, code=defaultNamedNotOptArg, Value=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(103, LCID, 1, (3, 0), ((3, 0), (5, 0)),code
-			, Value)
-
-	def SetGlobalB(self, name=defaultNamedNotOptArg, Value=defaultNamedNotOptArg):
-		"""method SetGlobalB"""
-		return self._oleobj_.InvokeTypes(117, LCID, 1, (3, 0), ((8, 0), (5, 0)),name
-			, Value)
-
-	def SetGlobalStringB(self, name=defaultNamedNotOptArg, strvalue=defaultNamedNotOptArg):
-		"""method SetGlobalStringB"""
-		return self._oleobj_.InvokeTypes(118, LCID, 1, (3, 0), ((8, 0), (8, 0)),name
-			, strvalue)
-
-	def SetGlobalStringV(self, name=defaultNamedNotOptArg, strvalue=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(105, LCID, 1, (3, 0), ((31, 0), (31, 0)),name
-			, strvalue)
-
-	def SetGlobalV(self, name=defaultNamedNotOptArg, Value=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(104, LCID, 1, (3, 0), ((31, 0), (5, 0)),name
-			, Value)
-
-	def SetGlobals(self, str=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(109, LCID, 1, (3, 0), ((31, 0),),str
-			)
-
-	def SetGlobalsB(self, str=defaultNamedNotOptArg):
-		"""method SetGlobalsB"""
-		return self._oleobj_.InvokeTypes(121, LCID, 1, (3, 0), ((8, 0),),str
-			)
-
-	def SetRefEpoc(self, EpocCode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(92, LCID, 1, (3, 0), ((3, 0),),EpocCode
-			)
-
-	def SetRefEpocB(self, EpocCode=defaultNamedNotOptArg):
-		"""method SetRefEpocB"""
-		return self._oleobj_.InvokeTypes(115, LCID, 1, (3, 0), ((8, 0),),EpocCode
-			)
-
-	def SetRefEpocV(self, EpocCode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(93, LCID, 1, (3, 0), ((31, 0),),EpocCode
-			)
-
-	def SetRefTime(self, TimeOS=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(31, LCID, 1, (3, 0), ((5, 0),),TimeOS
-			)
-
-	def SetUseSortName(self, sortID=defaultNamedNotOptArg):
-		"""method SetUseSortName"""
-		return self._oleobj_.InvokeTypes(112, LCID, 1, (3, 0), ((8, 0),),sortID
-			)
-
-	def StartRecord(self, BlockName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(45, LCID, 1, (3, 0), ((8, 0),),BlockName
-			)
-
-	def StopRecord(self):
-		return self._oleobj_.InvokeTypes(46, LCID, 1, (24, 0), (),)
-
-	def StringToEvCode(self, EvCode=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(37, LCID, 1, (3, 0), ((8, 0),),EvCode
-			)
-
-	def SwitchClient(self, ClientName=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(67, LCID, 1, (3, 0), ((8, 0),),ClientName
-			)
-
-	def ToTTD(self, ServName=defaultNamedNotOptArg, TankName=defaultNamedNotOptArg, BlockName=defaultNamedNotOptArg, EvName=defaultNamedNotOptArg
-			, ChanList=defaultNamedNotOptArg):
-		# Result is a Unicode object
-		return self._oleobj_.InvokeTypes(53, LCID, 1, (8, 0), ((8, 0), (8, 0), (8, 0), (8, 0), (16387, 0)),ServName
-			, TankName, BlockName, EvName, ChanList)
-
-	def WriteEvents(self, NumEv=defaultNamedNotOptArg):
-		return self._oleobj_.InvokeTypes(61, LCID, 1, (3, 0), ((3, 0),),NumEv
-			)
-
-	_prop_map_get_ = {
-		"ClientID": (6, 2, (3, 0), (), "ClientID", None),
-		"CurBlockMemo": (3, 2, (8, 0), (), "CurBlockMemo", None),
-		"CurBlockName": (1, 2, (8, 0), (), "CurBlockName", None),
-		"CurBlockNotes": (17, 2, (8, 0), (), "CurBlockNotes", None),
-		"CurBlockOwner": (2, 2, (8, 0), (), "CurBlockOwner", None),
-		"CurBlockStartTime": (4, 2, (5, 0), (), "CurBlockStartTime", None),
-		"CurBlockStopTime": (5, 2, (5, 0), (), "CurBlockStopTime", None),
-		"Domain": (15, 2, (8, 0), (), "Domain", None),
-		"EvChannel": (13, 2, (3, 0), (), "EvChannel", None),
-		"EvDForm": (10, 2, (3, 0), (), "EvDForm", None),
-		"EvDataSize": (8, 2, (3, 0), (), "EvDataSize", None),
-		"EvFirstTime": (9, 2, (5, 0), (), "EvFirstTime", None),
-		"EvSampFreq": (11, 2, (4, 0), (), "EvSampFreq", None),
-		"EvTimeStamp": (12, 2, (5, 0), (), "EvTimeStamp", None),
-		"EvType": (7, 2, (3, 0), (), "EvType", None),
-		"Password": (16, 2, (8, 0), (), "Password", None),
-		"Username": (14, 2, (8, 0), (), "Username", None),
-	}
-	_prop_map_put_ = {
-		"ClientID" : ((6, LCID, 4, 0),()),
-		"CurBlockMemo" : ((3, LCID, 4, 0),()),
-		"CurBlockName" : ((1, LCID, 4, 0),()),
-		"CurBlockNotes" : ((17, LCID, 4, 0),()),
-		"CurBlockOwner" : ((2, LCID, 4, 0),()),
-		"CurBlockStartTime" : ((4, LCID, 4, 0),()),
-		"CurBlockStopTime" : ((5, LCID, 4, 0),()),
-		"Domain" : ((15, LCID, 4, 0),()),
-		"EvChannel" : ((13, LCID, 4, 0),()),
-		"EvDForm" : ((10, LCID, 4, 0),()),
-		"EvDataSize" : ((8, LCID, 4, 0),()),
-		"EvFirstTime" : ((9, LCID, 4, 0),()),
-		"EvSampFreq" : ((11, LCID, 4, 0),()),
-		"EvTimeStamp" : ((12, LCID, 4, 0),()),
-		"EvType" : ((7, LCID, 4, 0),()),
-		"Password" : ((16, LCID, 4, 0),()),
-		"Username" : ((14, LCID, 4, 0),()),
-	}
-
-class _DTTankXEvents:
-	"""Event interface for TTankX Control"""
-	CLSID = CLSID_Sink = IID('{9C0BD59B-8842-47DA-8105-DC3E883D72D1}')
-	coclass_clsid = IID('{670490CE-57D2-4176-8E74-80C4C6A47D88}')
-	_public_methods_ = [] # For COM Server support
-	_dispid_to_func_ = {
-		}
-
-	def __init__(self, oobj = None):
-		if oobj is None:
-			self._olecp = None
-		else:
-			import win32com.server.util
-			from win32com.server.policy import EventHandlerPolicy
-			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
-			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
-			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
-			self._olecp,self._olecp_cookie = cp,cookie
-	def __del__(self):
-		try:
-			self.close()
-		except pythoncom.com_error:
-			pass
-	def close(self):
-		if self._olecp is not None:
-			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
-			cp.Unadvise(cookie)
-	def _query_interface_(self, iid):
-		import win32com.server.util
-		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
-
-	# Event Handlers
-	# If you create handlers, they should have the following prototypes:
-
-
-from win32com.client import CoClassBaseClass
-# This CoClass is known by the name 'TTANK.X'
-class TTankX(CoClassBaseClass): # A CoClass
-	# TTankX Control
-	CLSID = IID('{670490CE-57D2-4176-8E74-80C4C6A47D88}')
-	coclass_sources = [
-		_DTTankXEvents,
-	]
-	default_source = _DTTankXEvents
-	coclass_interfaces = [
-		_DTTankX,
-	]
-	default_interface = _DTTankX
-
-RecordMap = {
-}
-
-CLSIDToClassMap = {
-	'{670490CE-57D2-4176-8E74-80C4C6A47D88}' : TTankX,
-	'{9C0BD59B-8842-47DA-8105-DC3E883D72D1}' : _DTTankXEvents,
-	'{BE6CAD3F-28F1-4EAC-B210-9CAA5CA8B5B8}' : _DTTankX,
-}
-CLSIDToPackageMap = {}
-win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
-VTablesToPackageMap = {}
-VTablesToClassMap = {
-}
-
-
-NamesToIIDMap = {
-	'_DTTankX' : '{BE6CAD3F-28F1-4EAC-B210-9CAA5CA8B5B8}',
-	'_DTTankXEvents' : '{9C0BD59B-8842-47DA-8105-DC3E883D72D1}',
-}
-
-
+# -*- coding: utf-8 -*-
+# Created by makepy.py version 0.5.00
+# By python version 2.6.6 |EPD 6.3-2 (32-bit)| (r266:84292, Sep 20 2010, 11:26:16) [MSC v.1500 32 bit (Intel)]
+# From type library 'TTankX.ocx'
+# On Thu Dec 02 21:01:19 2010
+"""TTankX ActiveX Control module"""
+makepy_version = '0.5.00'
+python_version = 0x20606f0
+
+import win32com.client.CLSIDToClass, pythoncom, pywintypes
+import win32com.client.util
+from pywintypes import IID
+from win32com.client import Dispatch
+
+# The following 3 lines may need tweaking for the particular server
+# Candidates are pythoncom.Missing, .Empty and .ArgNotFound
+defaultNamedOptArg=pythoncom.Empty
+defaultNamedNotOptArg=pythoncom.Empty
+defaultUnnamedArg=pythoncom.Empty
+
+CLSID = IID('{3EABA0EF-2FBA-41F8-A970-3F238A4BAB01}')
+MajorVersion = 1
+MinorVersion = 0
+LibraryFlags = 10
+LCID = 0x0
+
+from win32com.client import DispatchBaseClass
+class _DTTankX(DispatchBaseClass):
+	"""Dispatch interface for TTankX Control"""
+	CLSID = IID('{BE6CAD3F-28F1-4EAC-B210-9CAA5CA8B5B8}')
+	coclass_clsid = IID('{670490CE-57D2-4176-8E74-80C4C6A47D88}')
+
+	def AboutBox(self):
+		return self._oleobj_.InvokeTypes(-552, LCID, 1, (24, 0), (),)
+
+	def AddClient(self, ClientName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(19, LCID, 1, (3, 0), ((8, 0),),ClientName
+			)
+
+	def AddServer(self, ServerName=defaultNamedNotOptArg, IPAddress=defaultNamedNotOptArg, Username=defaultNamedNotOptArg, Domain=defaultNamedNotOptArg
+			, Password=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(48, LCID, 1, (3, 0), ((8, 0), (8, 0), (8, 0), (8, 0), (8, 0)),ServerName
+			, IPAddress, Username, Domain, Password)
+
+	def AddTank(self, TankName=defaultNamedNotOptArg, FilePath=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(20, LCID, 1, (3, 0), ((8, 0), (8, 0)),TankName
+			, FilePath)
+
+	def BuildEpocEv(self, Index=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, Value=defaultNamedNotOptArg
+			, BuddyEpoc=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(69, LCID, 1, (3, 0), ((3, 0), (8, 0), (5, 0), (5, 0), (8, 0)),Index
+			, TankCode, TimeStamp, Value, BuddyEpoc)
+
+	def BuildFilterDesc(self, TankCode=defaultNamedNotOptArg, TestCode=defaultNamedNotOptArg, V1=defaultNamedNotOptArg, V2=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(81, LCID, 1, (8, 0), ((3, 0), (3, 0), (5, 0), (5, 0)),TankCode
+			, TestCode, V1, V2)
+
+	def BuildScalar(self, Index=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg
+			, Value=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(68, LCID, 1, (3, 0), ((3, 0), (8, 0), (3, 0), (5, 0), (5, 0)),Index
+			, TankCode, SortChan, TimeStamp, Value)
+
+	def BuildSnipEv(self, Index=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, HasSort=defaultNamedNotOptArg
+			, pData=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(71, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (3, 0), (16388, 0)),Index
+			, SortChan, TimeStamp, HasSort, pData)
+
+	def BuildSnipEvV(self, Index=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, HasSort=defaultNamedNotOptArg
+			, vData=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(73, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (3, 0), (16396, 0)),Index
+			, SortChan, TimeStamp, HasSort, vData)
+
+	def BuildStreamEv(self, Index=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, pData=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(72, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (16388, 0)),Index
+			, SortChan, TimeStamp, pData)
+
+	def BuildStreamEvV(self, Index=defaultNamedNotOptArg, SortChan=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, vData=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(74, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (12, 0)),Index
+			, SortChan, TimeStamp, vData)
+
+	def CheckTank(self, TankName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(21, LCID, 1, (3, 0), ((8, 0),),TankName
+			)
+
+	def ClearEpocIndexing(self):
+		return self._oleobj_.InvokeTypes(85, LCID, 1, (24, 0), (),)
+
+	def CloseTank(self):
+		return self._oleobj_.InvokeTypes(22, LCID, 1, (24, 0), (),)
+
+	def CodeToString(self, EvCode=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(23, LCID, 1, (8, 0), ((3, 0),),EvCode
+			)
+
+	def ConnectServer(self, ServerName=defaultNamedNotOptArg, ClientName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(18, LCID, 1, (3, 0), ((8, 0), (8, 0)),ServerName
+			, ClientName)
+
+	def CreateEpocIndexing(self):
+		return self._oleobj_.InvokeTypes(84, LCID, 1, (3, 0), (),)
+
+	def DFromToString(self, DFormCode=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(27, LCID, 1, (8, 0), ((3, 0),),DFormCode
+			)
+
+	def DeleteClient(self, ClientName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(24, LCID, 1, (24, 0), ((8, 0),),ClientName
+			)
+
+	def DeleteSortCode(self, sortName=defaultNamedNotOptArg, snipName=defaultNamedNotOptArg, idxChan=defaultNamedNotOptArg):
+		"""method DeleteSortCode"""
+		return self._oleobj_.InvokeTypes(125, LCID, 1, (3, 0), ((8, 0), (8, 0), (3, 0)),sortName
+			, snipName, idxChan)
+
+	def DisableTankDebug(self, TankName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(34, LCID, 1, (24, 0), ((8, 0),),TankName
+			)
+
+	def EnableTankDebug(self, TankName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(33, LCID, 1, (24, 0), ((8, 0),),TankName
+			)
+
+	def EvTypeToString(self, evTypeCode=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(26, LCID, 1, (8, 0), ((3, 0),),evTypeCode
+			)
+
+	def FancyTime(self, Time=defaultNamedNotOptArg, Format=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(44, LCID, 1, (8, 0), ((5, 0), (8, 0)),Time
+			, Format)
+
+	def FromTTD(self, TTD=defaultNamedNotOptArg, FieldCode=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(54, LCID, 1, (8, 0), ((8, 0), (8, 0)),TTD
+			, FieldCode)
+
+	def GetClientID(self, ClientName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(35, LCID, 1, (3, 0), ((8, 0),),ClientName
+			)
+
+	def GetCodeSpecs(self, EvCode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(36, LCID, 1, (3, 0), ((3, 0),),EvCode
+			)
+
+	def GetCodeSpecsLazy(self, EvCode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(111, LCID, 1, (3, 0), ((3, 0),),EvCode
+			)
+
+	def GetDebug(self, TankName=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(28, LCID, 1, (8, 0), ((8, 0),),TankName
+			)
+
+	def GetEnumServer(self, Index=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(51, LCID, 1, (8, 0), ((3, 0),),Index
+			)
+
+	def GetEnumTank(self, Index=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(47, LCID, 1, (8, 0), ((3, 0),),Index
+			)
+
+	def GetEpocCode(self, Index=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(58, LCID, 1, (8, 0), ((3, 0),),Index
+			)
+
+	def GetEpocs(self, pEPs=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, T1=defaultNamedNotOptArg, T2=defaultNamedNotOptArg
+			, MaxRet=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(60, LCID, 1, (3, 0), ((16389, 0), (3, 0), (5, 0), (5, 0), (3, 0)),pEPs
+			, TankCode, T1, T2, MaxRet)
+
+	def GetEpocsEx(self, pEPs=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, MaxReturn=defaultNamedNotOptArg, Mode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(94, LCID, 1, (3, 0), ((16389, 0), (3, 0), (3, 0), (3, 0)),pEPs
+			, TankCode, MaxReturn, Mode)
+
+	def GetEpocsExV(self, TankCode=defaultNamedNotOptArg, Mode=defaultNamedNotOptArg):
+		return self._ApplyTypes_(95, 1, (12, 0), ((8, 0), (3, 0)), u'GetEpocsExV', None,TankCode
+			, Mode)
+
+	def GetEpocsV(self, TankCode=defaultNamedNotOptArg, T1=defaultNamedNotOptArg, T2=defaultNamedNotOptArg, MaxEpocs=defaultNamedNotOptArg):
+		return self._ApplyTypes_(57, 1, (12, 0), ((8, 0), (5, 0), (5, 0), (3, 0)), u'GetEpocsV', None,TankCode
+			, T1, T2, MaxEpocs)
+
+	def GetError(self):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(29, LCID, 1, (8, 0), (),)
+
+	def GetEvTsqIdx(self):
+		"""method GetEvTsqIdx"""
+		return self._ApplyTypes_(122, 1, (12, 0), (), u'GetEvTsqIdx', None,)
+
+	def GetEventCodes(self, EvType=defaultNamedNotOptArg):
+		return self._ApplyTypes_(38, 1, (12, 0), ((3, 0),), u'GetEventCodes', None,EvType
+			)
+
+	def GetFilterTolerance(self):
+		return self._oleobj_.InvokeTypes(87, LCID, 1, (5, 0), (),)
+
+	def GetGlobal(self, code=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(106, LCID, 1, (5, 0), ((3, 0),),code
+			)
+
+	def GetGlobalB(self, name=defaultNamedNotOptArg):
+		"""method GetGlobalB"""
+		return self._oleobj_.InvokeTypes(119, LCID, 1, (5, 0), ((8, 0),),name
+			)
+
+	def GetGlobalStringB(self, name=defaultNamedNotOptArg):
+		"""method GetGlobalStringB"""
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(120, LCID, 1, (8, 0), ((8, 0),),name
+			)
+
+	def GetGlobalStringV(self, name=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(108, LCID, 1, (8, 0), ((31, 0),),name
+			)
+
+	def GetGlobalV(self, name=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(107, LCID, 1, (5, 0), ((31, 0),),name
+			)
+
+	def GetHotBlock(self):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(66, LCID, 1, (8, 0), (),)
+
+	def GetNPer(self, DForm=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(59, LCID, 1, (3, 0), ((3, 0),),DForm
+			)
+
+	def GetServerItem(self, ServerName=defaultNamedNotOptArg, ItemCode=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(50, LCID, 1, (8, 0), ((8, 0), (8, 0)),ServerName
+			, ItemCode)
+
+	def GetSortChanMap(self, sortName=defaultNamedNotOptArg, snipName=defaultNamedNotOptArg):
+		"""method GetSortChanMap"""
+		return self._ApplyTypes_(126, 1, (12, 0), ((8, 0), (8, 0)), u'GetSortChanMap', None,sortName
+			, snipName)
+
+	def GetSortCondition(self, sortName=defaultNamedNotOptArg, snipName=defaultNamedNotOptArg, idxChan=defaultNamedNotOptArg):
+		"""method GetSortCondition"""
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(124, LCID, 1, (8, 0), ((8, 0), (8, 0), (3, 0)),sortName
+			, snipName, idxChan)
+
+	def GetSortName(self, EventName=defaultNamedNotOptArg, idxSortID=defaultNamedNotOptArg):
+		"""method GetSortName"""
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(113, LCID, 1, (8, 0), ((8, 0), (3, 0)),EventName
+			, idxSortID)
+
+	def GetStatus(self, StatCode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(39, LCID, 1, (3, 0), ((3, 0),),StatCode
+			)
+
+	def GetTankItem(self, TankName=defaultNamedNotOptArg, ItemCode=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(52, LCID, 1, (8, 0), ((8, 0), (8, 0)),TankName
+			, ItemCode)
+
+	def GetValidTimeRanges(self, pRanges=defaultNamedNotOptArg, MaxReturn=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(99, LCID, 1, (3, 0), ((16389, 0), (3, 0)),pRanges
+			, MaxReturn)
+
+	def GetValidTimeRangesV(self):
+		return self._ApplyTypes_(100, 1, (12, 0), (), u'GetValidTimeRangesV', None,)
+
+	def IndexEvent(self, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg, SortCode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(83, LCID, 1, (3, 0), ((3, 0), (3, 0), (3, 0)),TankCode
+			, Channel, SortCode)
+
+	def InitializeTank(self, TankName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(40, LCID, 1, (3, 0), ((8, 0),),TankName
+			)
+
+	def OpenTank(self, TankName=defaultNamedNotOptArg, AccessMode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(30, LCID, 1, (3, 0), ((8, 0), (8, 0)),TankName
+			, AccessMode)
+
+	def ParseEv(self, RecIndex=defaultNamedNotOptArg, TimeStamp=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg, SortCode=defaultNamedNotOptArg
+			, Npts=defaultNamedNotOptArg, pData=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(75, LCID, 1, (3, 0), ((3, 0), (16389, 0), (16387, 0), (16387, 0), (16387, 0), (16388, 0)),RecIndex
+			, TimeStamp, Channel, SortCode, Npts, pData
+			)
+
+	def ParseEvInfoV(self, RecIndex=defaultNamedNotOptArg, nRecs=defaultNamedNotOptArg, nItem=defaultNamedNotOptArg):
+		return self._ApplyTypes_(77, 1, (12, 0), ((3, 0), (3, 0), (3, 0)), u'ParseEvInfoV', None,RecIndex
+			, nRecs, nItem)
+
+	def ParseEvV(self, RecIndex=defaultNamedNotOptArg, nRecs=defaultNamedNotOptArg):
+		return self._ApplyTypes_(76, 1, (12, 0), ((3, 0), (3, 0)), u'ParseEvV', None,RecIndex
+			, nRecs)
+
+	def ParseFilterDesc(self, FiltDesc=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, TestCode=defaultNamedNotOptArg, V1=defaultNamedNotOptArg
+			, V2=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(80, LCID, 1, (3, 0), ((8, 0), (16387, 0), (16387, 0), (16389, 0), (16389, 0)),FiltDesc
+			, TankCode, TestCode, V1, V2)
+
+	def QryEpocAt(self, TankCode=defaultNamedNotOptArg, rTime=defaultNamedNotOptArg, ReqItem=defaultNamedNotOptArg, RetVal=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(64, LCID, 1, (3, 0), ((3, 0), (5, 0), (3, 0), (16389, 0)),TankCode
+			, rTime, ReqItem, RetVal)
+
+	def QryEpocAtV(self, TankCode=defaultNamedNotOptArg, rTime=defaultNamedNotOptArg, ReqItem=defaultNamedNotOptArg):
+		return self._ApplyTypes_(65, 1, (12, 0), ((8, 0), (5, 0), (3, 0)), u'QryEpocAtV', None,TankCode
+			, rTime, ReqItem)
+
+	def QueryBlockName(self, BlockNumber=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(41, LCID, 1, (8, 0), ((3, 0),),BlockNumber
+			)
+
+	def ReadEvents(self, MaxRet=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg, SortCode=defaultNamedNotOptArg
+			, T1=defaultNamedNotOptArg, T2=defaultNamedNotOptArg, Options=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(62, LCID, 1, (3, 0), ((3, 0), (3, 0), (3, 0), (3, 0), (5, 0), (5, 0), (3, 0)),MaxRet
+			, TankCode, Channel, SortCode, T1, T2
+			, Options)
+
+	def ReadEventsSimple(self, EventName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(96, LCID, 1, (3, 0), ((8, 0),),EventName
+			)
+
+	def ReadEventsV(self, MaxRet=defaultNamedNotOptArg, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg, SortCode=defaultNamedNotOptArg
+			, T1=defaultNamedNotOptArg, T2=defaultNamedNotOptArg, Options=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(63, LCID, 1, (3, 0), ((3, 0), (8, 0), (3, 0), (3, 0), (5, 0), (5, 0), (8, 0)),MaxRet
+			, TankCode, Channel, SortCode, T1, T2
+			, Options)
+
+	def ReadWaves(self, TankCode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(97, LCID, 1, (3, 0), ((3, 0),),TankCode
+			)
+
+	def ReadWavesOnTimeRange(self, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(101, LCID, 1, (3, 0), ((3, 0), (3, 0)),TankCode
+			, Channel)
+
+	def ReadWavesOnTimeRangeB(self, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg):
+		"""method ReadWavesOnTimeRangeB"""
+		return self._ApplyTypes_(116, 1, (12, 0), ((8, 0), (3, 0)), u'ReadWavesOnTimeRangeB', None,TankCode
+			, Channel)
+
+	def ReadWavesOnTimeRangeV(self, TankCode=defaultNamedNotOptArg, Channel=defaultNamedNotOptArg):
+		return self._ApplyTypes_(102, 1, (12, 0), ((31, 0), (3, 0)), u'ReadWavesOnTimeRangeV', None,TankCode
+			, Channel)
+
+	def ReadWavesV(self, TankCode=defaultNamedNotOptArg):
+		return self._ApplyTypes_(98, 1, (12, 0), ((8, 0),), u'ReadWavesV', None,TankCode
+			)
+
+	def ReleaseServer(self):
+		return self._oleobj_.InvokeTypes(42, LCID, 1, (24, 0), (),)
+
+	def RemoveBlock(self, BlockName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(56, LCID, 1, (3, 0), ((8, 0),),BlockName
+			)
+
+	def RemoveEvents(self, BlockName=defaultNamedNotOptArg, RelTime1=defaultNamedNotOptArg, RelTime2=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(55, LCID, 1, (3, 0), ((8, 0), (5, 0), (5, 0)),BlockName
+			, RelTime1, RelTime2)
+
+	def RemoveServer(self, ServerName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(49, LCID, 1, (3, 0), ((8, 0),),ServerName
+			)
+
+	def RemoveTank(self, TankName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(25, LCID, 1, (3, 0), ((8, 0),),TankName
+			)
+
+	def ResetFilters(self):
+		return self._oleobj_.InvokeTypes(82, LCID, 1, (24, 0), (),)
+
+	def ResetGlobals(self):
+		return self._oleobj_.InvokeTypes(110, LCID, 1, (24, 0), (),)
+
+	def ResetTank(self, TankName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(43, LCID, 1, (3, 0), ((8, 0),),TankName
+			)
+
+	def SaveSortCodes(self, sortName=defaultNamedNotOptArg, snipName=defaultNamedNotOptArg, idxChan=defaultNamedNotOptArg, sortCondition=defaultNamedNotOptArg
+			, sortCodeArray=defaultNamedNotOptArg):
+		"""method SaveSortCodes"""
+		return self._oleobj_.InvokeTypes(123, LCID, 1, (3, 0), ((8, 0), (8, 0), (3, 0), (8, 0), (12, 0)),sortName
+			, snipName, idxChan, sortCondition, sortCodeArray)
+
+	def SelectBlock(self, BlockName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(32, LCID, 1, (3, 0), ((8, 0),),BlockName
+			)
+
+	def SetBuildHead(self, TankCode=defaultNamedNotOptArg, DataForm=defaultNamedNotOptArg, SampFreq=defaultNamedNotOptArg, nNet=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(70, LCID, 1, (24, 0), ((8, 0), (3, 0), (5, 0), (3, 0)),TankCode
+			, DataForm, SampFreq, nNet)
+
+	def SetEpocTimeFilter(self, EpocCode=defaultNamedNotOptArg, Offset=defaultNamedNotOptArg, Dur=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(90, LCID, 1, (3, 0), ((3, 0), (5, 0), (5, 0)),EpocCode
+			, Offset, Dur)
+
+	def SetEpocTimeFilterB(self, EpocCode=defaultNamedNotOptArg, Offset=defaultNamedNotOptArg, Dur=defaultNamedNotOptArg):
+		"""method SetEpocTimeFilterB"""
+		return self._oleobj_.InvokeTypes(114, LCID, 1, (3, 0), ((8, 0), (5, 0), (5, 0)),EpocCode
+			, Offset, Dur)
+
+	def SetEpocTimeFilterV(self, EpocCode=defaultNamedNotOptArg, Offset=defaultNamedNotOptArg, Dur=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(91, LCID, 1, (3, 0), ((31, 0), (5, 0), (5, 0)),EpocCode
+			, Offset, Dur)
+
+	def SetFilter(self, TankCode=defaultNamedNotOptArg, TestCode=defaultNamedNotOptArg, V1=defaultNamedNotOptArg, V2=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(78, LCID, 1, (3, 0), ((3, 0), (3, 0), (5, 0), (5, 0)),TankCode
+			, TestCode, V1, V2)
+
+	def SetFilterArray(self, Dim=defaultNamedNotOptArg, ID=defaultNamedNotOptArg, Filter=defaultNamedNotOptArg, Exclusive=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(89, LCID, 1, (3, 0), ((3, 0), (3, 0), (8, 0), (3, 0)),Dim
+			, ID, Filter, Exclusive)
+
+	def SetFilterTolerance(self, loosenFactor=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(86, LCID, 1, (3, 0), ((5, 0),),loosenFactor
+			)
+
+	def SetFilterWithDesc(self, FiltDesc=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(79, LCID, 1, (3, 0), ((8, 0),),FiltDesc
+			)
+
+	def SetFilterWithDescEx(self, Filter=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(88, LCID, 1, (3, 0), ((8, 0),),Filter
+			)
+
+	def SetGlobal(self, code=defaultNamedNotOptArg, Value=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(103, LCID, 1, (3, 0), ((3, 0), (5, 0)),code
+			, Value)
+
+	def SetGlobalB(self, name=defaultNamedNotOptArg, Value=defaultNamedNotOptArg):
+		"""method SetGlobalB"""
+		return self._oleobj_.InvokeTypes(117, LCID, 1, (3, 0), ((8, 0), (5, 0)),name
+			, Value)
+
+	def SetGlobalStringB(self, name=defaultNamedNotOptArg, strvalue=defaultNamedNotOptArg):
+		"""method SetGlobalStringB"""
+		return self._oleobj_.InvokeTypes(118, LCID, 1, (3, 0), ((8, 0), (8, 0)),name
+			, strvalue)
+
+	def SetGlobalStringV(self, name=defaultNamedNotOptArg, strvalue=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(105, LCID, 1, (3, 0), ((31, 0), (31, 0)),name
+			, strvalue)
+
+	def SetGlobalV(self, name=defaultNamedNotOptArg, Value=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(104, LCID, 1, (3, 0), ((31, 0), (5, 0)),name
+			, Value)
+
+	def SetGlobals(self, str=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(109, LCID, 1, (3, 0), ((31, 0),),str
+			)
+
+	def SetGlobalsB(self, str=defaultNamedNotOptArg):
+		"""method SetGlobalsB"""
+		return self._oleobj_.InvokeTypes(121, LCID, 1, (3, 0), ((8, 0),),str
+			)
+
+	def SetRefEpoc(self, EpocCode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(92, LCID, 1, (3, 0), ((3, 0),),EpocCode
+			)
+
+	def SetRefEpocB(self, EpocCode=defaultNamedNotOptArg):
+		"""method SetRefEpocB"""
+		return self._oleobj_.InvokeTypes(115, LCID, 1, (3, 0), ((8, 0),),EpocCode
+			)
+
+	def SetRefEpocV(self, EpocCode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(93, LCID, 1, (3, 0), ((31, 0),),EpocCode
+			)
+
+	def SetRefTime(self, TimeOS=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(31, LCID, 1, (3, 0), ((5, 0),),TimeOS
+			)
+
+	def SetUseSortName(self, sortID=defaultNamedNotOptArg):
+		"""method SetUseSortName"""
+		return self._oleobj_.InvokeTypes(112, LCID, 1, (3, 0), ((8, 0),),sortID
+			)
+
+	def StartRecord(self, BlockName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(45, LCID, 1, (3, 0), ((8, 0),),BlockName
+			)
+
+	def StopRecord(self):
+		return self._oleobj_.InvokeTypes(46, LCID, 1, (24, 0), (),)
+
+	def StringToEvCode(self, EvCode=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(37, LCID, 1, (3, 0), ((8, 0),),EvCode
+			)
+
+	def SwitchClient(self, ClientName=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(67, LCID, 1, (3, 0), ((8, 0),),ClientName
+			)
+
+	def ToTTD(self, ServName=defaultNamedNotOptArg, TankName=defaultNamedNotOptArg, BlockName=defaultNamedNotOptArg, EvName=defaultNamedNotOptArg
+			, ChanList=defaultNamedNotOptArg):
+		# Result is a Unicode object
+		return self._oleobj_.InvokeTypes(53, LCID, 1, (8, 0), ((8, 0), (8, 0), (8, 0), (8, 0), (16387, 0)),ServName
+			, TankName, BlockName, EvName, ChanList)
+
+	def WriteEvents(self, NumEv=defaultNamedNotOptArg):
+		return self._oleobj_.InvokeTypes(61, LCID, 1, (3, 0), ((3, 0),),NumEv
+			)
+
+	_prop_map_get_ = {
+		"ClientID": (6, 2, (3, 0), (), "ClientID", None),
+		"CurBlockMemo": (3, 2, (8, 0), (), "CurBlockMemo", None),
+		"CurBlockName": (1, 2, (8, 0), (), "CurBlockName", None),
+		"CurBlockNotes": (17, 2, (8, 0), (), "CurBlockNotes", None),
+		"CurBlockOwner": (2, 2, (8, 0), (), "CurBlockOwner", None),
+		"CurBlockStartTime": (4, 2, (5, 0), (), "CurBlockStartTime", None),
+		"CurBlockStopTime": (5, 2, (5, 0), (), "CurBlockStopTime", None),
+		"Domain": (15, 2, (8, 0), (), "Domain", None),
+		"EvChannel": (13, 2, (3, 0), (), "EvChannel", None),
+		"EvDForm": (10, 2, (3, 0), (), "EvDForm", None),
+		"EvDataSize": (8, 2, (3, 0), (), "EvDataSize", None),
+		"EvFirstTime": (9, 2, (5, 0), (), "EvFirstTime", None),
+		"EvSampFreq": (11, 2, (4, 0), (), "EvSampFreq", None),
+		"EvTimeStamp": (12, 2, (5, 0), (), "EvTimeStamp", None),
+		"EvType": (7, 2, (3, 0), (), "EvType", None),
+		"Password": (16, 2, (8, 0), (), "Password", None),
+		"Username": (14, 2, (8, 0), (), "Username", None),
+	}
+	_prop_map_put_ = {
+		"ClientID" : ((6, LCID, 4, 0),()),
+		"CurBlockMemo" : ((3, LCID, 4, 0),()),
+		"CurBlockName" : ((1, LCID, 4, 0),()),
+		"CurBlockNotes" : ((17, LCID, 4, 0),()),
+		"CurBlockOwner" : ((2, LCID, 4, 0),()),
+		"CurBlockStartTime" : ((4, LCID, 4, 0),()),
+		"CurBlockStopTime" : ((5, LCID, 4, 0),()),
+		"Domain" : ((15, LCID, 4, 0),()),
+		"EvChannel" : ((13, LCID, 4, 0),()),
+		"EvDForm" : ((10, LCID, 4, 0),()),
+		"EvDataSize" : ((8, LCID, 4, 0),()),
+		"EvFirstTime" : ((9, LCID, 4, 0),()),
+		"EvSampFreq" : ((11, LCID, 4, 0),()),
+		"EvTimeStamp" : ((12, LCID, 4, 0),()),
+		"EvType" : ((7, LCID, 4, 0),()),
+		"Password" : ((16, LCID, 4, 0),()),
+		"Username" : ((14, LCID, 4, 0),()),
+	}
+
+class _DTTankXEvents:
+	"""Event interface for TTankX Control"""
+	CLSID = CLSID_Sink = IID('{9C0BD59B-8842-47DA-8105-DC3E883D72D1}')
+	coclass_clsid = IID('{670490CE-57D2-4176-8E74-80C4C6A47D88}')
+	_public_methods_ = [] # For COM Server support
+	_dispid_to_func_ = {
+		}
+
+	def __init__(self, oobj = None):
+		if oobj is None:
+			self._olecp = None
+		else:
+			import win32com.server.util
+			from win32com.server.policy import EventHandlerPolicy
+			cpc=oobj._oleobj_.QueryInterface(pythoncom.IID_IConnectionPointContainer)
+			cp=cpc.FindConnectionPoint(self.CLSID_Sink)
+			cookie=cp.Advise(win32com.server.util.wrap(self, usePolicy=EventHandlerPolicy))
+			self._olecp,self._olecp_cookie = cp,cookie
+	def __del__(self):
+		try:
+			self.close()
+		except pythoncom.com_error:
+			pass
+	def close(self):
+		if self._olecp is not None:
+			cp,cookie,self._olecp,self._olecp_cookie = self._olecp,self._olecp_cookie,None,None
+			cp.Unadvise(cookie)
+	def _query_interface_(self, iid):
+		import win32com.server.util
+		if iid==self.CLSID_Sink: return win32com.server.util.wrap(self)
+
+	# Event Handlers
+	# If you create handlers, they should have the following prototypes:
+
+
+from win32com.client import CoClassBaseClass
+# This CoClass is known by the name 'TTANK.X'
+class TTankX(CoClassBaseClass): # A CoClass
+	# TTankX Control
+	CLSID = IID('{670490CE-57D2-4176-8E74-80C4C6A47D88}')
+	coclass_sources = [
+		_DTTankXEvents,
+	]
+	default_source = _DTTankXEvents
+	coclass_interfaces = [
+		_DTTankX,
+	]
+	default_interface = _DTTankX
+
+RecordMap = {
+}
+
+CLSIDToClassMap = {
+	'{670490CE-57D2-4176-8E74-80C4C6A47D88}' : TTankX,
+	'{9C0BD59B-8842-47DA-8105-DC3E883D72D1}' : _DTTankXEvents,
+	'{BE6CAD3F-28F1-4EAC-B210-9CAA5CA8B5B8}' : _DTTankX,
+}
+CLSIDToPackageMap = {}
+win32com.client.CLSIDToClass.RegisterCLSIDsFromDict( CLSIDToClassMap )
+VTablesToPackageMap = {}
+VTablesToClassMap = {
+}
+
+
+NamesToIIDMap = {
+	'_DTTankX' : '{BE6CAD3F-28F1-4EAC-B210-9CAA5CA8B5B8}',
+	'_DTTankXEvents' : '{9C0BD59B-8842-47DA-8105-DC3E883D72D1}',
+}
+
+
```

### Comparing `TDTPy-0.8.1/tdt/actxobjects/ZBUSx.py` & `TDTPy-0.9.0/tdt/actxobjects/ZBUSx.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/actxobjects/__init__.py` & `TDTPy-0.9.0/tdt/actxobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/components/data_reduction.rcx` & `TDTPy-0.9.0/tdt/components/data_reduction.rcx`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/components/test_RZ6_audio_out.rcx` & `TDTPy-0.9.0/tdt/components/test_RZ6_audio_out.rcx`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/components/test_physiology_RZ5.rcx` & `TDTPy-0.9.0/tdt/components/test_physiology_RZ5.rcx`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/components/test_physiology_RZ6.rcx` & `TDTPy-0.9.0/tdt/components/test_physiology_RZ6.rcx`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/components/test_read.rcx` & `TDTPy-0.9.0/tdt/components/test_read.rcx`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/constants.py` & `TDTPy-0.9.0/tdt/constants.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/convert.py` & `TDTPy-0.9.0/tdt/convert.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,125 +1,125 @@
-def ispow2(n):
-    '''
-    True if n is a power of 2, False otherwise
-
-    >>> ispow2(5)
-    False
-    >>> ispow2(4)
-    True
-    '''
-    return (n & (n-1)) == 0
-
-
-def nextpow2(n):
-    '''
-    Given n, return the nearest power of two that is >= n
-
-    >>> nextpow2(1)
-    1
-    >>> nextpow2(2)
-    2
-    >>> nextpow2(5)
-    8
-    >>> nextpow2(17)
-    32
-    '''
-    if ispow2(n):
-        return n
-
-    count = 0
-    while n != 0:
-        n = n >> 1
-        count += 1
-    return 1 << count
-
-
-class SamplingRateError(ValueError):
-    '''
-    Indicates that the conversion of frequency to sampling rate could not be
-    performed.
-    '''
-
-    def __init__(self, fs, requested_fs):
-        self.fs = fs
-        self.requested_fs = requested_fs
-
-    def __str__(self):
-        mesg = 'The requested sampling rate, %f Hz, is greater than ' + \
-               'the DSP clock frequency of %f Hz.'
-        return mesg % (self.requested_fs, self.fs)
-
-
-def convert(src_unit, dest_unit, value, dsp_fs):
-    '''
-    Converts value to desired unit give the sampling frequency of the DSP.
-
-    Parameters specified in paradigms are typically expressed as
-    frequency and time while many DSP parameters are expressed in number of
-    samples (referenced to the DSP sampling frequency).  This function provides
-    a convenience method for converting between conventional values and the
-    'digital' values used by the DSP.
-
-    Note that for converting units of time/frequency to n/nPer, we have to
-    coerce the value to a multiple of the DSP period (e.g. the number of
-    'ticks' of the DSP clock).
-
-    Appropriate strings for the unit types:
-
-        fs
-            sampling frequency
-        nPer
-            number of samples per period
-        n
-            number of samples
-        s
-            seconds
-        ms
-            milliseconds
-        nPow2
-            number of samples, coerced to the next greater power of 2 (used for
-            ensuring efficient FFT computation)
-
-    >>> convert('s', 'n', 0.5, 10000)
-    5000
-    >>> convert('fs', 'nPer', 500, 10000)
-    20
-    >>> convert('s', 'nPow2', 5, 97.5e3)
-    524288
-
-    Parameters
-    ----------
-    src_unit: string
-    dest_unit: string
-        Destination unit
-    value: numerical (e.g. integer or float)
-        Value to be converted
-
-    Returns
-    -------
-    converted unit : numerical value
-    '''
-    def fs_to_nPer(req_fs, dsp_fs):
-        if dsp_fs < req_fs:
-            raise SamplingRateError(dsp_fs, req_fs)
-        return int(dsp_fs/req_fs)
-
-    def nPer_to_fs(nPer, dsp_fs):
-        return dsp_fs/nPer
-
-    def n_to_s(n, dsp_fs):
-        return n/dsp_fs
-
-    def s_to_n(s, dsp_fs):
-        return int(s*dsp_fs)
-
-    def ms_to_n(ms, dsp_fs):
-        return int(ms*1e-3*dsp_fs)
-
-    def n_to_ms(n, dsp_fs):
-        return n/dsp_fs*1e3
-
-    def s_to_nPow2(s, dsp_fs):
-        return nextpow2(s_to_n(s, dsp_fs))
-
-    fun = '%s_to_%s' % (src_unit, dest_unit)
-    return locals()[fun](value, dsp_fs)
+def ispow2(n):
+    '''
+    True if n is a power of 2, False otherwise
+
+    >>> ispow2(5)
+    False
+    >>> ispow2(4)
+    True
+    '''
+    return (n & (n-1)) == 0
+
+
+def nextpow2(n):
+    '''
+    Given n, return the nearest power of two that is >= n
+
+    >>> nextpow2(1)
+    1
+    >>> nextpow2(2)
+    2
+    >>> nextpow2(5)
+    8
+    >>> nextpow2(17)
+    32
+    '''
+    if ispow2(n):
+        return n
+
+    count = 0
+    while n != 0:
+        n = n >> 1
+        count += 1
+    return 1 << count
+
+
+class SamplingRateError(ValueError):
+    '''
+    Indicates that the conversion of frequency to sampling rate could not be
+    performed.
+    '''
+
+    def __init__(self, fs, requested_fs):
+        self.fs = fs
+        self.requested_fs = requested_fs
+
+    def __str__(self):
+        mesg = 'The requested sampling rate, %f Hz, is greater than ' + \
+               'the DSP clock frequency of %f Hz.'
+        return mesg % (self.requested_fs, self.fs)
+
+
+def convert(src_unit, dest_unit, value, dsp_fs):
+    '''
+    Converts value to desired unit give the sampling frequency of the DSP.
+
+    Parameters specified in paradigms are typically expressed as
+    frequency and time while many DSP parameters are expressed in number of
+    samples (referenced to the DSP sampling frequency).  This function provides
+    a convenience method for converting between conventional values and the
+    'digital' values used by the DSP.
+
+    Note that for converting units of time/frequency to n/nPer, we have to
+    coerce the value to a multiple of the DSP period (e.g. the number of
+    'ticks' of the DSP clock).
+
+    Appropriate strings for the unit types:
+
+        fs
+            sampling frequency
+        nPer
+            number of samples per period
+        n
+            number of samples
+        s
+            seconds
+        ms
+            milliseconds
+        nPow2
+            number of samples, coerced to the next greater power of 2 (used for
+            ensuring efficient FFT computation)
+
+    >>> convert('s', 'n', 0.5, 10000)
+    5000
+    >>> convert('fs', 'nPer', 500, 10000)
+    20
+    >>> convert('s', 'nPow2', 5, 97.5e3)
+    524288
+
+    Parameters
+    ----------
+    src_unit: string
+    dest_unit: string
+        Destination unit
+    value: numerical (e.g. integer or float)
+        Value to be converted
+
+    Returns
+    -------
+    converted unit : numerical value
+    '''
+    def fs_to_nPer(req_fs, dsp_fs):
+        if dsp_fs < req_fs:
+            raise SamplingRateError(dsp_fs, req_fs)
+        return int(dsp_fs/req_fs)
+
+    def nPer_to_fs(nPer, dsp_fs):
+        return dsp_fs/nPer
+
+    def n_to_s(n, dsp_fs):
+        return n/dsp_fs
+
+    def s_to_n(s, dsp_fs):
+        return int(s*dsp_fs)
+
+    def ms_to_n(ms, dsp_fs):
+        return int(ms*1e-3*dsp_fs)
+
+    def n_to_ms(n, dsp_fs):
+        return n/dsp_fs*1e3
+
+    def s_to_nPow2(s, dsp_fs):
+        return nextpow2(s_to_n(s, dsp_fs))
+
+    fun = '%s_to_%s' % (src_unit, dest_unit)
+    return locals()[fun](value, dsp_fs)
```

### Comparing `TDTPy-0.8.1/tdt/device/RZ6.py` & `TDTPy-0.9.0/tdt/device/RZ6.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/dsp_buffer.py` & `TDTPy-0.9.0/tdt/dsp_buffer.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,84 +31,48 @@
         'dec_tag', 'src_type', 'dest_type', 'compression', 'resolution',
         'sf', 'dec_factor', 'fs', 'n_slots', 'n_samples', 'size',
         'n_slots_max', 'n_samples_max', 'size_max', 'channels',
         'block_size']
 
     def __init__(self, circuit, data_tag, idx_tag=None, size_tag=None,
                  sf_tag=None, cycle_tag=None, dec_tag=None, block_size=1,
-                 src_type='float32', dest_type='float32', channels=1):
+                 src_type='float32', dest_type='float32', channels=1,
+                 dec_factor=None):
 
         if data_tag not in circuit.tags:
             raise ValueError("%s: Does not have data tag %s"
                              % (circuit, data_tag))
         elif not circuit.tags[data_tag][1] == RCX_BUFFER:
             raise ValueError("Tag %s is not a buffer tag" % data_tag)
 
         self.circuit = circuit
         self._iface = circuit._iface
         self._zbus = circuit._zbus
         self.data_tag = data_tag
-        self.size_tag = size_tag
         self.channels = channels
         self.block_size = int(block_size)
 
-        if size_tag is None:
-            tag = data_tag + '_n'
-            if tag in circuit.tags:
-                size_tag = tag
-                log.debug("%s: found size_tag %s", self, self.size_tag)
-        elif size_tag not in circuit.tags:
-            raise ValueError("size_tag not found in circuit")
-        self.size_tag = size_tag
-
-        if idx_tag is None:
-            idx_tag = data_tag + '_i'
-            log.debug("%s: attempting to find idx_tag %s", self, idx_tag)
-        if idx_tag not in circuit.tags:
-            raise ValueError("Index tag must be present in circuit")
-        self.idx_tag = idx_tag
-
-        # Determine scaling factor if the scaling_factor tag is available
-        if sf_tag is None:
-            tag = data_tag + '_sf'
-            if tag in circuit.tags:
-                sf_tag = tag
-                log.debug("%s: found sf_tag %s", self, sf_tag)
-        self.sf_tag = sf_tag
-        if self.sf_tag is not None:
-            self.sf = self.circuit.get_tag(self.sf_tag)
-            log.debug("%s: scaling factor is %d", self, self.sf)
-        else:
-            self.sf = 1
-            log.debug("%s: no scaling factor found, using default", self)
-
-        if cycle_tag is None:
-            tag = data_tag + '_c'
-            if tag in circuit.tags:
-                cycle_tag = tag
-                log.debug("%s: found cycle_tag %s", self, cycle_tag)
-            else:
-                log.debug("%s: no cycle tag found", self)
-        self.cycle_tag = cycle_tag
-
-        # Compute sampling frequency of data stored in buffer given the
-        # decimation factor
-        if dec_tag is None:
-            tag = data_tag + '_d'
-            if tag in circuit.tags:
-                dec_tag = tag
-                log.debug("%s: found dec_tag %s", self, dec_tag)
-        self.dec_tag = dec_tag
-        if self.dec_tag is not None:
-            self.dec_factor = self.circuit.get_tag(self.dec_tag)
-            self.fs = circuit.fs/float(self.dec_factor)
-        else:
-            self.dec_factor = 1
-            self.fs = circuit.fs
-        log.debug("%s: decimation factor is %d", self, self.dec_factor)
+        self.size_tag = self.find_tag(size_tag, '_n', True, 'size')
+        self.idx_tag = self.find_tag(idx_tag, '_i', True, 'index')
+        self.sf_tag = self.find_tag(sf_tag, '_sf', False, 'scaling factor')
+        self.cycle_tag = self.find_tag(cycle_tag, '_c', False, 'cycles')
+        self.dec_tag = self.find_tag(dec_tag, '_d', False, 'decimation')
+        self.sf = self.get_tag(self.sf_tag, 1, 'scaling factor')
+
+        if dec_factor is not None:
+            if self.dec_tag is not None:
+                self.circuit.set_tag(self.dec_tag, dec_factor)
+            elif dec_factor != 1:
+                m = 'Decimation tag for %s must be available to set ' \
+                    'decimation factor to %d' % (self.data_tag, dec_factor)
+                raise ValueError(m)
+
+        self.dec_factor = self.get_tag(self.dec_tag, 1, 'decimation factor')
+        self.fs = circuit.fs / float(self.dec_factor)
+        log.debug('%s: Sampling rate %f', self, self.fs)
 
         # Numpy's dtype function is quite powerful and accepts a variety of
         # strings as well as other dtype objects and returns the right answer.
         self.src_type = np.dtype(src_type)
         self.dest_type = np.dtype(dest_type)
 
         # Number of samples compressed into a single slot.  The RPvds works
@@ -143,14 +107,84 @@
         if (self.n_slots % self.channels) != 0:
             mesg = 'Buffer size must be a multiple of the channel number'
             raise DSPError(self, mesg)
 
         # Spit out debugging information
         log.debug('Initialized %s', self._get_debug_info())
 
+    def find_tag(self, tag, default_prefix, required, name):
+        '''
+        Locates tag that tracks a feature of the buffer
+
+        Parameters
+        ----------
+        tag : {None, str}
+            Name provided by the end-user code
+        default_prefix : str
+            Prefix to append to the data tag name to create the default tag
+            name for the feature.
+        required : bool
+            If the tag is required and it is missing, raise an error.
+            Otherwise, return None.
+        name : str
+            What the tag represents. Used by the logging and exception
+            machinery to create a useful message.
+
+        Returns
+        -------
+        tag_name : {None, str}
+            Name of tag. If no tag found and it is not required, return None.
+
+        Raises
+        ------
+        ValueError
+            If tag cannot be found and it is required.
+        '''
+        # If no name was provided create a default one.
+        if tag is None:
+            tag = self.data_tag + default_prefix
+
+        # If tag exists, return it.
+        if tag in self.circuit.tags:
+            log.debug("%s: found %s tag %s", self, name, tag)
+            return tag
+
+        # If we have reached this point, the tag is missing. If it was
+        # required, raise an error.
+        if required:
+            m = '%s tag for %s must be present in circuit' % (name, self)
+            raise ValueError(m)
+        log.debug('%s: no tag found for %s', self, name)
+
+    def get_tag(self, tag, default, name):
+        '''
+        Returns value of tag that tracks a feature of the buffer
+
+        Parameters
+        ----------
+        tag : {None, str}
+            Name provided by the end-user code
+        default : {int, float}
+            Default value of feature if tag is missing.
+        name : str
+            What the tag represents. Used by the logging and exception
+            machinery to create a useful message.
+
+        Returns
+        -------
+        value : {int, float}
+            Value of tag. If no tag is present, default is returned.
+        '''
+        if tag is None:
+            log.debug('%s: %s is %r (default)', self, name, default)
+            return default
+        value = self.circuit.get_tag(tag)
+        log.debug('%s: %s is %r', self, name, value)
+        return value
+
     def _get_debug_info(self):
         attr_strings = ['{0}: {1}'.format(*a)
                         for a in self.attributes().items()]
         return '%s: %s' % (self, ', '.join(attr_strings))
 
     def attributes(self, attributes=None):
         if attributes is None:
```

### Comparing `TDTPy-0.8.1/tdt/dsp_circuit.py` & `TDTPy-0.9.0/tdt/dsp_circuit.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/dsp_process.py` & `TDTPy-0.9.0/tdt/dsp_process.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/dsp_project.py` & `TDTPy-0.9.0/tdt/dsp_project.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/dsp_server.py` & `TDTPy-0.9.0/tdt/dsp_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from six.moves import cStringIO as StringIO, cPickle as pickle
+from io import StringIO
+import pickle
 from tempfile import NamedTemporaryFile
 import uuid
 import socket
 import struct
 from select import select
 import numpy as np
 import logging
```

### Comparing `TDTPy-0.8.1/tdt/shared_ring_buffer.py` & `TDTPy-0.9.0/tdt/shared_ring_buffer.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/test_io_speed.py` & `TDTPy-0.9.0/tdt/test_io_speed.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/test_process.py` & `TDTPy-0.9.0/tdt/test_process.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/tests.py` & `TDTPy-0.9.0/tdt/tests.py`

 * *Files identical despite different names*

### Comparing `TDTPy-0.8.1/tdt/util.py` & `TDTPy-0.9.0/tdt/util.py`

 * *Files identical despite different names*

