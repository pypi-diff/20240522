# Comparing `tmp/aepo-0.1.3.tar.gz` & `tmp/aepo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aepo-0.1.3.tar", max compression
+gzip compressed data, was "aepo-0.1.4.tar", max compression
```

## Comparing `aepo-0.1.3.tar` & `aepo-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rwxr-xr-x   0        0        0     1074 2024-05-13 01:25:24.936000 aepo-0.1.3/LICENSE
--rwxr-xr-x   0        0        0      638 2024-05-15 08:48:40.716000 aepo-0.1.3/aepo/Makefile
--rwxr-xr-x   0        0        0       22 2024-05-13 06:47:06.243000 aepo-0.1.3/aepo/__init__.py
--rwxr-xr-x   0        0        0     6613 2024-05-15 10:09:09.810000 aepo-0.1.3/aepo/cli.py
--rwxr-xr-x   0        0        0      804 2024-05-15 08:48:40.731000 aepo-0.1.3/aepo/make.bat
--rwxr-xr-x   0        0        0        0 2024-05-13 01:21:42.945000 aepo-0.1.3/aepo/mbr/__init__.py
--rwxr-xr-x   0        0        0      144 2024-05-15 08:55:14.860000 aepo-0.1.3/aepo/mbr/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     2833 2024-05-15 09:05:56.140000 aepo-0.1.3/aepo/mbr/__pycache__/mbr_engine.cpython-310.pyc
--rwxr-xr-x   0        0        0     2792 2024-05-15 09:05:59.908000 aepo-0.1.3/aepo/mbr/__pycache__/reward_engine.cpython-310.pyc
--rwxr-xr-x   0        0        0    11661 2024-05-15 09:05:59.973000 aepo-0.1.3/aepo/mbr/__pycache__/reward_model.cpython-310.pyc
--rwxr-xr-x   0        0        0     3011 2024-05-15 09:05:57.218000 aepo-0.1.3/aepo/mbr/__pycache__/utility_func.cpython-310.pyc
--rwxr-xr-x   0        0        0     2997 2024-05-15 09:01:33.636000 aepo-0.1.3/aepo/mbr/mbr_engine.py
--rwxr-xr-x   0        0        0        0 2024-05-13 01:21:43.086000 aepo-0.1.3/aepo/mbr/policy/__init__.py
--rwxr-xr-x   0        0        0      151 2024-05-15 08:55:21.375000 aepo-0.1.3/aepo/mbr/policy/__pycache__/__init__.cpython-310.pyc
--rwxr-xr-x   0        0        0     4244 2024-05-15 08:55:21.521000 aepo-0.1.3/aepo/mbr/policy/__pycache__/diverse_mbr.cpython-310.pyc
--rwxr-xr-x   0        0        0     1910 2024-05-15 09:05:59.814000 aepo-0.1.3/aepo/mbr/policy/__pycache__/mbr.cpython-310.pyc
--rwxr-xr-x   0        0        0     4828 2024-05-15 08:36:47.107000 aepo-0.1.3/aepo/mbr/policy/diverse_mbr.py
--rwxr-xr-x   0        0        0     2040 2024-05-15 09:00:03.657000 aepo-0.1.3/aepo/mbr/policy/mbr.py
--rwxr-xr-x   0        0        0     2728 2024-05-15 09:03:59.289000 aepo-0.1.3/aepo/mbr/reward_engine.py
--rwxr-xr-x   0        0        0    12493 2024-05-15 09:04:12.762000 aepo-0.1.3/aepo/mbr/reward_model.py
--rwxr-xr-x   0        0        0     8001 2024-05-15 09:05:26.497000 aepo-0.1.3/aepo/mbr/utility_func.py
--rwxr-xr-x   0        0        0     2656 2024-05-15 08:39:25.164000 aepo-0.1.3/aepo/preprocess.py
--rwxr-xr-x   0        0        0      542 2024-05-13 01:21:51.271000 aepo-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      708 1970-01-01 00:00:00.000000 aepo-0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1074 2024-05-13 01:25:24.936000 aepo-0.1.4/LICENSE
+-rwxr-xr-x   0        0        0     3245 2024-05-13 07:13:07.938000 aepo-0.1.4/README.md
+-rwxr-xr-x   0        0        0      638 2024-05-15 08:48:40.706000 aepo-0.1.4/aepo/Makefile
+-rwxr-xr-x   0        0        0       22 2024-05-13 06:47:12.539000 aepo-0.1.4/aepo/__init__.py
+-rwxr-xr-x   0        0        0     6613 2024-05-15 10:09:17.525000 aepo-0.1.4/aepo/cli.py
+-rwxr-xr-x   0        0        0      804 2024-05-15 08:48:40.721000 aepo-0.1.4/aepo/make.bat
+-rwxr-xr-x   0        0        0        0 2024-05-13 01:21:42.945000 aepo-0.1.4/aepo/mbr/__init__.py
+-rwxr-xr-x   0        0        0      144 2024-05-15 08:55:14.869000 aepo-0.1.4/aepo/mbr/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2833 2024-05-15 09:06:06.113000 aepo-0.1.4/aepo/mbr/__pycache__/mbr_engine.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2792 2024-05-15 09:06:12.067000 aepo-0.1.4/aepo/mbr/__pycache__/reward_engine.cpython-310.pyc
+-rwxr-xr-x   0        0        0    11661 2024-05-15 09:06:14.176000 aepo-0.1.4/aepo/mbr/__pycache__/reward_model.cpython-310.pyc
+-rwxr-xr-x   0        0        0     3011 2024-05-15 09:06:08.087000 aepo-0.1.4/aepo/mbr/__pycache__/utility_func.cpython-310.pyc
+-rwxr-xr-x   0        0        0     2997 2024-05-15 09:01:40.322000 aepo-0.1.4/aepo/mbr/mbr_engine.py
+-rwxr-xr-x   0        0        0        0 2024-05-13 01:21:43.086000 aepo-0.1.4/aepo/mbr/policy/__init__.py
+-rwxr-xr-x   0        0        0      151 2024-05-15 08:55:21.386000 aepo-0.1.4/aepo/mbr/policy/__pycache__/__init__.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4244 2024-05-15 08:55:21.532000 aepo-0.1.4/aepo/mbr/policy/__pycache__/diverse_mbr.cpython-310.pyc
+-rwxr-xr-x   0        0        0     1910 2024-05-15 09:06:10.053000 aepo-0.1.4/aepo/mbr/policy/__pycache__/mbr.cpython-310.pyc
+-rwxr-xr-x   0        0        0     4828 2024-05-15 08:36:55.367000 aepo-0.1.4/aepo/mbr/policy/diverse_mbr.py
+-rwxr-xr-x   0        0        0     2040 2024-05-15 09:00:10.253000 aepo-0.1.4/aepo/mbr/policy/mbr.py
+-rwxr-xr-x   0        0        0     2728 2024-05-15 09:04:05.830000 aepo-0.1.4/aepo/mbr/reward_engine.py
+-rwxr-xr-x   0        0        0    12493 2024-05-15 09:04:19.342000 aepo-0.1.4/aepo/mbr/reward_model.py
+-rwxr-xr-x   0        0        0     8001 2024-05-15 09:05:33.205000 aepo-0.1.4/aepo/mbr/utility_func.py
+-rwxr-xr-x   0        0        0     2656 2024-05-15 08:39:32.300000 aepo-0.1.4/aepo/preprocess.py
+-rwxr-xr-x   0        0        0      712 2024-05-22 02:31:53.761000 aepo-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4309 2024-05-22 02:32:11.631355 aepo-0.1.4/setup.py
+-rw-r--r--   0        0        0     4184 2024-05-22 02:32:11.632192 aepo-0.1.4/PKG-INFO
```

### Comparing `aepo-0.1.3/LICENSE` & `aepo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/Makefile` & `aepo-0.1.4/aepo/Makefile`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/cli.py` & `aepo-0.1.4/aepo/cli.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/make.bat` & `aepo-0.1.4/aepo/make.bat`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/__pycache__/mbr_engine.cpython-310.pyc` & `aepo-0.1.4/aepo/mbr/__pycache__/mbr_engine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/__pycache__/reward_engine.cpython-310.pyc` & `aepo-0.1.4/aepo/mbr/__pycache__/reward_engine.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/__pycache__/reward_model.cpython-310.pyc` & `aepo-0.1.4/aepo/mbr/__pycache__/reward_model.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/__pycache__/utility_func.cpython-310.pyc` & `aepo-0.1.4/aepo/mbr/__pycache__/utility_func.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/mbr_engine.py` & `aepo-0.1.4/aepo/mbr/mbr_engine.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/policy/__pycache__/diverse_mbr.cpython-310.pyc` & `aepo-0.1.4/aepo/mbr/policy/__pycache__/diverse_mbr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/policy/__pycache__/mbr.cpython-310.pyc` & `aepo-0.1.4/aepo/mbr/policy/__pycache__/mbr.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/policy/diverse_mbr.py` & `aepo-0.1.4/aepo/mbr/policy/diverse_mbr.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/policy/mbr.py` & `aepo-0.1.4/aepo/mbr/policy/mbr.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/reward_engine.py` & `aepo-0.1.4/aepo/mbr/reward_engine.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/reward_model.py` & `aepo-0.1.4/aepo/mbr/reward_model.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/mbr/utility_func.py` & `aepo-0.1.4/aepo/mbr/utility_func.py`

 * *Files identical despite different names*

### Comparing `aepo-0.1.3/aepo/preprocess.py` & `aepo-0.1.4/aepo/preprocess.py`

 * *Files identical despite different names*

