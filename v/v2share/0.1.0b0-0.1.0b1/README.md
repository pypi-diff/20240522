# Comparing `tmp/v2share-0.1.0b0.tar.gz` & `tmp/v2share-0.1.0b1.tar.gz`

## Comparing `v2share-0.1.0b0.tar` & `v2share-0.1.0b1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0b0/requirements.txt
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0b0/.github/workflows/python-tests.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0b0/tests/__init__.py
--rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 v2share-0.1.0b0/tests/test_links.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/__init__.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/_version.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/clash.py
--rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/clashmeta.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/data.py
--rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/singbox.py
--rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/xray.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/templates/clash.yml
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/templates/singbox.json
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/templates/xray.json
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 v2share-0.1.0b0/v2share/templates/xray_mux.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0b0/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0b0/README.md
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 v2share-0.1.0b1/requirements.txt
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 v2share-0.1.0b1/.github/workflows/python-tests.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     1841 2020-02-02 00:00:00.000000 v2share-0.1.0b1/tests/test_links.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/__init__.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/_version.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/clash.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/clashmeta.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/data.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/links.py
+-rw-r--r--   0        0        0     6752 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/singbox.py
+-rw-r--r--   0        0        0    11033 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/xray.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/templates/clash.yml
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/templates/singbox.json
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/templates/xray.json
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 v2share-0.1.0b1/v2share/templates/xray_mux.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 v2share-0.1.0b1/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 v2share-0.1.0b1/README.md
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 v2share-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 v2share-0.1.0b1/PKG-INFO
```

### Comparing `v2share-0.1.0b0/.github/workflows/python-tests.yml` & `v2share-0.1.0b1/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/tests/test_links.py` & `v2share-0.1.0b1/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/v2share/clash.py` & `v2share-0.1.0b1/v2share/clash.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/v2share/clashmeta.py` & `v2share-0.1.0b1/v2share/clashmeta.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/v2share/data.py` & `v2share-0.1.0b1/v2share/data.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/v2share/singbox.py` & `v2share-0.1.0b1/v2share/singbox.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/v2share/xray.py` & `v2share-0.1.0b1/v2share/xray.py`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/v2share/templates/singbox.json` & `v2share-0.1.0b1/v2share/templates/singbox.json`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/v2share/templates/xray.json` & `v2share-0.1.0b1/v2share/templates/xray.json`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/.gitignore` & `v2share-0.1.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `v2share-0.1.0b0/pyproject.toml` & `v2share-0.1.0b1/pyproject.toml`

 * *Files identical despite different names*

