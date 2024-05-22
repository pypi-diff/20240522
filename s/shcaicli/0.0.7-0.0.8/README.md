# Comparing `tmp/shcaicli-0.0.7.tar.gz` & `tmp/shcaicli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shcaicli-0.0.7.tar", last modified: Sat Jan 13 14:19:48 2024, max compression
+gzip compressed data, was "shcaicli-0.0.8.tar", last modified: Wed May 22 14:14:46 2024, max compression
```

## Comparing `shcaicli-0.0.7.tar` & `shcaicli-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 14:19:48.911347 shcaicli-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-13 14:19:42.000000 shcaicli-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-01-13 14:19:48.911347 shcaicli-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-01-13 14:19:42.000000 shcaicli-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-13 14:19:42.000000 shcaicli-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 14:19:48.911347 shcaicli-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-13 14:19:42.000000 shcaicli-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 14:19:48.911347 shcaicli-0.0.7/shcaicli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 14:19:42.000000 shcaicli-0.0.7/shcaicli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-13 14:19:42.000000 shcaicli-0.0.7/shcaicli/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-01-13 14:19:42.000000 shcaicli-0.0.7/shcaicli/shcai_exc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 14:19:48.911347 shcaicli-0.0.7/shcaicli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-01-13 14:19:48.000000 shcaicli-0.0.7/shcaicli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-13 14:19:48.000000 shcaicli-0.0.7/shcaicli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 14:19:48.000000 shcaicli-0.0.7/shcaicli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-13 14:19:48.000000 shcaicli-0.0.7/shcaicli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-13 14:19:48.000000 shcaicli-0.0.7/shcaicli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:14:46.935244 shcaicli-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 14:14:39.000000 shcaicli-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-05-22 14:14:46.935244 shcaicli-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-22 14:14:39.000000 shcaicli-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 14:14:39.000000 shcaicli-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:14:46.935244 shcaicli-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-22 14:14:39.000000 shcaicli-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:14:46.935244 shcaicli-0.0.8/shcaicli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:14:39.000000 shcaicli-0.0.8/shcaicli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-22 14:14:39.000000 shcaicli-0.0.8/shcaicli/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-22 14:14:39.000000 shcaicli-0.0.8/shcaicli/shcai_exc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:14:46.935244 shcaicli-0.0.8/shcaicli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-05-22 14:14:46.000000 shcaicli-0.0.8/shcaicli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-22 14:14:46.000000 shcaicli-0.0.8/shcaicli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:14:46.000000 shcaicli-0.0.8/shcaicli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 14:14:46.000000 shcaicli-0.0.8/shcaicli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 14:14:46.000000 shcaicli-0.0.8/shcaicli.egg-info/top_level.txt
```

### Comparing `shcaicli-0.0.7/LICENSE` & `shcaicli-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shcaicli-0.0.7/PKG-INFO` & `shcaicli-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcaicli
-Version: 0.0.7
+Version: 0.0.8
 Summary: SHC.Ai Cli
 Home-page: https://www.ihealthgroup.com.br
 Author: iHealth Group
 Author-email: rafael.morais@ihealthgroup.com.br
 Project-URL: Bug Tracker, https://github.com/ihealth-group/shcai-cli/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

### Comparing `shcaicli-0.0.7/README.md` & `shcaicli-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `shcaicli-0.0.7/setup.py` & `shcaicli-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `shcaicli-0.0.7/shcaicli/api.py` & `shcaicli-0.0.8/shcaicli/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,24 @@
                ):
     self._api_root = api_root
     self._api_name = api_name[1:] if api_name.startswith('/') else api_name
     self._api_name = f'{self._api_name}?output_type=tokens' if tokens_mode else self._api_name
     self.api_version = api_version
     self.api_key = api_key
 
-  def infer(self, cn: str = None):
-    if cn is None or cn.strip() == '':
-      raise ValueError('invalid value for cn parameter')
+  def infer(self, cns: [] = None):
+    if cns is None or len(cns) == 0:
+      raise ValueError('invalid value for cns parameter')
 
     headers = {
       'Content-Type': 'application/json',
       'X-Gravitee-Api-Key': self.api_key,
     }
     url = f'{self._api_root}/{self._api_name}'
     data = {
-      'text': cn
+      'cns': cns
     }
-    response = requests.post(url, json=data, headers=headers)
+    response = requests.post(url, json=data, headers=headers, timeout=30)
     if response.status_code == 200:
       return json.loads(response.text)
     else:
       raise SHCAIException(f'Request failed with status code {response.status_code}. Response: {response.text}')
```

### Comparing `shcaicli-0.0.7/shcaicli.egg-info/PKG-INFO` & `shcaicli-0.0.8/shcaicli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shcaicli
-Version: 0.0.7
+Version: 0.0.8
 Summary: SHC.Ai Cli
 Home-page: https://www.ihealthgroup.com.br
 Author: iHealth Group
 Author-email: rafael.morais@ihealthgroup.com.br
 Project-URL: Bug Tracker, https://github.com/ihealth-group/shcai-cli/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

