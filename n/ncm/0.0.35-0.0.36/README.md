# Comparing `tmp/ncm-0.0.35.tar.gz` & `tmp/ncm-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncm-0.0.35.tar", last modified: Fri Apr 12 21:14:26 2024, max compression
+gzip compressed data, was "ncm-0.0.36.tar", last modified: Wed May 22 18:32:34 2024, max compression
```

## Comparing `ncm-0.0.35.tar` & `ncm-0.0.36.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:14:25.995735 ncm-0.0.35/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-12 21:14:14.000000 ncm-0.0.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-12 21:14:25.995735 ncm-0.0.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-12 21:14:14.000000 ncm-0.0.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:14:25.995735 ncm-0.0.35/ncm/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:14:14.000000 ncm-0.0.35/ncm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   148323 2024-04-12 21:14:14.000000 ncm-0.0.35/ncm/ncm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 21:14:25.995735 ncm-0.0.35/ncm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-12 21:14:25.000000 ncm-0.0.35/ncm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 21:14:25.995735 ncm-0.0.35/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      602 2024-04-12 21:14:23.000000 ncm-0.0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:32:34.727606 ncm-0.0.36/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-22 18:32:22.000000 ncm-0.0.36/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-22 18:32:34.727606 ncm-0.0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-22 18:32:22.000000 ncm-0.0.36/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:32:34.723606 ncm-0.0.36/ncm/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:32:22.000000 ncm-0.0.36/ncm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   149360 2024-05-22 18:32:22.000000 ncm-0.0.36/ncm/ncm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 18:32:34.723606 ncm-0.0.36/ncm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 18:32:34.000000 ncm-0.0.36/ncm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 18:32:34.727606 ncm-0.0.36/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      602 2024-05-22 18:32:32.000000 ncm-0.0.36/setup.py
```

### Comparing `ncm-0.0.35/LICENSE` & `ncm-0.0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `ncm-0.0.35/PKG-INFO` & `ncm-0.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.35
+Version: 0.0.36
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.35/README.md` & `ncm-0.0.36/README.md`

 * *Files identical despite different names*

### Comparing `ncm-0.0.35/ncm/ncm.py` & `ncm-0.0.36/ncm/ncm.py`

 * *Files 1% similar despite different names*

```diff
@@ -2089,14 +2089,38 @@
         ncm = self.session.patch(
             '{0}/configuration_managers/{1}/'.format(self.base_url,
                                                      str(config_man_id)),
             data=json.dumps(payload))  # Patch indie config with new values
         result = self._return_handler(ncm.status_code, ncm.text, call_type)
         return result
 
+    def set_router_fields(self, router_id: int, name: str = None, description: str = None, asset_id: str = None, custom1: str = None, custom2: str = None):
+        """
+        This method sets multiple fields for a router.
+        :param router_id: ID of router to update
+        :param name: Name/System ID to set
+        :param description: Description string to set
+        :param asset_id: Asset ID string to set
+        :param custom1: Custom1 field to set
+        :param custom2: Custom2 field to set
+        :return:
+        """
+        call_type = 'Router Fields'
+
+        put_url = '{0}/routers/{1}/'.format(self.base_url, str(router_id))
+
+        put_data = {}
+        for k,v in (('name', name), ('description', description), ('asset_id', asset_id), ('custom1', custom1), ('custom2', custom2)):
+            if v is not None:
+                put_data[k] = v
+
+        ncm = self.session.put(put_url, data=json.dumps(put_data))
+        result = self._return_handler(ncm.status_code, ncm.json(), call_type)
+        return result
+
 class NcmClientv3(BaseNcmClient):
     """
     This NCM Client class provides functions for interacting with =
     the Cradlepoint NCM API. Full documentation of the Cradlepoint API can be
     found at: https://developer.cradlepoint.com
     """
```

### Comparing `ncm-0.0.35/ncm.egg-info/PKG-INFO` & `ncm-0.0.36/ncm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncm
-Version: 0.0.35
+Version: 0.0.36
 Summary: Python client library for Cradlepoint NCM API
 Home-page: https://github.com/cradlepoint/api-samples/tree/master/ncm
 Author: Nathan Wiens - Cradlepoint
 Author-email: nathan.wiens@cradlepoint.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ncm-0.0.35/setup.py` & `ncm-0.0.36/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncm",
-    version="0.0.35",
+    version="0.0.36",
     author="Nathan Wiens - Cradlepoint",
     author_email="nathan.wiens@cradlepoint.com",
     description="Python client library for Cradlepoint NCM API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cradlepoint/api-samples/tree/master/ncm",
     packages=find_packages(),
```

